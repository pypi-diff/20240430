# Comparing `tmp/tool2schema-1.3.1.tar.gz` & `tmp/tool2schema-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tool2schema-1.3.1.tar", max compression
+gzip compressed data, was "tool2schema-2.0.0.tar", max compression
```

## Comparing `tool2schema-1.3.1.tar` & `tool2schema-2.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11338 2024-04-08 18:08:45.965268 tool2schema-1.3.1/LICENSE
--rw-r--r--   0        0        0     6780 2024-04-08 18:08:45.965268 tool2schema-1.3.1/README.md
--rw-r--r--   0        0        0      734 2024-04-08 18:09:22.897307 tool2schema-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      310 2024-04-08 18:09:22.897307 tool2schema-1.3.1/tool2schema/__init__.py
--rw-r--r--   0        0        0     2986 2024-04-08 18:08:45.969268 tool2schema-1.3.1/tool2schema/config.py
--rw-r--r--   0        0        0     3865 2024-04-08 18:08:45.969268 tool2schema-1.3.1/tool2schema/parameter_schema.py
--rw-r--r--   0        0        0    12911 2024-04-08 18:08:45.969268 tool2schema-1.3.1/tool2schema/schema.py
--rw-r--r--   0        0        0     9311 2024-04-08 18:08:45.969268 tool2schema-1.3.1/tool2schema/type_schema.py
--rw-r--r--   0        0        0     7513 1970-01-01 00:00:00.000000 tool2schema-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11338 2024-04-30 21:06:23.446210 tool2schema-2.0.0/LICENSE
+-rw-r--r--   0        0        0     9157 2024-04-30 21:06:23.446210 tool2schema-2.0.0/README.md
+-rw-r--r--   0        0        0      886 2024-04-30 21:06:31.730218 tool2schema-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      378 2024-04-30 21:06:31.730218 tool2schema-2.0.0/tool2schema/__init__.py
+-rw-r--r--   0        0        0     3478 2024-04-30 21:06:23.450210 tool2schema-2.0.0/tool2schema/config.py
+-rw-r--r--   0        0        0     3865 2024-04-30 21:06:23.450210 tool2schema-2.0.0/tool2schema/parameter_schema.py
+-rw-r--r--   0        0        0    15237 2024-04-30 21:06:23.450210 tool2schema-2.0.0/tool2schema/schema.py
+-rw-r--r--   0        0        0     9449 2024-04-30 21:06:23.450210 tool2schema-2.0.0/tool2schema/type_schema.py
+-rw-r--r--   0        0        0     9890 1970-01-01 00:00:00.000000 tool2schema-2.0.0/PKG-INFO
```

### Comparing `tool2schema-1.3.1/LICENSE` & `tool2schema-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tool2schema-1.3.1/tool2schema/config.py` & `tool2schema-2.0.0/tool2schema/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,44 @@
 from __future__ import annotations
 
 import copy
+from enum import Enum
 from typing import Optional
 
 
+class SchemaType(Enum):
+    """Enum for schema types."""
+
+    OPENAI_API = 0
+    OPENAI_TUNE = 1
+    ANTHROPIC_CLAUDE = 2
+
+
 class Config:
     """
     Configuration class for tool2schema.
     """
 
     def __init__(self, parent: Optional[Config] = None, **settings):
         self._parent = parent
         self._settings = settings
         self._initial_settings = copy.deepcopy(settings)
 
     @property
+    def schema_type(self) -> SchemaType:
+        """
+        Type of the schema to create.
+        """
+        return self._get_setting(Config.schema_type.fget.__name__, SchemaType.OPENAI_API)
+
+    @schema_type.setter
+    def schema_type(self, value: SchemaType):
+        self._set_setting(Config.schema_type.fget.__name__, value)
+
+    @property
     def ignore_parameters(self) -> list[str]:
         """
         List of parameter names to ignore when creating a schema.
         """
         return self._get_setting(Config.ignore_parameters.fget.__name__, ["self", "args", "kwargs"])
 
     @ignore_parameters.setter
```

### Comparing `tool2schema-1.3.1/tool2schema/parameter_schema.py` & `tool2schema-2.0.0/tool2schema/parameter_schema.py`

 * *Files identical despite different names*

### Comparing `tool2schema-1.3.1/tool2schema/schema.py` & `tool2schema-2.0.0/tool2schema/schema.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,113 +1,140 @@
+from __future__ import annotations
+
 import copy
 import functools
 import inspect
 import json
 import re
-from enum import Enum
+import sys
 from inspect import Parameter
 from types import ModuleType
