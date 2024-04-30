# Comparing `tmp/python_decorator-0.0.1.3.tar.gz` & `tmp/python_decorator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_decorator-0.0.1.3.tar", max compression
+gzip compressed data, was "python_decorator-0.0.2.tar", max compression
```

## Comparing `python_decorator-0.0.1.3.tar` & `python_decorator-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_decorator-0.0.1.3/LICENSE
--rwxr-xr-x   0        0        0     8754 2024-04-30 12:32:44.935851 python_decorator-0.0.1.3/decorator0/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_decorator-0.0.1.3/decorator0/py.typed
--rw-r--r--   0        0        0     1206 2024-04-30 12:33:41.653421 python_decorator-0.0.1.3/pyproject.toml
--rw-r--r--   0        0        0      201 2024-04-24 15:56:16.540240 python_decorator-0.0.1.3/readme.md
--rw-r--r--   0        0        0     1401 1970-01-01 00:00:00.000000 python_decorator-0.0.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_decorator-0.0.2/LICENSE
+-rwxr-xr-x   0        0        0     8754 2024-04-30 13:16:34.567545 python_decorator-0.0.2/decorator0/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_decorator-0.0.2/decorator0/py.typed
+-rwxr-xr-x   0        0        0     2527 2024-04-30 13:16:09.363535 python_decorator-0.0.2/decorator0/util.py
+-rw-r--r--   0        0        0     1204 2024-04-30 13:16:24.878498 python_decorator-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      201 2024-04-24 15:56:16.540240 python_decorator-0.0.2/readme.md
+-rw-r--r--   0        0        0     1399 1970-01-01 00:00:00.000000 python_decorator-0.0.2/PKG-INFO
```

### Comparing `python_decorator-0.0.1.3/LICENSE` & `python_decorator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_decorator-0.0.1.3/decorator0/__init__.py` & `python_decorator-0.0.2/decorator0/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding: utf-8
 
 """This module provides some decorators to decorate other 
 decorators, in order to simplify some boilerplate code.
 """
 
 __author__  = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 1)
+__version__ = (0, 0, 2)
 __all__ = ["decorated", "optional", "optional_args", "currying", "partialize"]
 
 from collections.abc import Callable
 from functools import partial, reduce, update_wrapper
 from inspect import signature
 from typing import cast, overload, Any, Concatenate, Optional, ParamSpec, TypeVar
```

### Comparing `python_decorator-0.0.1.3/pyproject.toml` & `python_decorator-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-decorator"
-version = "0.0.1.3"
+version = "0.0.2"
 description = "Python argument type."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decorator"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decorator"
 keywords = ["file", "reverse", "iter"]
```

### Comparing `python_decorator-0.0.1.3/PKG-INFO` & `python_decorator-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-decorator
-Version: 0.0.1.3
+Version: 0.0.2
 Summary: Python argument type.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-decorator
 License: MIT
 Keywords: file,reverse,iter
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

