# Comparing `tmp/adafruit_circuitpython_wiznet5k-6.0.0.tar.gz` & `tmp/adafruit_circuitpython_wiznet5k-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit_circuitpython_wiznet5k-6.0.0.tar", last modified: Sat Apr 27 13:58:59 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_wiznet5k-7.0.0.tar", last modified: Tue Apr 30 15:57:36 2024, max compression
```

## Comparing `adafruit_circuitpython_wiznet5k-6.0.0.tar` & `adafruit_circuitpython_wiznet5k-7.0.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.212026 adafruit_circuitpython_wiznet5k-6.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.204026 adafruit_circuitpython_wiznet5k-6.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.208026 adafruit_circuitpython_wiznet5k-6.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.208026 adafruit_circuitpython_wiznet5k-6.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.208026 adafruit_circuitpython_wiznet5k-6.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-27 13:58:59.212026 adafruit_circuitpython_wiznet5k-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.212026 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_circuitpython_wiznet5k.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-27 13:58:59.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-27 13:58:59.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 13:58:59.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-27 13:58:59.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 13:58:59.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.212026 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51779 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    26273 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11431 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
--rw-r--r--   0 runner    (1001) docker     (127)    29999 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k_socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.212026 adafruit_circuitpython_wiznet5k-6.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.212026 adafruit_circuitpython_wiznet5k-6.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:59.212026 adafruit_circuitpython_wiznet5k-6.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_aio_post.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2159 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_cheerlights.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1085 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_cpython_client_for_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_httpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_simpletest_manual_network.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-27 13:58:56.000000 adafruit_circuitpython_wiznet5k-6.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-27 13:58:49.000000 adafruit_circuitpython_wiznet5k-6.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 13:58:59.212026 adafruit_circuitpython_wiznet5k-6.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.901717 adafruit_circuitpython_wiznet5k-7.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.893717 adafruit_circuitpython_wiznet5k-7.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.897717 adafruit_circuitpython_wiznet5k-7.0.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.897717 adafruit_circuitpython_wiznet5k-7.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.897717 adafruit_circuitpython_wiznet5k-7.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-30 15:57:36.901717 adafruit_circuitpython_wiznet5k-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.901717 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_circuitpython_wiznet5k.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-30 15:57:36.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-30 15:57:36.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:57:36.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-30 15:57:36.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 15:57:36.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.901717 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51779 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26273 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11431 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31487 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k_socketpool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.901717 adafruit_circuitpython_wiznet5k-7.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.901717 adafruit_circuitpython_wiznet5k-7.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.901717 adafruit_circuitpython_wiznet5k-7.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_aio_post.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2159 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_cheerlights.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1085 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_cpython_client_for_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_httpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_simpletest_manual_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:57:36.901717 adafruit_circuitpython_wiznet5k-7.0.0/setup.cfg
```

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_wiznet5k-7.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/.gitignore` & `adafruit_circuitpython_wiznet5k-7.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/.pre-commit-config.yaml` & `adafruit_circuitpython_wiznet5k-7.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/.pylintrc` & `adafruit_circuitpython_wiznet5k-7.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_wiznet5k-7.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/LICENSE` & `adafruit_circuitpython_wiznet5k-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_wiznet5k-7.0.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/LICENSES/MIT.txt` & `adafruit_circuitpython_wiznet5k-7.0.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/LICENSES/Unlicense.txt` & `adafruit_circuitpython_wiznet5k-7.0.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/PKG-INFO` & `adafruit_circuitpython_wiznet5k-7.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wiznet5k
-Version: 6.0.0
+Version: 7.0.0
 Summary: Pure-Python interface for WIZNET 5k ethernet modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
 Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/README.rst` & `adafruit_circuitpython_wiznet5k-7.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO` & `adafruit_circuitpython_wiznet5k-7.0.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wiznet5k
-Version: 6.0.0
+Version: 7.0.0
 Summary: Pure-Python interface for WIZNET 5k ethernet modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
 Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt` & `adafruit_circuitpython_wiznet5k-7.0.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 adafruit_circuitpython_wiznet5k.egg-info/requires.txt
 adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
 adafruit_wiznet5k/__init__.py
 adafruit_wiznet5k/adafruit_wiznet5k.py
 adafruit_wiznet5k/adafruit_wiznet5k_debug.py
 adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
 adafruit_wiznet5k/adafruit_wiznet5k_dns.py
-adafruit_wiznet5k/adafruit_wiznet5k_socket.py
+adafruit_wiznet5k/adafruit_wiznet5k_socketpool.py
 docs/api.rst
 docs/api.rst.license
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
```

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k.py` & `adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         import digitalio
 
         IpAddress4Raw = Union[bytes, Tuple[int, int, int, int]]
         MacAddressRaw = Union[bytes, Tuple[int, int, int, int, int, int]]
 except ImportError:
     pass
 
-__version__ = "6.0.0"
+__version__ = "7.0.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k.git"
 
 from random import randint
 import time
 import gc
 from micropython import const
 from adafruit_ticks import ticks_ms, ticks_diff
