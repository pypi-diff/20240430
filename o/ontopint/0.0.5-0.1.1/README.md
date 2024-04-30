# Comparing `tmp/ontopint-0.0.5.tar.gz` & `tmp/ontopint-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontopint-0.0.5.tar", last modified: Thu Apr 25 08:36:57 2024, max compression
+gzip compressed data, was "ontopint-0.1.1.tar", last modified: Tue Apr 30 04:46:37 2024, max compression
```

## Comparing `ontopint-0.0.5.tar` & `ontopint-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:36:57.873694 ontopint-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:36:57.869693 ontopint-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:36:57.869693 ontopint-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-25 08:36:51.000000 ontopint-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-25 08:36:51.000000 ontopint-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-25 08:36:51.000000 ontopint-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-25 08:36:57.873694 ontopint-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-25 08:36:51.000000 ontopint-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-25 08:36:51.000000 ontopint-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 08:36:57.873694 ontopint-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:36:57.869693 ontopint-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:36:57.869693 ontopint-0.0.5/src/ontopint/
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-25 08:36:51.000000 ontopint-0.0.5/src/ontopint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:36:57.873694 ontopint-0.0.5/src/ontopint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-25 08:36:57.000000 ontopint-0.0.5/src/ontopint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-25 08:36:57.000000 ontopint-0.0.5/src/ontopint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:36:57.000000 ontopint-0.0.5/src/ontopint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-25 08:36:57.000000 ontopint-0.0.5/src/ontopint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-25 08:36:57.000000 ontopint-0.0.5/src/ontopint.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:36:57.869693 ontopint-0.0.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:36:57.873694 ontopint-0.0.5/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-25 08:36:51.000000 ontopint-0.0.5/tests/data/test_data.jsonld
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:46:37.817306 ontopint-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:46:37.813306 ontopint-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:46:37.817306 ontopint-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-30 04:46:11.000000 ontopint-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-30 04:46:11.000000 ontopint-0.1.1/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-30 04:46:11.000000 ontopint-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-30 04:46:11.000000 ontopint-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-30 04:46:37.817306 ontopint-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-30 04:46:11.000000 ontopint-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-30 04:46:11.000000 ontopint-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 04:46:37.817306 ontopint-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:46:37.813306 ontopint-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:46:37.817306 ontopint-0.1.1/src/ontopint/
+-rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-04-30 04:46:11.000000 ontopint-0.1.1/src/ontopint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:46:37.817306 ontopint-0.1.1/src/ontopint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-30 04:46:37.000000 ontopint-0.1.1/src/ontopint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-30 04:46:37.000000 ontopint-0.1.1/src/ontopint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 04:46:37.000000 ontopint-0.1.1/src/ontopint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 04:46:37.000000 ontopint-0.1.1/src/ontopint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 04:46:37.000000 ontopint-0.1.1/src/ontopint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:46:37.817306 ontopint-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-30 04:46:11.000000 ontopint-0.1.1/tests/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:46:37.817306 ontopint-0.1.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-30 04:46:11.000000 ontopint-0.1.1/tests/data/test_data_custom_keys.jsonld
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-30 04:46:11.000000 ontopint-0.1.1/tests/data/test_data_default_keys.jsonld
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-30 04:46:11.000000 ontopint-0.1.1/tests/test_010_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-30 04:46:11.000000 ontopint-0.1.1/tests/test_020_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-30 04:46:11.000000 ontopint-0.1.1/tests/test_030_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-30 04:46:11.000000 ontopint-0.1.1/tests/test_040_roundtrip.py
```

### Comparing `ontopint-0.0.5/.github/workflows/python-publish.yml` & `ontopint-0.1.1/.github/workflows/python-publish.yml`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,19 @@
       uses: actions/setup-python@v3
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
+        pip install .[dev]
+    - name: Test with pytest
+      run: |
+        pip install pytest
+        pytest
     - name: Build package
       run: python -m build
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `ontopint-0.0.5/.gitignore` & `ontopint-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ontopint-0.0.5/LICENSE` & `ontopint-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ontopint-0.0.5/pyproject.toml` & `ontopint-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -25,21 +25,23 @@
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
     "rdflib",
+    "sparqlwrapper",
     "pint",
     "pyld",
     "ucumvert",
 ]
 [project.optional-dependencies]
 dev = [
     "pytest",
+    "deepdiff",
 ]
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 "Homepage" = "https://github.com/hampusnasstrom/ontopint"
```

### Comparing `ontopint-0.0.5/tests/data/test_data.jsonld` & `ontopint-0.1.1/tests/data/test_data_custom_keys.jsonld`

 * *Files identical despite different names*

