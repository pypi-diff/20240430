# Comparing `tmp/asyncer_slim-0.0.1.tar.gz` & `tmp/asyncer_slim-0.0.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "asyncer_slim-0.0.7.dev1.tar", last modified: Tue Apr 30 01:08:43 2024, max compression
```

## Comparing `asyncer_slim-0.0.1.tar` & `asyncer_slim-0.0.7.dev1.tar`

### file list

```diff
@@ -1,7 +1,59 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 asyncer_slim-0.0.1/src/asyncer_slim/__about__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 asyncer_slim-0.0.1/src/asyncer_slim/__init__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 asyncer_slim-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 asyncer_slim-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 asyncer_slim-0.0.1/README.md
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 asyncer_slim-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 asyncer_slim-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-04-30 01:08:34.441447 asyncer_slim-0.0.7.dev1/LICENSE
+-rw-r--r--   0        0        0     5297 2024-04-30 01:08:34.441447 asyncer_slim-0.0.7.dev1/README.md
+-rw-r--r--   0        0        0      352 2024-04-30 01:08:34.441447 asyncer_slim-0.0.7.dev1/asyncer/__init__.py
+-rw-r--r--   0        0        0    13107 2024-04-30 01:08:34.441447 asyncer_slim-0.0.7.dev1/asyncer/_main.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:34.441447 asyncer_slim-0.0.7.dev1/asyncer/py.typed
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/tutorial/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/tutorial/asyncify/__init__.py
+-rw-r--r--   0        0        0      201 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/tutorial/asyncify/tutorial001.py
+-rw-r--r--   0        0        0      246 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/tutorial/asyncify/tutorial002.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/tutorial/first_steps/__init__.py
+-rw-r--r--   0        0        0      220 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/tutorial/first_steps/tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/tutorial/runnify/__init__.py
+-rw-r--r--   0        0        0      259 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/tutorial/runnify/tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/tutorial/soonify/__init__.py
+-rw-r--r--   0        0        0      279 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/tutorial/soonify/tutorial001.py
+-rw-r--r--   0        0        0      406 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/tutorial/soonify/tutorial002.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/tutorial/soonify_return/__init__.py
+-rw-r--r--   0        0        0      611 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/tutorial/soonify_return/tutorial001.py
+-rw-r--r--   0        0        0      644 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/tutorial/soonify_return/tutorial002.py
+-rw-r--r--   0        0        0      728 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/tutorial/soonify_return/tutorial003.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/tutorial/syncify/__init__.py
+-rw-r--r--   0        0        0      385 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/tutorial/syncify/tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/tutorial/syncify_no_raise/__init__.py
+-rw-r--r--   0        0        0      505 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/docs_src/tutorial/syncify_no_raise/tutorial001.py
+-rw-r--r--   0        0        0     1722 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/pdm_build.py
+-rw-r--r--   0        0        0     2428 2024-04-30 01:08:43.893420 asyncer_slim-0.0.7.dev1/pyproject.toml
+-rw-r--r--   0        0        0      438 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/requirements-docs.txt
+-rw-r--r--   0        0        0       80 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/requirements-tests.txt
+-rw-r--r--   0        0        0       85 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/requirements.txt
+-rwxr-xr-x   0        0        0      131 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/scripts/docs-live.sh
+-rwxr-xr-x   0        0        0       96 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/scripts/format.sh
+-rwxr-xr-x   0        0        0      126 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/scripts/lint.sh
+-rwxr-xr-x   0        0        0      105 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/scripts/test-files.sh
+-rwxr-xr-x   0        0        0      127 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/scripts/test.sh
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/__init__.py
+-rw-r--r--   0        0        0      309 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/conftest.py
+-rw-r--r--   0        0        0      100 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_others.py
+-rw-r--r--   0        0        0     2690 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_syncify_no_raise.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_tutorial/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_tutorial/test_asyncify/__init__.py
+-rw-r--r--   0        0        0      348 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_tutorial/test_asyncify/test_tutorial001.py
+-rw-r--r--   0        0        0      348 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_tutorial/test_asyncify/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_tutorial/test_first_steps/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_tutorial/test_first_steps/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_tutorial/test_runnify/__init__.py
+-rw-r--r--   0        0        0      351 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_tutorial/test_runnify/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_tutorial/test_soonify/__init__.py
+-rw-r--r--   0        0        0      385 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_tutorial/test_soonify/test_tutorial001.py
+-rw-r--r--   0        0        0      385 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_tutorial/test_soonify/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_tutorial/test_soonify_return/__init__.py
+-rw-r--r--   0        0        0      392 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_tutorial/test_soonify_return/test_tutorial001.py
+-rw-r--r--   0        0        0      833 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_tutorial/test_soonify_return/test_tutorial002.py
+-rw-r--r--   0        0        0      464 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_tutorial/test_soonify_return/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_tutorial/test_syncify/__init__.py
+-rw-r--r--   0        0        0      347 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_tutorial/test_syncify/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_tutorial/test_syncify_no_raise/__init__.py
+-rw-r--r--   0        0        0      379 2024-04-30 01:08:34.449447 asyncer_slim-0.0.7.dev1/tests/test_tutorial/test_syncify_no_raise/test_tutorial001.py
+-rw-r--r--   0        0        0     6612 1970-01-01 00:00:00.000000 asyncer_slim-0.0.7.dev1/PKG-INFO
```

### Comparing `asyncer_slim-0.0.1/LICENSE.txt` & `asyncer_slim-0.0.7.dev1/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,21 @@
-MIT License
+The MIT License (MIT)
 
