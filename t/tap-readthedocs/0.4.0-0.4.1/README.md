# Comparing `tmp/tap_readthedocs-0.4.0.tar.gz` & `tmp/tap_readthedocs-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Feb  6 01:38:47 2024, max compression
+gzip compressed data, last modified: Tue Apr 30 02:23:45 2024, max compression
```

## Comparing `tap_readthedocs-0.4.0.tar` & `tap_readthedocs-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1011 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      467 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/meltano.yml
--rw-r--r--   0        0        0      712 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/.github/FUNDING.yml
--rw-r--r--   0        0        0     1224 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/.github/dependabot.yml
--rw-r--r--   0        0        0       25 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/.github/workflows/constraints.txt
--rw-r--r--   0        0        0      809 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1598 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      409 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/output/.gitignore
--rw-r--r--   0        0        0       46 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/tap_readthedocs/__init__.py
--rw-r--r--   0        0        0      151 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/tap_readthedocs/__main__.py
--rw-r--r--   0        0        0     2537 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/tap_readthedocs/client.py
--rw-r--r--   0        0        0     9964 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/tap_readthedocs/streams.py
--rw-r--r--   0        0        0     1403 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/tap_readthedocs/tap.py
--rw-r--r--   0        0        0       38 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0       92 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0      617 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/tests/test_core.py
--rw-r--r--   0        0        0     2591 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/.gitignore
--rw-r--r--   0        0        0    11357 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/LICENSE
--rw-r--r--   0        0        0     3196 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/README.md
--rw-r--r--   0        0        0     3797 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    17596 2024-02-06 01:38:47.000000 tap_readthedocs-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1011 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      467 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/meltano.yml
+-rw-r--r--   0        0        0     1224 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/.github/dependabot.yml
+-rw-r--r--   0        0        0       23 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0      809 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1622 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      409 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/output/.gitignore
+-rw-r--r--   0        0        0       46 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/tap_readthedocs/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/tap_readthedocs/__main__.py
+-rw-r--r--   0        0        0     2537 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/tap_readthedocs/client.py
+-rw-r--r--   0        0        0     9965 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/tap_readthedocs/streams.py
+-rw-r--r--   0        0        0     1404 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/tap_readthedocs/tap.py
+-rw-r--r--   0        0        0       38 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0      617 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/tests/test_core.py
+-rw-r--r--   0        0        0     2591 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/.gitignore
+-rw-r--r--   0        0        0    11357 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3195 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/README.md
+-rw-r--r--   0        0        0     3662 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    17760 2024-04-30 02:23:45.000000 tap_readthedocs-0.4.1/PKG-INFO
```

### Comparing `tap_readthedocs-0.4.0/.pre-commit-config.yaml` & `tap_readthedocs-0.4.1/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 
   - repo: https://github.com/tox-dev/pyproject-fmt
     rev: "1.7.0"
     hooks:
       - id: pyproject-fmt
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.2.0"
+    rev: "v0.3.5"
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix, --show-fixes]
       - id: ruff-format
 
   - repo: https://github.com/pre-commit/pre-commit
-    rev: v3.6.0
+    rev: v3.7.0
     hooks:
       - id: validate_manifest
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.27.4
+    rev: 0.28.1
     hooks:
     - id: check-dependabot
     - id: check-github-workflows
