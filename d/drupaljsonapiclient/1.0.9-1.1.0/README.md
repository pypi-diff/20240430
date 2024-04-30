# Comparing `tmp/drupaljsonapiclient-1.0.9.tar.gz` & `tmp/drupaljsonapiclient-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drupaljsonapiclient-1.0.9.tar", max compression
+gzip compressed data, was "drupaljsonapiclient-1.1.0.tar", max compression
```

## Comparing `drupaljsonapiclient-1.0.9.tar` & `drupaljsonapiclient-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1690 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/LICENSE
--rw-r--r--   0        0        0     1244 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/README.md
--rw-r--r--   0        0        0      156 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/drupaljsonapiclient/__init__.py
--rw-r--r--   0        0        0     3605 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/drupaljsonapiclient/common.py
--rw-r--r--   0        0        0     4383 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/drupaljsonapiclient/document.py
--rw-r--r--   0        0        0      620 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/drupaljsonapiclient/exceptions.py
--rw-r--r--   0        0        0     3145 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/drupaljsonapiclient/filter.py
--rw-r--r--   0        0        0     4283 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/drupaljsonapiclient/objects.py
--rw-r--r--   0        0        0    14266 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/drupaljsonapiclient/relationships.py
--rw-r--r--   0        0        0    26615 2023-07-03 15:57:46.902012 drupaljsonapiclient-1.0.9/drupaljsonapiclient/resourceobject.py
--rw-r--r--   0        0        0    28123 2023-07-03 15:57:46.903012 drupaljsonapiclient-1.0.9/drupaljsonapiclient/session.py
--rw-r--r--   0        0        0     1066 2023-07-03 15:57:46.904012 drupaljsonapiclient-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     2164 1970-01-01 00:00:00.000000 drupaljsonapiclient-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1690 2024-04-30 20:24:31.474417 drupaljsonapiclient-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1244 2024-04-30 20:24:31.474417 drupaljsonapiclient-1.1.0/README.md
+-rw-r--r--   0        0        0      156 2024-04-30 20:24:31.474417 drupaljsonapiclient-1.1.0/drupaljsonapiclient/__init__.py
+-rw-r--r--   0        0        0     3165 2024-04-30 20:24:31.474417 drupaljsonapiclient-1.1.0/drupaljsonapiclient/common.py
+-rw-r--r--   0        0        0     4383 2024-04-30 20:24:31.474417 drupaljsonapiclient-1.1.0/drupaljsonapiclient/document.py
+-rw-r--r--   0        0        0      620 2024-04-30 20:24:31.474417 drupaljsonapiclient-1.1.0/drupaljsonapiclient/exceptions.py
+-rw-r--r--   0        0        0     3145 2024-04-30 20:24:31.474417 drupaljsonapiclient-1.1.0/drupaljsonapiclient/filter.py
+-rw-r--r--   0        0        0     4235 2024-04-30 20:24:31.475417 drupaljsonapiclient-1.1.0/drupaljsonapiclient/objects.py
+-rw-r--r--   0        0        0    14266 2024-04-30 20:24:31.475417 drupaljsonapiclient-1.1.0/drupaljsonapiclient/relationships.py
+-rw-r--r--   0        0        0    26438 2024-04-30 20:24:31.475417 drupaljsonapiclient-1.1.0/drupaljsonapiclient/resourceobject.py
+-rw-r--r--   0        0        0    28075 2024-04-30 20:24:31.475417 drupaljsonapiclient-1.1.0/drupaljsonapiclient/session.py
+-rw-r--r--   0        0        0     1155 2024-04-30 20:24:31.476417 drupaljsonapiclient-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 drupaljsonapiclient-1.1.0/PKG-INFO
```

### Comparing `drupaljsonapiclient-1.0.9/LICENSE` & `drupaljsonapiclient-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.9/README.md` & `drupaljsonapiclient-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.9/drupaljsonapiclient/common.py` & `drupaljsonapiclient-1.1.0/drupaljsonapiclient/common.py`

 * *Files 15% similar despite different names*

```diff
@@ -69,32 +69,14 @@
     try:
         error_str = response_content['errors'][0]['title']
     except Exception:
         error_str = '?'
     return error_str
 
 
-def jsonify_attribute_name(name):
-    return name.replace('__', '.').replace('_', '-')
-
-
-def dejsonify_attribute_name(name):
-    return name.replace('.', '__').replace('-', '_')
-
-
-def jsonify_attribute_names(iterable):
-    for i in iterable:
-        yield jsonify_attribute_name(i)
-
-
-def dejsonify_attribute_names(iterable):
-    for i in iterable:
-        yield dejsonify_attribute_name(i)
-
-
 async def execute_async(func, *args):
     """Shortcut to asynchronize normal blocking function"""
     loop = asyncio.get_event_loop()
     return await loop.run_in_executor(None, func, *args)
 
 
 class cached_property(object):
