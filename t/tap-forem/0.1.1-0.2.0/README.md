# Comparing `tmp/tap_forem-0.1.1.tar.gz` & `tmp/tap_forem-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Mar  4 14:55:06 2024, max compression
+gzip compressed data, last modified: Tue Apr 30 14:30:32 2024, max compression
```

## Comparing `tap_forem-0.1.1.tar` & `tap_forem-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      667 2024-03-04 14:55:06.000000 tap_forem-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      882 2024-03-04 14:55:06.000000 tap_forem-0.1.1/meltano.yml
--rw-r--r--   0        0        0      966 2024-03-04 14:55:06.000000 tap_forem-0.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0       56 2024-03-04 14:55:06.000000 tap_forem-0.1.1/.github/workflows/constraints.txt
--rw-r--r--   0        0        0      855 2024-03-04 14:55:06.000000 tap_forem-0.1.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1572 2024-03-04 14:55:06.000000 tap_forem-0.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      618 2024-03-04 14:55:06.000000 tap_forem-0.1.1/.vscode/launch.json
--rw-r--r--   0        0        0       77 2024-03-04 14:55:06.000000 tap_forem-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0      409 2024-03-04 14:55:06.000000 tap_forem-0.1.1/output/.gitignore
--rw-r--r--   0        0        0       36 2024-03-04 14:55:06.000000 tap_forem-0.1.1/tap_forem/__init__.py
--rw-r--r--   0        0        0      110 2024-03-04 14:55:06.000000 tap_forem-0.1.1/tap_forem/__main__.py
--rw-r--r--   0        0        0     1786 2024-03-04 14:55:06.000000 tap_forem-0.1.1/tap_forem/client.py
--rw-r--r--   0        0        0     4728 2024-03-04 14:55:06.000000 tap_forem-0.1.1/tap_forem/streams.py
--rw-r--r--   0        0        0     1068 2024-03-04 14:55:06.000000 tap_forem-0.1.1/tap_forem/tap.py
--rw-r--r--   0        0        0       32 2024-03-04 14:55:06.000000 tap_forem-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0       92 2024-03-04 14:55:06.000000 tap_forem-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0      303 2024-03-04 14:55:06.000000 tap_forem-0.1.1/tests/test_core.py
--rw-r--r--   0        0        0     1914 2024-03-04 14:55:06.000000 tap_forem-0.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2024-03-04 14:55:06.000000 tap_forem-0.1.1/LICENSE
--rw-r--r--   0        0        0     2308 2024-03-04 14:55:06.000000 tap_forem-0.1.1/README.md
--rw-r--r--   0        0        0     3225 2024-03-04 14:55:06.000000 tap_forem-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    16471 2024-03-04 14:55:06.000000 tap_forem-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      667 2024-04-30 14:30:32.000000 tap_forem-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      882 2024-04-30 14:30:32.000000 tap_forem-0.2.0/meltano.yml
+-rw-r--r--   0        0        0      966 2024-04-30 14:30:32.000000 tap_forem-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0       57 2024-04-30 14:30:32.000000 tap_forem-0.2.0/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0      855 2024-04-30 14:30:32.000000 tap_forem-0.2.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1596 2024-04-30 14:30:32.000000 tap_forem-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      618 2024-04-30 14:30:32.000000 tap_forem-0.2.0/.vscode/launch.json
+-rw-r--r--   0        0        0       77 2024-04-30 14:30:32.000000 tap_forem-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0      409 2024-04-30 14:30:32.000000 tap_forem-0.2.0/output/.gitignore
+-rw-r--r--   0        0        0       36 2024-04-30 14:30:32.000000 tap_forem-0.2.0/tap_forem/__init__.py
+-rw-r--r--   0        0        0      110 2024-04-30 14:30:32.000000 tap_forem-0.2.0/tap_forem/__main__.py
+-rw-r--r--   0        0        0     1868 2024-04-30 14:30:32.000000 tap_forem-0.2.0/tap_forem/client.py
+-rw-r--r--   0        0        0     4728 2024-04-30 14:30:32.000000 tap_forem-0.2.0/tap_forem/streams.py
+-rw-r--r--   0        0        0     1068 2024-04-30 14:30:32.000000 tap_forem-0.2.0/tap_forem/tap.py
+-rw-r--r--   0        0        0       32 2024-04-30 14:30:32.000000 tap_forem-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-30 14:30:32.000000 tap_forem-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      303 2024-04-30 14:30:32.000000 tap_forem-0.2.0/tests/test_core.py
+-rw-r--r--   0        0        0     1914 2024-04-30 14:30:32.000000 tap_forem-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11357 2024-04-30 14:30:32.000000 tap_forem-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2308 2024-04-30 14:30:32.000000 tap_forem-0.2.0/README.md
+-rw-r--r--   0        0        0     3225 2024-04-30 14:30:32.000000 tap_forem-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    16588 2024-04-30 14:30:32.000000 tap_forem-0.2.0/PKG-INFO
```

### Comparing `tap_forem-0.1.1/.pre-commit-config.yaml` & `tap_forem-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tap_forem-0.1.1/meltano.yml` & `tap_forem-0.2.0/meltano.yml`

 * *Files identical despite different names*

### Comparing `tap_forem-0.1.1/.github/dependabot.yml` & `tap_forem-0.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tap_forem-0.1.1/.github/workflows/release.yaml` & `tap_forem-0.2.0/.github/workflows/release.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -33,8 +33,8 @@
         path: dist
     - uses: svenstaro/upload-release-action@v2
       with:
         file: dist/*.whl
         tag: ${{ github.ref }}
         overwrite: true
         file_glob: true
-    - uses: pypa/gh-action-pypi-publish@v1.8.12
+    - uses: pypa/gh-action-pypi-publish@v1.8.14
```

### Comparing `tap_forem-0.1.1/.github/workflows/test.yml` & `tap_forem-0.2.0/.github/workflows/test.yml`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   - cron: "0 12 */4 * *"
 
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

