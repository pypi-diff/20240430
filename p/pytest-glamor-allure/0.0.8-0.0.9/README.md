# Comparing `tmp/pytest_glamor_allure-0.0.8.tar.gz` & `tmp/pytest_glamor_allure-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_glamor_allure-0.0.8.tar", last modified: Fri Nov 26 20:29:18 2021, max compression
+gzip compressed data, was "pytest_glamor_allure-0.0.9.tar", last modified: Thu May 19 05:27:15 2022, max compression
```

## Comparing `pytest_glamor_allure-0.0.8.tar` & `pytest_glamor_allure-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-26 20:29:18.494891 pytest_glamor_allure-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-26 20:29:18.490891 pytest_glamor_allure-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      620 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-26 20:29:18.490891 pytest_glamor_allure-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      574 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      679 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/.github/workflows/run_lint_and_tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1862 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10001 2021-11-26 20:29:18.494891 pytest_glamor_allure-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9010 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-26 20:29:18.490891 pytest_glamor_allure-0.0.8/glamor/
--rw-r--r--   0 runner    (1001) docker     (121)     2158 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/glamor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8134 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/glamor/patches.py
--rw-r--r--   0 runner    (1001) docker     (121)      698 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/pitest.py
--rw-r--r--   0 runner    (1001) docker     (121)      238 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-26 20:29:18.490891 pytest_glamor_allure-0.0.8/pytest_glamor_allure/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/pytest_glamor_allure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-11-26 20:29:18.000000 pytest_glamor_allure-0.0.8/pytest_glamor_allure/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     8634 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/pytest_glamor_allure/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-26 20:29:18.494891 pytest_glamor_allure-0.0.8/pytest_glamor_allure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10001 2021-11-26 20:29:18.000000 pytest_glamor_allure-0.0.8/pytest_glamor_allure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      783 2021-11-26 20:29:18.000000 pytest_glamor_allure-0.0.8/pytest_glamor_allure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-26 20:29:18.000000 pytest_glamor_allure-0.0.8/pytest_glamor_allure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2021-11-26 20:29:18.000000 pytest_glamor_allure-0.0.8/pytest_glamor_allure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-11-26 20:29:18.000000 pytest_glamor_allure-0.0.8/pytest_glamor_allure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-11-26 20:29:18.000000 pytest_glamor_allure-0.0.8/pytest_glamor_allure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      119 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-26 20:29:18.494891 pytest_glamor_allure-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1642 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-26 20:29:18.494891 pytest_glamor_allure-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      848 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/tests/matchers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/tests/test_allure.py
--rw-r--r--   0 runner    (1001) docker     (121)    16976 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/tests/test_glamor_decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     4014 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/tests/test_glamor_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (121)     7892 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/tests/test_glamor_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2021-11-26 20:29:06.000000 pytest_glamor_allure-0.0.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 05:27:15.120906 pytest_glamor_allure-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 05:27:15.116907 pytest_glamor_allure-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)      620 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 05:27:15.116907 pytest_glamor_allure-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2338 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      574 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/.github/workflows/run_lint_and_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    10088 2022-05-19 05:27:15.120906 pytest_glamor_allure-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     9117 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 05:27:15.116907 pytest_glamor_allure-0.0.9/glamor/
+-rw-r--r--   0 runner    (1001) docker     (121)     2158 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/glamor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8134 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/glamor/patches.py
+-rw-r--r--   0 runner    (1001) docker     (121)      698 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/pitest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 05:27:15.116907 pytest_glamor_allure-0.0.9/pytest_glamor_allure/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/pytest_glamor_allure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-05-19 05:27:13.000000 pytest_glamor_allure-0.0.9/pytest_glamor_allure/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8634 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/pytest_glamor_allure/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 05:27:15.116907 pytest_glamor_allure-0.0.9/pytest_glamor_allure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10088 2022-05-19 05:27:14.000000 pytest_glamor_allure-0.0.9/pytest_glamor_allure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      821 2022-05-19 05:27:15.000000 pytest_glamor_allure-0.0.9/pytest_glamor_allure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-19 05:27:14.000000 pytest_glamor_allure-0.0.9/pytest_glamor_allure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-05-19 05:27:14.000000 pytest_glamor_allure-0.0.9/pytest_glamor_allure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-05-19 05:27:14.000000 pytest_glamor_allure-0.0.9/pytest_glamor_allure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-05-19 05:27:15.000000 pytest_glamor_allure-0.0.9/pytest_glamor_allure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-19 05:27:15.120906 pytest_glamor_allure-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1642 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 05:27:15.120906 pytest_glamor_allure-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      848 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/tests/matchers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/tests/test_allure.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16976 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/tests/test_glamor_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4014 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/tests/test_glamor_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7892 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/tests/test_glamor_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-05-19 05:27:01.000000 pytest_glamor_allure-0.0.9/tox.ini
```

### Comparing `pytest_glamor_allure-0.0.8/.github/dependabot.yml` & `pytest_glamor_allure-0.0.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pytest_glamor_allure-0.0.8/.github/workflows/python-publish.yml` & `pytest_glamor_allure-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pytest_glamor_allure-0.0.8/.github/workflows/run_lint_and_tests.yml` & `pytest_glamor_allure-0.0.9/.github/workflows/run_lint_and_tests.yml`

 * *Files identical despite different names*

### Comparing `pytest_glamor_allure-0.0.8/.gitignore` & `pytest_glamor_allure-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_glamor_allure-0.0.8/LICENSE` & `pytest_glamor_allure-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_glamor_allure-0.0.8/PKG-INFO` & `pytest_glamor_allure-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pytest_glamor_allure
-Version: 0.0.8
+Version: 0.0.9
 Summary: Extends allure-pytest functionality
 Home-page: https://github.com/Denis-Alexeev/pytest-glamor-allure
 Author: Denis Alexeev
 Author-email: github.com@alexeev.ws
 Maintainer: Denis Alexeev
 Maintainer-email: github.com@alexeev.ws
 License: MIT