@@ -130,23 +112,23 @@
         return self._target_object[item]
 
     def __setitem__(self, key, value):
         self._target_object[key] = value
 
     def __getattr__(self, item):
         try:
-            return self[jsonify_attribute_name(item)]
+            return self[item]
         except KeyError:
             raise AttributeError
 
     def __setattr__(self, key, value):
         if key == '_target_object':
             return super().__setattr__(key, value)
         try:
-            self[jsonify_attribute_name(key)] = value
+            self[key] = value
         except KeyError:
             raise AttributeError
 
 
 class ResourceTuple(NamedTuple):
     id: str
     type: str
```

### Comparing `drupaljsonapiclient-1.0.9/drupaljsonapiclient/document.py` & `drupaljsonapiclient-1.1.0/drupaljsonapiclient/document.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.9/drupaljsonapiclient/exceptions.py` & `drupaljsonapiclient-1.1.0/drupaljsonapiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.9/drupaljsonapiclient/filter.py` & `drupaljsonapiclient-1.1.0/drupaljsonapiclient/filter.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.9/drupaljsonapiclient/objects.py` & `drupaljsonapiclient-1.1.0/drupaljsonapiclient/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from itertools import chain
 from typing import Optional, Union, Awaitable, TYPE_CHECKING
 from urllib.parse import urlparse
 
-from .common import AbstractJsonObject, jsonify_attribute_name, ResourceTuple
+from .common import AbstractJsonObject, ResourceTuple
 from .resourceobject import ResourceObject
 
 if TYPE_CHECKING:
     from .document import Document
 
 logger = logging.getLogger(__name__)
 
@@ -18,15 +18,15 @@
 
     http://jsonapi.org/format/#document-meta
     """
     def _handle_data(self, data):
         self.meta = data
 
     def __getattr__(self, name):
-        return self.meta.get(jsonify_attribute_name(name))
+        return self.meta.get(name)
 
     def __getitem__(self, name):
         return self.meta.get(name)
 
     def __str__(self):
         return str(self.meta)
```

### Comparing `drupaljsonapiclient-1.0.9/drupaljsonapiclient/relationships.py` & `drupaljsonapiclient-1.1.0/drupaljsonapiclient/relationships.py`

 * *Files identical despite different names*

### Comparing `drupaljsonapiclient-1.0.9/drupaljsonapiclient/resourceobject.py` & `drupaljsonapiclient-1.1.0/drupaljsonapiclient/resourceobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from itertools import chain
 from typing import Set, Optional, Awaitable, Union, Iterable, TYPE_CHECKING, List, IO
 
 from urllib.parse import urlparse, urljoin
 
-from .common import (jsonify_attribute_name, AbstractJsonObject,
-                     dejsonify_attribute_names, HttpMethod, HttpStatus, AttributeProxy,
+from .common import (AbstractJsonObject,
+                     HttpMethod, HttpStatus, AttributeProxy,
                      cached_property, RelationType)
 from .exceptions import ValidationError, DocumentInvalid
 
 NOT_FOUND = object()
 
 logger = logging.getLogger(__name__)
 
@@ -88,37 +88,37 @@
     def create_map(self, attr_name):
         """
         Create a new map of values (i.e. child AttributeDict) within this AttributeDict
 
         :param attr_name: Name of this map object.
         """
         self._check_invalid()
-        name = jsonify_attribute_name(attr_name)
+        name = attr_name
         self[name] = AttributeDict(data={}, name=name, parent=self, resource=self._resource)
 
     def _check_invalid(self):
         if self._invalid:
             raise DocumentInvalid('Resource has been invalidated.')
 
     def __getattr__(self, name):
-        name = jsonify_attribute_name(name)
+        name = name
         if name not in self:
             raise AttributeError(f'No such attribute '
                                  f'{self._resource.type}.{self._full_name}.{name}')
         return self[name]
 
     def __setitem__(self, key, value):
         if self.get(key) != value:
             self.mark_dirty(key)
         super().__setitem__(key, value)
 
     def __setattr__(self, name, value):
         if name.startswith('_'):
             return super().__setattr__(name, value)
-        name = jsonify_attribute_name(name)
+        name = name
         self[name] = value
 
     def mark_dirty(self, name: str):
         """
         Mark one attribute within this dictionary as dirty.
 
         :param name: Name of the attribute that is to be marked as dirty.
@@ -192,15 +192,15 @@
             if isinstance(value, AttributeDict):
                 value.change_resource(new_resource)
 
     def keys_python(self) -> Iterable[str]:
         """
         Pythonized version of contained keys (attribute names).
         """
-        yield from dejsonify_attribute_names(self.keys())
+        yield from self.keys()
 
 
 class RelationshipDict(dict):
     """
     Container for relationships that is stored in ResourceObject
     """
 
@@ -290,15 +290,15 @@
         for attr in self.values():
             attr.mark_clean()
 
     def keys_python(self) -> Iterable[str]:
         """
         Pythonized version of contained keys (relationship names)
         """
