# Comparing `tmp/dataclass_settings-0.3.0.tar.gz` & `tmp/dataclass_settings-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_settings-0.3.0.tar", max compression
+gzip compressed data, was "dataclass_settings-0.3.1.tar", max compression
```

## Comparing `dataclass_settings-0.3.0.tar` & `dataclass_settings-0.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-04-24 19:43:41.114278 dataclass_settings-0.3.0/LICENSE
--rw-r--r--   0        0        0     6119 2024-04-24 19:43:41.114278 dataclass_settings-0.3.0/README.md
--rw-r--r--   0        0        0     1904 2024-04-24 19:43:41.114278 dataclass_settings-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      246 2024-04-24 19:43:41.114278 dataclass_settings-0.3.0/src/dataclass_settings/__init__.py
--rw-r--r--   0        0        0     3456 2024-04-24 19:43:41.114278 dataclass_settings-0.3.0/src/dataclass_settings/base.py
--rw-r--r--   0        0        0     5991 2024-04-24 19:43:41.114278 dataclass_settings-0.3.0/src/dataclass_settings/class_inspect.py
--rw-r--r--   0        0        0     2071 2024-04-24 19:43:41.114278 dataclass_settings-0.3.0/src/dataclass_settings/context.py
--rw-r--r--   0        0        0     2471 2024-04-24 19:43:41.114278 dataclass_settings-0.3.0/src/dataclass_settings/loaders.py
--rw-r--r--   0        0        0        0 2024-04-24 19:43:41.114278 dataclass_settings-0.3.0/src/dataclass_settings/py.typed
--rw-r--r--   0        0        0     7047 1970-01-01 00:00:00.000000 dataclass_settings-0.3.0/setup.py
--rw-r--r--   0        0        0     6996 1970-01-01 00:00:00.000000 dataclass_settings-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-30 15:12:24.807372 dataclass_settings-0.3.1/LICENSE
+-rw-r--r--   0        0        0     6119 2024-04-30 15:12:24.807372 dataclass_settings-0.3.1/README.md
+-rw-r--r--   0        0        0     1904 2024-04-30 15:12:24.811372 dataclass_settings-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      246 2024-04-30 15:12:24.811372 dataclass_settings-0.3.1/src/dataclass_settings/__init__.py
+-rw-r--r--   0        0        0     3456 2024-04-30 15:12:24.811372 dataclass_settings-0.3.1/src/dataclass_settings/base.py
+-rw-r--r--   0        0        0     6518 2024-04-30 15:12:24.811372 dataclass_settings-0.3.1/src/dataclass_settings/class_inspect.py
+-rw-r--r--   0        0        0     2071 2024-04-30 15:12:24.811372 dataclass_settings-0.3.1/src/dataclass_settings/context.py
+-rw-r--r--   0        0        0     2471 2024-04-30 15:12:24.811372 dataclass_settings-0.3.1/src/dataclass_settings/loaders.py
+-rw-r--r--   0        0        0        0 2024-04-30 15:12:24.811372 dataclass_settings-0.3.1/src/dataclass_settings/py.typed
+-rw-r--r--   0        0        0     7047 1970-01-01 00:00:00.000000 dataclass_settings-0.3.1/setup.py
+-rw-r--r--   0        0        0     6996 1970-01-01 00:00:00.000000 dataclass_settings-0.3.1/PKG-INFO
```

### Comparing `dataclass_settings-0.3.0/LICENSE` & `dataclass_settings-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclass_settings-0.3.0/README.md` & `dataclass_settings-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dataclass_settings-0.3.0/pyproject.toml` & `dataclass_settings-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-settings"
-version = "0.3.0"
+version = "0.3.1"
 description = "Declarative dataclass settings."
 
 repository = "https://github.com/dancardin/dataclass-settings"
 authors = ["DanCardin <ddcardin@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 keywords = [
```

### Comparing `dataclass_settings-0.3.0/src/dataclass_settings/base.py` & `dataclass_settings-0.3.1/src/dataclass_settings/base.py`

 * *Files identical despite different names*

### Comparing `dataclass_settings-0.3.0/src/dataclass_settings/class_inspect.py` & `dataclass_settings-0.3.1/src/dataclass_settings/class_inspect.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import dataclasses
 from enum import Enum
-from typing import Any, Callable, Type
+from typing import Any, Callable, Tuple, Type
 
 import typing_inspect
 from typing_extensions import Annotated, Self, get_args, get_origin, get_type_hints
 
 from dataclass_settings.loaders import Loader
 
 __all__ = [
@@ -67,90 +67,96 @@
 class Field:
     name: str
     type: type
     annotations: tuple[Any, ...]
     mapper: Callable[..., Any] | None = None
 
     @classmethod
-    def from_dataclass(cls, typ: Type) -> list[Self]:
+    def from_dataclass(cls, typ: Type, type_hints: dict[str, Type]) -> list[Self]:
         fields = []
         for f in typ.__dataclass_fields__.values():
-            type_ = get_origin(f.type) or f.type
-            args = get_args(f.type) or ()
-            if type_ is Annotated:
-                type_, *_args = args
-                args = tuple(_args)
+            annotation = get_type(type_hints[f.name])
+
+            annotation, args = get_annotation_args(annotation)
 
             field = cls(
                 name=f.name,
-                type=type_,
+                type=annotation,
                 annotations=args,
-                mapper=type_,
+                mapper=annotation,
             )
             fields.append(field)
         return fields
 
     @classmethod
-    def from_pydantic(cls, typ: Type) -> list[Self]:
+    def from_pydantic(cls, typ: Type, type_hints: dict[str, Type]) -> list[Self]:
         fields = []
         for name, f in typ.model_fields.items():
-            annotation_type = get_type(f.annotation)
-            mapper = annotation_type if detect(annotation_type) else None
+            annotation = get_type(type_hints[name])
+            mapper = annotation if detect(annotation) else None
 
             field = cls(
                 name=name,
-                type=f.annotation,
+                type=annotation,
                 annotations=tuple(f.metadata),
                 mapper=mapper,
             )
             fields.append(field)
         return fields
 
     @classmethod
-    def from_pydantic_v1(cls, typ: Type) -> list[Self]:
+    def from_pydantic_v1(cls, typ: Type, type_hints: dict[str, Type]) -> list[Self]:
         fields = []
-        type_hints = get_type_hints(typ, include_extras=True)
         for name, f in typ.__fields__.items():
             annotation = get_type(type_hints[name])
+            annotation, args = get_annotation_args(annotation)
+
             mapper = annotation if detect(annotation) else None
 
             field = cls(
                 name=name,
-                type=f.annotation,
-                annotations=get_args(annotation) or (),
+                type=annotation,
+                annotations=args,
                 mapper=mapper,
             )
             fields.append(field)
         return fields
 
     @classmethod
-    def from_pydantic_dataclass(cls, typ: Type) -> list[Self]:
+    def from_pydantic_dataclass(
+        cls, typ: Type, type_hints: dict[str, Type]
+    ) -> list[Self]:
         fields = []
+
         for name, f in typ.__pydantic_fields__.items():
-            annotation_type = get_type(f.annotation)
-            mapper = annotation_type if detect(annotation_type) else None
+            annotation = get_type(type_hints[name])
+            mapper = annotation if detect(annotation) else None
 
             field = cls(
                 name=name,
-                type=f.annotation,
+                type=annotation,
                 annotations=tuple(f.metadata),
                 mapper=mapper,
             )
             fields.append(field)
         return fields
 
     @classmethod
-    def from_attrs(cls, typ: Type) -> list[Self]:
+    def from_attrs(cls, typ: Type, type_hints: dict[str, Type]) -> list[Self]:
         fields = []
+
         for f in typ.__attrs_attrs__:
+            annotation = get_type(type_hints[f.name])
+            annotation, args = get_annotation_args(annotation)
+
             field = cls(
                 name=f.name,
-                type=get_origin(f.type) or f.type,
-                annotations=get_args(f.type) or (),
-                mapper=f.type,
+                type=annotation,
+                annotations=args,
+                mapper=annotation,
             )
             fields.append(field)
         return fields
 
     def get_loaders(self, loaders: tuple[Type[Loader], ...]):
         for m in self.annotations:
             if isinstance(m, loaders):
@@ -185,29 +191,41 @@
             return self.mapper(value)
 
         return self.mapper(**value)
 
 
 def fields(cls: type):
     class_type = ClassTypes.from_cls(cls)
+
+    type_hints = get_type_hints(cls, include_extras=True)
     if class_type == ClassTypes.dataclass:
-        return Field.from_dataclass(cls)
+        return Field.from_dataclass(cls, type_hints)
 
     if class_type == ClassTypes.pydantic:
-        return Field.from_pydantic(cls)
+        return Field.from_pydantic(cls, type_hints)
 
     if class_type == ClassTypes.pydantic_v1:
-        return Field.from_pydantic_v1(cls)
+        return Field.from_pydantic_v1(cls, type_hints)
 
     if class_type == ClassTypes.pydantic_dataclass:
-        return Field.from_pydantic_dataclass(cls)
+        return Field.from_pydantic_dataclass(cls, type_hints)
 
     if class_type == ClassTypes.attrs:
-        return Field.from_attrs(cls)
+        return Field.from_attrs(cls, type_hints)
 
     raise NotImplementedError()  # pragma: no cover
 
 
 def get_type(typ):
     if typing_inspect.is_optional_type(typ):
         return get_args(typ)[0]
     return typ
+
+
+def get_annotation_args(annotation) -> Tuple[Type, Tuple[Any, ...]]:
+    args: Tuple[Any, ...] = ()
+    if get_origin(annotation) is Annotated:
+        args = get_args(annotation)
+        annotation, *_args = args
+        args = tuple(_args)
+
+    return annotation, args
```

### Comparing `dataclass_settings-0.3.0/src/dataclass_settings/context.py` & `dataclass_settings-0.3.1/src/dataclass_settings/context.py`

 * *Files identical despite different names*

### Comparing `dataclass_settings-0.3.0/src/dataclass_settings/loaders.py` & `dataclass_settings-0.3.1/src/dataclass_settings/loaders.py`

 * *Files identical despite different names*

### Comparing `dataclass_settings-0.3.0/setup.py` & `dataclass_settings-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['typing-extensions>=4.7.1', 'typing-inspect']
 
 setup_kwargs = {
     'name': 'dataclass-settings',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Declarative dataclass settings.',
     'long_description': '# dataclass-settings\n\n[![Actions Status](https://github.com/DanCardin/dataclass-settings/actions/workflows/test.yml/badge.svg)](https://github.com/dancardin/dataclass-settings/actions)\n[![Coverage Status](https://coveralls.io/repos/github/DanCardin/dataclass-settings/badge.svg?branch=main)](https://coveralls.io/github/DanCardin/dataclass-settings?branch=main)\n[![Documentation Status](https://readthedocs.org/projects/dataclass-settings/badge/?version=latest)](https://dataclass-settings.readthedocs.io/en/latest/?badge=latest)\n\n- [Full documentation here](https://dataclass-settings.readthedocs.io/en/latest/).\n- [Bundled Loaders](https://dataclass-settings.readthedocs.io/en/latest/loaders.html).\n\n`dataclass-settings` intends to work with any\n[PEP-681](https://peps.python.org/pep-0681/)-compliant dataclass-like object,\nincluding but not limited to:\n\n- [Pydantic models](https://pydantic-docs.helpmanual.io/) (v1/v2),\n- [dataclasses](https://docs.python.org/3/library/dataclasses.html)\n- [attrs classes](https://www.attrs.org/en/stable/).\n\n`dataclass-settings` owes its existence\n[pydantic-settings](https://github.com/pydantic/pydantic-settings), in that\npydantic-settings will be a benchmark for `dataclass-settings`\'s featureset.\nHowever it was bourne out of frustration with pydantic-setting\'s approach to\nimplementing that featureset.\n\n## Example\n\n```python\nfrom __future__ import annotations\nfrom dataclass_settings import load_settings, Env, Secret\nfrom pydantic import BaseModel\n\n\nclass Example(BaseModel):\n    env: Annotated[str, Env("ENVIRONMENT")] = "local"\n    dsn: Annotated[str, Env("DSN"), Secret(\'dsn\')] = "dsn://"\n\n    sub_config: SubConfig\n\n\nclass SubConfig(BaseModel):\n    nested: Annotated[int, Env("NESTED")] = "4"\n\n\nexample: Example = load_settings(Example)\n\n# or, if you want `nested` to be `SUB_CONFIG_NESTED`\nexample: Example = load_settings(Example, nested_delimiter=\'_\')\n```\n\n## vs Pydantic Settings\n\n### Simplicity\n\n- `pydantic-settings` alters how you go about defining your normal pydantic\n  models. You need to switch (some of the) base classes, you need to configure\n  the magical `model_config = SettingsConfigDict(...)` object, etc.\n\n  The model becomes inherently entangled with the settings-loading library.\n\n- `dataclass-settings` attaches targeted Annotations metadata to a vanilla\n  pydantic model. You can **choose** to not use `load_settings` (for example, in\n  tests), and construct the model instance however you\'d like.\n\n### Clarity\n\n- `pydantic-settings` makes it really, really difficult to intuit what the\n  concrete environment varibale that\'s going to be loaded for a given field is\n  **actually** going to be. Based on my own experience, and from perusing their\n  issue tracker, it seems like this is not an uncommon experience.\n\n  The combination of field name, `SettingsConfigDict` settings, casing,\n  `alias`/`validation_alias`/`serialization_alias`, and relative position of the\n  env var in the greater config all contribute to it being a **task** to deduce\n  which concrete name will be used when loading.\n\n- `dataclass-settings` by **default** requires an explicit, concrete name, which\n  maps directly to the value being loaded (`Env(\'FOO\')` loads `FOO`, for sure!)\n\n  If you want to opt into a less explcict, more inferred setup (like\n  pydantic-settings), you can do so by utilizing the `nested_delimiter=\'_\'` and\n  `infer_name=True` arguments.\n\n### Typing\n\n- `pydantic-settings` does not play **super** well with type checkers,\n  necessitating the use of a mypy plugin for it to not emit type errors into\n  user code.\n\n  The code recommended in their documentation for namespacing settings, looks\n  like:\n\n  ```python\n  class Settings(BaseSettings):\n      more_settings: SubModel = SubModel()\n  ```\n\n  This only type-checks with mypy (after using the plugin), but not\n  pyright/pylance. Additionally, this **actually** evaluates the `SubModel`\n  constructor during module parsing!\n\n  These issues seem(?) to be inherent to the strategy of subclassing\n  `BaseModel`, and building in its logic into the object construction process\n\n- `dataclass-settings` sidesteps this problem by decoupling the definition of\n  the settings from the loading of settings.\n\n  As such, you\'re more able to define the model, exactly as you would have with\n  vanilla pydantic:\n\n  ```python\n  class Settings(BaseModel):\n      more_settings: SubModel\n  ```\n\n  Internally, the `load_settings` function handles the work of constructing the\n  requisite input structure pydantic expects to construct the whole object tree.\n\n### Compatibility\n\n- `pydantic-settings`\'s `BaseSettings` inherits from pydantic\'s `BaseModel`. And\n  thus can only function against pydantic models, as the name would imply.\n\n- `dataclass-settings`\'s primary entrypoint is a function that accepts a\n  supportable type. As such, it can theoretically support any type that has a\n  well defined object structure, like all of `pydantic`, `dataclasses`, and\n  `attrs`.\n\n  Practically, `pydantic` has the most robust system for parsing/validating a\n  json-like structure into the models, so it\'s probably to be the most flexible\n  anyways. But for many simple cases, particuarly those without nesting, or that\n  only deal in simple types (like int, float, str, etc); then dataclasses/attrs\n  can certainly provide a similar experience.\n\n### Flexibility\n\n- At time of writing, `pydantic-settings`\'s strategy around "loaders", i.e.\n  supportable settings sources is relatively inflexible. Their issue tracker\n  contains a decent number of requests for a more flexible way of defining\n  settings priorities among different loaders, or even using different settings\n  from within a loader.\n\n  This, at least, doesn\'t seem to be an inherent issue to the library\n  necessarily. Just that at present, their API appears to try to reuse\n  pydantic\'s `Field` and `alias` mechanisms to infer the settings for all\n  loaders.\n\n- `dataclass-settings` instead annotates each field individually, with the\n  loaders that field should use. That means you can have different priorities\n  (or entirely different loaders!) per field.\n',
     'author': 'DanCardin',
     'author_email': 'ddcardin@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/dancardin/dataclass-settings',
```

### Comparing `dataclass_settings-0.3.0/PKG-INFO` & `dataclass_settings-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-settings
-Version: 0.3.0
+Version: 0.3.1
 Summary: Declarative dataclass settings.
 Home-page: https://github.com/dancardin/dataclass-settings
 License: Apache-2.0
 Keywords: dataclass,attrs,pydantic,settings
 Author: DanCardin
 Author-email: ddcardin@gmail.com
 Requires-Python: >=3.8,<4
```

