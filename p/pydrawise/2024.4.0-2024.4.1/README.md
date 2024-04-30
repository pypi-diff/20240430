# Comparing `tmp/pydrawise-2024.4.0.tar.gz` & `tmp/pydrawise-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydrawise-2024.4.0.tar", last modified: Mon Apr 22 12:22:11 2024, max compression
+gzip compressed data, was "pydrawise-2024.4.1.tar", last modified: Tue Apr 30 12:04:31 2024, max compression
```

## Comparing `pydrawise-2024.4.0.tar` & `pydrawise-2024.4.1.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:22:11.908944 pydrawise-2024.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/.devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:22:11.904944 pydrawise-2024.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:22:11.904944 pydrawise-2024.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/.github/workflows/publish-python.yml
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:22:11.904944 pydrawise-2024.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-22 12:22:11.908944 pydrawise-2024.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:22:11.904944 pydrawise-2024.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:22:11.904944 pydrawise-2024.4.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/docs/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/docs/reference/schema.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:22:11.904944 pydrawise-2024.4.0/pydrawise/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/pydrawise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-22 12:22:11.000000 pydrawise-2024.4.0/pydrawise/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/pydrawise/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/pydrawise/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17412 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/pydrawise/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/pydrawise/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    55590 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/pydrawise/hydrawise.graphql
--rw-r--r--   0 runner    (1001) docker     (127)    12815 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/pydrawise/legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)    16653 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/pydrawise/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/pydrawise/schema_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:22:11.908944 pydrawise-2024.4.0/pydrawise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-22 12:22:11.000000 pydrawise-2024.4.0/pydrawise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-22 12:22:11.000000 pydrawise-2024.4.0/pydrawise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 12:22:11.000000 pydrawise-2024.4.0/pydrawise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 12:22:11.000000 pydrawise-2024.4.0/pydrawise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-22 12:22:11.000000 pydrawise-2024.4.0/pydrawise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 12:22:11.000000 pydrawise-2024.4.0/pydrawise.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:22:11.908944 pydrawise-2024.4.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      324 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/scripts/setup
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 12:22:11.908944 pydrawise-2024.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:22:11.908944 pydrawise-2024.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    19840 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    25747 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/tests/test_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-22 12:21:57.000000 pydrawise-2024.4.0/tests/test_schema_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.066710 pydrawise-2024.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.062710 pydrawise-2024.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.062710 pydrawise-2024.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.github/workflows/publish-python.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.062710 pydrawise-2024.4.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-30 12:04:31.066710 pydrawise-2024.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.062710 pydrawise-2024.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.062710 pydrawise-2024.4.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/docs/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/docs/reference/schema.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.062710 pydrawise-2024.4.1/pydrawise/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-30 12:04:30.000000 pydrawise-2024.4.1/pydrawise/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17412 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55590 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/hydrawise.graphql
+-rw-r--r--   0 runner    (1001) docker     (127)    12815 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16653 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/schema_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.066710 pydrawise-2024.4.1/pydrawise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-30 12:04:31.000000 pydrawise-2024.4.1/pydrawise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-30 12:04:31.000000 pydrawise-2024.4.1/pydrawise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 12:04:31.000000 pydrawise-2024.4.1/pydrawise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 12:04:31.000000 pydrawise-2024.4.1/pydrawise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 12:04:31.000000 pydrawise-2024.4.1/pydrawise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 12:04:30.000000 pydrawise-2024.4.1/pydrawise.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.066710 pydrawise-2024.4.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      324 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/scripts/setup
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 12:04:31.066710 pydrawise-2024.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.066710 pydrawise-2024.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19840 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25747 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/tests/test_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/tests/test_schema_utils.py
```

### Comparing `pydrawise-2024.4.0/.devcontainer.json` & `pydrawise-2024.4.1/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/.github/workflows/build-and-test.yml` & `pydrawise-2024.4.1/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/.github/workflows/publish-python.yml` & `pydrawise-2024.4.1/.github/workflows/publish-python.yml`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/.gitignore` & `pydrawise-2024.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/.pre-commit-config.yaml` & `pydrawise-2024.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/LICENSE` & `pydrawise-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/PKG-INFO` & `pydrawise-2024.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydrawise
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Python API for interacting with Hydrawise sprinkler controllers.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pydrawise
 Project-URL: Source Code, https://github.com/dknowles2/pydrawise
 Project-URL: Bug Reports, https://github.com/dknowles2/pydrawise/issues
 Keywords: hydrawise,api,iot
```

### Comparing `pydrawise-2024.4.0/README.md` & `pydrawise-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/docs/index.md` & `pydrawise-2024.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/mkdocs.yml` & `pydrawise-2024.4.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/pydrawise/__init__.py` & `pydrawise-2024.4.1/pydrawise/__init__.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/pydrawise/auth.py` & `pydrawise-2024.4.1/pydrawise/auth.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/pydrawise/base.py` & `pydrawise-2024.4.1/pydrawise/base.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/pydrawise/client.py` & `pydrawise-2024.4.1/pydrawise/client.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/pydrawise/exceptions.py` & `pydrawise-2024.4.1/pydrawise/exceptions.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/pydrawise/hydrawise.graphql` & `pydrawise-2024.4.1/pydrawise/hydrawise.graphql`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/pydrawise/legacy.py` & `pydrawise-2024.4.1/pydrawise/legacy.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/pydrawise/schema.py` & `pydrawise-2024.4.1/pydrawise/schema.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/pydrawise/schema_utils.py` & `pydrawise-2024.4.1/pydrawise/schema_utils.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/pydrawise.egg-info/PKG-INFO` & `pydrawise-2024.4.1/pydrawise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydrawise
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Python API for interacting with Hydrawise sprinkler controllers.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pydrawise
 Project-URL: Source Code, https://github.com/dknowles2/pydrawise
 Project-URL: Bug Reports, https://github.com/dknowles2/pydrawise/issues
 Keywords: hydrawise,api,iot
```

### Comparing `pydrawise-2024.4.0/pydrawise.egg-info/SOURCES.txt` & `pydrawise-2024.4.1/pydrawise.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 pydrawise/_version.py
 pydrawise/auth.py
 pydrawise/base.py
 pydrawise/client.py
 pydrawise/exceptions.py
 pydrawise/hydrawise.graphql
 pydrawise/legacy.py
+pydrawise/py.typed
 pydrawise/schema.py
 pydrawise/schema_utils.py
 pydrawise.egg-info/PKG-INFO
 pydrawise.egg-info/SOURCES.txt
 pydrawise.egg-info/dependency_links.txt
 pydrawise.egg-info/requires.txt
 pydrawise.egg-info/top_level.txt
```

### Comparing `pydrawise-2024.4.0/pyproject.toml` & `pydrawise-2024.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/tests/test_auth.py` & `pydrawise-2024.4.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/tests/test_client.py` & `pydrawise-2024.4.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.0/tests/test_legacy.py` & `pydrawise-2024.4.1/tests/test_legacy.py`

 * *Files identical despite different names*

