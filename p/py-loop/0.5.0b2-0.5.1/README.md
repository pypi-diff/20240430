# Comparing `tmp/py_loop-0.5.0b2.tar.gz` & `tmp/py_loop-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_loop-0.5.0b2.tar", max compression
+gzip compressed data, was "py_loop-0.5.1.tar", max compression
```

## Comparing `py_loop-0.5.0b2.tar` & `py_loop-0.5.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1057 2023-04-21 07:43:58.970714 py_loop-0.5.0b2/LICENSE
--rw-r--r--   0        0        0       51 2022-10-04 08:45:08.684461 py_loop-0.5.0b2/py_loop/__init__.py
--rw-r--r--   0        0        0     3639 2023-12-12 14:11:55.955004 py_loop-0.5.0b2/py_loop/looper.py
--rwxr-xr-x   0        0        0     1737 2023-12-12 14:11:55.955004 py_loop-0.5.0b2/py_loop/main.py
--rw-r--r--   0        0        0      528 2024-04-09 09:03:17.763668 py_loop-0.5.0b2/pyproject.toml
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 py_loop-0.5.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-04-21 07:43:58.970714 py_loop-0.5.1/LICENSE
+-rw-r--r--   0        0        0       51 2022-10-04 08:45:08.684461 py_loop-0.5.1/py_loop/__init__.py
+-rw-r--r--   0        0        0     3639 2023-12-12 14:11:55.955004 py_loop-0.5.1/py_loop/looper.py
+-rwxr-xr-x   0        0        0     1799 2024-04-30 14:27:49.862145 py_loop-0.5.1/py_loop/main.py
+-rw-r--r--   0        0        0      529 2024-04-30 14:27:49.866145 py_loop-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      462 1970-01-01 00:00:00.000000 py_loop-0.5.1/PKG-INFO
```

### Comparing `py_loop-0.5.0b2/LICENSE` & `py_loop-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_loop-0.5.0b2/py_loop/looper.py` & `py_loop-0.5.1/py_loop/looper.py`

 * *Files identical despite different names*

### Comparing `py_loop-0.5.0b2/py_loop/main.py` & `py_loop-0.5.1/py_loop/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,7 +56,11 @@
         stop_on_first_fail=args_ns.stop_on_first_fail,
         capture=(not args_ns.no_capture),
         delay=args_ns.delay,
         total_time=args_ns.total_time,
     )
     looper.loop()
     return looper
+
+
+def cli_main(args: ArgsList = None) -> None:
+    main(args)
```

### Comparing `py_loop-0.5.0b2/pyproject.toml` & `py_loop-0.5.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "py-loop"
-version = "0.5.0b2"
+version = "0.5.1"
 description = "Run commands until it fails"
 authors = ["jerem <jeremy.tellaa@tanker.io>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 cli-ui = "^0.17.2"
 
 [tool.poetry.group.dev.dependencies]
-twine = "^4.0.2"
-black = "23.12.1"
+twine = "^5.0.0"
+black = "24.3.0"
 codecov = "^2.1.13"
-flake8 = "6.1.0"
-mypy = "1.8.0"
-pytest = "^7.4.3"
-pytest-cov = "^4.1.0"
+flake8 = "7.0.0"
+mypy = "1.9.0"
+pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
 isort = "^5.13.2"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry.scripts]
-looper = 'py_loop.main:main'
+looper = 'py_loop.main:cli_main'
```

