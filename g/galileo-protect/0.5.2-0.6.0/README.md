# Comparing `tmp/galileo_protect-0.5.2.tar.gz` & `tmp/galileo_protect-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galileo_protect-0.5.2.tar", max compression
+gzip compressed data, was "galileo_protect-0.6.0.tar", max compression
```

## Comparing `galileo_protect-0.5.2.tar` & `galileo_protect-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0    10946 2024-04-16 19:24:12.362363 galileo_protect-0.5.2/LICENSE
--rw-r--r--   0        0        0      118 2024-04-16 19:24:12.362363 galileo_protect-0.5.2/README.md
--rw-r--r--   0        0        0     2529 2024-04-16 19:24:13.258363 galileo_protect-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      422 2024-04-16 19:24:13.258363 galileo_protect-0.5.2/src/galileo_protect/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 19:24:12.362363 galileo_protect-0.5.2/src/galileo_protect/constants/__init__.py
--rw-r--r--   0        0        0      324 2024-04-16 19:24:12.362363 galileo_protect-0.5.2/src/galileo_protect/constants/routes.py
--rw-r--r--   0        0        0        0 2024-04-16 19:24:12.362363 galileo_protect-0.5.2/src/galileo_protect/helpers/__init__.py
--rw-r--r--   0        0        0      530 2024-04-16 19:24:12.362363 galileo_protect-0.5.2/src/galileo_protect/helpers/config.py
--rw-r--r--   0        0        0     1403 2024-04-16 19:24:12.362363 galileo_protect-0.5.2/src/galileo_protect/invoke.py
--rw-r--r--   0        0        0      638 2024-04-16 19:24:12.362363 galileo_protect-0.5.2/src/galileo_protect/project.py
--rw-r--r--   0        0        0      665 2024-04-16 19:24:12.362363 galileo_protect-0.5.2/src/galileo_protect/schemas/__init__.py
--rw-r--r--   0        0        0      212 2024-04-16 19:24:12.362363 galileo_protect-0.5.2/src/galileo_protect/schemas/invoke.py
--rw-r--r--   0        0        0      308 2024-04-16 19:24:12.362363 galileo_protect-0.5.2/src/galileo_protect/schemas/rule.py
--rw-r--r--   0        0        0      124 2024-04-16 19:24:12.362363 galileo_protect-0.5.2/src/galileo_protect/schemas/stage.py
--rw-r--r--   0        0        0     3529 2024-04-16 19:24:12.362363 galileo_protect-0.5.2/src/galileo_protect/stage.py
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 galileo_protect-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    10946 2024-04-30 02:12:57.377982 galileo_protect-0.6.0/LICENSE
+-rw-r--r--   0        0        0      118 2024-04-30 02:12:57.377982 galileo_protect-0.6.0/README.md
+-rw-r--r--   0        0        0     2583 2024-04-30 02:12:58.273980 galileo_protect-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      431 2024-04-30 02:12:58.273980 galileo_protect-0.6.0/src/galileo_protect/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 02:12:57.377982 galileo_protect-0.6.0/src/galileo_protect/constants/__init__.py
+-rw-r--r--   0        0        0       80 2024-04-30 02:12:57.377982 galileo_protect-0.6.0/src/galileo_protect/constants/invoke.py
+-rw-r--r--   0        0        0      324 2024-04-30 02:12:57.377982 galileo_protect-0.6.0/src/galileo_protect/constants/routes.py
+-rw-r--r--   0        0        0        0 2024-04-30 02:12:57.377982 galileo_protect-0.6.0/src/galileo_protect/helpers/__init__.py
+-rw-r--r--   0        0        0      530 2024-04-30 02:12:57.377982 galileo_protect-0.6.0/src/galileo_protect/helpers/config.py
+-rw-r--r--   0        0        0     2088 2024-04-30 02:12:57.377982 galileo_protect-0.6.0/src/galileo_protect/invoke.py
+-rw-r--r--   0        0        0      638 2024-04-30 02:12:57.377982 galileo_protect-0.6.0/src/galileo_protect/project.py
+-rw-r--r--   0        0        0      665 2024-04-30 02:12:57.381982 galileo_protect-0.6.0/src/galileo_protect/schemas/__init__.py
+-rw-r--r--   0        0        0      212 2024-04-30 02:12:57.381982 galileo_protect-0.6.0/src/galileo_protect/schemas/invoke.py
+-rw-r--r--   0        0        0      308 2024-04-30 02:12:57.381982 galileo_protect-0.6.0/src/galileo_protect/schemas/rule.py
+-rw-r--r--   0        0        0      124 2024-04-30 02:12:57.381982 galileo_protect-0.6.0/src/galileo_protect/schemas/stage.py
+-rw-r--r--   0        0        0     3529 2024-04-30 02:12:57.381982 galileo_protect-0.6.0/src/galileo_protect/stage.py
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 galileo_protect-0.6.0/PKG-INFO
```

### Comparing `galileo_protect-0.5.2/LICENSE` & `galileo_protect-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.5.2/pyproject.toml` & `galileo_protect-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "galileo-protect"
-version = "0.5.2"
+version = "0.6.0"
 description = "🛡️ Secure your Generative AI applications with Galileo Protect!"
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 packages = [{include = "galileo_protect", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<3.13"
@@ -14,28 +14,29 @@
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 coverage = "^7.3.4"
 pytest-cov = "^5.0.0"
 pytest-xdist = "^3.5.0"
 pytest-socket = "^0.7.0"
 requests-mock = "^1.12.1"
+pytest-asyncio = "^0.23.6"
 
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.8.0"
 pre-commit = "^3.5.0"
 invoke = "^2.2.0"
 types-requests = "^2.31.0.20240406"
 pydantic = { extras = ["mypy"], version = "^2.6.0" }
 
 
 [tool.poetry.group.docs.dependencies]
 furo = "^2024.0.0"
 sphinx-autodoc-typehints = "^2.0.0"
-myst-parser = "^2.0.0"
+myst-parser = "^3.0.1"
 sphinx-markdown-builder = "^0.6.5"
 sphinx-autobuild = "^2021.3.14"
 autodoc-pydantic = "^2.0.1"
 
 
 [build-system]
 requires = ["poetry-core"]
@@ -56,14 +57,15 @@
     "console_output_style=progress",
     # Disable warnings.
     "--disable-warnings",
     # Show slowest 10 test durations.
     "--durations=10",
     # Disable internet access.
     "--disable-socket",
+    "--allow-unix-socket",
 ]
 
 # Formatters.
 [tool.black]
 line-length = 120
 
 [tool.isort]
```

### Comparing `galileo_protect-0.5.2/src/galileo_protect/helpers/config.py` & `galileo_protect-0.6.0/src/galileo_protect/helpers/config.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.5.2/src/galileo_protect/project.py` & `galileo_protect-0.6.0/src/galileo_protect/project.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.5.2/src/galileo_protect/schemas/__init__.py` & `galileo_protect-0.6.0/src/galileo_protect/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.5.2/src/galileo_protect/stage.py` & `galileo_protect-0.6.0/src/galileo_protect/stage.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.5.2/PKG-INFO` & `galileo_protect-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galileo-protect
-Version: 0.5.2
+Version: 0.6.0
 Summary: 🛡️ Secure your Generative AI applications with Galileo Protect!
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