```

### Comparing `tap_readthedocs-0.4.0/.github/dependabot.yml` & `tap_readthedocs-0.4.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tap_readthedocs-0.4.0/.github/workflows/release.yaml` & `tap_readthedocs-0.4.1/.github/workflows/release.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -31,8 +31,8 @@
         path: dist
     - uses: svenstaro/upload-release-action@v2
       with:
         file: dist/*.whl
         tag: ${{ github.ref }}
         overwrite: true
         file_glob: true
-    - uses: pypa/gh-action-pypi-publish@v1.8.11
+    - uses: pypa/gh-action-pypi-publish@v1.8.14
```

### Comparing `tap_readthedocs-0.4.0/.github/workflows/test.yml` & `tap_readthedocs-0.4.1/.github/workflows/test.yml`

 * *Files 6% similar despite different names*

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

### Comparing `tap_readthedocs-0.4.0/tap_readthedocs/client.py` & `tap_readthedocs-0.4.1/tap_readthedocs/client.py`

 * *Files identical despite different names*

### Comparing `tap_readthedocs-0.4.0/tap_readthedocs/streams.py` & `tap_readthedocs-0.4.1/tap_readthedocs/streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Stream type classes for tap-readthedocs."""
+
 from __future__ import annotations
 
 import logging
 import typing as t
 
 from singer_sdk import typing as th
 from toolz.dicttoolz import update_in
```

### Comparing `tap_readthedocs-0.4.0/tap_readthedocs/tap.py` & `tap_readthedocs-0.4.1/tap_readthedocs/tap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ReadTheDocs tap class."""
+
 from __future__ import annotations
 
 import typing as t
 
 from singer_sdk import Tap
 from singer_sdk import typing as th
```

### Comparing `tap_readthedocs-0.4.0/tests/test_core.py` & `tap_readthedocs-0.4.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_readthedocs-0.4.0/.gitignore` & `tap_readthedocs-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tap_readthedocs-0.4.0/LICENSE` & `tap_readthedocs-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_readthedocs-0.4.0/README.md` & `tap_readthedocs-0.4.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 ```
 
 ### Create and Run Tests
 
 Run integration tests:
 
 ```bash
-hatch run tests:integration
+hatch run test:integration
 ```
 
 You can also test the `tap-readthedocs` CLI interface directly:
 
 ```bash
 hatch run sync:console -- --about --format=json
 ```
```

#### html2text {}

```diff
@@ -11,17 +11,17 @@
 install tap-readthedocs ``` ### Source Authentication and Authorization
 Generate a token: https://readthedocs.org/accounts/tokens/. ## Usage You can
 easily run `tap-readthedocs` by itself or in a pipeline using [Meltano](https:/
 /meltano.com/). ### Executing the Tap Directly ```bash tap-readthedocs --
 version tap-readthedocs --help tap-readthedocs --config CONFIG --discover > ./
 catalog.json ``` ## Developer Resources ### Initialize your Development
 Environment ```bash pipx install hatch ``` ### Create and Run Tests Run
-integration tests: ```bash hatch run tests:integration ``` You can also test
-the `tap-readthedocs` CLI interface directly: ```bash hatch run sync:console -
-- --about --format=json ``` ### Testing with [Meltano](https://www.meltano.com)
+integration tests: ```bash hatch run test:integration ``` You can also test the
+`tap-readthedocs` CLI interface directly: ```bash hatch run sync:console -- --
+about --format=json ``` ### Testing with [Meltano](https://www.meltano.com)
 _**Note:** This tap will work in any Singer environment and does not require
 Meltano. Examples here are for convenience and to streamline end-to-end
 orchestration scenarios._ Your project comes with a custom `meltano.yml`
 project file already created. Go ahead and [install Meltano](https://
 docs.meltano.com/getting-started/installation/) if you haven't already. 1.
 Install all plugins ```bash meltano install ``` 2. Check that the extractor is
 working properly ```bash meltano invoke tap-readthedocs --version ``` 3.
```

### Comparing `tap_readthedocs-0.4.0/pyproject.toml` & `tap_readthedocs-0.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -27,24 +27,24 @@
   "Programming Language :: Python :: 3.12",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
   "requests-cache~=1.0",
-  "singer-sdk~=0.35.0",
+  "singer-sdk~=0.37.0",
   "toolz~=0.12.0",
 ]
 optional-dependencies.dev = [
   "tap-readthedocs[testing,typing]",
 ]
 optional-dependencies.testing = [
   "deptry>=0.12",
   "pytest>=7.4",
-  "singer-sdk[testing]~=0.35.0",
+  "singer-sdk[testing]~=0.37.0",
 ]
 optional-dependencies.typing = [
   "mypy",
   "types-requests",
 ]
 urls.Documentation = "https://github.com/edgarrmondragon/tap-readthedocs#readme"
 urls.Homepage = "https://github.com/edgarrmondragon/tap-readthedocs"
@@ -72,15 +72,14 @@
 [tool.hatch.envs.typing]
 features = ["testing", "typing"]
 [tool.hatch.envs.typing.scripts]
 check = "mypy --strict {args:tap_readthedocs tests}"
 
 [tool.ruff]
 line-length = 88
-target-version = "py38"
 
 [tool.ruff.lint]
 ignore = [
   "ANN101",  # missing-type-self
   "DJ",      # flake8-django
   "FIX002",  # line-contains-todo
   "COM812",  # missing-trailing-comma
@@ -121,15 +120,14 @@
   "pytest",
 ]
 
 [tool.pytest.ini_options]
 addopts = "-vvv"
 filterwarnings = [
   "error",
-  """ignore:datetime.datetime.utcnow\\(\\) is deprecated:DeprecationWarning:requests_cache.models.response""",
   "default:Fields in transformed catalog but not in records:UserWarning",
   "default:No records returned in stream 'projects:UserWarning",
   "default:No records returned in stream 'redirects:UserWarning",
   "default:No records returned in stream 'subprojects:UserWarning",
   "default:No records returned in stream 'translations:UserWarning",
   "default:No records returned in stream 'versions:UserWarning",
   "default:No records were available to test:UserWarning",
```

### Comparing `tap_readthedocs-0.4.0/PKG-INFO` & `tap_readthedocs-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tap-readthedocs
-Version: 0.4.0
+Version: 0.4.1
 Summary: `tap-readthedocs` is a Singer tap for ReadTheDocs, built with the Meltano SDK for Singer Taps.
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-readthedocs#readme
 Project-URL: Homepage, https://github.com/edgarrmondragon/tap-readthedocs
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-readthedocs
 Author-email: Edgar Ramírez-Mondragón <edgarrm358@gmail.com>
 Maintainer-email: Edgar Ramírez-Mondragón <edgarrm358@gmail.com>
 License:                                  Apache License
@@ -214,22 +214,26 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: requests-cache~=1.0
-Requires-Dist: singer-sdk~=0.35.0
+Requires-Dist: singer-sdk~=0.37.0
 Requires-Dist: toolz~=0.12.0
 Provides-Extra: dev
-Requires-Dist: tap-readthedocs[testing,typing]; extra == 'dev'
+Requires-Dist: deptry>=0.12; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: pytest>=7.4; extra == 'dev'
+Requires-Dist: singer-sdk[testing]~=0.37.0; extra == 'dev'
+Requires-Dist: types-requests; extra == 'dev'
 Provides-Extra: testing
 Requires-Dist: deptry>=0.12; extra == 'testing'
 Requires-Dist: pytest>=7.4; extra == 'testing'
-Requires-Dist: singer-sdk[testing]~=0.35.0; extra == 'testing'
+Requires-Dist: singer-sdk[testing]~=0.37.0; extra == 'testing'
 Provides-Extra: typing
 Requires-Dist: mypy; extra == 'typing'
 Requires-Dist: types-requests; extra == 'typing'
 Description-Content-Type: text/markdown
 
 <div align="center">
 
@@ -305,15 +309,15 @@
 ```
 
 ### Create and Run Tests
 
 Run integration tests:
 
 ```bash
-hatch run tests:integration
+hatch run test:integration
 ```
 
 You can also test the `tap-readthedocs` CLI interface directly:
 
 ```bash
 hatch run sync:console -- --about --format=json
 ```
```

