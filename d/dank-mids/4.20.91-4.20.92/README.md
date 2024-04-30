# Comparing `tmp/dank_mids-4.20.91.tar.gz` & `tmp/dank_mids-4.20.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dank_mids-4.20.91.tar", last modified: Fri Apr 26 20:36:27 2024, max compression
+gzip compressed data, was "dank_mids-4.20.92.tar", last modified: Tue Apr 30 10:14:18 2024, max compression
```

## Comparing `dank_mids-4.20.91.tar` & `dank_mids-4.20.92.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.947580 dank_mids-4.20.91/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.935580 dank_mids-4.20.91/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.939580 dank_mids-4.20.91/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-26 20:36:17.000000 dank_mids-4.20.91/.github/workflows/deploy-docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-26 20:36:17.000000 dank_mids-4.20.91/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-26 20:36:17.000000 dank_mids-4.20.91/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-26 20:36:17.000000 dank_mids-4.20.91/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-26 20:36:17.000000 dank_mids-4.20.91/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-26 20:36:17.000000 dank_mids-4.20.91/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-26 20:36:27.947580 dank_mids-4.20.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-26 20:36:17.000000 dank_mids-4.20.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.939580 dank_mids-4.20.91/dank_mids/
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_batch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.943580 dank_mids-4.20.91/dank_mids/_debugging/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_debugging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_debugging/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_debugging/failures.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_demo_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_envs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    41591 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/_uid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.943580 dank_mids-4.20.91/dank_mids/brownie_patch/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/brownie_patch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/brownie_patch/_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/brownie_patch/_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/brownie_patch/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/brownie_patch/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/brownie_patch/overloaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/brownie_patch/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12236 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.943580 dank_mids-4.20.91/dank_mids/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/helpers/_codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/helpers/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/helpers/_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/semaphore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/semaphores.py
--rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-04-26 20:36:17.000000 dank_mids-4.20.91/dank_mids/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.947580 dank_mids-4.20.91/dank_mids.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-26 20:36:27.000000 dank_mids-4.20.91/dank_mids.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-26 20:36:27.000000 dank_mids-4.20.91/dank_mids.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:36:27.000000 dank_mids-4.20.91/dank_mids.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-26 20:36:27.000000 dank_mids-4.20.91/dank_mids.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 20:36:27.000000 dank_mids-4.20.91/dank_mids.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.943580 dank_mids-4.20.91/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.935580 dank_mids-4.20.91/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.935580 dank_mids-4.20.91/docs/_build/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.947580 dank_mids-4.20.91/docs/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/alabaster.css
--rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-26 20:36:17.000000 dank_mids-4.20.91/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.947580 dank_mids-4.20.91/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-26 20:36:17.000000 dank_mids-4.20.91/examples/dank_brownie_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 20:36:17.000000 dank_mids-4.20.91/license
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-26 20:36:17.000000 dank_mids-4.20.91/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 20:36:17.000000 dank_mids-4.20.91/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-26 20:36:17.000000 dank_mids-4.20.91/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-26 20:36:27.947580 dank_mids-4.20.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-26 20:36:17.000000 dank_mids-4.20.91/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:27.947580 dank_mids-4.20.91/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:17.000000 dank_mids-4.20.91/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-26 20:36:17.000000 dank_mids-4.20.91/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    16155 2024-04-26 20:36:17.000000 dank_mids-4.20.91/tests/test_brownie_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-26 20:36:17.000000 dank_mids-4.20.91/tests/test_dank_mids.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-26 20:36:17.000000 dank_mids-4.20.91/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.149071 dank_mids-4.20.92/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.137071 dank_mids-4.20.92/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.141071 dank_mids-4.20.92/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-30 10:14:06.000000 dank_mids-4.20.92/.github/workflows/deploy-docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-30 10:14:06.000000 dank_mids-4.20.92/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-30 10:14:06.000000 dank_mids-4.20.92/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-30 10:14:06.000000 dank_mids-4.20.92/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-30 10:14:06.000000 dank_mids-4.20.92/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-30 10:14:06.000000 dank_mids-4.20.92/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-30 10:14:18.149071 dank_mids-4.20.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-30 10:14:06.000000 dank_mids-4.20.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.141071 dank_mids-4.20.92/dank_mids/
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.145071 dank_mids-4.20.92/dank_mids/_debugging/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_debugging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_debugging/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_debugging/failures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_demo_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_envs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41591 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_uid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.145071 dank_mids-4.20.92/dank_mids/brownie_patch/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/brownie_patch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/brownie_patch/_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/brownie_patch/_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/brownie_patch/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/brownie_patch/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/brownie_patch/overloaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/brownie_patch/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12236 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.145071 dank_mids-4.20.92/dank_mids/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/helpers/_codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/helpers/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/helpers/_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/semaphores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.149071 dank_mids-4.20.92/dank_mids.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-30 10:14:18.000000 dank_mids-4.20.92/dank_mids.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-30 10:14:18.000000 dank_mids-4.20.92/dank_mids.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 10:14:18.000000 dank_mids-4.20.92/dank_mids.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-30 10:14:18.000000 dank_mids-4.20.92/dank_mids.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 10:14:18.000000 dank_mids-4.20.92/dank_mids.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.145071 dank_mids-4.20.92/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.137071 dank_mids-4.20.92/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.137071 dank_mids-4.20.92/docs/_build/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.149071 dank_mids-4.20.92/docs/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.149071 dank_mids-4.20.92/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-30 10:14:06.000000 dank_mids-4.20.92/examples/dank_brownie_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 10:14:06.000000 dank_mids-4.20.92/license
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-30 10:14:06.000000 dank_mids-4.20.92/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-30 10:14:06.000000 dank_mids-4.20.92/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-30 10:14:06.000000 dank_mids-4.20.92/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-30 10:14:18.149071 dank_mids-4.20.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-30 10:14:06.000000 dank_mids-4.20.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.149071 dank_mids-4.20.92/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:06.000000 dank_mids-4.20.92/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-30 10:14:06.000000 dank_mids-4.20.92/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16155 2024-04-30 10:14:06.000000 dank_mids-4.20.92/tests/test_brownie_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-30 10:14:06.000000 dank_mids-4.20.92/tests/test_dank_mids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-30 10:14:06.000000 dank_mids-4.20.92/tests/test_examples.py
```

### Comparing `dank_mids-4.20.91/.github/workflows/deploy-docs.yaml` & `dank_mids-4.20.92/.github/workflows/deploy-docs.yaml`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/.github/workflows/mypy.yaml` & `dank_mids-4.20.92/.github/workflows/mypy.yaml`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/.github/workflows/pytest.yaml` & `dank_mids-4.20.92/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/.github/workflows/release.yaml` & `dank_mids-4.20.92/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/PKG-INFO` & `dank_mids-4.20.92/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: dank_mids
-Version: 4.20.91
+Version: 4.20.92
 Summary: Multicall batching middleware for asynchronous scripts using web3.py
 Home-page: https://github.com/BobTheBuidler/dank_mids
 Author: BobTheBuidler
 Author-email: bobthebuidlerdefi@gmail.com
 License: MIT
 Requires-Dist: aiofiles
 Requires-Dist: eth_retry<0.2,>=0.1.15
