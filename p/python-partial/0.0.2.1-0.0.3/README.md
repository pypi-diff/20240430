# Comparing `tmp/python_partial-0.0.2.1.tar.gz` & `tmp/python_partial-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_partial-0.0.2.1.tar", max compression
+gzip compressed data, was "python_partial-0.0.3.tar", max compression
```

## Comparing `python_partial-0.0.2.1.tar` & `python_partial-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_partial-0.0.2.1/LICENSE
--rw-r--r--   0        0        0      185 2024-04-22 16:11:25.751372 python_partial-0.0.2.1/partial/__init__.py
--rw-r--r--   0        0        0     5113 2024-04-24 16:00:15.673641 python_partial-0.0.2.1/partial/partial.py
--rwxr-xr-x   0        0        0      849 2024-04-22 15:23:50.704838 python_partial-0.0.2.1/partial/placeholder.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_partial-0.0.2.1/partial/py.typed
--rw-r--r--   0        0        0     1176 2024-04-24 16:01:54.562788 python_partial-0.0.2.1/pyproject.toml
--rw-r--r--   0        0        0      212 2024-04-22 15:32:04.972596 python_partial-0.0.2.1/readme.md
--rw-r--r--   0        0        0     1376 1970-01-01 00:00:00.000000 python_partial-0.0.2.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_partial-0.0.3/LICENSE
+-rw-r--r--   0        0        0      185 2024-04-29 15:21:28.593758 python_partial-0.0.3/partial/__init__.py
+-rw-r--r--   0        0        0     5546 2024-04-29 15:22:33.713972 python_partial-0.0.3/partial/partial.py
+-rwxr-xr-x   0        0        0      849 2024-04-22 15:23:50.704838 python_partial-0.0.3/partial/placeholder.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_partial-0.0.3/partial/py.typed
+-rw-r--r--   0        0        0     1174 2024-04-29 15:22:47.630833 python_partial-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      212 2024-04-22 15:32:04.972596 python_partial-0.0.3/readme.md
+-rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 python_partial-0.0.3/PKG-INFO
```

### Comparing `python_partial-0.0.2.1/LICENSE` & `python_partial-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_partial-0.0.2.1/partial/partial.py` & `python_partial-0.0.3/partial/partial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # /usr/bin/env python3
 # coding: utf-8
 
 __author__  = "ChenyangGao <https://chenyanggao.github.io>"
 __all__ = ["partial", "ppartial", "skippartial"]
 
 from collections.abc import Callable, Iterable, Sequence
-from functools import partial, update_wrapper
-from inspect import signature, BoundArguments
+from functools import cached_property, partial, update_wrapper
+from inspect import signature, BoundArguments, Signature
 from itertools import chain
 
 from undefined import undefined
 from .placeholder import _
 
 
 def _exist_placeholder(args: Iterable) -> bool:
@@ -50,14 +50,24 @@
     def wrap(cls, func: Callable, /) -> Callable:
         def wrapper(*args, **kwargs):
             if _exist_placeholder(args) or _exist_placeholder(kwargs.values()):
                 return cls(func, *args, **kwargs)
             return func(*args, **kwargs)
         return update_wrapper(wrapper, func)
 
+    @cached_property
+    def __signature__(self, /) -> Signature:
+        bound_args = signature(self.func).bind_partial(*self.args, **self.keywords)
+        arguments = bound_args.arguments
+        return Signature([
+            param.replace(default=arguments[key]) 
+            if key in arguments else param 
+            for key, param in bound_args.signature.parameters.items()
+        ])
+
 
 class skippartial(partial):
     skip: int | Sequence[int]
 
     def __new__(
         cls, 
         skip: int | Iterable[int],
```

### Comparing `python_partial-0.0.2.1/partial/placeholder.py` & `python_partial-0.0.3/partial/placeholder.py`

 * *Files identical despite different names*

### Comparing `python_partial-0.0.2.1/pyproject.toml` & `python_partial-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-partial"
-version = "0.0.2.1"
+version = "0.0.3"
 description = "Python partial types."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-partial"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-partial"
 keywords = ["file", "reverse", "iter"]
```

### Comparing `python_partial-0.0.2.1/PKG-INFO` & `python_partial-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-partial
-Version: 0.0.2.1
+Version: 0.0.3
 Summary: Python partial types.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-partial
 License: MIT
 Keywords: file,reverse,iter
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