```

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py` & `adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py` & `adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py` & `adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/adafruit_wiznet5k/adafruit_wiznet5k_socket.py` & `adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k_socketpool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 # SPDX-FileCopyrightText: 2019 ladyada for Adafruit Industries
 # SPDX-FileCopyrightText: 2020 Brent Rubell for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
-#
-# CPython uses type as an argument in socket.socket, so disable checking in Pylint
-# pylint: disable=redefined-builtin
 """
-`adafruit_wiznet5k_socket`
+`adafruit_wiznet5k_socketpool`
 ================================================================================
 
 A socket compatible interface with the Wiznet5k module.
 
 * Author(s): ladyada, Brent Rubell, Patrick Van Oosterwijck, Adam Cummick, Martin Stephens
 
 """
@@ -29,252 +26,263 @@
 from errno import ETIMEDOUT
 
 from micropython import const
 from adafruit_ticks import ticks_ms, ticks_diff
 
 import adafruit_wiznet5k as wiznet5k
 
-# pylint: disable=invalid-name
-_the_interface: Optional[WIZNET5K] = None
-_default_socket_timeout = None
-
-
-def _is_ipv4_string(ipv4_address: str) -> bool:
-    """Check for a valid IPv4 address in dotted-quad string format
-    (for example, "123.45.67.89").
-
-    :param: str ipv4_address: The string to test.
 
-    :return bool: True if a valid IPv4 address, False otherwise.
-    """
-    octets = ipv4_address.split(".", 3)
-    if len(octets) == 4 and "".join(octets).isdigit():
-        if all((0 <= int(octet) <= 255 for octet in octets)):
-            return True
-    return False
-
-
-def set_interface(iface: WIZNET5K) -> None:
-    """
-    Helper to set the global internet interface.
-
-    :param wiznet5k.adafruit_wiznet5k.WIZNET5K iface: The ethernet interface.
-    """
-    global _the_interface  # pylint: disable=global-statement, invalid-name
-    _the_interface = iface
-
-
-def getdefaulttimeout() -> Optional[float]:
-    """
-    Return the default timeout in seconds for new socket objects. A value of
-    None indicates that new socket objects have no timeout. When the socket module is
-    first imported, the default is None.
-    """
-    return _default_socket_timeout
+_SOCKET_TYPE_TO_WIZNET = b"\0\x21\2"
+_SOCKET_INVALID = const(255)
 
+_global_socketpool = {}
 
-def setdefaulttimeout(_timeout: Optional[float]) -> None:
-    """
-    Set the default timeout in seconds (float) for new socket objects. When the socket
-    module is first imported, the default is None. See settimeout() for possible values
-    and their respective meanings.
 
-    :param Optional[float] _timeout: The default timeout in seconds or None.
-    """
-    global _default_socket_timeout  # pylint: disable=global-statement
-    if _timeout is None or _timeout >= 0:
-        _default_socket_timeout = _timeout
-    else:
-        raise ValueError("Timeout must be None, 0.0 or a positive numeric value.")
+class SocketPoolContants:  # pylint: disable=too-few-public-methods
+    """Helper class for the constants that are needed everywhere"""
 
+    # These must match circuitpython "socketpoool" values. However, we cannot
+    # depend on socketpool being importable, so hard-code them here.
+    SOCK_STREAM = 1
+    SOCK_DGRAM = 2
 
-def htonl(x: int) -> int:
-    """
-    Convert 32-bit positive integer from host to network byte order.
+    SOL_SOCKET = 0xFFF
+    SO_REUSEADDR = 0x0004
 
-    :param int x: 32-bit positive integer from host.
+    AF_INET = const(3)
 
-    :return int: 32-bit positive integer in network byte order.
-    """
-    if byteorder == "big":
-        return x
-    return int.from_bytes(x.to_bytes(4, "little"), "big")
 
+class SocketPool(SocketPoolContants):
+    """WIZNET5K SocketPool library"""
 
-def htons(x: int) -> int:
-    """
-    Convert 16-bit positive integer from host to network byte order.
+    def __new__(cls, iface: WIZNET5K):
+        # We want to make sure to return the same pool for the same interface
+        if iface not in _global_socketpool:
+            _global_socketpool[iface] = super().__new__(cls)
+        return _global_socketpool[iface]
 
-    :param int x: 16-bit positive integer from host.
+    def __init__(self, iface: WIZNET5K):
+        self._interface = iface
+        self._default_socket_timeout = None
 
-    :return int: 16-bit positive integer in network byte order.
-    """
-    if byteorder == "big":
-        return x
-    return ((x << 8) & 0xFF00) | ((x >> 8) & 0xFF)
+    @staticmethod
+    def _is_ipv4_string(ipv4_address: str) -> bool:
+        """Check for a valid IPv4 address in dotted-quad string format
+        (for example, "123.45.67.89").
 
+        :param: str ipv4_address: The string to test.
 
-def inet_aton(ip_address: str) -> bytes:
-    """
-    Convert an IPv4 address from dotted-quad string format (for example, "123.45.67.89")
-    to 32-bit packed binary format, as a bytes object four characters in length. This is
-    useful when conversing with a program that uses the standard C library and needs
-    objects of type struct in_addr, which is the C type for the 32-bit packed binary this
-    function returns.
+        :return bool: True if a valid IPv4 address, False otherwise.
+        """
+        octets = ipv4_address.split(".", 3)
+        if len(octets) == 4 and "".join(octets).isdigit():
+            if all((0 <= int(octet) <= 255 for octet in octets)):
+                return True
+        return False
 
-    :param str ip_address: The IPv4 address to convert.
+    def getdefaulttimeout(self) -> Optional[float]:
+        """
+        Return the default timeout in seconds for new socket objects. A value of
+        None indicates that new socket objects have no timeout. When the socket module is
+        first imported, the default is None.
+        """
+        return self._default_socket_timeout
 
-    :return bytes: The converted IPv4 address.
-    """
-    if not _is_ipv4_string(ip_address):
-        raise ValueError("The IPv4 address must be a dotted-quad string.")
-    return _the_interface.unpretty_ip(ip_address)
+    def setdefaulttimeout(self, _timeout: Optional[float]) -> None:
+        """
+        Set the default timeout in seconds (float) for new socket objects. When the socket
+        module is first imported, the default is None. See settimeout() for possible values
+        and their respective meanings.
 
+        :param Optional[float] _timeout: The default timeout in seconds or None.
+        """
+        if _timeout is None or _timeout >= 0:
+            self._default_socket_timeout = _timeout
+        else:
+            raise ValueError("Timeout must be None, 0.0 or a positive numeric value.")
 
-def inet_ntoa(ip_address: Union[bytes, bytearray]) -> str:
-    """
-    Convert a 32-bit packed IPv4 address (a bytes-like object four bytes in length) to
-    its standard dotted-quad string representation (for example, ‘123.45.67.89’). This is
-    useful when conversing with a program that uses the standard C library and needs
-    objects of type struct in_addr, which is the C type for the 32-bit packed binary data
-    this function takes as an argument.
+    @staticmethod
+    def htonl(x: int) -> int:
+        """
+        Convert 32-bit positive integer from host to network byte order.
 
-    :param Union[bytes, bytearray ip_address: The IPv4 address to convert.
+        :param int x: 32-bit positive integer from host.
 
-    :return str: The converted ip_address:
-    """
-    if len(ip_address) != 4:
-        raise ValueError("The IPv4 address must be 4 bytes.")
-    return _the_interface.pretty_ip(ip_address)
+        :return int: 32-bit positive integer in network byte order.
+        """
+        if byteorder == "big":
+            return x
+        return int.from_bytes(x.to_bytes(4, "little"), "big")
 
+    @staticmethod
+    def htons(x: int) -> int:
+        """
+        Convert 16-bit positive integer from host to network byte order.
 
-# These must match circuitpython "socketpoool" values. However, we cannot
-# depend on socketpool being importable, so hard-code them here.
-SOCK_STREAM = 1
-SOCK_DGRAM = 2
+        :param int x: 16-bit positive integer from host.
 
-_SOCKET_TYPE_TO_WIZNET = b"\0\x21\2"
+        :return int: 16-bit positive integer in network byte order.
+        """
+        if byteorder == "big":
+            return x
+        return ((x << 8) & 0xFF00) | ((x >> 8) & 0xFF)
 
-SOL_SOCKET = 0xFFF
-SO_REUSEADDR = 0x0004
+    def inet_aton(self, ip_address: str) -> bytes:
+        """
+        Convert an IPv4 address from dotted-quad string format (for example, "123.45.67.89")
+        to 32-bit packed binary format, as a bytes object four characters in length. This is
+        useful when conversing with a program that uses the standard C library and needs
+        objects of type struct in_addr, which is the C type for the 32-bit packed binary this
+        function returns.
 
-AF_INET = const(3)
-_SOCKET_INVALID = const(255)
+        :param str ip_address: The IPv4 address to convert.
 
+        :return bytes: The converted IPv4 address.
+        """
+        if not self._is_ipv4_string(ip_address):
+            raise ValueError("The IPv4 address must be a dotted-quad string.")
+        return self._interface.unpretty_ip(ip_address)
 
-# pylint: disable=too-many-arguments, unused-argument
-def getaddrinfo(
-    host: str,
-    port: int,
-    family: int = 0,
-    type: int = 0,
-    proto: int = 0,
-    flags: int = 0,
-) -> List[Tuple[int, int, int, str, Tuple[str, int]]]:
-    """
-    Translate the host/port argument into a sequence of 5-tuples that contain all the necessary
-    arguments for creating a socket connected to that service.
+    def inet_ntoa(self, ip_address: Union[bytes, bytearray]) -> str:
+        """
+        Convert a 32-bit packed IPv4 address (a bytes-like object four bytes in length) to
+        its standard dotted-quad string representation (for example, ‘123.45.67.89’). This is
+        useful when conversing with a program that uses the standard C library and needs
+        objects of type struct in_addr, which is the C type for the 32-bit packed binary data
+        this function takes as an argument.
 
-    :param str host: a domain name, a string representation of an IPv4 address or
-        None.
-    :param int port: Port number to connect to (0 - 65536).
-    :param int family: Ignored and hardcoded as 0x03 (the only family implemented) by the function.
-    :param int type: The type of socket, either SOCK_STREAM (0x21) for TCP or SOCK_DGRAM (0x02)
-        for UDP, defaults to 0.
-    :param int proto: Unused in this implementation of socket.
-    :param int flags: Unused in this implementation of socket.
-
-    :return List[Tuple[int, int, int, str, Tuple[str, int]]]: Address info entries in the form
-        (family, type, proto, canonname, sockaddr). In these tuples, family, type, proto are meant
-        to be passed to the socket() function. canonname will always be an empty string, sockaddr
-        is a tuple describing a socket address, whose format is (address, port), and is meant to be
-        passed to the socket.connect() method.
-    """
-    if not isinstance(port, int):
-        raise ValueError("Port must be an integer")
-    if not _is_ipv4_string(host):
-        host = gethostbyname(host)
-    return [(AF_INET, type, proto, "", (host, port))]
+        :param Union[bytes, bytearray ip_address: The IPv4 address to convert.
 
+        :return str: The converted ip_address:
+        """
+        if len(ip_address) != 4:
+            raise ValueError("The IPv4 address must be 4 bytes.")
+        return self._interface.pretty_ip(ip_address)
 
-def gethostbyname(hostname: str) -> str:
-    """
-    Translate a host name to IPv4 address format. The IPv4 address is returned as a string, such
-    as '100.50.200.5'. If the host name is an IPv4 address itself it is returned unchanged.
+    def getaddrinfo(  # pylint: disable=redefined-builtin,too-many-arguments,unused-argument
+        self,
+        host: str,
+        port: int,
+        family: int = 0,
+        type: int = 0,
+        proto: int = 0,
+        flags: int = 0,
+    ) -> List[Tuple[int, int, int, str, Tuple[str, int]]]:
+        """
+        Translate the host/port argument into a sequence of 5-tuples that contain all the necessary
+        arguments for creating a socket connected to that service.
 
-    :param str hostname: Hostname to lookup.
+        :param str host: a domain name, a string representation of an IPv4 address or
+            None.
+        :param int port: Port number to connect to (0 - 65536).
+        :param int family: Ignored and hardcoded as 0x03 (the only family implemented) by the
+            function.
+        :param int type: The type of socket, either SOCK_STREAM (0x21) for TCP or SOCK_DGRAM (0x02)
+            for UDP, defaults to 0.
+        :param int proto: Unused in this implementation of socket.
+        :param int flags: Unused in this implementation of socket.
+
+        :return List[Tuple[int, int, int, str, Tuple[str, int]]]: Address info entries in the form
+            (family, type, proto, canonname, sockaddr). In these tuples, family, type, proto are
+            meant to be passed to the socket() function. canonname will always be an empty string,
+            sockaddr is a tuple describing a socket address, whose format is (address, port), and
+            is meant to be passed to the socket.connect() method.
+        """
+        if not isinstance(port, int):
+            raise ValueError("Port must be an integer")
+        if not self._is_ipv4_string(host):
+            host = self.gethostbyname(host)
+        return [(SocketPoolContants.AF_INET, type, proto, "", (host, port))]
+
+    def gethostbyname(self, hostname: str) -> str:
+        """
+        Translate a host name to IPv4 address format. The IPv4 address is returned as a string, such
+        as '100.50.200.5'. If the host name is an IPv4 address itself it is returned unchanged.
+
+        :param str hostname: Hostname to lookup.
+
+        :return str: IPv4 address (a string of the form '0.0.0.0').
+        """
+        if self._is_ipv4_string(hostname):
+            return hostname
+        address = self._interface.get_host_by_name(hostname)
+        address = "{}.{}.{}.{}".format(address[0], address[1], address[2], address[3])
+        return address
 
-    :return str: IPv4 address (a string of the form '0.0.0.0').
-    """
-    if _is_ipv4_string(hostname):
-        return hostname
-    address = _the_interface.get_host_by_name(hostname)
-    address = "{}.{}.{}.{}".format(address[0], address[1], address[2], address[3])
-    return address
+    def socket(  # pylint: disable=redefined-builtin
+        self,
+        family: int = SocketPoolContants.AF_INET,
+        type: int = SocketPoolContants.SOCK_STREAM,
+        proto: int = 0,
+        fileno: Optional[int] = None,
+    ):
+        """Create a new socket and return it"""
+        return Socket(self, family, type, proto, fileno)
 
 
-# pylint: disable=invalid-name, too-many-public-methods
-class socket:
+class Socket:
     """
     A simplified implementation of the Python 'socket' class for connecting
     to a Wiznet5k module.
     """
 
-    # pylint: disable=redefined-builtin,unused-argument
-    def __init__(
+    def __init__(  # pylint: disable=redefined-builtin,too-many-arguments,unused-argument
         self,
-        family: int = AF_INET,
-        type: int = SOCK_STREAM,
+        socket_pool: SocketPool,
+        family: int = SocketPool.AF_INET,
+        type: int = SocketPool.SOCK_STREAM,
         proto: int = 0,
         fileno: Optional[int] = None,
     ) -> None:
         """
         :param int family: Socket address (and protocol) family, defaults to AF_INET.
         :param int type: Socket type, use SOCK_STREAM for TCP and SOCK_DGRAM for UDP,
             defaults to SOCK_STREAM.
         :param int proto: Unused, retained for compatibility.
         :param Optional[int] fileno: Unused, retained for compatibility.
         """
-        if family != AF_INET:
+        if family != SocketPool.AF_INET:
             raise RuntimeError("Only AF_INET family supported by W5K modules.")
+        self._socket_pool = socket_pool
+        self._interface = self._socket_pool._interface
         self._socket_closed = False
         self._sock_type = type
         self._buffer = b""
-        self._timeout = _default_socket_timeout
+        self._timeout = self._socket_pool._default_socket_timeout
         self._listen_port = None
 
-        self._socknum = _the_interface.get_socket(reserve_socket=True)
+        self._socknum = self._interface.get_socket(reserve_socket=True)
         if self._socknum == _SOCKET_INVALID:
             raise RuntimeError("Failed to allocate socket.")
 
     def __del__(self):
-        _the_interface.release_socket(self._socknum)
+        self._interface.release_socket(self._socknum)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
-        _the_interface.release_socket(self._socknum)
-        if self._sock_type == SOCK_STREAM:
-            _the_interface.write_snir(
+        self._interface.release_socket(self._socknum)
+        if self._sock_type == SocketPool.SOCK_STREAM:
+            self._interface.write_snir(
                 self._socknum, 0xFF & (~wiznet5k.adafruit_wiznet5k.SNIR_DISCON)
             )  # Reset socket interrupt register.
-            _the_interface.socket_disconnect(self._socknum)
+            self._interface.socket_disconnect(self._socknum)
             mask = (
                 wiznet5k.adafruit_wiznet5k.SNIR_TIMEOUT
                 | wiznet5k.adafruit_wiznet5k.SNIR_DISCON
             )
-            while not _the_interface.read_snir(self._socknum) & mask:
+            while not self._interface.read_snir(self._socknum) & mask:
                 pass
-        _the_interface.write_snir(
+        self._interface.write_snir(
             self._socknum, 0xFF
         )  # Reset socket interrupt register.
-        _the_interface.socket_close(self._socknum)
+        self._interface.socket_close(self._socknum)
         while (
-            _the_interface.socket_status(self._socknum)
+            self._interface.socket_status(self._socknum)
             != wiznet5k.adafruit_wiznet5k.SNSR_SOCK_CLOSED
         ):
             pass
 
     # This works around problems with using a class method as a decorator.
     def _check_socket_closed(func):  # pylint: disable=no-self-argument
         """Decorator to check whether the socket object has been closed."""
@@ -289,28 +297,27 @@
     @property
     def _status(self) -> int:
         """
         Return the status of the socket.
 
         :return int: Status of the socket.
         """
-        return _the_interface.socket_status(self._socknum)
+        return self._interface.socket_status(self._socknum)
 
     @property
     def _connected(self) -> bool:
         """
         Return whether connected to the socket.
 
         :return bool: Whether connected.
         """
-        # pylint: disable=protected-access
 
-        if self._socknum >= _the_interface.max_sockets:
+        if self._socknum >= self._interface.max_sockets:
             return False
-        status = _the_interface.socket_status(self._socknum)
+        status = self._interface.socket_status(self._socknum)
         if (
             status == wiznet5k.adafruit_wiznet5k.SNSR_SOCK_CLOSE_WAIT
             and self._available() == 0
         ):
             result = False
         else:
             result = status not in (
@@ -326,15 +333,15 @@
     @_check_socket_closed
     def getpeername(self) -> Tuple[str, int]:
         """
         Return the remote address to which the socket is connected.
 
         :return Tuple[str, int]: IPv4 address and port the socket is connected to.
         """
-        return _the_interface.remote_ip(self._socknum), _the_interface.remote_port(
+        return self._interface.remote_ip(self._socknum), self._interface.remote_port(
             self._socknum
         )
 
     @_check_socket_closed
     def bind(self, address: Tuple[Optional[str], int]) -> None:
         """
         Bind the socket to address. The socket must not already be bound.
@@ -356,50 +363,50 @@
         """
         Helper function to allow bind() to check for an existing connection and for
         accept() to generate a new socket connection.
 
         :param Tuple[Optional[str], int] address: Address as a (host, port) tuple.
         """
         if address[0]:
-            if gethostbyname(address[0]) != _the_interface.pretty_ip(
-                _the_interface.ip_address
+            if self._socket_pool.gethostbyname(address[0]) != self._interface.pretty_ip(
+                self._interface.ip_address
             ):
                 raise ValueError(
                     "The IPv4 address requested must match {}, "
                     "the one assigned to the WIZNET5K interface.".format(
-                        _the_interface.pretty_ip(_the_interface.ip_address)
+                        self._interface.pretty_ip(self._interface.ip_address)
                     )
                 )
         self._listen_port = address[1]
         # For UDP servers we need to open the socket here because we won't call
         # listen
-        if self._sock_type == SOCK_DGRAM:
-            _the_interface.socket_listen(
+        if self._sock_type == SocketPool.SOCK_DGRAM:
+            self._interface.socket_listen(
                 self._socknum,
                 self._listen_port,
                 wiznet5k.adafruit_wiznet5k.SNMR_UDP,
             )
             self._buffer = b""
 
     @_check_socket_closed
-    def listen(self, backlog: int = 0) -> None:
+    def listen(self, backlog: int = 0) -> None:  # pylint: disable=unused-argument
         """
         Enable a server to accept connections.
 
         :param int backlog: Included for compatibility but ignored.
         """
         if self._listen_port is None:
             raise RuntimeError("Use bind to set the port before listen!")
-        _the_interface.socket_listen(self._socknum, self._listen_port)
+        self._interface.socket_listen(self._socknum, self._listen_port)
         self._buffer = b""
 
     @_check_socket_closed
     def accept(
         self,
-    ) -> Tuple[socket, Tuple[str, int]]:
+    ) -> Tuple[Socket, Tuple[str, int]]:
         """
         Accept a connection. The socket must be bound to an address and listening for connections.
 
         :return Tuple[socket, Tuple[str, int]]: The return value is a pair
             (conn, address) where conn is a new socket object to send and receive data on
             the connection, and address is the address bound to the socket on the other
             end of the connection.
@@ -418,18 +425,18 @@
             if self._status == wiznet5k.adafruit_wiznet5k.SNSR_SOCK_CLOSE_WAIT:
                 self._disconnect()
                 self.listen()
             if self._status == wiznet5k.adafruit_wiznet5k.SNSR_SOCK_CLOSED:
                 self.close()
                 self.listen()
 
-        _, addr = _the_interface.socket_accept(self._socknum)
+        _, addr = self._interface.socket_accept(self._socknum)
         current_socknum = self._socknum
         # Create a new socket object and swap socket nums, so we can continue listening
-        client_sock = socket()
+        client_sock = Socket(self._socket_pool)
         self._socknum = client_sock._socknum  # pylint: disable=protected-access
         client_sock._socknum = current_socknum  # pylint: disable=protected-access
         self._bind((None, self._listen_port))
         self.listen()
         if self._status != wiznet5k.adafruit_wiznet5k.SNSR_SOCK_LISTEN:
             raise RuntimeError("Failed to open new listening socket")
         return client_sock, addr
@@ -438,22 +445,22 @@
     def connect(self, address: Tuple[str, int]) -> None:
         """
         Connect to a remote socket at address.
 
         :param Tuple[str, int] address: Remote socket as a (host, port) tuple.
         """
         if self._listen_port is not None:
-            _the_interface.src_port = self._listen_port
-        result = _the_interface.socket_connect(
+            self._interface.src_port = self._listen_port
+        result = self._interface.socket_connect(
             self._socknum,
-            _the_interface.unpretty_ip(gethostbyname(address[0])),
+            self._interface.unpretty_ip(self._socket_pool.gethostbyname(address[0])),
             address[1],
             _SOCKET_TYPE_TO_WIZNET[self._sock_type],
         )
-        _the_interface.src_port = 0
+        self._interface.src_port = 0
         if not result:
             raise RuntimeError("Failed to connect to host ", address[0])
         self._buffer = b""
 
     @_check_socket_closed
     def send(self, data: Union[bytes, bytearray]) -> int:
         """
@@ -463,15 +470,15 @@
         delivery of the remaining data.
 
         :param bytearray data: Data to send to the socket.
 
         :return int: Number of bytes sent.
         """
         _timeout = 0 if self._timeout is None else self._timeout
-        bytes_sent = _the_interface.socket_write(self._socknum, data, _timeout)
+        bytes_sent = self._interface.socket_write(self._socknum, data, _timeout)
         gc.collect()
         return bytes_sent
 
     @_check_socket_closed
     def sendto(self, data: bytearray, *flags_and_or_address: any) -> int:
         """
         Send data to the socket. The socket should not be connected to a remote socket, since the
@@ -492,16 +499,15 @@
             address = other_args[-1]
         else:
             raise ValueError("Incorrect number of arguments, should be 2 or 3.")
         self.connect(address)
         return self.send(data)
 
     @_check_socket_closed
-    def recv(
-        # pylint: disable=too-many-branches
+    def recv(  # pylint: disable=unused-argument
         self,
         bufsize: int,
         flags: int = 0,
     ) -> bytes:
         """
         Receive data from the socket. The return value is a bytes object representing the data
         received. The maximum amount of data to be received at once is specified by bufsize.
@@ -515,61 +521,65 @@
         nread = self.recv_into(buf, bufsize)
         if nread == 0:
             return b""
         if nread < bufsize:
             return bytes(buf[:nread])
         return bytes(buf)
 
-    def _embed_recv(
+    def _embed_recv(  # pylint: disable=unused-argument
         self, bufsize: int = 0, flags: int = 0
-    ) -> bytes:  # pylint: disable=too-many-branches
+    ) -> bytes:
         """
         Read from the connected remote address.
 
         :param int bufsize: Maximum number of bytes to receive, ignored by the
             function, defaults to 0.
         :param int flags: ignored, present for compatibility.
 
         :return bytes: All data available from the connection.
         """
         avail = self._available()
         if avail:
-            if self._sock_type == SOCK_STREAM:
-                self._buffer += _the_interface.socket_read(self._socknum, avail)[1]
-            elif self._sock_type == SOCK_DGRAM:
-                self._buffer += _the_interface.read_udp(self._socknum, avail)[1]
+            if self._sock_type == SocketPool.SOCK_STREAM:
+                self._buffer += self._interface.socket_read(self._socknum, avail)[1]
+            elif self._sock_type == SocketPool.SOCK_DGRAM:
+                self._buffer += self._interface.read_udp(self._socknum, avail)[1]
         gc.collect()
         ret = self._buffer
         self._buffer = b""
         gc.collect()
         return ret
 
     @_check_socket_closed
-    def recvfrom(self, bufsize: int, flags: int = 0) -> Tuple[bytes, Tuple[str, int]]:
+    def recvfrom(  # pylint: disable=unused-argument
+        self, bufsize: int, flags: int = 0
+    ) -> Tuple[bytes, Tuple[str, int]]:
         """
         Receive data from the socket. The return value is a pair (bytes, address) where bytes is
         a bytes object representing the data received and address is the address of the socket
         sending the data.
 
         :param int bufsize: Maximum number of bytes to receive.
         :param int flags: Ignored, present for compatibility.
 
         :return Tuple[bytes, Tuple[str, int]]: a tuple (bytes, address)
             where address is a tuple (address, port)
         """
         return (
             self.recv(bufsize),
             (
-                _the_interface.pretty_ip(_the_interface.udp_from_ip[self._socknum]),
-                _the_interface.udp_from_port[self._socknum],
+                self._interface.pretty_ip(self._interface.udp_from_ip[self._socknum]),
+                self._interface.udp_from_port[self._socknum],
             ),
         )
 
     @_check_socket_closed
-    def recv_into(self, buffer: bytearray, nbytes: int = 0, flags: int = 0) -> int:
+    def recv_into(  # pylint: disable=unused-argument
+        self, buffer: bytearray, nbytes: int = 0, flags: int = 0
+    ) -> int:
         """
         Receive up to nbytes bytes from the socket, storing the data into a buffer
         rather than creating a new bytestring.
 
         :param bytearray buffer: Data buffer to read into.
         :param nbytes: Maximum number of bytes to receive (if 0, use length of buffer).
         :param int flags: ignored, present for compatibility.
@@ -596,20 +606,20 @@
                 # explicitly recheck num_to_read to avoid extra checks
                 continue
 
             num_avail = self._available()
             if num_avail > 0:
                 last_read_time = ticks_ms()
                 bytes_to_read = min(num_to_read, num_avail)
-                if self._sock_type == SOCK_STREAM:
-                    bytes_read = _the_interface.socket_read(
+                if self._sock_type == SocketPool.SOCK_STREAM:
+                    bytes_read = self._interface.socket_read(
                         self._socknum, bytes_to_read
                     )[1]
                 else:
-                    bytes_read = _the_interface.read_udp(self._socknum, bytes_to_read)[
+                    bytes_read = self._interface.read_udp(self._socknum, bytes_to_read)[
                         1
                     ]
                 buffer[num_read : num_read + len(bytes_read)] = bytes_read
                 num_read += len(bytes_read)
                 num_to_read -= len(bytes_read)
             elif num_read > 0:
                 # We got a message, but there are no more bytes to read, so we can stop.
@@ -628,15 +638,15 @@
                 # non-blocking mode
                 break
             if ticks_diff(ticks_ms(), last_read_time) / 1000 > self._timeout:
                 raise timeout("timed out")
         return num_read
 
     @_check_socket_closed
-    def recvfrom_into(
+    def recvfrom_into(  # pylint: disable=unused-argument
         self, buffer: bytearray, nbytes: int = 0, flags: int = 0
     ) -> Tuple[int, Tuple[str, int]]:
         """
         Receive data from the socket, writing it into buffer instead of creating a new bytestring.
         The return value is a pair (nbytes, address) where nbytes is the number of bytes received
         and address is the address of the socket sending the data.
 
@@ -645,16 +655,16 @@
         :param int flags: Unused, present for compatibility.
 
         :return Tuple[int, Tuple[str, int]]: The number of bytes and address.
         """
         return (
             self.recv_into(buffer, nbytes),
             (
-                _the_interface.remote_ip(self._socknum),
-                _the_interface.remote_port(self._socknum),
+                self._interface.remote_ip(self._socknum),
+                self._interface.remote_port(self._socknum),
             ),
         )
 
     def _readline(self) -> bytes:
         """
         Read a line from the socket.
 
@@ -665,66 +675,67 @@
 
         :return bytes: The data read from the socket.
         """
         stamp = ticks_ms()
         while b"\r\n" not in self._buffer:
             avail = self._available()
             if avail:
-                if self._sock_type == SOCK_STREAM:
-                    self._buffer += _the_interface.socket_read(self._socknum, avail)[1]
-                elif self._sock_type == SOCK_DGRAM:
-                    self._buffer += _the_interface.read_udp(self._socknum, avail)[1]
+                if self._sock_type == SocketPool.SOCK_STREAM:
+                    self._buffer += self._interface.socket_read(self._socknum, avail)[1]
+                elif self._sock_type == SocketPool.SOCK_DGRAM:
+                    self._buffer += self._interface.read_udp(self._socknum, avail)[1]
                 if (
                     self._timeout
                     and not avail
                     and 0 < self._timeout < ticks_diff(ticks_ms(), stamp) / 1000
                 ):
                     self.close()
                     raise RuntimeError("Didn't receive response, failing out...")
         firstline, self._buffer = self._buffer.split(b"\r\n", 1)
         gc.collect()
         return firstline
 
     def _disconnect(self) -> None:
         """Disconnect a TCP socket."""
-        if self._sock_type != SOCK_STREAM:
+        if self._sock_type != SocketPool.SOCK_STREAM:
             raise RuntimeError("Socket must be a TCP socket.")
-        _the_interface.socket_disconnect(self._socknum)
+        self._interface.socket_disconnect(self._socknum)
 
     @_check_socket_closed
     def close(self) -> None:
         """
         Mark the socket closed. Once that happens, all future operations on the socket object
         will fail. The remote end will receive no more data.
         """
-        _the_interface.release_socket(self._socknum)
-        _the_interface.socket_close(self._socknum)
+        self._interface.release_socket(self._socknum)
+        self._interface.socket_close(self._socknum)
         self._socket_closed = True
 
     def _available(self) -> int:
         """
         Return how many bytes of data are available to be read from the socket.
 
         :return int: Number of bytes available.
         """
-        return _the_interface.socket_available(
-            self._socknum, _SOCKET_TYPE_TO_WIZNET[self._sock_type]
+        return self._interface.socket_available(
+            self._socknum,
+            _SOCKET_TYPE_TO_WIZNET[self._sock_type],
         )
 
     @_check_socket_closed
-    def setsockopt(  # pylint: disable=no-self-use
+    def setsockopt(  # pylint: disable=no-self-use,unused-argument
         self, level: int, opt: int, value: any
     ) -> None:
         """
         Set a socket option.
 
         Only SOL_SOCKET SO_REUSEADDR is accepted (and the value is ignored).
 
         Other calls result in OSError."""
-        if level == SOL_SOCKET and opt == SO_REUSEADDR:
+        if level == SocketPool.SOL_SOCKET and opt == SocketPool.SO_REUSEADDR:
             return
         raise OSError
 
     @_check_socket_closed
     def settimeout(self, value: Optional[float]) -> None:
         """
         Set a timeout on blocking socket operations. The value argument can be a
@@ -800,16 +811,13 @@
     @property
     @_check_socket_closed
     def proto(self):
         """Socket protocol (always 0x00 in this implementation)."""
         return 0
 
 
-class timeout(TimeoutError):
+class timeout(TimeoutError):  # pylint: disable=invalid-name
     """TimeoutError class. An instance of this error will be raised by recv_into() if
     the timeout has elapsed and we haven't received any data yet."""
 
     def __init__(self, msg):
         super().__init__(ETIMEDOUT, msg)
-
-
-# pylint: enable=unused-argument, redefined-builtin, invalid-name
```

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/docs/_static/favicon.ico` & `adafruit_circuitpython_wiznet5k-7.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/docs/conf.py` & `adafruit_circuitpython_wiznet5k-7.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/docs/index.rst` & `adafruit_circuitpython_wiznet5k-7.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_aio_post.py` & `adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_cheerlights.py` & `adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_cpython_client_for_simpleserver.py` & `adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_cpython_client_for_simpleserver.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_httpserver.py` & `adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_httpserver.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # SPDX-FileCopyrightText: 2023 Tim C for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
 import board
 import digitalio
 from adafruit_httpserver import Server, Request, Response
 from adafruit_wiznet5k.adafruit_wiznet5k import WIZNET5K