-from typing import Any, Callable, Optional
+from typing import Any, Callable, Generic, Optional, TypeVar, overload
 
 import tool2schema
-from tool2schema.config import Config
+from tool2schema.config import Config, SchemaType
 from tool2schema.parameter_schema import ParameterSchema
 
+if sys.version_info < (3, 10):
+    from typing_extensions import ParamSpec
+else:
+    from typing import ParamSpec
 
-class SchemaType(Enum):
-    """Enum for schema types."""
-
-    API = 0
-    TUNE = 1
 
-
-def FindGPTEnabled(module: ModuleType) -> list[Callable]:
+def FindToolEnabled(module: ModuleType) -> list[ToolEnabled]:
     """
-    Find all functions with the GPTEnabled decorator.
+    Find all functions with the EnableTool decorator.
 
-    :param module: Module to search for GPTEnabled functions
+    :param module: Module to search for ToolEnabled functions
     """
-    return [x for x in module.__dict__.values() if hasattr(x, "gpt_enabled")]
+    return [x for x in module.__dict__.values() if hasattr(x, "tool_enabled")]
 
 
-def FindGPTEnabledSchemas(
-    module: ModuleType, schema_type: SchemaType = SchemaType.API
+def FindToolEnabledSchemas(
+    module: ModuleType, schema_type: Optional[SchemaType] = None
 ) -> list[dict]:
     """
-    Find all function schemas with the GPTEnabled decorator.
+    Find all function schemas with the EnableTool decorator.
 
-    :param module: Module to search for GPTEnabled functions
-    :param schema_type: Type of schema to return
+    :param module: Module to search for ToolEnabled functions
+    :param schema_type: Type of schema to return (None indicates default)
     """
-    return [x.schema.to_json(schema_type) for x in FindGPTEnabled(module)]
+    return [x.to_json(schema_type) for x in FindToolEnabled(module)]
 
 
-def FindGPTEnabledByName(module: ModuleType, name: str) -> Optional[Callable]:
+def FindToolEnabledByName(module: ModuleType, name: str) -> Optional[ToolEnabled]:
     """
-    Find a function with the GPTEnabled decorator by name.
+    Find a function with the EnableTool decorator by name.
 
-    :param module: Module to search for GPTEnabled functions
+    :param module: Module to search for ToolEnabled functions
     :param name: Name of the function to find
     """
-    for func in FindGPTEnabled(module):
+    for func in FindToolEnabled(module):
         if func.__name__ == name:
             return func
     return None
 
 
-def FindGPTEnabledByTag(module: ModuleType, tag: str) -> list[Callable]:
+def FindToolEnabledByNameSchema(
+    module: ModuleType, name: str, schema_type: Optional[SchemaType] = None
+) -> Optional[dict]:
+    """
+    Find a function schema with the EnableTool decorator by name.
+
+    :param module: Module to search for ToolEnabled functions
+    :param name: Name of the function to find
+    :param schema_type: Type of schema to return (None indicates default)
+    """
+    if (func := FindToolEnabledByName(module, name)) is None:
+        return None
+    return func.to_json(schema_type)
+
+
+def FindToolEnabledByTag(module: ModuleType, tag: str) -> list[ToolEnabled]:
+    """
+    Find all functions with the EnableTool decorator by tag.
+
+    :param module: Module to search for ToolEnabled functions
+    :param tag: Tag to search for
+    """
+    return [x for x in FindToolEnabled(module) if x.has(tag)]
+
+
+def FindToolEnabledByTagSchemas(
+    module: ModuleType, tag: str, schema_type: Optional[SchemaType] = None
+) -> list[dict]:
     """
-    Find all functions with the GPTEnabled decorator by tag.
+    Find all function schemas with the EnableTool decorator by tag.
 
-    :param module: Module to search for GPTEnabled functions
+    :param module: Module to search for ToolEnabled functions
     :param tag: Tag to search for
+    :param schema_type: Type of schema to return (None indicates default)
     """
-    return [x for x in FindGPTEnabled(module) if x.has(tag)]
+    return [x.to_json(schema_type) for x in FindToolEnabledByTag(module, tag)]
 
 
-def SaveGPTEnabled(module: ModuleType, path: str, schema_type: SchemaType = SchemaType.API):
+def SaveToolEnabled(module: ModuleType, path: str, schema_type: Optional[SchemaType] = None):
     """
-    Save all function schemas with the GPTEnabled decorator to a file.
+    Save all function schemas with the EnableTool decorator to a file.
 
-    :param module: Module to search for GPTEnabled functions
+    :param module: Module to search for ToolEnabled functions
     :param path: Path to save the schemas to
-    :param schema_type: Type of schema to return
+    :param schema_type: Type of schema to return (None indicates default)
     """
-    schemas = FindGPTEnabledSchemas(module, schema_type)
+    schemas = FindToolEnabledSchemas(module, schema_type)
     json.dump(schemas, open(path, "w"))
 
 
 class ParseException(Exception):
     """Exception for schema parsing errors."""
-
     pass
 
 
-def LoadGPTEnabled(
+def LoadToolEnabled(
     module: ModuleType,
     function: dict,
     validate: bool = True,
     ignore_hallucinations: bool = True,
 ) -> tuple[Callable, dict[str, Any]]:
     """
     Given a function dictionary containing the name of a function and the arguments to pass to it,
-    retrieve the corresponding function among those with the `GPTEnabled` decorator defined in
+    retrieve the corresponding function among those with the `EnableTool` decorator defined in
     `module`. When `validate` is true, validate the arguments and raise `ParseException` if the
     arguments are not valid (see more information below).
 
     :param module: The module where the function is defined
     :param function: A dictionary with keys `name` and `arguments`, where `name` is the name of
         the function to find, and `arguments` is either a dictionary of argument values or a JSON
         string that can be parsed to a dictionary of argument values.
     :param validate: Whether to validate the function arguments
     :param ignore_hallucinations: When true, any hallucinated arguments are ignored; when false,
         an exception is raised if any hallucinated arguments are found. `validate` must be true.
     :return: A tuple consisting of the function and a dictionary of argument values
     :raises ParseException: Thrown when any of the following conditions is met:
-        - Function isn't defined in the given module, or is not decorated with `GPTEnabled`
+        - Function isn't defined in the given module, or is not decorated with `EnableTool`
         - The arguments are given as string and the string is not valid, meaning it is:
             - Not parsable as JSON, or;
             - Is not parsed into a dictionary of argument values
         - A required argument is missing and `validate` is true
         - An argument has a value that is not of the expected type and `validate` is true
         - The dictionary contains an argument that is not expected by the function, `validate` is
           true and `ignore_hallucinations` is false
@@ -134,36 +161,36 @@
         if type(arguments) is not dict:
             raise ParseException("Arguments are not in the form of a dictionary")
 
     else:
         # Invalid type
         raise ParseException(f"Arguments cannot be of type {type(arguments)}")
 
-    f = FindGPTEnabledByName(module, name)
+    f = FindToolEnabledByName(module, name)
 
     if not f:
         # A function with the given name was not found
         raise ParseException(
             f"Function with name '{name}' is not defined in given module "
-            f"'{module.__name__}' or is missing 'GPTEnabled' decorator"
+            f"'{module.__name__}' or is missing 'EnableTool' decorator"
         )
 
     if validate:
         arguments = _validate_arguments(f, arguments, ignore_hallucinations)
 
     return f, arguments
 
 
-def _validate_arguments(f: Callable, arguments: dict, ignore_hallucinations: bool) -> dict:
+def _validate_arguments(f: ToolEnabled, arguments: dict, ignore_hallucinations: bool) -> dict:
     """
     Verify that all required arguments are present, and the arguments are of the expected type.
     Raise an exception if any of these conditions is not met, or if there are any hallucinated
     arguments and `ignore_hallucinations` is false.
 
-    :param f: A GPTEnabled-decorated function
+    :param f: A EnableTool-decorated function
     :param arguments: Arguments to validate
     :param ignore_hallucinations: Whether to ignore hallucinated arguments or throw an exception
         if any are present
     :return: A dictionary of validated arguments
     """
     validated = {}
 
@@ -183,23 +210,27 @@
 
     if not ignore_hallucinations and arguments:
         raise ParseException(f"Hallucinated argument(s): {', '.join(arguments.keys())}")
 
     return validated
 
 
-class _GPTEnabled:
-    def __init__(self, func, **kwargs) -> None:
+P = ParamSpec("P")  # User-provided function parameters type
+T = TypeVar("T")  # User-provided function return type
+
+
+class ToolEnabled(Generic[P, T]):
+    def __init__(self, func: Callable[P, T], **kwargs) -> None:
         self.func = func
         self.tags = kwargs.pop("tags", [])
         self.config = Config(tool2schema.CONFIG, **kwargs)
         self.schema = FunctionSchema(func, self.config)
         functools.update_wrapper(self, func)
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> T:
 
         args = list(args)  # Tuple is immutable, thus convert to list
 
         for i, arg in enumerate(args):
             for p in self.schema.parameter_schemas.values():
                 if p.index == i:
                     # Convert the JSON value to the type expected by the method
@@ -208,29 +239,46 @@
         for key in kwargs:
             if key in self.schema.parameter_schemas:
                 # Convert the JSON value to the type expected by the method
                 kwargs[key] = self.schema.parameter_schemas[key].type_schema.decode(kwargs[key])
 
         return self.func(*args, **kwargs)
 
-    def gpt_enabled(self) -> bool:
+    def tool_enabled(self) -> bool:
         return True
 
+    def to_json(self, schema_type: Optional[SchemaType] = None) -> dict:
+        """
+        Return JSON schema for the function.
+
+        :param schema_type: None indicates default schema type
+        :return: JSON schema
+        """
+        return self.schema.to_json(schema_type)
+
     def has(self, tag: str) -> bool:
         return tag in self.tags
 
 
-def GPTEnabled(func=None, **kwargs):
+@overload
+def EnableTool(func: Callable[P, T], **kwargs) -> ToolEnabled[P, T]: ...
+
+
+@overload
+def EnableTool(**kwargs) -> Callable[[Callable[P, T]], ToolEnabled[P, T]]: ...
+
+
+def EnableTool(func=None, **kwargs):
     """Decorator to generate a function schema for OpenAI."""
-    if func:
-        return _GPTEnabled(func, **kwargs)
+    if func is not None:
+        return ToolEnabled(func, **kwargs)
     else:
 
-        def wrapper(function):
-            return _GPTEnabled(function, **kwargs)
+        def wrapper(function: Callable[P, T]) -> ToolEnabled[P, T]:
+            return ToolEnabled(function, **kwargs)
 
         return wrapper
 
 
 class FunctionSchema:
     """Automatically create a function schema for OpenAI."""
 
@@ -241,50 +289,60 @@
         :param f: The function to create a schema for
         :param config: Configuration settings
         """
         self.f = f
         self.config = config
         self._all_parameter_schemas: dict[str, ParameterSchema] = self._get_all_parameter_schemas()
 
-    def to_json(self, schema_type: SchemaType = SchemaType.API) -> dict:
+    def to_json(self, schema_type: Optional[SchemaType] = None) -> dict:
         """
         Convert schema to JSON.
         :param schema_type: Type of schema to return
         """
-        if schema_type == SchemaType.TUNE:
+        schema_type = schema_type or self.config.schema_type
+        if schema_type == SchemaType.OPENAI_TUNE:
+            return self._get_function_schema(schema_type)
+        elif schema_type == SchemaType.ANTHROPIC_CLAUDE:
             return self._get_function_schema(schema_type)
 
         return self._get_schema()
 
-    def add_enum(self, n: str, enum: list) -> "FunctionSchema":
+    def add_enum(self, n: str, enum: list) -> FunctionSchema:
         """
         Add enum property to a particular function parameter.
 
         :param n: The name of the parameter with the enum values
         :param enum: The list of values for the enum parameter
+        :return: This function schema
         """
         self._all_parameter_schemas[n].add_enum(enum)
         return self
 
     def _get_schema(self) -> dict:
         """
         Get the complete schema dictionary.
         """
         # This dictionary is only used with the API schema type
-        return {"type": "function", "function": self._get_function_schema(SchemaType.API)}
+        return {"type": "function", "function": self._get_function_schema(SchemaType.OPENAI_API)}
 
     def _get_function_schema(self, schema_type: SchemaType) -> dict:
         """
         Get the function schema dictionary.
         """
-        schema = {"name": self.f.__name__}
+        schema: dict[str, Any] = {"name": self.f.__name__}
 
-        if self.parameter_schemas or schema_type == SchemaType.TUNE:
+        need_empty_param = schema_type in [
+            SchemaType.OPENAI_TUNE,
+            SchemaType.ANTHROPIC_CLAUDE]
+        if self.parameter_schemas or need_empty_param:
             # If the schema type is tune, add the dictionary even if there are no parameters
-            schema["parameters"] = self._get_parameters_schema()
+            if schema_type == SchemaType.ANTHROPIC_CLAUDE:
+                schema["input_schema"] = self._get_parameters_schema()
+            else:
+                schema["parameters"] = self._get_parameters_schema()
 
         if (description := self._get_description()) is not None:
             # Add the function description even if it is an empty string
             schema["description"] = description
 
         return schema
```

### Comparing `tool2schema-1.3.1/tool2schema/type_schema.py` & `tool2schema-2.0.0/tool2schema/type_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Literal, Optional, Type, Union
 
 # Order matters: specific classes should appear before more generic ones,
 # because the first matching schema will be used
 TYPE_SCHEMAS: list[Type[TypeSchema]] = []
 
 
-def GPTTypeSchema(cls: Type[TypeSchema]):
+def ToolTypeSchema(cls: Type[TypeSchema]):
     """
     Decorator to register a type schema class.
     """
     cls.priority = len(TYPE_SCHEMAS)
     TYPE_SCHEMAS.insert(0, cls)  # Push to the front
     return cls
 
@@ -116,15 +116,15 @@
             "enum": self._get_enum(),
             **self._get_type(),
         }
 
         return {f: v for f, v in fields.items() if v != Parameter.empty}
 
 
-@GPTTypeSchema
+@ToolTypeSchema
 class ValueTypeSchema(TypeSchema):
     """
     Type schema for value types.
     """
 
     TYPE_MAP = {
         "int": "integer",
@@ -135,14 +135,17 @@
     }
 
     @staticmethod
     def matches(p_type) -> bool:
         return True
 
     def validate(self, value) -> bool:
+        # Allow implicit conversion from int to float
+        if self.type is float and type(value) is int:
+            return True
         return self.type == type(value)
 
     def _get_type(self) -> dict:
         return {"type": self.TYPE_MAP.get(self.type.__name__, "object")}
 
 
 class GenericTypeSchema(TypeSchema):
@@ -162,15 +165,15 @@
             or None if there is none. If there are multiple arguments, the first
             one is returned.
         """
         if args := self._get_sub_types():
             return args[0]
 
 
-@GPTTypeSchema
+@ToolTypeSchema
 class ListTypeSchema(GenericTypeSchema):
     """
     Type schema for list (array) types, including typing.List.
     """
 
     @staticmethod
     def matches(p_type: Type) -> bool:
@@ -203,15 +206,15 @@
 
         if sub_type := self._get_sub_type():
             return all(sub_type.validate(v) for v in value)
 
         return True
 
 
-@GPTTypeSchema
+@ToolTypeSchema
 class UnionTypeSchema(GenericTypeSchema):
     """
     Type schema for typing.Optional types.
     """
 
     @staticmethod
     def matches(p_type: Type) -> bool:
@@ -262,15 +265,15 @@
     def _get_enum(self) -> Union[list, Parameter.empty]:
         return self.enum_values
 
     def validate(self, value) -> bool:
         return value in self.enum_values
 
 
-@GPTTypeSchema
+@ToolTypeSchema
 class EnumClassTypeSchema(EnumTypeSchema):
     """
     Type schema for enum.Enum types.
     """
 
     def __init__(self, p_type: Enum):
         super().__init__([e.name for e in p_type], p_type)
@@ -297,15 +300,15 @@
             # Convert to an enum instance
             return self.type[value]
 
         # The user is invoking the method directly passing the enum instance
         return value
 
 
-@GPTTypeSchema
+@ToolTypeSchema
 class LiteralTypeSchema(EnumTypeSchema):
     """
     Type schema for typing.Literal types.
     """
 
     def __init__(self, p_type):
         values = list(typing.get_args(p_type))
```

### Comparing `tool2schema-1.3.1/PKG-INFO` & `tool2schema-2.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,208 +1,233 @@
-Metadata-Version: 2.1
-Name: tool2schema
-Version: 1.3.1
-Summary: A library to generate function schemas for use in the OpenAI API.
-Home-page: https://github.com/cadifyai/tool2schema
-License: Apache-2.0
-Keywords: openai,llm
-Author: Angus Stewart
-Author-email: siliconlad@protonmail.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Project-URL: Repository, https://github.com/cadifyai/tool2schema
-Description-Content-Type: text/markdown
+<div align="center">
+<img src="media/logo.jpg" height=200>
 
-# tool2schema
+<h1>
+tool2schema
+</h1>
+
+Inspired by [janekb04/py2gpt](https://github.com/janekb04/py2gpt) and [fastai/lm-hackers](https://github.com/fastai/lm-hackers)
 
 [![Check Code](https://github.com/cadifyai/tool2schema/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/cadifyai/tool2schema/actions/workflows/python-package.yml)
 [![Downloads](https://static.pepy.tech/badge/tool2schema)](https://pepy.tech/project/tool2schema)
+![Stars](https://img.shields.io/github/stars/cadifyai/tool2schema)
 
-A library to convert Python functions to schemas supported by the OpenAI API.
-
-Inspired by [janekb04/py2gpt](https://github.com/janekb04/py2gpt) and [fastai/lm-hackers](https://github.com/fastai/lm-hackers).
+</div>
 
-## Why tool2schema?
+# Why tool2schema?
 
-The OpenAI API supports [function calling](https://platform.openai.com/docs/guides/function-calling). However, to tell GPT what functions it can call, you must send the functions [in a JSON format](https://platform.openai.com/docs/api-reference/chat/create#chat-create-tools). With `tool2schema`, functions can be automatically converted to the correct JSON schema!
+Sometimes you can provide a large language model (LLM) with functions for it to call, but it needs to follow a specific schema. `tool2schema` is a small depedency-free library that converts your functions into that specific schema. So yeah, it's in the name!
 
-## Installation
+# Installation
 
 You can install `tool2schema` using `pip`.
 
 ```bash
 pip3 install tool2schema
 ```
 
-## Usage
+# Usage
 
-On all functions that you would like to get JSON schema for, simply add the `GPTEnabled` decorator.
+On all functions that you would like to get the schema for, simply add the `EnableTool` decorator. Then use the return value of `FindToolEnabledSchemas` method directly in your requests to whatever LLM you are using.
 
 ```python
-# my_functions.py
-from tool2schema import GPTEnabled
+from tool2schema import EnableTool
 
-@GPTEnabled
+@EnableTool
 def my_function1(a: int, b: str = "Hello"):
     """
     Example function description.
 
     :param a: First parameter
     :param b: Second parameter
     """
     # Function code here...
+```
 
-@GPTEnabled(tags=["tag1"])
-def my_function2(a: int, b: str = "Hello"):
-    """
-    Example function description.
+**Note**: To understand the appropriate format required for `tool2schema` to generate the appropriate schema, see the ['How it Works' section](#how-it-works).
 
-    :param a: First parameter
-    :param b: Second parameter
-    """
-    # Function code here...
+## OpenAI
+
+```python
+import my_tools  # Module with your functions
+
+from openai import OpenAI
+from tool2schema import FindToolEnabledSchemas
+
+client = OpenAI()
+completion = client.chat.completions.create(
+  model="gpt-4-turbo",
+  tools=FindToolEnabledSchemas(my_tools)  # <-- As easy as that!
+  messages=[
+    {"role": "system", "content": "You are a helpful assistant."},
+    {"role": "user", "content": "Hello!"}
+  ]
+)
 ```
 
-`tool2schema` provides some methods to easily retrieve your functions.
+<details>
+<summary><b>If finetuning an OpenAI model, then the schema is slightly different.</b></summary>
 
 ```python
-import my_functions  # Module containing your functions
-import tool2schema
+import my_tools  # Module with your functions
 
-# Return functions with GPTEnabled decorator
-gpt_enable = tool2schema.FindGPTEnabled(my_functions)
+from openai import OpenAI
+from tool2schema import FindToolEnabledSchemas, SchemaType
 
-# Return all function schemas
-schemas = tool2schema.FindGPTEnabledSchemas(my_functions)
+client = OpenAI()
+completion = client.chat.completions.create(
+  model="gpt-4-turbo",
+  tools=FindToolEnabledSchemas(my_tools, SchemaType.OPENAI_TUNE)  # <-- As easy as that!
+  messages=[
+    {"role": "system", "content": "You are a helpful assistant."},
+    {"role": "user", "content": "Hello!"}
+  ]
+)
+```
+
+</details>
 
-# Return function with given name
-f = tool2schema.FindGPTEnabledByName(my_functions, "my_function1")
+## Anthropic
 
-# Returns all functions with given tag
-fs = tool2schema.FindGPTEnabledByTag(my_functions, "tag1")
+```python
+import my_tools  # Module with your functions
 
-# Saves function schemas to JSON file
-json_path = # Path to JSON file
-tool2schema.SaveGPTEnabled(my_functions, json_path)
+import anthropic
+from tool2schema import FindToolEnabledSchemas, SchemaType
+
+client = anthropic.Anthropic()
+response = client.beta.tools.messages.create(
+    model="claude-3-opus-20240229",
+    tools=FindToolEnabledSchemas(my_tools, SchemaType.ANTHROPIC_CLAUDE), # <-- As easy as that!
+    messages=[{"role": "user", "content": "What's the weather like in San Francisco?"}],
+)
 ```
 
-## How it Works
+## Mistral
 
-`tool2schema` uses certain features of your function to correctly populate the schema.
+Currently the same as OpenAI.
 
-- Parameter type hints
-- Parameter default values
-- Docstring with parameter descriptions
+# Public API
 
-The docstring must be of a specific format. An example function is defined below that utilises all of the above features.
+In this section we describe in more detail how to utilise this library to its fullest extent.
 
-```python
-def my_function(a: int, b: str = "Hello"):
-    """
-    Example function description.
+## Configuration
 
-    :param a: First parameter
-    :param b: Second parameter
-    """
-```
+There are a number of setting available for you to tweak.
+
+| Name | Description | Default Value |
+|----------|----------|--------------|
+|   `ignore_parameters`  |   A list of parameter names to exclude from the schema  |  `[]`
+|   `ignore_all_parameters`  |   A boolean value indicating whether to exclude all parameters from the schema. When set to true, `ignore_parameters` and `ignore_parameter_descriptions` will be ignored.  | `False` |
+|   `ignore_function_description`  |   A boolean value indicating whether to exclude the function description from the schema.  | `False` |
+|   `ignore_parameter_descriptions`  |   A boolean value indicating whether to exclude all parameter descriptions from the schema  | `False` |
+| `schema_type` | Default schema type to use. | `SchemaType.OPENAI_API` |
+
+### Decorator Configuration
 
-To get the schema for this function, simply use the `GPTEnabled` decorator. The decorator will return a class with some additional attributes but can still be called as a function.
+You can provide the `EnableTool` decorator with the settings listed above.
 
-The schema of the function be accessed using the `schema` attribute.
+For example, to omit parameters `b` and `c`:
 
 ```python
-my_function.schema.to_json()
+@GPTEnabled(ignore_parameters=["b", "c"])
+def my_function(a: int, b: str, c: float):
+    # Function code here...
 ```
 
-This returns the function schema in JSON format.
+### Global Configuration
 
-### Supported Parameter Types
+It is also possible to specify the settings globally, so that they apply to all functions
+unless explicitly overridden. It can be done by editing the global configuration as follows:
 
-The following parameter types are supported:
+```python
+import tool2schema
 
-- `int`
-- `float`
-- `str`
-- `bool`
-- `list`
+# Ignore all parameters named "a" or "b" by default
+tool2schema.CONFIG.ignore_parameters = ["a", "b"]
+```
 
-Any other parameter types will be listed as `object` in the schema.
+## Module Operations
 
-### Enumerations
+`tool2schema` has methods available to get functions from a module. See below for example usage of each of the public API methods that `tool2schema` exposes.
 
-If you want to limit the possible values of a parameter, you can use a `typing.Literal` type hint or a
-subclass of `enum.Enum`. For example, using `typing.Literal`:
+<details>
+<summary><b>The examples assume the existance of this my_functions module.</b></summary>
 
 ```python
-import typing
-
+from tool2schema import GPTEnabled
 
 @GPTEnabled
-def my_function(a: int, b: typing.Literal["yes", "no"]):
+def my_function1(a: int, b: str = "Hello"):
     """
     Example function description.
 
     :param a: First parameter
     :param b: Second parameter
     """
     # Function code here...
-```
-
-Equivalent example using `enum.Enum`:
-
-```python
-from enum import Enum
-
-class MyEnum(Enum):
-    YES = 0
-    NO = 1
 
 
-@GPTEnabled
-def my_function(a: int, b: MyEnum):
+@GPTEnabled(tags=["tag1"])
+def my_function2(a: int, b: str = "Hello"):
     """
     Example function description.
 
     :param a: First parameter
     :param b: Second parameter
     """
     # Function code here...
 ```
+</details>
 
-In the case of `Enum` subclasses, note that the schema will include the enumeration names rather than the values.
-In the example above, the schema will include `["YES", "NO"]` rather than `[0, 1]`.
+<br>
+
+```python
+import my_functions
+import tool2schema
 
-The `@GPTEnabled` decorator also allows to invoke the function using the name of the enum member rather than an
-instance of the class. For example, you may invoke `my_function(1, MyEnum.YES)` as `my_function(1, "YES")`.
+# Return all functions with the ToolEnable decorator
+functions = tool2schema.FindToolEnabled(my_functions)
+schemas = tool2schema.FindToolEnabledSchemas(my_functions)
 
-If the enumeration values are not known at the time of defining the function,
-you can add them later using the `add_enum` method.
+# Return the function with a ToolEnable decorator and the given name
+function = tool2schema.FindToolEnabledByName(my_functions, "my_function1")
+schema = tool2schema.FindToolEnabledByNameSchema(my_functions, "my_function1")
+
+# Return all functions with a ToolEnable decorator and the given tag
+functions = tool2schema.FindToolEnabledByTag(my_functions, "tag1")
+schemas = tool2schema.FindToolEnabledByTagSchemas(my_functions, "tag1")
+
+# Save the schemas of all functions with a ToolEnable decorator to a JSON file
+json_path = "path/to/json/file"
+tool2schema.SaveToolEnabled(my_functions, json_path)
+```
+
+## Function Schema
+
+To get the schema (in JSON format) for a function with the `EnableTool` decorator, either use the methods in the [Method Operations](#module-operations) section, or call the `to_json()` method on the function directly.
 
 ```python
 @GPTEnabled
-def my_function(a: int, b: str,):
+def my_function(a: int):
     """
     Example function description.
 
     :param a: First parameter
-    :param b: Second parameter
     """
     # Function code here...
 
-my_function.schema.add_enum("b", ["yes", "no"])
+my_function.to_json()  # <-- returns the function schema
 ```
 
-### Tags
+**Note**: that the decorator returns a new `ToolEnabled` object with additional attributes, but can be called just like the original function.
 
-The `GPTEnabled` decorator also supports the `tags` keyword argument. This allows you to add tags to your function schema.
+## Function Tags
+
+The `EnableTool` decorator also supports the `tags` keyword argument. This allows you to add tags to your function schema.
 
 ```python
 @GPTEnabled(tags=["tag1", "tag2"])
 def my_function(a: int, b: str = "Hello"):
     """
     Example function description.
 
@@ -220,38 +245,45 @@
 
 You can check if a function has a certain tag using the `has_tag` method.
 
 ```python
 my_function.has_tag("tag1")  # True
 ```
 
-### Disable parts of the schema
+# How it Works
 
-You can provide `GPTEnabled` with a number of settings to selectively disable parts of the schema.
-For example, to omit certain parameters:
+`tool2schema` uses certain features of your function definition to correctly populate the schema.
 
-```python
-@GPTEnabled(ignore_parameters=["b", "c"])  # b and c will not be included in the schema
-def my_function(a: int, b: str, c: float):
-    # Function code here...
-```
+- Parameter type hints
+- Parameter default values
+- Docstring with parameter descriptions
 
-The available settings are:
-- `ignore_parameters`: A list of parameter names to exclude from the schema (defaults to `[]`).
-- `ignore_all_parameters`: A boolean value indicating whether to exclude all parameters from the schema
-  (defaults to `False`). When set to true, all other parameter-related settings (`ignore_parameters` and
-  `ignore_parameter_descriptions`) will be ignored.
-- `ignore_function_description`: A boolean value indicating whether to exclude the function description from
-  the schema (defaults to `False`).
-- `ignore_parameter_descriptions`: A boolean value indicating whether to exclude all parameter descriptions
-  from the schema (defaults to `False`).
+The docstring must be using the [Sphinx docstring](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html) format.
+**Note**: We use the parameter type hints instead of the docstring for parameter types.
 
-It is also possible to specify the settings globally, so that they apply to all functions
-unless explicitly overridden. It can be done by editing the global configuration as follows:
+## Supported Parameter Types
+
+Most of the common types are supported. See [type_schema.py](./tool2schema/type_schema.py) for more details.
+
+Any parameter types not supported will be listed as `object` in the schema.
+
+## Enumerations
+
+Enumeration in the schema are listed as strings of the enumeration names rather than the values. This was a design choice we felt made more sense for use with LLMs. We introduce some additional pre-processing to ensure that the enumeration name strings are mapped back to the correct enum value. Therefore, `@EnableTool` decorator allows to invoke the function using the name of the enum member rather than an instance of the class. For example, you may invoke `my_function(1, MyEnum.YES)` as `my_function(1, "YES")`. See the code for more details.
+
+> Enumerations are used to explcitly indicate what values are permitted for the parameter value.
+
+If the enumeration values are not known at the time of defining the function, you can add them later using the `add_enum` method.
 
 ```python
-import tool2schema
+@GPTEnabled
+def my_function(a: int, b: str):
+    """
+    Example function description.
 
-# Ignore all parameters named "a" or "b" by default
-tool2schema.CONFIG.ignore_parameters = ["a", "b"]
-```
+    :param a: First parameter
+    :param b: Second parameter
+    """
+    # Function code here...
 
+my_function.schema.add_enum("b", ["yes", "no"])  #  <-- Add enum values for parameter 'b'
+```
```

