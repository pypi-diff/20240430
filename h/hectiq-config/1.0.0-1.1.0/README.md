# Comparing `tmp/hectiq_config-1.0.0.tar.gz` & `tmp/hectiq_config-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hectiq_config-1.0.0.tar", last modified: Mon Apr 29 15:44:26 2024, max compression
+gzip compressed data, was "hectiq_config-1.1.0.tar", last modified: Tue Apr 30 19:15:55 2024, max compression
```

## Comparing `hectiq_config-1.0.0.tar` & `hectiq_config-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:44:26.283584 hectiq_config-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-29 15:44:12.000000 hectiq_config-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-29 15:44:26.283584 hectiq_config-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-29 15:44:12.000000 hectiq_config-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:44:26.283584 hectiq_config-1.0.0/hectiq_config/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 15:44:12.000000 hectiq_config-1.0.0/hectiq_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9415 2024-04-29 15:44:12.000000 hectiq_config-1.0.0/hectiq_config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-29 15:44:12.000000 hectiq_config-1.0.0/hectiq_config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:44:26.283584 hectiq_config-1.0.0/hectiq_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-29 15:44:26.000000 hectiq_config-1.0.0/hectiq_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-29 15:44:26.000000 hectiq_config-1.0.0/hectiq_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:44:26.000000 hectiq_config-1.0.0/hectiq_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 15:44:26.000000 hectiq_config-1.0.0/hectiq_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-29 15:44:26.000000 hectiq_config-1.0.0/hectiq_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-29 15:44:12.000000 hectiq_config-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:44:26.283584 hectiq_config-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:15:55.739119 hectiq_config-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-30 19:15:46.000000 hectiq_config-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-30 19:15:55.739119 hectiq_config-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-30 19:15:46.000000 hectiq_config-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:15:55.735119 hectiq_config-1.1.0/hectiq_config/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 19:15:46.000000 hectiq_config-1.1.0/hectiq_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-04-30 19:15:46.000000 hectiq_config-1.1.0/hectiq_config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-30 19:15:46.000000 hectiq_config-1.1.0/hectiq_config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:15:55.739119 hectiq_config-1.1.0/hectiq_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-30 19:15:55.000000 hectiq_config-1.1.0/hectiq_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-30 19:15:55.000000 hectiq_config-1.1.0/hectiq_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:15:55.000000 hectiq_config-1.1.0/hectiq_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 19:15:55.000000 hectiq_config-1.1.0/hectiq_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 19:15:55.000000 hectiq_config-1.1.0/hectiq_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-30 19:15:46.000000 hectiq_config-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:15:55.739119 hectiq_config-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:15:55.735119 hectiq_config-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-30 19:15:46.000000 hectiq_config-1.1.0/tests/test_config.py
```

### Comparing `hectiq_config-1.0.0/LICENSE` & `hectiq_config-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hectiq_config-1.0.0/PKG-INFO` & `hectiq_config-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hectiq-config
-Version: 1.0.0
+Version: 1.1.0
 Summary: A simple API to manipulate configuration files
 Author-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Maintainer-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Project-URL: Repository, https://github.com/HectiqAI/hectiq-config
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hectiq_config-1.0.0/README.md` & `hectiq_config-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hectiq_config-1.0.0/hectiq_config/config.py` & `hectiq_config-1.1.0/hectiq_config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import orjson
 import re
 
 from pydantic import BaseModel, ValidationError
 from pydantic.fields import FieldInfo
 from typing import Optional, Any, Type, Iterator, Union, Literal
 
-from hectiq_config.utils import template_to_model
+from hectiq_config.utils import template_to_model, is_numeric_key
+
 
 class Config:
     """
     A Config object is an abstract object designed to store
     your configurations with a simple API.
 
     The Config object is a dictionary-like object that supports
@@ -80,16 +81,19 @@
             self.to_model(template=template, extra=extra)
         except ValidationError as e:
             if raise_exception:
                 raise e
             return False
         return True
 
-    def cast(self, template: Union[dict[str, tuple[type, Any]], type[BaseModel], type[None]] = None, 
-             extra: Optional[Literal["allow", "ignore", "forbid"]] = "allow") -> "Config":
+    def cast(
+        self,
+        template: Union[dict[str, tuple[type, Any]], type[BaseModel], type[None]] = None,
+        extra: Optional[Literal["allow", "ignore", "forbid"]] = "allow",
+    ) -> "Config":
         """Cast the values of a configuration to a new Config object using a template.
         Args:
             template (dict or pydantic.BaseModel, optional): A template to cast the configuration
                 against. Default: None.
             extra (str, optional): How to handle extra fields that are not specified in the template.
                 Default: "allow". Can be "ignore" or "forbid".
         Returns:
