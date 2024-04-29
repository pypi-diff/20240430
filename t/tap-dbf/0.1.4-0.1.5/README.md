# Comparing `tmp/tap_dbf-0.1.4.tar.gz` & `tmp/tap_dbf-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Mar  1 23:59:18 2024, max compression
+gzip compressed data, last modified: Mon Apr 29 23:17:24 2024, max compression
```

## Comparing `tap_dbf-0.1.4.tar` & `tap_dbf-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       53 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/.flake8
--rw-r--r--   0        0        0      803 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      239 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/docker-compose.yaml
--rw-r--r--   0        0        0     1333 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/.github/dependabot.yml
--rw-r--r--   0        0        0       23 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/.github/workflows/constraints.txt
--rw-r--r--   0        0        0      787 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1396 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/.github/workflows/test.yml
--rw-r--r--   0        0        0       33 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/tap_dbf/__init__.py
--rw-r--r--   0        0        0      144 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/tap_dbf/__main__.py
--rw-r--r--   0        0        0     5112 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/tap_dbf/client.py
--rw-r--r--   0        0        0     7862 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/tap_dbf/tap.py
--rw-r--r--   0        0        0       25 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0       85 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0      477 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/tests/test_core.py
--rw-r--r--   0        0        0       74 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/tests/data/config.json
--rw-r--r--   0        0        0      198 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/tests/data/configGCS.json
--rw-r--r--   0        0        0       98 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/tests/data/configOS.json
--rw-r--r--   0        0        0      197 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/tests/data/configS3.json
--rw-r--r--   0        0        0    10450 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/tests/data/files/contacts.dbf
--rw-r--r--   0        0        0     2489 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/.gitignore
--rw-r--r--   0        0        0    11357 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/LICENSE
--rw-r--r--   0        0        0     3895 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/README.md
--rw-r--r--   0        0        0     3164 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5579 2024-03-01 23:59:18.000000 tap_dbf-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       53 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/.flake8
+-rw-r--r--   0        0        0      803 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      239 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/docker-compose.yaml
+-rw-r--r--   0        0        0     1333 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/.github/dependabot.yml
+-rw-r--r--   0        0        0       23 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0      787 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1420 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0       33 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/tap_dbf/__init__.py
+-rw-r--r--   0        0        0      144 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/tap_dbf/__main__.py
+-rw-r--r--   0        0        0     5112 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/tap_dbf/client.py
+-rw-r--r--   0        0        0     7862 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/tap_dbf/tap.py
+-rw-r--r--   0        0        0       25 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0      477 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/tests/test_core.py
+-rw-r--r--   0        0        0       74 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/tests/data/config.json
+-rw-r--r--   0        0        0      198 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/tests/data/configGCS.json
+-rw-r--r--   0        0        0       98 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/tests/data/configOS.json
+-rw-r--r--   0        0        0      197 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/tests/data/configS3.json
+-rw-r--r--   0        0        0    10450 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/tests/data/files/contacts.dbf
+-rw-r--r--   0        0        0     2489 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/.gitignore
+-rw-r--r--   0        0        0    11357 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3895 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/README.md
+-rw-r--r--   0        0        0     3164 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5579 2024-04-29 23:17:24.000000 tap_dbf-0.1.5/PKG-INFO
```

### Comparing `tap_dbf-0.1.4/.pre-commit-config.yaml` & `tap_dbf-0.1.5/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
 - repo: https://github.com/tox-dev/pyproject-fmt
   rev: "1.7.0"
   hooks:
     - id: pyproject-fmt
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.2.0
+  rev: v0.3.5
   hooks:
   - id: ruff
     name: Ruff lint
     args: [--fix, --exit-non-zero-on-fix, --show-fixes]
   - id: ruff-format
     name: Ruff format
 
 - repo: https://github.com/pre-commit/pre-commit
-  rev: v3.6.0
+  rev: v3.7.0
   hooks:
   - id: validate_manifest
