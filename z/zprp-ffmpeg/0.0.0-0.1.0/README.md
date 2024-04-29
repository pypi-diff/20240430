# Comparing `tmp/zprp-ffmpeg-0.0.0.tar.gz` & `tmp/zprp_ffmpeg-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zprp-ffmpeg-0.0.0.tar", last modified: Tue Mar 19 12:50:53 2024, max compression
+gzip compressed data, was "zprp_ffmpeg-0.1.0.tar", last modified: Mon Apr 29 22:30:32 2024, max compression
```

## Comparing `zprp-ffmpeg-0.0.0.tar` & `zprp_ffmpeg-0.1.0.tar`

### file list

```diff
@@ -1,58 +1,66 @@
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-03-19 12:50:53.814061 zprp-ffmpeg-0.0.0/
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      736 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/.bumpversion.cfg
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1992 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/.cookiecutterrc
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      179 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/.coveragerc
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      353 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/.editorconfig
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-03-19 12:50:53.804061 zprp-ffmpeg-0.0.0/.github/
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-03-19 12:50:53.814061 zprp-ffmpeg-0.0.0/.github/workflows/
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     8432 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/.github/workflows/github-actions.yml
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      686 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/.pre-commit-config.yaml
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      282 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/.readthedocs.yml
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       83 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/AUTHORS.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       86 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/CHANGELOG.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     2348 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/CONTRIBUTING.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1088 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/LICENSE
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      427 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/MANIFEST.in
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     2182 2024-03-19 12:50:53.814061 zprp-ffmpeg-0.0.0/PKG-INFO
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     2448 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/README.rst
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-03-19 12:50:53.814061 zprp-ffmpeg-0.0.0/ci/
--rwxr-xr-x   0 tomwez    (1000) tomwez    (1000)     2867 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/ci/bootstrap.py
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       72 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/ci/requirements.txt
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-03-19 12:50:53.804061 zprp-ffmpeg-0.0.0/ci/templates/
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-03-19 12:50:53.804061 zprp-ffmpeg-0.0.0/ci/templates/.github/
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-03-19 12:50:53.814061 zprp-ffmpeg-0.0.0/ci/templates/.github/workflows/
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     4006 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-03-19 12:50:53.814061 zprp-ffmpeg-0.0.0/docs/
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       28 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/docs/authors.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       30 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/docs/changelog.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1139 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/docs/conf.py
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       33 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/docs/contributing.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      244 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/docs/index.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       91 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/docs/installation.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       27 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/docs/readme.rst
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-03-19 12:50:53.814061 zprp-ffmpeg-0.0.0/docs/reference/
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       63 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/docs/reference/index.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      174 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/docs/reference/zprp_ffmpeg.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       29 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/docs/requirements.txt
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      109 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/docs/spelling_wordlist.txt
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       74 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/docs/usage.rst
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1227 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/pyproject.toml
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      776 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/pytest.ini
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       38 2024-03-19 12:50:53.814061 zprp-ffmpeg-0.0.0/setup.cfg
--rwxr-xr-x   0 tomwez    (1000) tomwez    (1000)     4096 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/setup.py
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-03-19 12:50:53.804061 zprp-ffmpeg-0.0.0/src/
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-03-19 12:50:53.814061 zprp-ffmpeg-0.0.0/src/zprp_ffmpeg/
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       86 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/src/zprp_ffmpeg/__init__.py
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      392 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/src/zprp_ffmpeg/__main__.py
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1812 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/src/zprp_ffmpeg/_zprp_ffmpeg.c
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      826 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/src/zprp_ffmpeg/cli.py
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-03-19 12:50:53.814061 zprp-ffmpeg-0.0.0/src/zprp_ffmpeg.egg-info/
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     2182 2024-03-19 12:50:53.000000 zprp-ffmpeg-0.0.0/src/zprp_ffmpeg.egg-info/PKG-INFO
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      955 2024-03-19 12:50:53.000000 zprp-ffmpeg-0.0.0/src/zprp_ffmpeg.egg-info/SOURCES.txt
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)        1 2024-03-19 12:50:53.000000 zprp-ffmpeg-0.0.0/src/zprp_ffmpeg.egg-info/dependency_links.txt
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       53 2024-03-19 12:50:53.000000 zprp-ffmpeg-0.0.0/src/zprp_ffmpeg.egg-info/entry_points.txt
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)        1 2024-03-19 09:50:16.000000 zprp-ffmpeg-0.0.0/src/zprp_ffmpeg.egg-info/not-zip-safe
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)       12 2024-03-19 12:50:53.000000 zprp-ffmpeg-0.0.0/src/zprp_ffmpeg.egg-info/top_level.txt
-drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-03-19 12:50:53.814061 zprp-ffmpeg-0.0.0/tests/
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)      183 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/tests/test_zprp_ffmpeg.py
--rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1706 2024-03-19 10:18:25.000000 zprp-ffmpeg-0.0.0/tox.ini
+drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)      740 2024-04-29 20:46:48.000000 zprp_ffmpeg-0.1.0/.bumpversion.cfg
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1992 2024-04-29 20:46:48.000000 zprp_ffmpeg-0.1.0/.cookiecutterrc
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)      179 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/.coveragerc
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)      353 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/.editorconfig
+drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.926673 zprp_ffmpeg-0.1.0/.github/
+drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/.github/workflows/
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)     8747 2024-04-23 06:21:23.000000 zprp_ffmpeg-0.1.0/.github/workflows/github-actions.yml
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)      686 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)      282 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/.readthedocs.yml
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)       83 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/AUTHORS.rst
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1263 2024-04-29 22:13:47.000000 zprp_ffmpeg-0.1.0/CHANGELOG.rst
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)     2348 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1088 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/LICENSE
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)      427 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/MANIFEST.in
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)     5175 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/PKG-INFO
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)     4266 2024-04-29 20:46:48.000000 zprp_ffmpeg-0.1.0/README.rst
+drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/ci/
+-rwxr-xr-x   0 tomwez    (1000) tomwez    (1000)     2867 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/ci/bootstrap.py
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)       72 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/ci/requirements.txt
+drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.926673 zprp_ffmpeg-0.1.0/ci/templates/
+drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.926673 zprp_ffmpeg-0.1.0/ci/templates/.github/
+drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/ci/templates/.github/workflows/
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)     4006 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/docs/
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)       28 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/authors.rst
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)       30 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/changelog.rst
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1139 2024-04-29 20:46:48.000000 zprp_ffmpeg-0.1.0/docs/conf.py
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)       33 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/contributing.rst
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)      244 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/index.rst
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)       91 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/installation.rst
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)       27 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/readme.rst
+drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/docs/reference/
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)       63 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/reference/index.rst
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)      174 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/reference/zprp_ffmpeg.rst
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)       29 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/requirements.txt
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)      109 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)       74 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/docs/usage.rst
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1297 2024-04-23 06:21:23.000000 zprp_ffmpeg-0.1.0/pyproject.toml
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)      843 2024-04-10 14:40:08.000000 zprp_ffmpeg-0.1.0/pytest.ini
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)       38 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/setup.cfg
+-rwxr-xr-x   0 tomwez    (1000) tomwez    (1000)     4096 2024-04-29 20:46:48.000000 zprp_ffmpeg-0.1.0/setup.py
+drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.926673 zprp_ffmpeg-0.1.0/src/
+drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)      638 2024-04-23 06:21:23.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/BaseConnector.py
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)     2598 2024-04-23 06:21:23.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/FilterGraph.py
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)        0 2024-04-23 06:21:23.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/PopenCommunicator.py
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1326 2024-04-23 06:21:23.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/ProcessConnector.py
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)      327 2024-04-29 20:46:48.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/__init__.py
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)      392 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/__main__.py
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)      991 2024-04-23 06:21:23.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/_api_compat.py
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1812 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/_zprp_ffmpeg.c
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)      826 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/cli.py
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)      153 2024-04-10 16:02:25.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/filters.py
+drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg.egg-info/
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)     5175 2024-04-29 22:30:32.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg.egg-info/PKG-INFO
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1209 2024-04-29 22:30:32.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg.egg-info/SOURCES.txt
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)        1 2024-04-29 22:30:32.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg.egg-info/dependency_links.txt
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)       53 2024-04-29 22:30:32.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg.egg-info/entry_points.txt
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)        1 2024-03-19 09:50:16.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg.egg-info/not-zip-safe
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)       12 2024-04-29 22:30:32.000000 zprp_ffmpeg-0.1.0/src/zprp_ffmpeg.egg-info/top_level.txt
+drwxr-xr-x   0 tomwez    (1000) tomwez    (1000)        0 2024-04-29 22:30:32.936673 zprp_ffmpeg-0.1.0/tests/
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)      290 2024-04-10 14:40:08.000000 zprp_ffmpeg-0.1.0/tests/test_ProcessConnector.py
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)      257 2024-04-10 16:11:09.000000 zprp_ffmpeg-0.1.0/tests/test_kkroening_api.py
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)       83 2024-04-10 14:40:08.000000 zprp_ffmpeg-0.1.0/tests/test_zprp_ffmpeg.py
+-rw-r--r--   0 tomwez    (1000) tomwez    (1000)     1706 2024-03-19 10:18:25.000000 zprp_ffmpeg-0.1.0/tox.ini
```

### Comparing `zprp-ffmpeg-0.0.0/.bumpversion.cfg` & `zprp_ffmpeg-0.1.0/.bumpversion.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.0.0
+current_version = 0.1.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
 