@@ -138,15 +142,14 @@
         -------------
         d = {"a": {"b": 4}}
         config = Config.from_dict(d)
         assert config.a.b == 4
         """
         if not isinstance(data, dict):
             return data
-
         config = cls(**data)
         return config
 
     @classmethod
     def from_model(cls, model: BaseModel) -> "Config":
         """Convert a pydantic model to a Config object.
         `model` can be nested (model within model), which will generate sub configs.
@@ -220,15 +223,15 @@
         return dict(zip(self.keys(), self.values())).items()
 
     def copy(self) -> "Config":
         return Config.from_dict(self.to_dict())
 
     def get(self, name: str, default: Optional[Any] = None) -> Any:
         # Nested keys
-        if self.seperator in name:
+        if self.seperator in name and not is_numeric_key(name):
             root_key, *keys = name.split(self.seperator)
             return self._state.get(root_key, Config()).get(self.seperator.join(keys), default)
 
         # Extract value
         value = self._state.get(name, default)
 
         # Alias value
```

### Comparing `hectiq_config-1.0.0/hectiq_config/utils.py` & `hectiq_config-1.1.0/hectiq_config/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,51 @@
 from pydantic import create_model, BaseModel, ConfigDict
 from pydantic.fields import FieldInfo
-from typing import  Any, Type
+from typing import Any, Type
+
+
+def is_numeric_key(key: str) -> bool:
+    """Check if a key is a float number.
+
+    Args:
+        key (str): The key to check.
+
+    Returns:
+        bool: True if the key is a float number, False otherwise.
+    """
+    if key.isnumeric():
+        return True
+    if len(key.split(".")) <= 2:
+        return key.replace(".", "").isnumeric()
+    return False
+
 
 def template_to_model(
     name: str, template_dict: dict[str, tuple[type, Any]], *, extra: str = "ignore"
 ) -> Type[BaseModel]:
     """Create a pydantic model from a template dict.
 
     Args:
         name (str): The name of the model.
         template_dict (dict): A dictionary with the template.
         extra (str, optional): How to handle extra fields that are not specified in the template.
             Default: "ignore".
-    
+
     Returns:
         pydantic.BaseModel: A pydantic model with the specified fields.
     """
     fields = {}
     for key, value in template_dict.items():
         if isinstance(value, dict):
             fields[key] = (template_to_model(key, value, extra=extra), ...)
         else:
             fields[key] = value
     return create_model(name, **fields, __config__=ConfigDict(extra=extra))
 
+
 def model_to_template(model: BaseModel) -> dict[str, tuple[type, FieldInfo]]:
     """
     Return a template associated to the configuration.
 
     Args:
         model (pydantic.BaseModel): A pydantic model.
```

### Comparing `hectiq_config-1.0.0/hectiq_config.egg-info/PKG-INFO` & `hectiq_config-1.1.0/hectiq_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hectiq-config
-Version: 1.0.0
+Version: 1.1.0
 Summary: A simple API to manipulate configuration files
 Author-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Maintainer-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Project-URL: Repository, https://github.com/HectiqAI/hectiq-config
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hectiq_config-1.0.0/pyproject.toml` & `hectiq_config-1.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 [build-system]
-requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
+requires = ["setuptools >= 61.0"]
 
 [tool.setuptools]
 packages = ["hectiq_config"]
 
 [project]
-name = "hectiq-config"
-version = "1.0.0"
-description = "A simple API to manipulate configuration files"
-readme = "README.md"
-requires-python = ">=3.8"
 authors = [
   {name = "Edward Laurence", email = "edwardl@hectiq.ai"},
   {name = "Charles Murphy", email = "cmurphy@hectiq.ai"},
 ]
+dependencies = [
+  "pydantic",
+  "orjson",
+]
+description = "A simple API to manipulate configuration files"
 maintainers = [
   {name = "Edward Laurence", email = "edwardl@hectiq.ai"},
   {name = "Charles Murphy", email = "cmurphy@hectiq.ai"},
 ]
-dependencies = [
-    "pydantic",
-    "orjson"
-]
+name = "hectiq-config"
+readme = "README.md"
+requires-python = ">=3.8"
+version = "1.1.0"
 
 [project.urls]
 Repository = "https://github.com/HectiqAI/hectiq-config"
-
-
```