-        yield from dejsonify_attribute_names(self.keys())
+        yield from self.keys()
 
     @property
     def is_dirty(self) -> bool:
         return any(r.is_dirty for r in self.values())
 
 
 class ResourceObject(AbstractJsonObject):
```

### Comparing `drupaljsonapiclient-1.0.9/drupaljsonapiclient/session.py` & `drupaljsonapiclient-1.1.0/drupaljsonapiclient/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 )
 from urllib.parse import ParseResult, urlparse
 
 from pathlib import Path
 
 import jsonschema
 
-from .common import jsonify_attribute_name, error_from_response, \
+from .common import error_from_response, \
     HttpStatus, HttpMethod
 from .exceptions import DocumentError, AsyncError
 
 if TYPE_CHECKING:
     from asyncio import AbstractEventLoop
     from .objects import ResourceIdentifier
     from .document import Document
@@ -178,15 +178,15 @@
         attrs: dict = {}
         rels: dict = {}
         schema = self.schema.schema_for_model(_type)
         more_fields.update(fields)
 
         for key, value in more_fields.items():
             if key not in fields:
-                key = jsonify_attribute_name(key)
+                key = key
             props = schema['properties'].get(key, {})
             if 'relation' in props:
                 res_types = props.get('resource', [])
                 if isinstance(value, RESOURCE_TYPES + (str,)):
                     value = self._value_to_dict(value, res_types)
                 elif isinstance(value, collections.abc.Iterable):
                     value = [self._value_to_dict(id_, res_types) for id_ in value]
```

### Comparing `drupaljsonapiclient-1.0.9/pyproject.toml` & `drupaljsonapiclient-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 [tool.poetry]
 name = "drupaljsonapiclient"
-version = "1.0.9"
+version = "1.1.0"
 description = "Drupal CMS JSON:API client for Python."
 authors = ["Martins Bruvelis <martins.bruvelis@gmail.com>"]
 readme = "README.md"
 packages = [{include = "drupaljsonapiclient"}]
 repository = "https://gitlab.com/martins-bruvelis/drupaljsonapiclient"
 documentation = "https://gitlab.com/martins-bruvelis/drupaljsonapiclient/-/blob/main/README.md"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.12"
 requests = "^2.31.0"
-jsonschema = "^4.17.3"
-aiohttp = {version = "^3.8.4", optional = true}
-aiofiles = {version = "^23.1.0", optional = true}
+jsonschema = "^4.22.0"
+aiohttp = {version = "^3.9.5", optional = true}
+aiofiles = {version = "^23.2.1", optional = true}
 
+[tool.poetry.extras]
+async = ["aiohttp", "aiofiles"]
 
 [tool.poetry.group.dev.dependencies]
-jupyterlab = "^4.0.2"
-ipywidgets = "^8.0.6"
-plotly = "^5.15.0"
+jupyterlab = "^4.1.8"
+ipywidgets = "^8.1.2"
+plotly = "^5.21.0"
 jupyter-dash = "^0.4.2"
 jupyterlab-hdf = "^1.3.0"
 nest-asyncio = "^1.5.6"
-tqdm = "^4.65.0"
-solara = "^1.16.2"
-matplotlib = "^3.7.1"
+tqdm = "^4.66.2"
+solara = "^1.32.0"
+matplotlib = "^3.8.4"
 tabulate = "^0.9.0"
-flatjsondict = "^1.0.3"
-pandas = "^2.0.2"
-pyjanitor = "^0.24.0"
-gspread = "^5.9.0"
+flatjsondict = "^1.2.2"
+pandas = "^2.2.2"
+pyjanitor = "^0.27.0"
+gspread = "^6.1.0"
 gspread-pandas = "^3.2.2"
-jsonmerge = "^1.9.0"
+jsonmerge = "^1.9.2"
+jupyter = "^1.0.0"
+nest = "^0.4.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `drupaljsonapiclient-1.0.9/PKG-INFO` & `drupaljsonapiclient-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: drupaljsonapiclient
-Version: 1.0.9
+Version: 1.1.0
 Summary: Drupal CMS JSON:API client for Python.
 Home-page: https://gitlab.com/martins-bruvelis/drupaljsonapiclient
 Author: Martins Bruvelis
 Author-email: martins.bruvelis@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: async
+Requires-Dist: aiofiles (>=23.2.1,<24.0.0) ; extra == "async"
+Requires-Dist: aiohttp (>=3.9.5,<4.0.0) ; extra == "async"
+Requires-Dist: jsonschema (>=4.22.0,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Documentation, https://gitlab.com/martins-bruvelis/drupaljsonapiclient/-/blob/main/README.md
 Project-URL: Repository, https://gitlab.com/martins-bruvelis/drupaljsonapiclient
 Description-Content-Type: text/markdown
 
 # drupaljsonapiclient: Drupal CMS JSON:API client for Python
```

