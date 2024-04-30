# Comparing `tmp/ssvc-1.0.4.tar.gz` & `tmp/ssvc-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssvc-1.0.4.tar", max compression
+gzip compressed data, was "ssvc-1.0.5.tar", max compression
```

## Comparing `ssvc-1.0.4.tar` & `ssvc-1.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2024-03-24 22:36:13.565774 ssvc-1.0.4/LICENSE
--rw-r--r--   0        0        0     1949 2024-04-12 12:13:50.233414 ssvc-1.0.4/PYPI.md
--rw-r--r--   0        0        0      617 2024-04-12 12:14:57.727869 ssvc-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     6463 2024-04-12 12:03:21.776208 ssvc-1.0.4/src/ssvc/__init__.py
--rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 ssvc-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-03-25 11:16:25.817155 ssvc-1.0.5/LICENSE
+-rw-r--r--   0        0        0     1949 2024-04-18 11:26:03.741779 ssvc-1.0.5/PYPI.md
+-rw-r--r--   0        0        0      640 2024-04-30 13:08:28.469191 ssvc-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6463 2024-04-18 11:26:03.748446 ssvc-1.0.5/src/ssvc/__init__.py
+-rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 ssvc-1.0.5/PKG-INFO
```

### Comparing `ssvc-1.0.4/LICENSE` & `ssvc-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ssvc-1.0.4/PYPI.md` & `ssvc-1.0.5/PYPI.md`

 * *Files identical despite different names*

### Comparing `ssvc-1.0.4/pyproject.toml` & `ssvc-1.0.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "ssvc"
-version = "1.0.4"
+version = "1.0.5"
 description = "A Python implementation of the Stakeholder-Specific Vulnerability Categorization framework."
 authors = ["Christopher Langton <chris@langton.cloud>"]
 readme = "PYPI.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 
 [tool.poetry.dev-dependencies]
-uv = "^0.1.29"
+setuptools = "^69.5.1"
+uv = "^0.1.39"
 isort = "^5.13.2"
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 coverage-badge = "^1.1.0"
-ruff = "^0.3.5"
+ruff = "^0.4.1"
 poetry = "^1.8.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
```

### Comparing `ssvc-1.0.4/src/ssvc/__init__.py` & `ssvc-1.0.5/src/ssvc/__init__.py`

 * *Files identical despite different names*

### Comparing `ssvc-1.0.4/PKG-INFO` & `ssvc-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssvc
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python implementation of the Stakeholder-Specific Vulnerability Categorization framework.
 Author: Christopher Langton
 Author-email: chris@langton.cloud
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