-Copyright (c) 2023-present Sebastián Ramírez <tiangolo@gmail.com>
+Copyright (c) 2022 Sebastián Ramírez
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

### Comparing `asyncer_slim-0.0.1/pyproject.toml` & `asyncer_slim-0.0.7.dev1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,157 +1,116 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
 
 [project]
 name = "asyncer-slim"
-dynamic = ["version"]
-description = ''
+dynamic = []
+description = "Asyncer, async and await, focused on developer experience."
 readme = "README.md"
-requires-python = ">=3.7"
-license = "MIT"
-keywords = []
+requires-python = ">=3.8"
 authors = [
-  { name = "Sebastián Ramírez", email = "tiangolo@gmail.com" },
+    { name = "Sebastián Ramírez", email = "tiangolo@gmail.com" },
 ]
 classifiers = [
-  "Development Status :: 4 - Beta",
-  "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: Implementation :: CPython",
-  "Programming Language :: Python :: Implementation :: PyPy",
+    "Development Status :: 4 - Beta",
+    "Framework :: AsyncIO",
+    "Framework :: Trio",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Education",
+    "Intended Audience :: Information Technology",
+    "Intended Audience :: Science/Research",
+    "Intended Audience :: System Administrators",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Topic :: Internet",
+    "Typing :: Typed",
+]
+dependencies = [
+    "anyio >=3.4.0,<5.0",
+    "typing_extensions >=4.8.0; python_version < '3.10'",
 ]
-dependencies = []
+version = "0.0.7.dev1"
 
 [project.urls]
-Documentation = "https://github.com/tiangolo/asyncer#readme"
-Issues = "https://github.com/tiangolo/asyncer/issues"
-Source = "https://github.com/tiangolo/asyncer"
+Homepage = "https://github.com/tiangolo/asyncer"
+Documentation = "https://asyncer.tiangolo.com"
+Repository = "https://github.com/tiangolo/asyncer"
+
+[tool.pdm]
+distribution = true
+
+[tool.pdm.version]
+source = "file"
+path = "asyncer/__init__.py"
+
+[tool.pdm.build]
+source-includes = [
+    "tests/",
+    "docs_src/",
+    "requirements*.txt",
+    "scripts/",
+]
+
+[tool.tiangolo._internal-slim-build.packages.asyncer-slim.project]
+name = "asyncer-slim"
 
-[tool.hatch.version]
-path = "src/asyncer_slim/__about__.py"
+[tool.tiangolo._internal-slim-build.packages.asyncer.project.optional-dependencies]
 
