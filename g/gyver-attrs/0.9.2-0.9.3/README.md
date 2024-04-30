# Comparing `tmp/gyver_attrs-0.9.2.tar.gz` & `tmp/gyver_attrs-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gyver_attrs-0.9.2.tar", max compression
+gzip compressed data, was "gyver_attrs-0.9.3.tar", max compression
```

## Comparing `gyver_attrs-0.9.2.tar` & `gyver_attrs-0.9.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11352 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/LICENSE
--rw-r--r--   0        0        0     5279 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/README.md
--rw-r--r--   0        0        0       80 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/gyver/__init__.py
--rw-r--r--   0        0        0      721 2024-04-24 16:51:22.740497 gyver_attrs-0.9.2/gyver/attrs/__init__.py
--rw-r--r--   0        0        0     3508 2024-04-16 17:07:30.546888 gyver_attrs-0.9.2/gyver/attrs/camel.py
--rw-r--r--   0        0        0      146 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/gyver/attrs/converters/__init__.py
--rw-r--r--   0        0        0      751 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/gyver/attrs/converters/json.py
--rw-r--r--   0        0        0     1463 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/gyver/attrs/converters/utils.py
--rw-r--r--   0        0        0     9316 2024-04-17 01:24:16.620998 gyver_attrs-0.9.2/gyver/attrs/field.py
--rw-r--r--   0        0        0     6142 2024-04-17 01:24:16.620998 gyver_attrs-0.9.2/gyver/attrs/helpers.py
--rw-r--r--   0        0        0    29147 2024-04-17 01:24:16.620998 gyver_attrs-0.9.2/gyver/attrs/main.py
--rw-r--r--   0        0        0     5072 2024-04-17 01:24:16.620998 gyver_attrs-0.9.2/gyver/attrs/methods.py
--rw-r--r--   0        0        0        0 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/gyver/attrs/py.typed
--rw-r--r--   0        0        0     4348 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/gyver/attrs/resolver.py
--rw-r--r--   0        0        0     4032 2024-04-17 01:24:16.620998 gyver_attrs-0.9.2/gyver/attrs/schema.py
--rw-r--r--   0        0        0     5653 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/gyver/attrs/shortcuts.py
--rw-r--r--   0        0        0        0 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/gyver/attrs/utils/__init__.py
--rw-r--r--   0        0        0      847 2024-04-24 16:43:28.681989 gyver_attrs-0.9.2/gyver/attrs/utils/factory.py
--rw-r--r--   0        0        0     5797 2024-04-16 17:06:15.778349 gyver_attrs-0.9.2/gyver/attrs/utils/functions.py
--rw-r--r--   0        0        0      641 2024-03-28 22:15:25.253687 gyver_attrs-0.9.2/gyver/attrs/utils/typedef.py
--rw-r--r--   0        0        0     1149 2024-04-24 16:51:22.747164 gyver_attrs-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     5920 1970-01-01 00:00:00.000000 gyver_attrs-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11352 2024-03-28 22:15:25.253687 gyver_attrs-0.9.3/LICENSE
+-rw-r--r--   0        0        0     5279 2024-03-28 22:15:25.253687 gyver_attrs-0.9.3/README.md
+-rw-r--r--   0        0        0       80 2024-03-28 22:15:25.253687 gyver_attrs-0.9.3/gyver/__init__.py
+-rw-r--r--   0        0        0      882 2024-04-30 02:15:31.948773 gyver_attrs-0.9.3/gyver/attrs/__init__.py
+-rw-r--r--   0        0        0     3508 2024-04-16 17:07:30.546888 gyver_attrs-0.9.3/gyver/attrs/camel.py
+-rw-r--r--   0        0        0      146 2024-03-28 22:15:25.253687 gyver_attrs-0.9.3/gyver/attrs/converters/__init__.py
+-rw-r--r--   0        0        0      751 2024-03-28 22:15:25.253687 gyver_attrs-0.9.3/gyver/attrs/converters/json.py
+-rw-r--r--   0        0        0     1463 2024-03-28 22:15:25.253687 gyver_attrs-0.9.3/gyver/attrs/converters/utils.py
+-rw-r--r--   0        0        0     9316 2024-04-24 16:56:24.121528 gyver_attrs-0.9.3/gyver/attrs/field.py
+-rw-r--r--   0        0        0     6255 2024-04-30 02:13:40.966035 gyver_attrs-0.9.3/gyver/attrs/helpers.py
+-rw-r--r--   0        0        0    29147 2024-04-17 01:24:16.620998 gyver_attrs-0.9.3/gyver/attrs/main.py
+-rw-r--r--   0        0        0     5072 2024-04-17 01:24:16.620998 gyver_attrs-0.9.3/gyver/attrs/methods.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:15:25.253687 gyver_attrs-0.9.3/gyver/attrs/py.typed
+-rw-r--r--   0        0        0     4348 2024-03-28 22:15:25.253687 gyver_attrs-0.9.3/gyver/attrs/resolver.py
+-rw-r--r--   0        0        0     4032 2024-04-17 01:24:16.620998 gyver_attrs-0.9.3/gyver/attrs/schema.py
+-rw-r--r--   0        0        0     5653 2024-03-28 22:15:25.253687 gyver_attrs-0.9.3/gyver/attrs/shortcuts.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:15:25.253687 gyver_attrs-0.9.3/gyver/attrs/utils/__init__.py
+-rw-r--r--   0        0        0      847 2024-04-24 16:43:28.681989 gyver_attrs-0.9.3/gyver/attrs/utils/factory.py
+-rw-r--r--   0        0        0     5797 2024-04-16 17:06:15.778349 gyver_attrs-0.9.3/gyver/attrs/utils/functions.py
+-rw-r--r--   0        0        0      641 2024-03-28 22:15:25.253687 gyver_attrs-0.9.3/gyver/attrs/utils/typedef.py
+-rw-r--r--   0        0        0     1149 2024-04-30 02:15:31.955440 gyver_attrs-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     5920 1970-01-01 00:00:00.000000 gyver_attrs-0.9.3/PKG-INFO
```

### Comparing `gyver_attrs-0.9.2/LICENSE` & `gyver_attrs-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.2/README.md` & `gyver_attrs-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.2/gyver/attrs/camel.py` & `gyver_attrs-0.9.3/gyver/attrs/camel.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.2/gyver/attrs/converters/json.py` & `gyver_attrs-0.9.3/gyver/attrs/converters/json.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.2/gyver/attrs/converters/utils.py` & `gyver_attrs-0.9.3/gyver/attrs/converters/utils.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.2/gyver/attrs/field.py` & `gyver_attrs-0.9.3/gyver/attrs/field.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.2/gyver/attrs/helpers.py` & `gyver_attrs-0.9.3/gyver/attrs/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,24 @@
 from .utils.functions import disassemble_type, get_forwardrefs, rebuild_type_from_depth
 
 T = TypeVar('T')
 R = TypeVar('R')
 P = ParamSpec('P')
 
 