-Platform: UNKNOWN
 Classifier: Framework :: Pytest
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
@@ -29,14 +28,15 @@
 
 pytest plugin extending allure behaviour
 
 ---
 
 ![](https://github.com/Denis-Alexeev/pytest-glamor-allure/actions/workflows/python-publish.yml/badge.svg)
 ![](https://github.com/Denis-Alexeev/pytest-glamor-allure/actions/workflows/run_lint_and_tests.yml/badge.svg)
+![](https://github.com/Denis-Alexeev/pytest-glamor-allure/actions/workflows/codeql-analysis.yml/badge.svg)
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-glamor-allure)](https://pypi.org/project/pytest-glamor-allure/)
 [![PyPI](https://img.shields.io/pypi/v/pytest-glamor-allure)](https://pypi.org/project/pytest-glamor-allure/)
 [![PyPI - Status](https://img.shields.io/pypi/status/pytest-glamor-allure)](https://pypi.org/project/pytest-glamor-allure/)
 [![Downloads](https://pepy.tech/badge/pytest-glamor-allure)](https://pypi.org/project/pytest-glamor-allure/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![linter: flake8](https://img.shields.io/badge/linter-flake8-blue)](https://pypi.org/project/flake8/)
@@ -316,9 +316,7 @@
 ## Pleasant bonus 🎁<a id="pleasant_bonus"></a>
 
 Type `import pitest as pytest` instead of `import pytest` and get direct access to a bunch of objects from `pytest` and `_pytest` modules.
 
 ## How can I help?<a name="how_help"></a>
 
 Your contribution is highly appreciated. Please read [CONTRIBUTING.md](https://github.com/Denis-Alexeev/pytest-glamor-allure/blob/master/CONTRIBUTING.md) before you start.
-
-
```

### Comparing `pytest_glamor_allure-0.0.8/README.md` & `pytest_glamor_allure-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 pytest plugin extending allure behaviour
 
 ---
 
 ![](https://github.com/Denis-Alexeev/pytest-glamor-allure/actions/workflows/python-publish.yml/badge.svg)
 ![](https://github.com/Denis-Alexeev/pytest-glamor-allure/actions/workflows/run_lint_and_tests.yml/badge.svg)
+![](https://github.com/Denis-Alexeev/pytest-glamor-allure/actions/workflows/codeql-analysis.yml/badge.svg)
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-glamor-allure)](https://pypi.org/project/pytest-glamor-allure/)
 [![PyPI](https://img.shields.io/pypi/v/pytest-glamor-allure)](https://pypi.org/project/pytest-glamor-allure/)
 [![PyPI - Status](https://img.shields.io/pypi/status/pytest-glamor-allure)](https://pypi.org/project/pytest-glamor-allure/)
 [![Downloads](https://pepy.tech/badge/pytest-glamor-allure)](https://pypi.org/project/pytest-glamor-allure/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![linter: flake8](https://img.shields.io/badge/linter-flake8-blue)](https://pypi.org/project/flake8/)
```

### Comparing `pytest_glamor_allure-0.0.8/glamor/__init__.py` & `pytest_glamor_allure-0.0.9/glamor/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_glamor_allure-0.0.8/glamor/patches.py` & `pytest_glamor_allure-0.0.9/glamor/patches.py`

 * *Files identical despite different names*

### Comparing `pytest_glamor_allure-0.0.8/pitest.py` & `pytest_glamor_allure-0.0.9/pitest.py`

 * *Files identical despite different names*

### Comparing `pytest_glamor_allure-0.0.8/pytest_glamor_allure/plugin.py` & `pytest_glamor_allure-0.0.9/pytest_glamor_allure/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_glamor_allure-0.0.8/pytest_glamor_allure.egg-info/PKG-INFO` & `pytest_glamor_allure-0.0.9/pytest_glamor_allure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pytest-glamor-allure
-Version: 0.0.8
+Version: 0.0.9
 Summary: Extends allure-pytest functionality
 Home-page: https://github.com/Denis-Alexeev/pytest-glamor-allure
 Author: Denis Alexeev
 Author-email: github.com@alexeev.ws
 Maintainer: Denis Alexeev
 Maintainer-email: github.com@alexeev.ws
 License: MIT
-Platform: UNKNOWN
 Classifier: Framework :: Pytest
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
@@ -29,14 +28,15 @@
 
 pytest plugin extending allure behaviour
 
 ---
 
 ![](https://github.com/Denis-Alexeev/pytest-glamor-allure/actions/workflows/python-publish.yml/badge.svg)
 ![](https://github.com/Denis-Alexeev/pytest-glamor-allure/actions/workflows/run_lint_and_tests.yml/badge.svg)
+![](https://github.com/Denis-Alexeev/pytest-glamor-allure/actions/workflows/codeql-analysis.yml/badge.svg)
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-glamor-allure)](https://pypi.org/project/pytest-glamor-allure/)
 [![PyPI](https://img.shields.io/pypi/v/pytest-glamor-allure)](https://pypi.org/project/pytest-glamor-allure/)
 [![PyPI - Status](https://img.shields.io/pypi/status/pytest-glamor-allure)](https://pypi.org/project/pytest-glamor-allure/)
 [![Downloads](https://pepy.tech/badge/pytest-glamor-allure)](https://pypi.org/project/pytest-glamor-allure/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![linter: flake8](https://img.shields.io/badge/linter-flake8-blue)](https://pypi.org/project/flake8/)
@@ -316,9 +316,7 @@
 ## Pleasant bonus 🎁<a id="pleasant_bonus"></a>
 
 Type `import pitest as pytest` instead of `import pytest` and get direct access to a bunch of objects from `pytest` and `_pytest` modules.
 
 ## How can I help?<a name="how_help"></a>
 
 Your contribution is highly appreciated. Please read [CONTRIBUTING.md](https://github.com/Denis-Alexeev/pytest-glamor-allure/blob/master/CONTRIBUTING.md) before you start.
-
-
```

### Comparing `pytest_glamor_allure-0.0.8/pytest_glamor_allure.egg-info/SOURCES.txt` & `pytest_glamor_allure-0.0.9/pytest_glamor_allure.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 README.md
 pitest.py
 pyproject.toml
 requirements.txt
 setup.py
 tox.ini
 .github/dependabot.yml
+.github/workflows/codeql-analysis.yml
 .github/workflows/python-publish.yml
 .github/workflows/run_lint_and_tests.yml
 glamor/__init__.py
 glamor/patches.py
 pytest_glamor_allure/__init__.py
 pytest_glamor_allure/_version.py
 pytest_glamor_allure/plugin.py
```

### Comparing `pytest_glamor_allure-0.0.8/setup.py` & `pytest_glamor_allure-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `pytest_glamor_allure-0.0.8/tests/conftest.py` & `pytest_glamor_allure-0.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_glamor_allure-0.0.8/tests/matchers.py` & `pytest_glamor_allure-0.0.9/tests/matchers.py`

 * *Files identical despite different names*

### Comparing `pytest_glamor_allure-0.0.8/tests/test_allure.py` & `pytest_glamor_allure-0.0.9/tests/test_allure.py`

 * *Files identical despite different names*

### Comparing `pytest_glamor_allure-0.0.8/tests/test_glamor_decorators.py` & `pytest_glamor_allure-0.0.9/tests/test_glamor_decorators.py`

 * *Files identical despite different names*

### Comparing `pytest_glamor_allure-0.0.8/tests/test_glamor_dynamic.py` & `pytest_glamor_allure-0.0.9/tests/test_glamor_dynamic.py`

 * *Files identical despite different names*

### Comparing `pytest_glamor_allure-0.0.8/tests/test_glamor_functions.py` & `pytest_glamor_allure-0.0.9/tests/test_glamor_functions.py`

 * *Files identical despite different names*

### Comparing `pytest_glamor_allure-0.0.8/tox.ini` & `pytest_glamor_allure-0.0.9/tox.ini`

 * *Files identical despite different names*

