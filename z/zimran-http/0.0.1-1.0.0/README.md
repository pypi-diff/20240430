# Comparing `tmp/zimran-http-0.0.1.tar.gz` & `tmp/zimran_http-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimran-http-0.0.1.tar", last modified: Mon Feb 20 08:37:43 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `zimran-http-0.0.1.tar` & `zimran_http-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:37:43.745356 zimran-http-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-02-20 08:37:43.741356 zimran-http-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-02-20 08:37:28.000000 zimran-http-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 08:37:43.745356 zimran-http-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-02-20 08:37:28.000000 zimran-http-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:37:43.741356 zimran-http-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-02-20 08:37:28.000000 zimran-http-0.0.1/tests/test_async_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-20 08:37:28.000000 zimran-http-0.0.1/tests/test_http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:37:43.741356 zimran-http-0.0.1/zimran/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:37:43.741356 zimran-http-0.0.1/zimran/http/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-20 08:37:28.000000 zimran-http-0.0.1/zimran/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-20 08:37:28.000000 zimran-http-0.0.1/zimran/http/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-20 08:37:28.000000 zimran-http-0.0.1/zimran/http/async_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-20 08:37:28.000000 zimran-http-0.0.1/zimran/http/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:37:43.741356 zimran-http-0.0.1/zimran_http.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-02-20 08:37:43.000000 zimran-http-0.0.1/zimran_http.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-02-20 08:37:43.000000 zimran-http-0.0.1/zimran_http.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 08:37:43.000000 zimran-http-0.0.1/zimran_http.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-20 08:37:43.000000 zimran-http-0.0.1/zimran_http.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-20 08:37:43.000000 zimran-http-0.0.1/zimran_http.egg-info/top_level.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 zimran_http-1.0.0/.coveragerc
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 zimran_http-1.0.0/.editorconfig
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 zimran_http-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 zimran_http-1.0.0/pytest.ini
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 zimran_http-1.0.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 zimran_http-1.0.0/.github/scripts/release.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 zimran_http-1.0.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 zimran_http-1.0.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 zimran_http-1.0.0/tests/test_client.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 zimran_http-1.0.0/zimran/http_client/__init__.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 zimran_http-1.0.0/zimran/http_client/_async_http.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 zimran_http-1.0.0/zimran/http_client/_http.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 zimran_http-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 zimran_http-1.0.0/LICENSE
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 zimran_http-1.0.0/README.md
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 zimran_http-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 zimran_http-1.0.0/PKG-INFO
```