-Requires-Dist: ez-a-sync<0.22,>=0.20.6
+Requires-Dist: ez-a-sync<0.24,>=0.20.6
 Requires-Dist: msgspec
 Requires-Dist: multicall<1,>=0.6.2
 Requires-Dist: typed-envs>=0.0.2
 Requires-Dist: web3!=5.29.*,!=5.30.*,!=5.31.1,!=5.31.2,>=5.27
```

### Comparing `dank_mids-4.20.91/README.md` & `dank_mids-4.20.92/README.md`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/ENVIRONMENT_VARIABLES.py` & `dank_mids-4.20.92/dank_mids/ENVIRONMENT_VARIABLES.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/__init__.py` & `dank_mids-4.20.92/dank_mids/__init__.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/_batch.py` & `dank_mids-4.20.92/dank_mids/_batch.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/_debugging/_base.py` & `dank_mids-4.20.92/dank_mids/_debugging/_base.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/_debugging/failures.py` & `dank_mids-4.20.92/dank_mids/_debugging/failures.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/_exceptions.py` & `dank_mids-4.20.92/dank_mids/_exceptions.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/_mode.py` & `dank_mids-4.20.92/dank_mids/_mode.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/_requests.py` & `dank_mids-4.20.92/dank_mids/_requests.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/_uid.py` & `dank_mids-4.20.92/dank_mids/_uid.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/brownie_patch/__init__.py` & `dank_mids-4.20.92/dank_mids/brownie_patch/__init__.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/brownie_patch/_method.py` & `dank_mids-4.20.92/dank_mids/brownie_patch/_method.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/brownie_patch/call.py` & `dank_mids-4.20.92/dank_mids/brownie_patch/call.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/brownie_patch/contract.py` & `dank_mids-4.20.92/dank_mids/brownie_patch/contract.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/brownie_patch/overloaded.py` & `dank_mids-4.20.92/dank_mids/brownie_patch/overloaded.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/brownie_patch/types.py` & `dank_mids-4.20.92/dank_mids/brownie_patch/types.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/constants.py` & `dank_mids-4.20.92/dank_mids/constants.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/controller.py` & `dank_mids-4.20.92/dank_mids/controller.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/helpers/_codec.py` & `dank_mids-4.20.92/dank_mids/helpers/_codec.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/helpers/_helpers.py` & `dank_mids-4.20.92/dank_mids/helpers/_helpers.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/helpers/_session.py` & `dank_mids-4.20.92/dank_mids/helpers/_session.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/middleware.py` & `dank_mids-4.20.92/dank_mids/middleware.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/semaphores.py` & `dank_mids-4.20.92/dank_mids/semaphores.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/stats.py` & `dank_mids-4.20.92/dank_mids/stats.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids/types.py` & `dank_mids-4.20.92/dank_mids/types.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/dank_mids.egg-info/PKG-INFO` & `dank_mids-4.20.92/dank_mids.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: dank_mids
-Version: 4.20.91
+Version: 4.20.92
 Summary: Multicall batching middleware for asynchronous scripts using web3.py
 Home-page: https://github.com/BobTheBuidler/dank_mids
 Author: BobTheBuidler
 Author-email: bobthebuidlerdefi@gmail.com
 License: MIT
 Requires-Dist: aiofiles
 Requires-Dist: eth_retry<0.2,>=0.1.15
-Requires-Dist: ez-a-sync<0.22,>=0.20.6
+Requires-Dist: ez-a-sync<0.24,>=0.20.6
 Requires-Dist: msgspec
 Requires-Dist: multicall<1,>=0.6.2
 Requires-Dist: typed-envs>=0.0.2
 Requires-Dist: web3!=5.29.*,!=5.30.*,!=5.31.1,!=5.31.2,>=5.27
```