+def is_gattrs_defined(instance_or_klass: Union[type, object]):
+    return hasattr(instance_or_klass, '__gyver_attrs__')
+
+
 def validate_type(
     func: Callable[Concatenate[T, P], R],
 ) -> Callable[Concatenate[T, P], R]:
     @wraps(func)
     def inner(obj: T, *args: P.args, **kwargs: P.kwargs) -> R:
-        if not hasattr(obj, '__gyver_attrs__'):
+        if not is_gattrs_defined(obj):
             raise TypeError(f'Type {obj} is not defined by gyver-attrs', obj)
         return func(obj, *args, **kwargs)
 
     return inner
 
 
 @validate_type
```

### Comparing `gyver_attrs-0.9.2/gyver/attrs/main.py` & `gyver_attrs-0.9.3/gyver/attrs/main.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.2/gyver/attrs/methods.py` & `gyver_attrs-0.9.3/gyver/attrs/methods.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.2/gyver/attrs/resolver.py` & `gyver_attrs-0.9.3/gyver/attrs/resolver.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.2/gyver/attrs/schema.py` & `gyver_attrs-0.9.3/gyver/attrs/schema.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.2/gyver/attrs/shortcuts.py` & `gyver_attrs-0.9.3/gyver/attrs/shortcuts.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.2/gyver/attrs/utils/factory.py` & `gyver_attrs-0.9.3/gyver/attrs/utils/factory.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.2/gyver/attrs/utils/functions.py` & `gyver_attrs-0.9.3/gyver/attrs/utils/functions.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.2/gyver/attrs/utils/typedef.py` & `gyver_attrs-0.9.3/gyver/attrs/utils/typedef.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.2/pyproject.toml` & `gyver_attrs-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gyver-attrs"
-version = "0.9.2"
+version = "0.9.3"
 description = ""
 authors = ["Gustavo Cardoso <self.gustavocorrea@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "gyver" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gyver_attrs-0.9.2/PKG-INFO` & `gyver_attrs-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gyver-attrs
-Version: 0.9.2
+Version: 0.9.3
 Summary: 
 Author: Gustavo Cardoso
 Author-email: self.gustavocorrea@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