### Comparing `tap_forem-0.1.1/.vscode/launch.json` & `tap_forem-0.2.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `tap_forem-0.1.1/tap_forem/client.py` & `tap_forem-0.2.0/tap_forem/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,18 @@
             value=self.config["api_key"],
             location="header",
         )
 
     @property
     def http_headers(self) -> dict[str, str]:
         """Return the http headers needed."""
-        return {"User-Agent": f"{self.tap_name}/{self._tap.plugin_version}"}
+        return {
+            "User-Agent": f"{self.tap_name}/{self._tap.plugin_version}",
+            "Accept": "application/vnd.forem.api-v1+json",
+        }
 
 
 class PaginatedForemStream(ForemStream):
     """Forem stream with pagination."""
 
     def get_new_paginator(self) -> BasePageNumberPaginator:
         """Get a fresh paginator.
```

### Comparing `tap_forem-0.1.1/tap_forem/streams.py` & `tap_forem-0.2.0/tap_forem/streams.py`

 * *Files identical despite different names*

### Comparing `tap_forem-0.1.1/tap_forem/tap.py` & `tap_forem-0.2.0/tap_forem/tap.py`

 * *Files identical despite different names*

### Comparing `tap_forem-0.1.1/.gitignore` & `tap_forem-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tap_forem-0.1.1/LICENSE` & `tap_forem-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_forem-0.1.1/README.md` & `tap_forem-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tap_forem-0.1.1/pyproject.toml` & `tap_forem-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  "singer-sdk~=0.36.0",
+  "singer-sdk~=0.37.0",
 ]
 optional-dependencies.dev = [
   "tap-forem[testing,typing]",
 ]
 optional-dependencies.testing = [
   "deptry>=0.12",
   "pytest>=7.4",
```

### Comparing `tap_forem-0.1.1/PKG-INFO` & `tap_forem-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tap-forem
-Version: 0.1.1
+Version: 0.2.0
 Summary: `tap-forem` is a Singer tap for Forem, built with the Meltano SDK for Singer Taps.
 Project-URL: Issue Tracker, https://github.com/edgarrmondragon/tap-forem/issues
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-forem
 Author-email: Edgar Ramírez-Mondragón <edgarrm358@gmail.com>
 Maintainer-email: Edgar Ramírez-Mondragón <edgarrm358@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
@@ -212,17 +212,20 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
-Requires-Dist: singer-sdk~=0.36.0
+Requires-Dist: singer-sdk~=0.37.0
 Provides-Extra: dev
-Requires-Dist: tap-forem[testing,typing]; extra == 'dev'
+Requires-Dist: deptry>=0.12; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: pytest>=7.4; extra == 'dev'
+Requires-Dist: singer-sdk[testing]; extra == 'dev'
 Provides-Extra: testing
 Requires-Dist: deptry>=0.12; extra == 'testing'
 Requires-Dist: pytest>=7.4; extra == 'testing'
 Requires-Dist: singer-sdk[testing]; extra == 'testing'
 Provides-Extra: typing
 Requires-Dist: mypy; extra == 'typing'
 Description-Content-Type: text/markdown
```

