# Comparing `tmp/edfio-0.4.0.tar.gz` & `tmp/edfio-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edfio-0.4.0.tar", max compression
+gzip compressed data, was "edfio-0.4.1.tar", max compression
```

## Comparing `edfio-0.4.0.tar` & `edfio-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-12-22 11:01:56.079231 edfio-0.4.0/LICENSE
--rw-r--r--   0        0        0     3322 2023-12-22 11:01:56.083231 edfio-0.4.0/README.md
--rw-r--r--   0        0        0      299 2023-12-22 11:02:05.511189 edfio-0.4.0/edfio/__init__.py
--rw-r--r--   0        0        0     5289 2023-12-22 11:01:56.083231 edfio-0.4.0/edfio/_header_field.py
--rw-r--r--   0        0        0     2532 2023-12-22 11:01:56.083231 edfio-0.4.0/edfio/_utils.py
--rw-r--r--   0        0        0    62379 2023-12-22 11:01:56.083231 edfio-0.4.0/edfio/edf.py
--rw-r--r--   0        0        0        0 2023-12-22 11:01:56.083231 edfio-0.4.0/edfio/py.typed
--rw-r--r--   0        0        0     1607 2023-12-22 11:02:05.511189 edfio-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 edfio-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-30 09:51:37.185584 edfio-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3200 2024-04-30 09:51:37.189584 edfio-0.4.1/README.md
+-rw-r--r--   0        0        0      481 2024-04-30 09:51:37.189584 edfio-0.4.1/edfio/__init__.py
+-rw-r--r--   0        0        0     2349 2024-04-30 09:51:37.189584 edfio-0.4.1/edfio/_header_field.py
+-rw-r--r--   0        0        0    40733 2024-04-30 09:51:37.189584 edfio-0.4.1/edfio/edf.py
+-rw-r--r--   0        0        0     4733 2024-04-30 09:51:37.189584 edfio-0.4.1/edfio/edf_annotations.py
+-rw-r--r--   0        0        0     9612 2024-04-30 09:51:37.189584 edfio-0.4.1/edfio/edf_header.py
+-rw-r--r--   0        0        0    14927 2024-04-30 09:51:37.189584 edfio-0.4.1/edfio/edf_signal.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:51:37.189584 edfio-0.4.1/edfio/py.typed
+-rw-r--r--   0        0        0     1577 2024-04-30 09:51:48.585663 edfio-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 edfio-0.4.1/PKG-INFO
```

### Comparing `edfio-0.4.0/LICENSE` & `edfio-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edfio-0.4.0/README.md` & `edfio-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 [![PyPI](https://img.shields.io/pypi/v/edfio)](https://pypi.org/project/edfio/)
 [![conda-forge](https://img.shields.io/conda/v/conda-forge/edfio.svg?label=conda-forge)](https://anaconda.org/conda-forge/edfio)
 [![License](https://img.shields.io/pypi/l/edfio)](https://github.com/the-siesta-group/edfio/blob/main/LICENSE)
 [![Docs](https://readthedocs.org/projects/edfio/badge)](https://edfio.readthedocs.io/en/stable/index.html)
 
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Linting: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 edfio is a Python package for reading and writing [EDF](https://www.edfplus.info/specs/edf.html) and [EDF+C](https://www.edfplus.info/specs/edfplus.html) files.
 
 It requires Python>=3.9 and NumPy>=1.22 and is available on PyPI:
 
     pip install edfio
```

### Comparing `edfio-0.4.0/pyproject.toml` & `edfio-0.4.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edfio"
-version = "0.4.0"
+version = "0.4.1"
 description = "Read and write EDF/EDF+ files."
 license = "Apache-2.0"
 authors = ["The Siesta Group <opensource@thesiestagroup.com>"]
 readme = "README.md"
 repository = "https://github.com/the-siesta-group/edfio"
 documentation = "https://edfio.readthedocs.io"
 
@@ -12,34 +12,35 @@
 python = "^3.9"
 numpy = ">=1.22.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "7.4.3"
 pytest-cov = "4.1.0"
 pre-commit = "3.5.0"
-black = "23.11.0"
 mypy = "1.6.1"
-ruff = "0.1.5"
+ruff = "0.3.4"
 sphinx = "7.2.6"
 myst-parser = "2.0.0"
 pydata-sphinx-theme = "0.14.3"
 numpydoc = "1.6.0"
 
 [tool.poetry-dynamic-versioning]
 vcs = "git"
 style = "semver"
+enable = false
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.black]
-target-version = ["py39", "py310", "py311", "py312"]
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.ruff]
+target-version = "py39"
+fix = true
+
+[tool.ruff.lint]
 select = [
     "F",
     "E",
     "W",
     "I",
     "N",
     "D",
@@ -55,31 +56,27 @@
     "RET",
     "TID",
     "PTH",
     "PL",
     "RUF",
 ]
 ignore = ["E501", "E741", "B028", "D100", "D104", "D105", "PLR0913"]
-target-version = "py39"
-fix = true
 fixable = ["I001"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*" = ["S101", "PLR2004", "B018", "D"]
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
 [tool.mypy]
 python_version = "3.9"
 ignore_missing_imports = true
 disallow_untyped_defs = true
 warn_unreachable = true
 strict_equality = true
 pretty = true
+warn_unused_ignores = true
 packages = ["edfio"]
-
-[tool.coverage.report]
-exclude_lines = ["@abstractmethod", "@overload"]
```

### Comparing `edfio-0.4.0/PKG-INFO` & `edfio-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edfio
-Version: 0.4.0
+Version: 0.4.1
 Summary: Read and write EDF/EDF+ files.
 Home-page: https://github.com/the-siesta-group/edfio
 License: Apache-2.0
 Author: The Siesta Group
 Author-email: opensource@thesiestagroup.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -24,16 +24,15 @@
 [![PyPI](https://img.shields.io/pypi/v/edfio)](https://pypi.org/project/edfio/)
 [![conda-forge](https://img.shields.io/conda/v/conda-forge/edfio.svg?label=conda-forge)](https://anaconda.org/conda-forge/edfio)
 [![License](https://img.shields.io/pypi/l/edfio)](https://github.com/the-siesta-group/edfio/blob/main/LICENSE)
 [![Docs](https://readthedocs.org/projects/edfio/badge)](https://edfio.readthedocs.io/en/stable/index.html)
 
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Linting: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 
 edfio is a Python package for reading and writing [EDF](https://www.edfplus.info/specs/edf.html) and [EDF+C](https://www.edfplus.info/specs/edfplus.html) files.
 
 It requires Python>=3.9 and NumPy>=1.22 and is available on PyPI:
 
     pip install edfio
```