-import adafruit_wiznet5k.adafruit_wiznet5k_socket as socket
+import adafruit_wiznet5k.adafruit_wiznet5k_socketpool as socketpool
 
 print("Wiznet5k HTTPServer Test")
 
 # For Adafruit Ethernet FeatherWing
 cs = digitalio.DigitalInOut(board.D10)
 # For Particle Ethernet FeatherWing
 # cs = digitalio.DigitalInOut(board.D5)
 spi_bus = board.SPI()
 
 # Initialize ethernet interface with DHCP
 eth = WIZNET5K(spi_bus, cs)
 
-# set the interface on the socket source
-socket.set_interface(eth)
+# Create a socket pool
+pool = socketpool.SocketPool(eth)
 
 # initialize the server
-server = Server(socket, "/static", debug=True)
+server = Server(pool, "/static", debug=True)
 
 
 @server.route("/")
 def base(request: Request):
     """
     Serve a default static plain text message.
     """
```

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_simpleserver.py` & `adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_simpleserver.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 #
 # SPDX-License-Identifier: MIT
 
 import board
 import busio
 import digitalio
 from adafruit_wiznet5k.adafruit_wiznet5k import WIZNET5K
-import adafruit_wiznet5k.adafruit_wiznet5k_socket as socket
+import adafruit_wiznet5k.adafruit_wiznet5k_socketpool as socketpool
 
 print("Wiznet5k SimpleServer Test")
 
 # For Adafruit Ethernet FeatherWing
 cs = digitalio.DigitalInOut(board.D10)
 # For Particle Ethernet FeatherWing
 # cs = digitalio.DigitalInOut(board.D5)
 spi_bus = busio.SPI(board.SCK, MOSI=board.MOSI, MISO=board.MISO)
 
 # Initialize ethernet interface
 eth = WIZNET5K(spi_bus, cs, is_dhcp=True)
 
 # Initialize a socket for our server
-socket.set_interface(eth)
-server = socket.socket()  # Allocate socket for the server
+pool = socketpool.SocketPool(eth)
+server = pool.socket()  # Allocate socket for the server
 server_ip = eth.pretty_ip(eth.ip_address)  # IP address of server
 server_port = 50007  # Port to listen on
 server.bind((server_ip, server_port))  # Bind to IP and Port
 server.listen()  # Begin listening for incoming clients
 
 while True:
     print(f"Accepting connections on {server_ip}:{server_port}")
```

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_simpletest.py` & `adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/examples/wiznet5k_simpletest_manual_network.py` & `adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_simpletest_manual_network.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-6.0.0/pyproject.toml` & `adafruit_circuitpython_wiznet5k-7.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-wiznet5k"
 description = "Pure-Python interface for WIZNET 5k ethernet modules."
-version = "6.0.0"
+version = "7.0.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k"}
 keywords = [
     "adafruit",
```