### Comparing `dank_mids-4.20.91/dank_mids.egg-info/SOURCES.txt` & `dank_mids-4.20.92/dank_mids.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/docs/Makefile` & `dank_mids-4.20.92/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/docs/_build/html/_static/alabaster.css` & `dank_mids-4.20.92/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/docs/_build/html/_static/basic.css` & `dank_mids-4.20.92/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/docs/_build/html/_static/doctools.js` & `dank_mids-4.20.92/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/docs/_build/html/_static/language_data.js` & `dank_mids-4.20.92/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/docs/_build/html/_static/pygments.css` & `dank_mids-4.20.92/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/docs/_build/html/_static/searchtools.js` & `dank_mids-4.20.92/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/docs/_build/html/_static/sphinx_highlight.js` & `dank_mids-4.20.92/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/docs/conf.py` & `dank_mids-4.20.92/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 intersphinx_mapping = {
     'a_sync': ('https://bobthebuidler.github.io/ez-a-sync', None),
     'brownie': ('https://eth-brownie.readthedocs.io/en/stable/', None),
     'hexbytes': ('https://hexbytes.readthedocs.io/en/stable/', None),
     'python': ('https://docs.python.org/3', None),
+    'typing_extensions': ('https://typing-extensions.readthedocs.io/en/latest/', None),
     'web3': ('https://web3py.readthedocs.io/en/stable/', None),
 }
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = 'sphinx_rtd_theme'
```

### Comparing `dank_mids-4.20.91/docs/make.bat` & `dank_mids-4.20.92/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/examples/dank_brownie_example.py` & `dank_mids-4.20.92/examples/dank_brownie_example.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/license` & `dank_mids-4.20.92/license`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/setup.py` & `dank_mids-4.20.92/setup.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/tests/test_brownie_patch.py` & `dank_mids-4.20.92/tests/test_brownie_patch.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.91/tests/test_dank_mids.py` & `dank_mids-4.20.92/tests/test_dank_mids.py`

 * *Files identical despite different names*