-[tool.hatch.envs.default]
-dependencies = [
-  "coverage[toml]>=6.5",
-  "pytest",
+[tool.coverage.run]
+parallel = true
+source = [
+    "docs_src",
+    "tests",
+    "asyncer",
 ]
-[tool.hatch.envs.default.scripts]
-test = "pytest {args:tests}"
-test-cov = "coverage run -m pytest {args:tests}"
-cov-report = [
-  "- coverage combine",
-  "coverage report",
-]
-cov = [
-  "test-cov",
-  "cov-report",
+context = "${CONTEXT}"
+
+[tool.coverage.report]
+omit = [
+    "docs_src/tutorial/soonify_return/tutorial002.py",
 ]
 
-[[tool.hatch.envs.all.matrix]]
-python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
+[tool.mypy]
+strict = true
 
-[tool.hatch.envs.lint]
-detached = true
-dependencies = [
-  "black>=23.1.0",
-  "mypy>=1.0.0",
-  "ruff>=0.0.243",
-]
-[tool.hatch.envs.lint.scripts]
-typing = "mypy --install-types --non-interactive {args:src/asyncer_slim tests}"
-style = [
-  "ruff {args:.}",
-  "black --check --diff {args:.}",
-]
-fmt = [
-  "black {args:.}",
-  "ruff --fix {args:.}",
-  "style",
-]
-all = [
-  "style",
-  "typing",
-]
-
-[tool.black]
-target-version = ["py37"]
-line-length = 120
-skip-string-normalization = true
-
-[tool.ruff]
-target-version = "py37"
-line-length = 120
+[[tool.mypy.overrides]]
+module = "docs_src.*"
+disallow_incomplete_defs = false
+disallow_untyped_defs = false
+disallow_untyped_calls = false
+warn_no_return = false
+
+[tool.ruff.lint]
 select = [
-  "A",
-  "ARG",
-  "B",
-  "C",
-  "DTZ",
-  "E",
-  "EM",
-  "F",
-  "FBT",
-  "I",
-  "ICN",
-  "ISC",
-  "N",
-  "PLC",
-  "PLE",
-  "PLR",
-  "PLW",
-  "Q",
-  "RUF",
-  "S",
-  "T",
-  "TID",
-  "UP",
-  "W",
-  "YTT",
+    "E",
+    "W",
+    "F",
+    "I",
+    "B",
+    "C4",
+    "UP",
 ]
 ignore = [
-  # Allow non-abstract empty methods in abstract base classes
-  "B027",
-  # Allow boolean positional values in function calls, like `dict.get(... True)`
-  "FBT003",
-  # Ignore checks for possible passwords
-  "S105", "S106", "S107",
-  # Ignore complexity
-  "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
-]
-unfixable = [
-  # Don't touch unused imports
-  "F401",
-]
-
-[tool.ruff.isort]
-known-first-party = ["asyncer_slim"]
-
-[tool.ruff.flake8-tidy-imports]
-ban-relative-imports = "all"
-
-[tool.ruff.per-file-ignores]
-# Tests can use magic values, assertions, and relative imports
-"tests/**/*" = ["PLR2004", "S101", "TID252"]
-
-[tool.coverage.run]
-source_pkgs = ["asyncer_slim", "tests"]
-branch = true
-parallel = true
-omit = [
-  "src/asyncer_slim/__about__.py",
+    "E501",
+    "B008",
+    "C901",
+    "W191",
 ]
 
-[tool.coverage.paths]
-asyncer_slim = ["src/asyncer_slim", "*/asyncer-slim/src/asyncer_slim"]
-tests = ["tests", "*/asyncer-slim/tests"]
+[tool.ruff.lint.per-file-ignores]
 
-[tool.coverage.report]
-exclude_lines = [
-  "no cov",
-  "if __name__ == .__main__.:",
-  "if TYPE_CHECKING:",
+[tool.ruff.lint.isort]
+known-third-party = [
+    "asyncer",
+    "anyio",
 ]
+
+[tool.ruff.lint.pyupgrade]
+keep-runtime-typing = true
```

