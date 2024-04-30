# Comparing `tmp/adafruit_circuitpython_connectionmanager-1.2.0.tar.gz` & `tmp/adafruit_circuitpython_connectionmanager-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit_circuitpython_connectionmanager-1.2.0.tar", last modified: Sun Apr 28 04:21:43 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_connectionmanager-1.2.1.tar", last modified: Mon Apr 29 19:14:54 2024, max compression
```

## Comparing `adafruit_circuitpython_connectionmanager-1.2.0.tar` & `adafruit_circuitpython_connectionmanager-1.2.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.792328 adafruit_circuitpython_connectionmanager-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.784328 adafruit_circuitpython_connectionmanager-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.784328 adafruit_circuitpython_connectionmanager-1.2.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.788328 adafruit_circuitpython_connectionmanager-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.788328 adafruit_circuitpython_connectionmanager-1.2.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-28 04:21:43.792328 adafruit_circuitpython_connectionmanager-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.792328 adafruit_circuitpython_connectionmanager-1.2.0/adafruit_circuitpython_connectionmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-28 04:21:43.000000 adafruit_circuitpython_connectionmanager-1.2.0/adafruit_circuitpython_connectionmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-28 04:21:43.000000 adafruit_circuitpython_connectionmanager-1.2.0/adafruit_circuitpython_connectionmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 04:21:43.000000 adafruit_circuitpython_connectionmanager-1.2.0/adafruit_circuitpython_connectionmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-28 04:21:43.000000 adafruit_circuitpython_connectionmanager-1.2.0/adafruit_circuitpython_connectionmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-28 04:21:43.000000 adafruit_circuitpython_connectionmanager-1.2.0/adafruit_circuitpython_connectionmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11910 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/adafruit_connection_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.788328 adafruit_circuitpython_connectionmanager-1.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.788328 adafruit_circuitpython_connectionmanager-1.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.792328 adafruit_circuitpython_connectionmanager-1.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/examples/connectionmanager_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11045 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/examples/connectionmanager_ssltest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 04:21:43.792328 adafruit_circuitpython_connectionmanager-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:21:43.792328 adafruit_circuitpython_connectionmanager-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/close_socket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/connection_manager_close_all_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/free_socket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/get_connection_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/get_radio_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/get_socket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/mocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/protocol_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-28 04:21:41.000000 adafruit_circuitpython_connectionmanager-1.2.0/tests/ssl_context_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-28 04:21:34.000000 adafruit_circuitpython_connectionmanager-1.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:54.805358 adafruit_circuitpython_connectionmanager-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:54.793358 adafruit_circuitpython_connectionmanager-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:54.797358 adafruit_circuitpython_connectionmanager-1.2.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:54.797358 adafruit_circuitpython_connectionmanager-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:54.797358 adafruit_circuitpython_connectionmanager-1.2.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-29 19:14:54.801358 adafruit_circuitpython_connectionmanager-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:54.801358 adafruit_circuitpython_connectionmanager-1.2.1/adafruit_circuitpython_connectionmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-29 19:14:54.000000 adafruit_circuitpython_connectionmanager-1.2.1/adafruit_circuitpython_connectionmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-29 19:14:54.000000 adafruit_circuitpython_connectionmanager-1.2.1/adafruit_circuitpython_connectionmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:14:54.000000 adafruit_circuitpython_connectionmanager-1.2.1/adafruit_circuitpython_connectionmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-29 19:14:54.000000 adafruit_circuitpython_connectionmanager-1.2.1/adafruit_circuitpython_connectionmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-29 19:14:54.000000 adafruit_circuitpython_connectionmanager-1.2.1/adafruit_circuitpython_connectionmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12913 2024-04-29 19:14:52.000000 adafruit_circuitpython_connectionmanager-1.2.1/adafruit_connection_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:54.801358 adafruit_circuitpython_connectionmanager-1.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:54.801358 adafruit_circuitpython_connectionmanager-1.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:54.801358 adafruit_circuitpython_connectionmanager-1.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-29 19:14:52.000000 adafruit_circuitpython_connectionmanager-1.2.1/examples/connectionmanager_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11045 2024-04-29 19:14:52.000000 adafruit_circuitpython_connectionmanager-1.2.1/examples/connectionmanager_ssltest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-29 19:14:52.000000 adafruit_circuitpython_connectionmanager-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 19:14:54.805358 adafruit_circuitpython_connectionmanager-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:14:54.801358 adafruit_circuitpython_connectionmanager-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-29 19:14:52.000000 adafruit_circuitpython_connectionmanager-1.2.1/tests/close_socket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-29 19:14:52.000000 adafruit_circuitpython_connectionmanager-1.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-04-29 19:14:52.000000 adafruit_circuitpython_connectionmanager-1.2.1/tests/connection_manager_close_all_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-29 19:14:52.000000 adafruit_circuitpython_connectionmanager-1.2.1/tests/free_socket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-29 19:14:52.000000 adafruit_circuitpython_connectionmanager-1.2.1/tests/get_connection_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-29 19:14:52.000000 adafruit_circuitpython_connectionmanager-1.2.1/tests/get_radio_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-04-29 19:14:52.000000 adafruit_circuitpython_connectionmanager-1.2.1/tests/get_socket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-29 19:14:52.000000 adafruit_circuitpython_connectionmanager-1.2.1/tests/mocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-29 19:14:52.000000 adafruit_circuitpython_connectionmanager-1.2.1/tests/protocol_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-29 19:14:52.000000 adafruit_circuitpython_connectionmanager-1.2.1/tests/ssl_context_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-29 19:14:45.000000 adafruit_circuitpython_connectionmanager-1.2.1/tox.ini
```

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_connectionmanager-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/.gitignore` & `adafruit_circuitpython_connectionmanager-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/.pre-commit-config.yaml` & `adafruit_circuitpython_connectionmanager-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/.pylintrc` & `adafruit_circuitpython_connectionmanager-1.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_connectionmanager-1.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/LICENSE` & `adafruit_circuitpython_connectionmanager-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_connectionmanager-1.2.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/LICENSES/MIT.txt` & `adafruit_circuitpython_connectionmanager-1.2.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/LICENSES/Unlicense.txt` & `adafruit_circuitpython_connectionmanager-1.2.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/PKG-INFO` & `adafruit_circuitpython_connectionmanager-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-connectionmanager
-Version: 1.2.0
+Version: 1.2.1
 Summary: A urllib3.poolmanager/urllib3.connectionpool-like library for managing sockets and connections
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ConnectionManager
 Keywords: adafruit,blinka,circuitpython,micropython,connectionmanager,sockets,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/README.rst` & `adafruit_circuitpython_connectionmanager-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/adafruit_circuitpython_connectionmanager.egg-info/PKG-INFO` & `adafruit_circuitpython_connectionmanager-1.2.1/adafruit_circuitpython_connectionmanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-connectionmanager
-Version: 1.2.0
+Version: 1.2.1
 Summary: A urllib3.poolmanager/urllib3.connectionpool-like library for managing sockets and connections
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ConnectionManager
 Keywords: adafruit,blinka,circuitpython,micropython,connectionmanager,sockets,networking
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/adafruit_circuitpython_connectionmanager.egg-info/SOURCES.txt` & `adafruit_circuitpython_connectionmanager-1.2.1/adafruit_circuitpython_connectionmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/adafruit_connection_manager.py` & `adafruit_circuitpython_connectionmanager-1.2.1/adafruit_connection_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 
 """
 
 # imports
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ConnectionManager.git"
 
 import errno
 import sys
 
 WIZNET5K_SSL_SUPPORT_VERSION = (9, 1)
 
@@ -95,20 +95,21 @@
        <https://www.adafruit.com/product/4264>`_
     """
     socket_pool.set_interface(iface)
     return _FakeSSLContext(iface)
 
 
 _global_connection_managers = {}
+_global_key_by_socketpool = {}
 _global_socketpools = {}
 _global_ssl_contexts = {}
 
 
 def get_radio_socketpool(radio):
-    """Helper to get a socket pool for common boards
+    """Helper to get a socket pool for common boards.
 
     Currently supported:
 
      * Boards with onboard WiFi (ESP32S2, ESP32S3, Pico W, etc)
      * Using the ESP32 WiFi Co-Processor (like the Adafruit AirLift)
      * Using a WIZ5500 (Like the Adafruit Ethernet FeatherWing)
     """