```

### Comparing `tap_dbf-0.1.4/.github/dependabot.yml` & `tap_dbf-0.1.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tap_dbf-0.1.4/.github/workflows/release.yaml` & `tap_dbf-0.1.5/.github/workflows/release.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -31,8 +31,8 @@
         with:
           file: dist/*.whl
           tag: ${{ github.ref }}
           overwrite: true
           file_glob: true
 
       - name: Publish
-        uses: pypa/gh-action-pypi-publish@v1.8.12
+        uses: pypa/gh-action-pypi-publish@v1.8.14
```

### Comparing `tap_dbf-0.1.4/.github/workflows/test.yml` & `tap_dbf-0.1.5/.github/workflows/test.yml`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   workflow_dispatch:
 
 jobs:
   tests:
     runs-on: ubuntu-latest
     env:
       FORCE_COLOR: "1"
-      PIP_CONSTRAINT: .github/workflows/constraints.txt
+      PIP_CONSTRAINT: ${{ github.workspace }}/.github/workflows/constraints.txt
     strategy:
       fail-fast: false
       matrix:
         script: ["test:integration"]
         python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
         include:
         - { script: "test:dependencies", python-version: "3.12" }
```

### Comparing `tap_dbf-0.1.4/tap_dbf/client.py` & `tap_dbf-0.1.5/tap_dbf/client.py`

 * *Files identical despite different names*

### Comparing `tap_dbf-0.1.4/tap_dbf/tap.py` & `tap_dbf-0.1.5/tap_dbf/tap.py`

 * *Files identical despite different names*

### Comparing `tap_dbf-0.1.4/tests/data/files/contacts.dbf` & `tap_dbf-0.1.5/tests/data/files/contacts.dbf`

 * *Files identical despite different names*

### Comparing `tap_dbf-0.1.4/.gitignore` & `tap_dbf-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `tap_dbf-0.1.4/LICENSE` & `tap_dbf-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_dbf-0.1.4/README.md` & `tap_dbf-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tap_dbf-0.1.4/pyproject.toml` & `tap_dbf-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -30,31 +30,31 @@
   "Topic :: Database",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
   "dbfread~=2.0.7",
-  "fsspec~=2024.2.0",
-  "singer-sdk~=0.36.0",
+  "fsspec~=2024.3.1",
+  "singer-sdk~=0.37.0",
 ]
 optional-dependencies.dev = [
   "singer-sdk[gcs,s3,testing,typing]",
 ]
 optional-dependencies.gcs = [
-  "gcsfs~=2024.2.0",
+  "gcsfs~=2024.3.1",
 ]
 optional-dependencies.s3 = [
-  "s3fs~=2024.2.0",
+  "s3fs~=2024.3.1",
 ]
 optional-dependencies.testing = [
   "deptry>=0.12",
   "pytest>=7.4",
   "pytest-github-actions-annotate-failures~=0.2.0",
-  "singer-sdk[testing]~=0.36.0",
+  "singer-sdk[testing]~=0.37.0",
 ]
 optional-dependencies.typing = [
   "mypy",
   'typing-extensions>=4.7.1; python_version < "3.11"',
 ]
 urls.documentation = "https://github.com/edgarrmondragon/tap-dbf#readme"
 urls.homepage = "https://github.com/edgarrmondragon/tap-dbf"
```

### Comparing `tap_dbf-0.1.4/PKG-INFO` & `tap_dbf-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tap-dbf
-Version: 0.1.4
+Version: 0.1.5
 Summary: Singer tap for .DBF files
 Project-URL: documentation, https://github.com/edgarrmondragon/tap-dbf#readme
 Project-URL: homepage, https://github.com/edgarrmondragon/tap-dbf
 Project-URL: repository, https://github.com/edgarrmondragon/tap-dbf
 Author-email: "Edgar R. Mondragón" <edgarrm358@gmail.com>
 Maintainer-email: "Edgar R. Mondragón" <edgarrm358@gmail.com>
 License-Expression: Apache-2.0
@@ -16,27 +16,27 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database
 Requires-Python: >=3.8
 Requires-Dist: dbfread~=2.0.7
-Requires-Dist: fsspec~=2024.2.0
-Requires-Dist: singer-sdk~=0.36.0
+Requires-Dist: fsspec~=2024.3.1
+Requires-Dist: singer-sdk~=0.37.0
 Provides-Extra: dev
 Requires-Dist: singer-sdk[gcs,s3,testing,typing]; extra == 'dev'
 Provides-Extra: gcs
-Requires-Dist: gcsfs~=2024.2.0; extra == 'gcs'
+Requires-Dist: gcsfs~=2024.3.1; extra == 'gcs'
 Provides-Extra: s3
-Requires-Dist: s3fs~=2024.2.0; extra == 's3'
+Requires-Dist: s3fs~=2024.3.1; extra == 's3'
 Provides-Extra: testing
 Requires-Dist: deptry>=0.12; extra == 'testing'
 Requires-Dist: pytest-github-actions-annotate-failures~=0.2.0; extra == 'testing'
 Requires-Dist: pytest>=7.4; extra == 'testing'
-Requires-Dist: singer-sdk[testing]~=0.36.0; extra == 'testing'
+Requires-Dist: singer-sdk[testing]~=0.37.0; extra == 'testing'
 Provides-Extra: typing
 Requires-Dist: mypy; extra == 'typing'
 Requires-Dist: typing-extensions>=4.7.1; (python_version < '3.11') and extra == 'typing'
 Description-Content-Type: text/markdown
 
 # tap-dbf
```