@@ -20,9 +20,9 @@
 replace = version = release = "{new_version}"
 
 [bumpversion:file:src/zprp_ffmpeg/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
 [bumpversion:file:.cookiecutterrc]
-search = version: {current_version}
-replace = version: {new_version}
+search = version: "{current_version}"
+replace = version: "{new_version}"
```

### Comparing `zprp-ffmpeg-0.0.0/.cookiecutterrc` & `zprp_ffmpeg-0.1.0/.cookiecutterrc`

 * *Files 1% similar despite different names*

```diff
@@ -50,12 +50,12 @@
     scrutinizer: "no"
     setup_py_uses_setuptools_scm: "no"
     sphinx_docs: "yes"
     sphinx_docs_hosting: "https://zprp-ffmpeg.readthedocs.io/"
     sphinx_doctest: "no"
     sphinx_theme: "sphinx-rtd-theme"
     test_matrix_separate_coverage: "no"
-    version: "0.0.0"
+    version: "0.1.0"
     version_manager: "bump2version"
     website: ""
     year_from: "2024"
     year_to: "2024"
```

### Comparing `zprp-ffmpeg-0.0.0/.github/workflows/github-actions.yml` & `zprp_ffmpeg-0.1.0/.github/workflows/github-actions.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 name: build
-on: [push, pull_request]
+on:
+  workflow_run:
+    workflows: [lint]
+    types:
+      - completed
 jobs:
   test:
     name: ${{ matrix.name }}
     runs-on: ${{ matrix.os }}
     timeout-minutes: 30
     strategy:
       fail-fast: false
@@ -23,14 +27,15 @@
             python: '3.8'
             toxpython: 'python3.8'
             python_arch: 'x64'
             tox_env: 'py38'
             cibw_arch: 'x86_64'
             cibw_build: false
             os: 'ubuntu-latest'
+            cover: true
           - name: 'py38 (windows/AMD64)'
             python: '3.8'
             toxpython: 'python3.8'
             python_arch: 'x64'
             tox_env: 'py38'
             cibw_arch: 'AMD64'
             cibw_build: false
@@ -243,26 +248,34 @@
           tox-direct
         CIBW_TEST_COMMAND: >
           cd {project} &&
           tox --skip-pkg-install --direct-yolo -e ${{ matrix.tox_env }} -v
         CIBW_TEST_COMMAND_WINDOWS: >
           cd /d {project} &&
           tox --skip-pkg-install --direct-yolo -e ${{ matrix.tox_env }} -v
+    - name: install ffmpeg
+      uses: FedericoCarboni/setup-ffmpeg@v3
+      with:
+        ffmpeg-version: release
+
     - name: regular build and test
       env:
         TOXPYTHON: '${{ matrix.toxpython }}'
       if: >
         !matrix.cibw_build
       run: >
         tox -e ${{ matrix.tox_env }} -v
-    - uses: codecov/codecov-action@v3
+    - name: Upload coverage reports to Codecov
+      uses: codecov/codecov-action@v3
       if: matrix.cover
       with:
         verbose: true
         flags: ${{ matrix.tox_env }}
+        token: ${{ secrets.CODECOV_TOKEN }}
+        slug: ffmpeg-zprp/zprp-ffmpeg
     - name: check wheel
       if: matrix.cibw_build
       run: twine check wheelhouse/*.whl
     - name: upload wheel
       uses: actions/upload-artifact@v3
       if: matrix.cibw_build
       with:
```

### Comparing `zprp-ffmpeg-0.0.0/.pre-commit-config.yaml` & `zprp_ffmpeg-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `zprp-ffmpeg-0.0.0/CONTRIBUTING.rst` & `zprp_ffmpeg-0.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `zprp-ffmpeg-0.0.0/LICENSE` & `zprp_ffmpeg-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zprp-ffmpeg-0.0.0/ci/bootstrap.py` & `zprp_ffmpeg-0.1.0/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `zprp-ffmpeg-0.0.0/ci/templates/.github/workflows/github-actions.yml` & `zprp_ffmpeg-0.1.0/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `zprp-ffmpeg-0.0.0/docs/conf.py` & `zprp_ffmpeg-0.1.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "zprp-ffmpeg"
 year = "2024"
 author = ""
 copyright = f"{year}, {author}"
-version = release = "0.0.0"
+version = release = "0.1.0"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/Madghostek/zprp-ffmpeg/issues/%s", "#"),
     "pr": ("https://github.com/Madghostek/zprp-ffmpeg/pull/%s", "PR #"),
 }
```

### Comparing `zprp-ffmpeg-0.0.0/pyproject.toml` & `zprp_ffmpeg-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -48,7 +48,10 @@
 [tool.ruff.lint.isort]
 forced-separate = ["conftest"]
 force-single-line = true
 
 [tool.black]
 line-length = 140
 target-version = ["py38"]
+
+[tool.mypy]
+disable_error_code = ["import-not-found"] # temporarytem
```

### Comparing `zprp-ffmpeg-0.0.0/pytest.ini` & `zprp_ffmpeg-0.1.0/pytest.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 [pytest]
 # If a pytest section is found in one of the possible config files
 # (pytest.ini, tox.ini or setup.cfg), then pytest will not look for any others,
 # so if you add a pytest config section elsewhere,
 # you will need to delete this section from setup.cfg.
+markers =
+    starts_process: opens ffmpeg process, might be slow
+
 norecursedirs =
     migrations
 
 python_files =
     test_*.py
     *_test.py
     tests.py
```

### Comparing `zprp-ffmpeg-0.0.0/setup.py` & `zprp_ffmpeg-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="zprp-ffmpeg",
-    version="0.0.0",
+    version="0.1.0",
     license="MIT",
     description="Implementation of the successor to the ffmpeg-python library",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
     author="",
```

### Comparing `zprp-ffmpeg-0.0.0/src/zprp_ffmpeg/_zprp_ffmpeg.c` & `zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/_zprp_ffmpeg.c`

 * *Files identical despite different names*

### Comparing `zprp-ffmpeg-0.0.0/src/zprp_ffmpeg/cli.py` & `zprp_ffmpeg-0.1.0/src/zprp_ffmpeg/cli.py`

 * *Files identical despite different names*

### Comparing `zprp-ffmpeg-0.0.0/src/zprp_ffmpeg.egg-info/SOURCES.txt` & `zprp_ffmpeg-0.1.0/src/zprp_ffmpeg.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -26,18 +26,26 @@
 docs/installation.rst
 docs/readme.rst
 docs/requirements.txt
 docs/spelling_wordlist.txt
 docs/usage.rst
 docs/reference/index.rst
 docs/reference/zprp_ffmpeg.rst
+src/zprp_ffmpeg/BaseConnector.py
+src/zprp_ffmpeg/FilterGraph.py
+src/zprp_ffmpeg/PopenCommunicator.py
+src/zprp_ffmpeg/ProcessConnector.py
 src/zprp_ffmpeg/__init__.py
 src/zprp_ffmpeg/__main__.py
+src/zprp_ffmpeg/_api_compat.py
 src/zprp_ffmpeg/_zprp_ffmpeg.c
 src/zprp_ffmpeg/cli.py
+src/zprp_ffmpeg/filters.py
 src/zprp_ffmpeg.egg-info/PKG-INFO
 src/zprp_ffmpeg.egg-info/SOURCES.txt
 src/zprp_ffmpeg.egg-info/dependency_links.txt
 src/zprp_ffmpeg.egg-info/entry_points.txt
 src/zprp_ffmpeg.egg-info/not-zip-safe
 src/zprp_ffmpeg.egg-info/top_level.txt
+tests/test_ProcessConnector.py
+tests/test_kkroening_api.py
 tests/test_zprp_ffmpeg.py
```

### Comparing `zprp-ffmpeg-0.0.0/tox.ini` & `zprp_ffmpeg-0.1.0/tox.ini`

 * *Files identical despite different names*