@@ -147,22 +148,23 @@
 
             if ssl_context is None:
                 ssl_context = create_fake_ssl_context(pool, radio)
 
         else:
             raise AttributeError(f"Unsupported radio class: {class_name}")
 
+        _global_key_by_socketpool[pool] = class_name
         _global_socketpools[class_name] = pool
         _global_ssl_contexts[class_name] = ssl_context
 
     return _global_socketpools[class_name]
 
 
 def get_radio_ssl_context(radio):
-    """Helper to get ssl_contexts for common boards
+    """Helper to get ssl_contexts for common boards.
 
     Currently supported:
 
      * Boards with onboard WiFi (ESP32S2, ESP32S3, Pico W, etc)
      * Using the ESP32 WiFi Co-Processor (like the Adafruit AirLift)
      * Using a WIZ5500 (Like the Adafruit Ethernet FeatherWing)
     """
@@ -171,15 +173,15 @@
     return _global_ssl_contexts[class_name]
 
 
 # main class
 
 
 class ConnectionManager:
-    """Connection manager for sharing open sockets (aka connections)."""
+    """A library for managing sockets accross libraries."""
 
     def __init__(
         self,
         socket_pool: SocketpoolModuleType,
     ) -> None:
         self._socket_pool = socket_pool
         # Hang onto open sockets so that we can reuse them.
@@ -224,34 +226,38 @@
             socket.close()
             return exc
 
         return socket
 
     @property
     def available_socket_count(self) -> int:
-        """Get the count of freeable open sockets"""
+        """Get the count of available (freed) managed sockets."""
         return len(self._available_sockets)
 
     @property
     def managed_socket_count(self) -> int:
-        """Get the count of open sockets"""
+        """Get the count of managed sockets."""
         return len(self._managed_socket_by_key)
 
     def close_socket(self, socket: SocketType) -> None:
-        """Close a previously opened socket."""
+        """
+        Close a previously managed and connected socket.
+
+        - **socket_pool** *(SocketType)* – The socket you want to close
+        """
         if socket not in self._managed_socket_by_key.values():
             raise RuntimeError("Socket not managed")
         socket.close()
         key = self._key_by_managed_socket.pop(socket)
         del self._managed_socket_by_key[key]
         if socket in self._available_sockets:
             self._available_sockets.remove(socket)
 
     def free_socket(self, socket: SocketType) -> None:
-        """Mark a previously opened socket as available so it can be reused if needed."""
+        """Mark a managed socket as available so it can be reused."""
         if socket not in self._managed_socket_by_key.values():
             raise RuntimeError("Socket not managed")
         self._available_sockets.add(socket)
 
     def get_socket(
         self,
         host: str,
@@ -259,15 +265,28 @@
         proto: str,
         session_id: Optional[str] = None,
         *,
         timeout: float = 1,
         is_ssl: bool = False,
         ssl_context: Optional[SSLContextType] = None,
     ) -> CircuitPythonSocketType:
-        """Get a new socket and connect"""
+        """
+        Get a new socket and connect.
+
+        - **host** *(str)* – The host you are want to connect to: "www.adaftuit.com"
+        - **port** *(int)* – The port you want to connect to: 80
+        - **proto** *(str)* – The protocal you want to use: "http:"
+        - **session_id** *(Optional[str])* – A unique Session ID, when wanting to have multiple open
+          connections to the same host
+        - **timeout** *(float)* – Time timeout used for connecting
+        - **is_ssl** *(bool)* – If the connection is to be over SSL (auto set when proto is
+          "https:")
+        - **ssl_context** *(Optional[SSLContextType])* – The SSL context to use when making SSL
+          requests
+        """
         if session_id:
             session_id = str(session_id)
         key = (host, port, proto, session_id)
         if key in self._managed_socket_by_key:
             socket = self._managed_socket_by_key[key]
             if socket in self._available_sockets:
                 self._available_sockets.remove(socket)
@@ -311,43 +330,48 @@
 
 # global helpers
 
 
 def connection_manager_close_all(
     socket_pool: Optional[SocketpoolModuleType] = None, release_references: bool = False
 ) -> None:
-    """Close all open sockets for pool"""
+    """
+    Close all open sockets for pool, optionally release references.
+
+    - **socket_pool** *(Optional[SocketpoolModuleType])* – A specifc SocketPool you want to close
+      sockets for, leave blank for all SocketPools
+    - **release_references** *(bool)* – Set to True if you want to also clear stored references to
+      the SocketPool and SSL contexts
+    """
     if socket_pool:
         socket_pools = [socket_pool]
     else:
         socket_pools = _global_connection_managers.keys()
 
     for pool in socket_pools:
         connection_manager = _global_connection_managers.get(pool, None)
         if connection_manager is None:
             raise RuntimeError("SocketPool not managed")
 
         connection_manager._free_sockets(force=True)  # pylint: disable=protected-access
 
-        if release_references:
-            radio_key = None
-            for radio_check, pool_check in _global_socketpools.items():
-                if pool == pool_check:
-                    radio_key = radio_check
-                    break
-
-            if radio_key:
-                if radio_key in _global_socketpools:
-                    del _global_socketpools[radio_key]
+        if not release_references:
+            continue
 
-                if radio_key in _global_ssl_contexts:
-                    del _global_ssl_contexts[radio_key]
+        key = _global_key_by_socketpool.pop(pool)
+        if key:
+            _global_socketpools.pop(key, None)
+            _global_ssl_contexts.pop(key, None)
 
-            if pool in _global_connection_managers:
-                del _global_connection_managers[pool]
+        _global_connection_managers.pop(pool, None)
 
 
 def get_connection_manager(socket_pool: SocketpoolModuleType) -> ConnectionManager:
-    """Get the ConnectionManager singleton for the given pool"""
+    """
+    Get the ConnectionManager singleton for the given pool.
+
+    - **socket_pool** *(Optional[SocketpoolModuleType])* – The SocketPool you want the
+      ConnectionManager for
+    """
     if socket_pool not in _global_connection_managers:
         _global_connection_managers[socket_pool] = ConnectionManager(socket_pool)
     return _global_connection_managers[socket_pool]
```

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/docs/_static/favicon.ico` & `adafruit_circuitpython_connectionmanager-1.2.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/docs/conf.py` & `adafruit_circuitpython_connectionmanager-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/docs/examples.rst` & `adafruit_circuitpython_connectionmanager-1.2.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/docs/index.rst` & `adafruit_circuitpython_connectionmanager-1.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/examples/connectionmanager_helpers.py` & `adafruit_circuitpython_connectionmanager-1.2.1/examples/connectionmanager_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,39 +23,39 @@
 ssl_context = adafruit_connection_manager.get_radio_ssl_context(radio)
 
 # get request session
 requests = adafruit_requests.Session(pool, ssl_context)
 connection_manager = adafruit_connection_manager.get_connection_manager(pool)
 print("-" * 40)
 print("Nothing yet opened")
-print(f"Open Sockets: {connection_manager.managed_socket_count}")
-print(f"Freeable Open Sockets: {connection_manager.available_socket_count}")
+print(f"Managed Sockets: {connection_manager.managed_socket_count}")
+print(f"Available Managed Sockets: {connection_manager.available_socket_count}")
 
 # make request
 print("-" * 40)
 print(f"Fetching from {TEXT_URL} in a context handler")
 with requests.get(TEXT_URL) as response:
     response_text = response.text
     print(f"Text Response {response_text}")
 
 print("-" * 40)
-print("1 request, opened and freed")
-print(f"Open Sockets: {connection_manager.managed_socket_count}")
-print(f"Freeable Open Sockets: {connection_manager.available_socket_count}")
+print("1 request, opened and closed")
+print(f"Managed Sockets: {connection_manager.managed_socket_count}")
+print(f"Available Managed Sockets: {connection_manager.available_socket_count}")
 
 print("-" * 40)
 print(f"Fetching from {TEXT_URL} not in a context handler")
 response = requests.get(TEXT_URL)
 
 print("-" * 40)
-print("1 request, opened but not freed")
-print(f"Open Sockets: {connection_manager.managed_socket_count}")
-print(f"Freeable Open Sockets: {connection_manager.available_socket_count}")
+print("1 request, opened but not closed")
+print(f"Managed Sockets: {connection_manager.managed_socket_count}")
+print(f"Available Managed Sockets: {connection_manager.available_socket_count}")
 
 print("-" * 40)
 print("Closing everything in the pool")
 adafruit_connection_manager.connection_manager_close_all(pool)
 
 print("-" * 40)
 print("Everything closed")
-print(f"Open Sockets: {connection_manager.managed_socket_count}")
-print(f"Freeable Open Sockets: {connection_manager.available_socket_count}")
+print(f"Managed Sockets: {connection_manager.managed_socket_count}")
+print(f"Available Managed Sockets: {connection_manager.available_socket_count}")
```

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/examples/connectionmanager_ssltest.py` & `adafruit_circuitpython_connectionmanager-1.2.1/examples/connectionmanager_ssltest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/pyproject.toml` & `adafruit_circuitpython_connectionmanager-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-connectionmanager"
 description = "A urllib3.poolmanager/urllib3.connectionpool-like library for managing sockets and connections"
-version = "1.2.0"
+version = "1.2.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ConnectionManager"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/tests/close_socket_test.py` & `adafruit_circuitpython_connectionmanager-1.2.1/tests/close_socket_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/tests/conftest.py` & `adafruit_circuitpython_connectionmanager-1.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/tests/connection_manager_close_all_test.py` & `adafruit_circuitpython_connectionmanager-1.2.1/tests/connection_manager_close_all_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/tests/free_socket_test.py` & `adafruit_circuitpython_connectionmanager-1.2.1/tests/free_socket_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/tests/get_connection_manager_test.py` & `adafruit_circuitpython_connectionmanager-1.2.1/tests/get_connection_manager_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/tests/get_radio_test.py` & `adafruit_circuitpython_connectionmanager-1.2.1/tests/get_radio_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/tests/get_socket_test.py` & `adafruit_circuitpython_connectionmanager-1.2.1/tests/get_socket_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/tests/mocket.py` & `adafruit_circuitpython_connectionmanager-1.2.1/tests/mocket.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/tests/protocol_test.py` & `adafruit_circuitpython_connectionmanager-1.2.1/tests/protocol_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/tests/ssl_context_test.py` & `adafruit_circuitpython_connectionmanager-1.2.1/tests/ssl_context_test.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_connectionmanager-1.2.0/tox.ini` & `adafruit_circuitpython_connectionmanager-1.2.1/tox.ini`

 * *Files identical despite different names*

