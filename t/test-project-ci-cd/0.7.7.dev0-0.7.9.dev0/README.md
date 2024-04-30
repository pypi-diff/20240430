# Comparing `tmp/test_project_ci_cd-0.7.7.dev0.tar.gz` & `tmp/test_project_ci_cd-0.7.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_project_ci_cd-0.7.7.dev0.tar", max compression
+gzip compressed data, was "test_project_ci_cd-0.7.9.dev0.tar", max compression
```

## Comparing `test_project_ci_cd-0.7.7.dev0.tar` & `test_project_ci_cd-0.7.9.dev0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       67 2024-04-26 21:27:32.143944 test_project_ci_cd-0.7.7.dev0/README.md
--rw-r--r--   0        0        0     1204 2024-04-26 21:27:32.143944 test_project_ci_cd-0.7.7.dev0/pyproject.toml
--rw-r--r--   0        0        0      993 2024-04-26 21:27:32.143944 test_project_ci_cd-0.7.7.dev0/src/test_project_ci_cd/__init__.py
--rw-r--r--   0        0        0      232 2024-04-26 21:27:32.143944 test_project_ci_cd-0.7.7.dev0/src/test_project_ci_cd/__main__.py
--rw-r--r--   0        0        0      414 2024-04-26 21:27:32.143944 test_project_ci_cd-0.7.7.dev0/src/test_project_ci_cd/calc.py
--rw-r--r--   0        0        0        0 2024-04-26 21:27:32.143944 test_project_ci_cd-0.7.7.dev0/src/test_project_ci_cd/py.typed
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 test_project_ci_cd-0.7.7.dev0/PKG-INFO
+-rw-r--r--   0        0        0       67 2024-04-29 19:22:10.026170 test_project_ci_cd-0.7.9.dev0/README.md
+-rw-r--r--   0        0        0     1204 2024-04-29 19:22:10.026170 test_project_ci_cd-0.7.9.dev0/pyproject.toml
+-rw-r--r--   0        0        0      993 2024-04-29 19:22:10.026170 test_project_ci_cd-0.7.9.dev0/src/test_project_ci_cd/__init__.py
+-rw-r--r--   0        0        0      232 2024-04-29 19:22:10.026170 test_project_ci_cd-0.7.9.dev0/src/test_project_ci_cd/__main__.py
+-rw-r--r--   0        0        0      414 2024-04-29 19:22:10.026170 test_project_ci_cd-0.7.9.dev0/src/test_project_ci_cd/calc.py
+-rw-r--r--   0        0        0        0 2024-04-29 19:22:10.026170 test_project_ci_cd-0.7.9.dev0/src/test_project_ci_cd/py.typed
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 test_project_ci_cd-0.7.9.dev0/PKG-INFO
```

### Comparing `test_project_ci_cd-0.7.7.dev0/pyproject.toml` & `test_project_ci_cd-0.7.9.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "test-project-ci-cd"
-version = "0.7.7-dev"
+version = "0.7.9-dev"
 description = "test project for github actions"
 authors = ["Daryl Stark <daryl@dstark.nl>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "test_project_ci_cd", from = "src" }
 ]
@@ -23,15 +23,15 @@
 pytest-sugar = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "0.7.7-dev"
+current_version = "0.7.9-dev"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Version {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `test_project_ci_cd-0.7.7.dev0/src/test_project_ci_cd/__init__.py` & `test_project_ci_cd-0.7.9.dev0/src/test_project_ci_cd/__init__.py`

 * *Files identical despite different names*

### Comparing `test_project_ci_cd-0.7.7.dev0/PKG-INFO` & `test_project_ci_cd-0.7.9.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-project-ci-cd
-Version: 0.7.7.dev0
+Version: 0.7.9.dev0
 Summary: test project for github actions
 License: MIT
 Author: Daryl Stark
 Author-email: daryl@dstark.nl
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

