# Comparing `tmp/pyaction-0.5.7.tar.gz` & `tmp/pyaction-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaction-0.5.7.tar", last modified: Fri Apr 19 14:54:07 2024, max compression
+gzip compressed data, was "pyaction-0.6.0.tar", last modified: Tue Apr 30 20:30:34 2024, max compression
```

## Comparing `pyaction-0.5.7.tar` & `pyaction-0.6.0.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:54:07.970106 pyaction-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-19 14:54:03.000000 pyaction-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 14:54:03.000000 pyaction-0.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-19 14:54:07.970106 pyaction-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-19 14:54:03.000000 pyaction-0.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:54:07.966106 pyaction-0.5.7/pyaction/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:54:07.966106 pyaction-0.5.7/pyaction/issues/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/issues/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/issues/rendering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:54:07.966106 pyaction-0.5.7/pyaction/template/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/template/copier.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:54:07.966106 pyaction-0.5.7/pyaction/template/{{action_slug}}/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/template/{{action_slug}}/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/template/{{action_slug}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/template/{{action_slug}}/Dockerfile.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/template/{{action_slug}}/README.md.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/template/{{action_slug}}/action.yml.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/template/{{action_slug}}/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/template/{{action_slug}}/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:54:07.962106 pyaction-0.5.7/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:54:07.966106 pyaction-0.5.7/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/test.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:54:07.970106 pyaction-0.5.7/pyaction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-19 14:54:07.000000 pyaction-0.5.7/pyaction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-19 14:54:07.000000 pyaction-0.5.7/pyaction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:54:07.000000 pyaction-0.5.7/pyaction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 14:54:07.000000 pyaction-0.5.7/pyaction.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-19 14:54:07.000000 pyaction-0.5.7/pyaction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 14:54:07.000000 pyaction-0.5.7/pyaction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-19 14:54:03.000000 pyaction-0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:54:07.970106 pyaction-0.5.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:30:34.593747 pyaction-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-30 20:30:30.000000 pyaction-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 20:30:30.000000 pyaction-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-30 20:30:34.593747 pyaction-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-30 20:30:30.000000 pyaction-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:30:34.589748 pyaction-0.6.0/pyaction/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:30:34.589748 pyaction-0.6.0/pyaction/issues/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/issues/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/issues/rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:30:34.589748 pyaction-0.6.0/pyaction/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/template/copier.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:30:34.589748 pyaction-0.6.0/pyaction/template/{{action_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/template/{{action_slug}}/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/template/{{action_slug}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/template/{{action_slug}}/Dockerfile.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/template/{{action_slug}}/README.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/template/{{action_slug}}/action.yml.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/template/{{action_slug}}/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/template/{{action_slug}}/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:30:34.585747 pyaction-0.6.0/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:30:34.589748 pyaction-0.6.0/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:30:34.589748 pyaction-0.6.0/pyaction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-30 20:30:34.000000 pyaction-0.6.0/pyaction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-30 20:30:34.000000 pyaction-0.6.0/pyaction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:30:34.000000 pyaction-0.6.0/pyaction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-30 20:30:34.000000 pyaction-0.6.0/pyaction.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-30 20:30:34.000000 pyaction-0.6.0/pyaction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 20:30:34.000000 pyaction-0.6.0/pyaction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 20:30:34.593747 pyaction-0.6.0/setup.cfg
```

### Comparing `pyaction-0.5.7/LICENSE` & `pyaction-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.7/PKG-INFO` & `pyaction-0.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaction
-Version: 0.5.7
+Version: 0.6.0
 Summary: Create GitHub Actions using Python
 Author-email: Sadra Yahyapour <lnxpylnxpy@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sadra Yahyapour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,38 +23,42 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Documentation, https://pyaction.imsadra.me
 Project-URL: Repository, https://github.com/lnxpy/pyaction
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: copier>=9.2
 Requires-Dist: click>=8.1
+Requires-Dist: pydantic>=2.7.0
 Requires-Dist: pygithub>=2.3.0
-Requires-Dist: markdown-to-json==2.1.0
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pytest-cookies; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: cairosvg; extra == "docs"
 Requires-Dist: pillow; extra == "docs"
 
-## PyAction ![Version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyaction?logo=python&logoColor=949DA5&label=Python&labelColor=2A3035) [![Package Testing](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml) [![Docs CI](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml)
+## PyAction ![Version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version) ![Python Versions](https://img.shields.io/pypi/pyversions/pyaction?logo=python&logoColor=949DA5&label=Python&labelColor=2A3035) [![codecov](https://codecov.io/gh/lnxpy/pyaction/graph/badge.svg?token=59XAONX5S1)](https://codecov.io/gh/lnxpy/pyaction) [![Package Testing](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml) [![Docs CI](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml)
 
 PyAction helps you to develop [GitHub Actions](https://docs.github.com/en/actions) using Python. It's delivered as an installable package with the ability to test the action locally before any deployment.
 
 Check out the [official docs](https://pyaction.imsadra.me) for more detailed information. There is also a [Quickstart](https://pyaction.imsadra.me/quickstart) demo tutorial that walks you through a simple hello-world action.
 
 ### Requirements
 - Python >= 3.8
```

### Comparing `pyaction-0.5.7/README.md` & `pyaction-0.6.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## PyAction ![Version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyaction?logo=python&logoColor=949DA5&label=Python&labelColor=2A3035) [![Package Testing](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml) [![Docs CI](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml)
+## PyAction ![Version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version) ![Python Versions](https://img.shields.io/pypi/pyversions/pyaction?logo=python&logoColor=949DA5&label=Python&labelColor=2A3035) [![codecov](https://codecov.io/gh/lnxpy/pyaction/graph/badge.svg?token=59XAONX5S1)](https://codecov.io/gh/lnxpy/pyaction) [![Package Testing](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml) [![Docs CI](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml)
 
 PyAction helps you to develop [GitHub Actions](https://docs.github.com/en/actions) using Python. It's delivered as an installable package with the ability to test the action locally before any deployment.
 
 Check out the [official docs](https://pyaction.imsadra.me) for more detailed information. There is also a [Quickstart](https://pyaction.imsadra.me/quickstart) demo tutorial that walks you through a simple hello-world action.
 
 ### Requirements
 - Python >= 3.8
```

### Comparing `pyaction-0.5.7/pyaction/cli.py` & `pyaction-0.6.0/pyaction/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import subprocess
 
 import click
 from copier import run_copy
 
 from pyaction import __version__
-from pyaction.consts import TEMPLATE_PATH, PROJECT_NAME
+from pyaction.consts import PROJECT_NAME, TEMPLATE_PATH
 
 
 @click.version_option(
     __version__,
     prog_name=PROJECT_NAME,
     message="%(prog)s - v%(version)s",
 )
```

### Comparing `pyaction-0.5.7/pyaction/io.py` & `pyaction-0.6.0/pyaction/io.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,50 @@
+from __future__ import annotations
+
 import os
-from typing import Dict
+from contextlib import nullcontext
+from io import TextIOWrapper
 
 from pyaction.consts import GITHUB_OUTPUT
 from pyaction.exceptions import WorkflowParameterNotFound
 
 
-def write(context: Dict[str, str]) -> None:
-    """writes the key(s) (as variables) and value(s) (as values) to the output env variable
+def write(context: dict[str, str], stream: str | TextIOWrapper = GITHUB_OUTPUT) -> None:
+    """writes the key(s) (as variables) and value(s) (as values) to the output stream
 
     Args:
-        context: variables and values
+        context (dict[str, str]): variables and values
+        stream (str, TextIOWrapper): output stream (set to STDOUT locally and `GITHUB_OUTPUT` on production)
 
     Examples:
-        In your project, use this function like:
+        In your action, use this function like:
 
         >>> write({"name": "John", "age": 20, ...})
 
-        `name` will be the variable name and `John` is the value.
+        `name` and `age` are the variables and `John` and `20` are the values.
     """
 
-    with open(GITHUB_OUTPUT, "a") as _env:
+    with nullcontext(stream) if isinstance(stream, TextIOWrapper) else open(
+        stream, "w+"
+    ) as streamline:
         for var, val in context.items():
-            _env.write(f"{var}={val}\r\n")
+            streamline.write(f"{var}={val}\r\n")
 
 
 def read(param: str) -> str | int | bool | None:
     """reads a parameter from the inputs
 
     Args:
         param (str): parameter name
 
+    Raises:
+        WorkflowParameterNotFound: if the `param` is missing
+
     Returns:
-        str | int | bool: value of `param`
+        str | int | bool | None: value of `param`
     """
 
     prefix = "INPUT_"
     var_name = prefix + param.upper()
 
     try:
         value = os.environ[var_name]
```

### Comparing `pyaction-0.5.7/pyaction/issues/connector.py` & `pyaction-0.6.0/pyaction/issues/connector.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.7/pyaction/template/copier.yml` & `pyaction-0.6.0/pyaction/template/copier.yml`

 * *Files identical despite different names*

### Comparing `pyaction-0.5.7/pyaction.egg-info/PKG-INFO` & `pyaction-0.6.0/pyaction.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaction
-Version: 0.5.7
+Version: 0.6.0
 Summary: Create GitHub Actions using Python
 Author-email: Sadra Yahyapour <lnxpylnxpy@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sadra Yahyapour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,38 +23,42 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Documentation, https://pyaction.imsadra.me
 Project-URL: Repository, https://github.com/lnxpy/pyaction
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: copier>=9.2
 Requires-Dist: click>=8.1
+Requires-Dist: pydantic>=2.7.0
 Requires-Dist: pygithub>=2.3.0
-Requires-Dist: markdown-to-json==2.1.0
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: pytest-cookies; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: cairosvg; extra == "docs"
 Requires-Dist: pillow; extra == "docs"
 
-## PyAction ![Version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyaction?logo=python&logoColor=949DA5&label=Python&labelColor=2A3035) [![Package Testing](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml) [![Docs CI](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml)
+## PyAction ![Version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version) ![Python Versions](https://img.shields.io/pypi/pyversions/pyaction?logo=python&logoColor=949DA5&label=Python&labelColor=2A3035) [![codecov](https://codecov.io/gh/lnxpy/pyaction/graph/badge.svg?token=59XAONX5S1)](https://codecov.io/gh/lnxpy/pyaction) [![Package Testing](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml) [![Docs CI](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml)
 
 PyAction helps you to develop [GitHub Actions](https://docs.github.com/en/actions) using Python. It's delivered as an installable package with the ability to test the action locally before any deployment.
 
 Check out the [official docs](https://pyaction.imsadra.me) for more detailed information. There is also a [Quickstart](https://pyaction.imsadra.me/quickstart) demo tutorial that walks you through a simple hello-world action.
 
 ### Requirements
 - Python >= 3.8
```

### Comparing `pyaction-0.5.7/pyaction.egg-info/SOURCES.txt` & `pyaction-0.6.0/pyaction.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 pyproject.toml
 pyaction/__init__.py
 pyaction/auth.py
 pyaction/cli.py
 pyaction/consts.py
 pyaction/exceptions.py
 pyaction/io.py
+pyaction/logger.py
+pyaction/utils.py
+pyaction/workflow.py
 pyaction.egg-info/PKG-INFO
 pyaction.egg-info/SOURCES.txt
 pyaction.egg-info/dependency_links.txt
 pyaction.egg-info/entry_points.txt
 pyaction.egg-info/requires.txt
 pyaction.egg-info/top_level.txt
 pyaction/issues/__init__.py
```

### Comparing `pyaction-0.5.7/pyproject.toml` & `pyaction-0.6.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyaction"
-version = "0.5.7"
+version = "0.6.0"
 description = "Create GitHub Actions using Python"
 authors = [{ name = "Sadra Yahyapour", email = "lnxpylnxpy@gmail.com" }]
 requires-python = ">=3.8"
 dependencies = [
     "copier >= 9.2",
     "click >= 8.1",
+    "pydantic >= 2.7.0",
     "pygithub >= 2.3.0",
-    "markdown-to-json == 2.1.0",
 ]
 readme = { file = "README.md", content-type = "text/markdown" }
 license = { file = "LICENSE" }
 classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Environment :: Console",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3 :: Only",
 ]
 
 [project.scripts]
 pyaction = "pyaction.cli:cli"
 
 [project.optional-dependencies]
 dev = ["coverage", "pytest-cookies"]
 docs = ["mkdocs-material", "cairosvg", "pillow"]
 
 [project.urls]
 Documentation = "https://pyaction.imsadra.me"
 Repository = "https://github.com/lnxpy/pyaction"
 
 [tool.bumpversion]
-current_version = "0.5.7"
+current_version = "0.6.0"
 commit = "true"
 tag = "true"
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 
 [[tool.bumpversion.files]]
```

