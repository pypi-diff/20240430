# Comparing `tmp/fuzzfetch-6.0.0.tar.gz` & `tmp/fuzzfetch-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzfetch-6.0.0.tar", last modified: Wed Mar 13 21:02:54 2024, max compression
+gzip compressed data, was "fuzzfetch-7.0.0.tar", last modified: Tue Apr 30 19:48:25 2024, max compression
```

## Comparing `fuzzfetch-6.0.0.tar` & `fuzzfetch-7.0.0.tar`

### file list

```diff
@@ -1,1069 +1,1076 @@
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.866838 fuzzfetch-6.0.0/
--rw-r--r--   0 worker    (1000) worker    (1000)       55 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/.codecov.yml
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.746838 fuzzfetch-6.0.0/.github/
--rw-r--r--   0 worker    (1000) worker    (1000)       42 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/.github/CODEOWNERS
--rw-r--r--   0 worker    (1000) worker    (1000)      386 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/.gitignore
--rw-r--r--   0 worker    (1000) worker    (1000)     1784 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/.pre-commit-config.yaml
--rw-r--r--   0 worker    (1000) worker    (1000)     3600 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/.taskcluster.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      689 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 worker    (1000) worker    (1000)    15550 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/LICENSE.md
--rw-r--r--   0 worker    (1000) worker    (1000)     5450 2024-03-13 21:02:54.866838 fuzzfetch-6.0.0/PKG-INFO
--rw-r--r--   0 worker    (1000) worker    (1000)     4609 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/README.md
--rw-r--r--   0 worker    (1000) worker    (1000)      891 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/pyproject.toml
--rw-r--r--   0 worker    (1000) worker    (1000)      970 2024-03-13 21:02:54.866838 fuzzfetch-6.0.0/setup.cfg
--rwxr-xr-x   0 worker    (1000) worker    (1000)      370 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/setup.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.690838 fuzzfetch-6.0.0/src/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.746838 fuzzfetch-6.0.0/src/fuzzfetch/
--rw-r--r--   0 worker    (1000) worker    (1000)      586 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/src/fuzzfetch/__init__.py
--rw-r--r--   0 worker    (1000) worker    (1000)      288 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/src/fuzzfetch/__main__.py
--rw-r--r--   0 worker    (1000) worker    (1000)     9933 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/src/fuzzfetch/args.py
--rw-r--r--   0 worker    (1000) worker    (1000)    33878 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/src/fuzzfetch/core.py
--rw-r--r--   0 worker    (1000) worker    (1000)     3637 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/src/fuzzfetch/download.py
--rw-r--r--   0 worker    (1000) worker    (1000)      358 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/src/fuzzfetch/errors.py
--rw-r--r--   0 worker    (1000) worker    (1000)     5634 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/src/fuzzfetch/extract.py
--rw-r--r--   0 worker    (1000) worker    (1000)    13306 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/src/fuzzfetch/models.py
--rw-r--r--   0 worker    (1000) worker    (1000)     2685 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/src/fuzzfetch/path.py
--rw-r--r--   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/src/fuzzfetch/py.typed
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.862838 fuzzfetch-6.0.0/src/fuzzfetch.egg-info/
--rw-r--r--   0 worker    (1000) worker    (1000)     5450 2024-03-13 21:02:54.000000 fuzzfetch-6.0.0/src/fuzzfetch.egg-info/PKG-INFO
--rw-r--r--   0 worker    (1000) worker    (1000)    54234 2024-03-13 21:02:54.000000 fuzzfetch-6.0.0/src/fuzzfetch.egg-info/SOURCES.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        1 2024-03-13 21:02:54.000000 fuzzfetch-6.0.0/src/fuzzfetch.egg-info/dependency_links.txt
--rw-r--r--   0 worker    (1000) worker    (1000)       53 2024-03-13 21:02:54.000000 fuzzfetch-6.0.0/src/fuzzfetch.egg-info/entry_points.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        1 2024-03-13 21:02:54.000000 fuzzfetch-6.0.0/src/fuzzfetch.egg-info/not-zip-safe
--rw-r--r--   0 worker    (1000) worker    (1000)       36 2024-03-13 21:02:54.000000 fuzzfetch-6.0.0/src/fuzzfetch.egg-info/requires.txt
--rw-r--r--   0 worker    (1000) worker    (1000)       10 2024-03-13 21:02:54.000000 fuzzfetch-6.0.0/src/fuzzfetch.egg-info/top_level.txt
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.750838 fuzzfetch-6.0.0/tests/
--rw-r--r--   0 worker    (1000) worker    (1000)     4127 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/conftest.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.690838 fuzzfetch-6.0.0/tests/mock-firefoxci/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.690838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.690838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.754838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/
--rw-r--r--   0 worker    (1000) worker    (1000)      351 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2022.12.31
--rw-r--r--   0 worker    (1000) worker    (1000)      351 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2023.01.02
--rw-r--r--   0 worker    (1000) worker    (1000)      522 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2023.01.03
--rw-r--r--   0 worker    (1000) worker    (1000)      864 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2023.01.04
--rw-r--r--   0 worker    (1000) worker    (1000)      693 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2023.01.05
--rw-r--r--   0 worker    (1000) worker    (1000)      693 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2023.11.23
--rw-r--r--   0 worker    (1000) worker    (1000)      522 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2024.01.01
--rw-r--r--   0 worker    (1000) worker    (1000)      351 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2024.01.02
--rw-r--r--   0 worker    (1000) worker    (1000)       23 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2024.01.03
--rw-r--r--   0 worker    (1000) worker    (1000)      341 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2022.12.31
--rw-r--r--   0 worker    (1000) worker    (1000)      341 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2023.01.02
--rw-r--r--   0 worker    (1000) worker    (1000)      341 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2023.01.03
--rw-r--r--   0 worker    (1000) worker    (1000)      341 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2023.01.04
--rw-r--r--   0 worker    (1000) worker    (1000)      341 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2023.01.05
--rw-r--r--   0 worker    (1000) worker    (1000)      341 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2023.11.23
--rw-r--r--   0 worker    (1000) worker    (1000)      341 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2024.01.01
--rw-r--r--   0 worker    (1000) worker    (1000)      341 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2024.01.02
--rw-r--r--   0 worker    (1000) worker    (1000)       23 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2024.01.03
--rw-r--r--   0 worker    (1000) worker    (1000)      349 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-esr115.pushdate.2023.12.30
--rw-r--r--   0 worker    (1000) worker    (1000)      349 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-esr115.pushdate.2024.01.02
--rw-r--r--   0 worker    (1000) worker    (1000)      339 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-esr115.shippable.2023.12.30
--rw-r--r--   0 worker    (1000) worker    (1000)       23 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-esr115.shippable.2024.01.02
--rw-r--r--   0 worker    (1000) worker    (1000)    11775 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2023.12.29
--rw-r--r--   0 worker    (1000) worker    (1000)     6051 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2024.01.02
--rw-r--r--   0 worker    (1000) worker    (1000)      317 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.shippable.2023.12.29
--rw-r--r--   0 worker    (1000) worker    (1000)      317 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.shippable.2024.01.02
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.806838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/
--rw-r--r--   0 worker    (1000) worker    (1000)      188 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      187 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      193 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      210 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-ccov-fuzzing-asan-nyx-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      201 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-ccov-fuzzing-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      184 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-ccov-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      190 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      205 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-asan-nyx-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      201 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      198 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      201 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-tsan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      191 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-searchfox-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      193 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-tsan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      210 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-aarch64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      207 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-aarch64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      191 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      202 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      199 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      202 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.sm-linux64-fuzzilli-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      188 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win32-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      196 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win32-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      196 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-aarch64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      191 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      199 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-ccov-fuzzing-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      182 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-ccov-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      188 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      196 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      193 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.mobile.android-arm-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      215 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2023.11.23.20231123095534.firefox.linux64-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      216 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      221 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux64-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      229 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux64-ccov-fuzzing-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      212 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux64-ccov-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      218 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      229 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      226 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      229 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux64-fuzzing-tsan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      216 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      221 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux64-tsan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      238 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.macosx64-aarch64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      235 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.macosx64-aarch64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      219 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.macosx64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      230 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.macosx64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      227 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.macosx64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      216 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.win32-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      224 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.win32-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      224 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.win64-aarch64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      219 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.win64-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      227 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.win64-ccov-fuzzing-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      210 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.win64-ccov-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      216 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.win64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      224 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.win64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      221 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.mobile.android-arm-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      208 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.latest.firefox.linux64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      231 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.10aa7423789835a7dbd24b0b44ad1ae2ad77b59b.firefox.linux64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      231 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      236 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux64-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      244 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux64-ccov-fuzzing-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      227 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux64-ccov-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      233 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      244 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      241 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      244 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux64-fuzzing-tsan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      231 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      236 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux64-tsan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      253 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.macosx64-aarch64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      250 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.macosx64-aarch64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      234 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.macosx64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      245 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.macosx64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      242 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.macosx64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      231 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win32-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      239 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win32-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      239 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win64-aarch64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      234 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win64-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      242 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win64-ccov-fuzzing-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      225 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win64-ccov-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      231 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      239 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      229 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      236 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.mobile.android-arm-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      230 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.8366d9b1b0ca63aa3b706dd53ce23f052221c11b.firefox.linux64-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      231 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.9d96d2c96d8fe1d9365fdaee30d8fda048c48aa1.firefox.linux64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      232 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.cd184ad5b96078dbc9d4251ed366d7acff965d7a.firefox.macosx64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      209 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2023.01.02.latest.firefox.linux64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      209 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2023.01.03.latest.firefox.linux64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      209 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2023.01.04.latest.firefox.linux64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      209 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2023.01.05.latest.firefox.linux64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      218 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.01.latest.firefox.macosx64-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      210 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.01.latest.firefox.macosx64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      207 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.02.latest.firefox.linux-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      209 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.02.latest.firefox.linux64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      207 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.02.latest.firefox.win32-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      215 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.02.latest.firefox.win64-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      207 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.02.latest.firefox.win64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      216 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.02.latest.mobile.android-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      212 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.02.latest.mobile.android-arm-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      212 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.02.latest.mobile.android-x86-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      215 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.02.latest.mobile.android-x86_64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      196 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.linux-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      198 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.linux64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      207 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.macosx64-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      199 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.macosx64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      196 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.win32-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      204 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.win64-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      196 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.win64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      205 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.mobile.android-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      201 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.mobile.android-arm-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      201 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.mobile.android-x86-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      204 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.mobile.android-x86_64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      239 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      239 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win32-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      247 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win64-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      248 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.mobile.android-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      244 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.mobile.android-arm-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      244 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.mobile.android-x86-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      247 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.mobile.android-x86_64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      250 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.cd184ad5b96078dbc9d4251ed366d7acff965d7a.firefox.macosx64-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      187 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.linux-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      192 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.linux64-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      189 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.linux64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      200 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.linux64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      197 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.linux64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      190 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.macosx64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      201 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.macosx64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      198 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.macosx64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      187 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.win32-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      187 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.win64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      220 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2023.12.30.20231230171938.firefox.linux64-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      228 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2023.12.30.20231230171938.firefox.linux64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      218 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2023.12.30.20231230171938.firefox.macosx64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      226 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2023.12.30.20231230171938.firefox.macosx64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      215 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2024.01.02.20240102145026.firefox.linux-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      217 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2024.01.02.20240102145026.firefox.linux64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      225 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2024.01.02.20240102145026.firefox.linux64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      229 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2024.01.02.20240102145026.firefox.macosx64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      215 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2024.01.02.20240102145026.firefox.win32-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      215 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2024.01.02.20240102145026.firefox.win64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      230 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.636a9054f04b5c65a4fbe1b79b91f1ee32629a99.firefox.linux-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      232 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.636a9054f04b5c65a4fbe1b79b91f1ee32629a99.firefox.linux64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      240 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.636a9054f04b5c65a4fbe1b79b91f1ee32629a99.firefox.linux64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      244 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.636a9054f04b5c65a4fbe1b79b91f1ee32629a99.firefox.macosx64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      230 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.636a9054f04b5c65a4fbe1b79b91f1ee32629a99.firefox.win32-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      230 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.636a9054f04b5c65a4fbe1b79b91f1ee32629a99.firefox.win64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      235 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.b8d6f1fcefecf913f749aa0b95daeb0874bda967.firefox.linux64-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      243 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.b8d6f1fcefecf913f749aa0b95daeb0874bda967.firefox.linux64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      233 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.b8d6f1fcefecf913f749aa0b95daeb0874bda967.firefox.macosx64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      241 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.b8d6f1fcefecf913f749aa0b95daeb0874bda967.firefox.macosx64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      228 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.b8d6f1fcefecf913f749aa0b95daeb0874bda967.firefox.win32-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      206 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.2023.12.30.latest.firefox.linux-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      208 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.2023.12.30.latest.firefox.linux64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      209 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.2023.12.30.latest.firefox.macosx64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      206 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.2023.12.30.latest.firefox.win32-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      206 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.2023.12.30.latest.firefox.win64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      195 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.latest.firefox.linux-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      197 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.latest.firefox.linux64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      198 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.latest.firefox.macosx64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      195 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.latest.firefox.win32-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      195 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.latest.firefox.win64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      238 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.revision.b8d6f1fcefecf913f749aa0b95daeb0874bda967.firefox.linux-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      240 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.revision.b8d6f1fcefecf913f749aa0b95daeb0874bda967.firefox.linux64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      241 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.revision.b8d6f1fcefecf913f749aa0b95daeb0874bda967.firefox.macosx64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      238 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.revision.b8d6f1fcefecf913f749aa0b95daeb0874bda967.firefox.win64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      176 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      187 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      184 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      175 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      181 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      178 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      189 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      186 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      189 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-fuzzing-tsan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      181 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-tsan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      198 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-aarch64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      195 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-aarch64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      179 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      190 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      187 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      176 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win32-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      184 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win32-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      184 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win64-aarch64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      176 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      184 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      181 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.mobile.android-arm-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      209 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2023.12.29.20231229173843.mobile.android-arm-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      215 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2023.12.29.20231229181418.firefox.linux-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      212 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2023.12.29.20231229181418.firefox.linux-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      206 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102004535.firefox.linux64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      209 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102004535.firefox.linux64-tsan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      207 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102004535.firefox.macosx64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      204 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102004535.firefox.win32-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      204 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102004535.firefox.win64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      209 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102024042.firefox.linux64-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      203 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.linux64-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      217 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.linux64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      214 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.linux64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      217 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.linux64-fuzzing-tsan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      226 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.macosx64-aarch64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      223 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.macosx64-aarch64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      218 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.macosx64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      215 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.macosx64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      212 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.win32-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      212 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.win64-aarch64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      212 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.win64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      204 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102103153.firefox.linux-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      217 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.40c9a6c168c2e2f0fd8154c4e566ed7670a08fb6.firefox.win32-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      217 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.40c9a6c168c2e2f0fd8154c4e566ed7670a08fb6.firefox.win64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      224 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.50ea3793201650ea9a2c841a7e0c4904fc45e782.firefox.linux64-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      221 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.50ea3793201650ea9a2c841a7e0c4904fc45e782.firefox.linux64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      224 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.50ea3793201650ea9a2c841a7e0c4904fc45e782.firefox.linux64-tsan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      222 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.50ea3793201650ea9a2c841a7e0c4904fc45e782.firefox.macosx64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      219 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.50ea3793201650ea9a2c841a7e0c4904fc45e782.firefox.win32-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      219 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.50ea3793201650ea9a2c841a7e0c4904fc45e782.firefox.win64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      230 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.50f00cc1d403ff2c42e97aa0ac7bf953d370fead.firefox.linux-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      227 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.50f00cc1d403ff2c42e97aa0ac7bf953d370fead.firefox.linux-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      224 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.50f00cc1d403ff2c42e97aa0ac7bf953d370fead.mobile.android-arm-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      218 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.584364cc704f114b73f6d0ecea71f4435dd0d49b.firefox.linux64-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      219 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.584364cc704f114b73f6d0ecea71f4435dd0d49b.firefox.linux64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      219 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.d0e78ab7f522d06f92bebfcd18f806a2dd1bd391.firefox.linux-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      226 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.d0e78ab7f522d06f92bebfcd18f806a2dd1bd391.mobile.android-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      232 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.linux64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      229 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.linux64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      232 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.linux64-fuzzing-tsan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      241 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.macosx64-aarch64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      238 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.macosx64-aarch64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      233 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.macosx64-fuzzing-asan-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      230 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.macosx64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      227 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.win32-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      227 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.win64-aarch64-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      227 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.win64-fuzzing-debug
--rw-r--r--   0 worker    (1000) worker    (1000)      195 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.firefox.linux-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      197 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.firefox.linux64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      206 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.firefox.macosx64-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      198 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.firefox.macosx64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      195 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.firefox.win32-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      203 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.firefox.win64-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      195 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.firefox.win64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      204 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.mobile.android-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      200 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.mobile.android-arm-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      200 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.mobile.android-x86-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      203 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.mobile.android-x86_64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      184 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.linux-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      186 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.linux64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      195 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.macosx64-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      187 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.macosx64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      184 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.win32-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      192 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.win64-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      184 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.win64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      193 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.mobile.android-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      189 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.mobile.android-arm-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      189 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.mobile.android-x86-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      192 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.mobile.android-x86_64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      227 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.d0e78ab7f522d06f92bebfcd18f806a2dd1bd391.firefox.linux-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      238 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.d0e78ab7f522d06f92bebfcd18f806a2dd1bd391.firefox.macosx64-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      230 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.d0e78ab7f522d06f92bebfcd18f806a2dd1bd391.firefox.macosx64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      235 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.d0e78ab7f522d06f92bebfcd18f806a2dd1bd391.firefox.win64-aarch64-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      232 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.d0e78ab7f522d06f92bebfcd18f806a2dd1bd391.mobile.android-arm-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      232 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.d0e78ab7f522d06f92bebfcd18f806a2dd1bd391.mobile.android-x86-opt
--rw-r--r--   0 worker    (1000) worker    (1000)      235 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.d0e78ab7f522d06f92bebfcd18f806a2dd1bd391.mobile.android-x86_64-opt
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.742838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/AGuXN_zgSTa4G2cOowM6tw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.806838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/AGuXN_zgSTa4G2cOowM6tw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7502 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/AGuXN_zgSTa4G2cOowM6tw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/AGuXN_zgSTa4G2cOowM6tw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.806838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/AGuXN_zgSTa4G2cOowM6tw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1133 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/AGuXN_zgSTa4G2cOowM6tw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Agexc3H0RvCxvLshb-oAkA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.806838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Agexc3H0RvCxvLshb-oAkA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Agexc3H0RvCxvLshb-oAkA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Agexc3H0RvCxvLshb-oAkA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.810838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Agexc3H0RvCxvLshb-oAkA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      956 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Agexc3H0RvCxvLshb-oAkA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/BMzeSq6sTVyo9tPp5vXCDg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.810838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/BMzeSq6sTVyo9tPp5vXCDg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     6983 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/BMzeSq6sTVyo9tPp5vXCDg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/BMzeSq6sTVyo9tPp5vXCDg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.810838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/BMzeSq6sTVyo9tPp5vXCDg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      975 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/BMzeSq6sTVyo9tPp5vXCDg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Bs_nyxXCTNm5hMfjX7DFwg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.810838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Bs_nyxXCTNm5hMfjX7DFwg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Bs_nyxXCTNm5hMfjX7DFwg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Bs_nyxXCTNm5hMfjX7DFwg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.810838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Bs_nyxXCTNm5hMfjX7DFwg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1120 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Bs_nyxXCTNm5hMfjX7DFwg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/C7bbCHVySOCJsQ24TJvNig/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.810838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/C7bbCHVySOCJsQ24TJvNig/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7692 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/C7bbCHVySOCJsQ24TJvNig/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/C7bbCHVySOCJsQ24TJvNig/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.810838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/C7bbCHVySOCJsQ24TJvNig/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1125 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/C7bbCHVySOCJsQ24TJvNig/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/C9C2cj1aS_q_Nx4Bj8YImg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.810838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/C9C2cj1aS_q_Nx4Bj8YImg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     4600 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/C9C2cj1aS_q_Nx4Bj8YImg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/C9C2cj1aS_q_Nx4Bj8YImg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.810838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/C9C2cj1aS_q_Nx4Bj8YImg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      924 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/C9C2cj1aS_q_Nx4Bj8YImg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CE-2EnNGTKSY_gd7i6nqsA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.810838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CE-2EnNGTKSY_gd7i6nqsA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7517 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CE-2EnNGTKSY_gd7i6nqsA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CE-2EnNGTKSY_gd7i6nqsA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.810838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CE-2EnNGTKSY_gd7i6nqsA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1104 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CE-2EnNGTKSY_gd7i6nqsA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CGU4FyPTS9eHQD5QApPhPA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.810838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CGU4FyPTS9eHQD5QApPhPA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7722 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CGU4FyPTS9eHQD5QApPhPA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CGU4FyPTS9eHQD5QApPhPA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.810838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CGU4FyPTS9eHQD5QApPhPA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      842 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CGU4FyPTS9eHQD5QApPhPA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CSTlwpXDRDyEUfFA22wvcQ/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.810838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CSTlwpXDRDyEUfFA22wvcQ/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CSTlwpXDRDyEUfFA22wvcQ/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CSTlwpXDRDyEUfFA22wvcQ/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.810838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CSTlwpXDRDyEUfFA22wvcQ/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      960 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CSTlwpXDRDyEUfFA22wvcQ/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Cyn7JDoPRwuRs_eShI9x4w/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.810838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Cyn7JDoPRwuRs_eShI9x4w/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     4589 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Cyn7JDoPRwuRs_eShI9x4w/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.694838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Cyn7JDoPRwuRs_eShI9x4w/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.814838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Cyn7JDoPRwuRs_eShI9x4w/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1068 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Cyn7JDoPRwuRs_eShI9x4w/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/D12fNQbWTgCF6SYMi7fdew/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.814838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/D12fNQbWTgCF6SYMi7fdew/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7502 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/D12fNQbWTgCF6SYMi7fdew/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/D12fNQbWTgCF6SYMi7fdew/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.814838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/D12fNQbWTgCF6SYMi7fdew/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1130 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/D12fNQbWTgCF6SYMi7fdew/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/DTDhDQy_Te-8TX2GWjDyRA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.814838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/DTDhDQy_Te-8TX2GWjDyRA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7708 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/DTDhDQy_Te-8TX2GWjDyRA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/DTDhDQy_Te-8TX2GWjDyRA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.814838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/DTDhDQy_Te-8TX2GWjDyRA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1079 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/DTDhDQy_Te-8TX2GWjDyRA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Db65HT83SdCGu8IcAEMSJw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.814838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Db65HT83SdCGu8IcAEMSJw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7711 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Db65HT83SdCGu8IcAEMSJw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Db65HT83SdCGu8IcAEMSJw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.814838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Db65HT83SdCGu8IcAEMSJw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1011 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Db65HT83SdCGu8IcAEMSJw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/DvotWT9VS4---6k12rWy2g/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.814838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/DvotWT9VS4---6k12rWy2g/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/DvotWT9VS4---6k12rWy2g/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/DvotWT9VS4---6k12rWy2g/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.814838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/DvotWT9VS4---6k12rWy2g/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      972 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/DvotWT9VS4---6k12rWy2g/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/F-2XbyLdRoOWYqs1Wkz1bw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.814838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/F-2XbyLdRoOWYqs1Wkz1bw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/F-2XbyLdRoOWYqs1Wkz1bw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/F-2XbyLdRoOWYqs1Wkz1bw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.814838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/F-2XbyLdRoOWYqs1Wkz1bw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      963 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/F-2XbyLdRoOWYqs1Wkz1bw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/FK4OkxYcQWqYpmxP1ay0_A/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.814838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/FK4OkxYcQWqYpmxP1ay0_A/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7703 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/FK4OkxYcQWqYpmxP1ay0_A/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/FK4OkxYcQWqYpmxP1ay0_A/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.814838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/FK4OkxYcQWqYpmxP1ay0_A/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1007 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/FK4OkxYcQWqYpmxP1ay0_A/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/FWlvKTVwRUqznJSgpz4mSA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.814838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/FWlvKTVwRUqznJSgpz4mSA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7697 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/FWlvKTVwRUqznJSgpz4mSA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/FWlvKTVwRUqznJSgpz4mSA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.814838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/FWlvKTVwRUqznJSgpz4mSA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1161 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/FWlvKTVwRUqznJSgpz4mSA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Fy4__LJrS7yOddt0JlST1g/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.814838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Fy4__LJrS7yOddt0JlST1g/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7517 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Fy4__LJrS7yOddt0JlST1g/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Fy4__LJrS7yOddt0JlST1g/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.814838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Fy4__LJrS7yOddt0JlST1g/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1105 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Fy4__LJrS7yOddt0JlST1g/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GSN2ZF03SvGfJWTNQOR66Q/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.818838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GSN2ZF03SvGfJWTNQOR66Q/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     6803 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GSN2ZF03SvGfJWTNQOR66Q/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GSN2ZF03SvGfJWTNQOR66Q/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.818838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GSN2ZF03SvGfJWTNQOR66Q/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1148 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GSN2ZF03SvGfJWTNQOR66Q/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Glj2IKdJQ1OoKLUOshkKuw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.818838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Glj2IKdJQ1OoKLUOshkKuw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7517 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Glj2IKdJQ1OoKLUOshkKuw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Glj2IKdJQ1OoKLUOshkKuw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.818838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Glj2IKdJQ1OoKLUOshkKuw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1116 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Glj2IKdJQ1OoKLUOshkKuw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GrUeski1SfiJNpkgzaWWww/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.818838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GrUeski1SfiJNpkgzaWWww/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     4600 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GrUeski1SfiJNpkgzaWWww/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.698838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GrUeski1SfiJNpkgzaWWww/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.818838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GrUeski1SfiJNpkgzaWWww/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      924 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GrUeski1SfiJNpkgzaWWww/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.702838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GxgYQf58TRaWVJ-2vy4tLg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.818838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GxgYQf58TRaWVJ-2vy4tLg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7500 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GxgYQf58TRaWVJ-2vy4tLg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.702838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GxgYQf58TRaWVJ-2vy4tLg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.818838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GxgYQf58TRaWVJ-2vy4tLg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1110 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GxgYQf58TRaWVJ-2vy4tLg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.702838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/H_rT971WQQayQyE8l4ABqA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.822838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/H_rT971WQQayQyE8l4ABqA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     4589 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/H_rT971WQQayQyE8l4ABqA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.702838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/H_rT971WQQayQyE8l4ABqA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.822838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/H_rT971WQQayQyE8l4ABqA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1013 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/H_rT971WQQayQyE8l4ABqA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.702838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/I1ojS418TMeExBMFJ3LcIA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.822838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/I1ojS418TMeExBMFJ3LcIA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/I1ojS418TMeExBMFJ3LcIA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.702838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/I1ojS418TMeExBMFJ3LcIA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.822838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/I1ojS418TMeExBMFJ3LcIA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      968 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/I1ojS418TMeExBMFJ3LcIA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.702838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/I2nBckWWSRahjagcQD3aCg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.822838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/I2nBckWWSRahjagcQD3aCg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     4589 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/I2nBckWWSRahjagcQD3aCg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.702838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/I2nBckWWSRahjagcQD3aCg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.822838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/I2nBckWWSRahjagcQD3aCg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1068 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/I2nBckWWSRahjagcQD3aCg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.702838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/IMcMRzZvTVyh5X4GdIMKUg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.822838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/IMcMRzZvTVyh5X4GdIMKUg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/IMcMRzZvTVyh5X4GdIMKUg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.702838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/IMcMRzZvTVyh5X4GdIMKUg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.822838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/IMcMRzZvTVyh5X4GdIMKUg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      955 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/IMcMRzZvTVyh5X4GdIMKUg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.702838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/INMgwWKtT7Kp5SH7zAfQ7w/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.822838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/INMgwWKtT7Kp5SH7zAfQ7w/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7711 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/INMgwWKtT7Kp5SH7zAfQ7w/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.702838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/INMgwWKtT7Kp5SH7zAfQ7w/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.822838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/INMgwWKtT7Kp5SH7zAfQ7w/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      993 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/INMgwWKtT7Kp5SH7zAfQ7w/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.702838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Je_Ek1ecSgidmukgi1oGjA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.822838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Je_Ek1ecSgidmukgi1oGjA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7517 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Je_Ek1ecSgidmukgi1oGjA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.702838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Je_Ek1ecSgidmukgi1oGjA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.822838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Je_Ek1ecSgidmukgi1oGjA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1104 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Je_Ek1ecSgidmukgi1oGjA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.702838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/JwuxI9J2Q5qC4D9dzziQmg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.826838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/JwuxI9J2Q5qC4D9dzziQmg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7517 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/JwuxI9J2Q5qC4D9dzziQmg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.702838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/JwuxI9J2Q5qC4D9dzziQmg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.826838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/JwuxI9J2Q5qC4D9dzziQmg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1117 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/JwuxI9J2Q5qC4D9dzziQmg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.702838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KbaNeW1hTJqiQyiUjsPz-Q/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.826838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KbaNeW1hTJqiQyiUjsPz-Q/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KbaNeW1hTJqiQyiUjsPz-Q/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.702838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KbaNeW1hTJqiQyiUjsPz-Q/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.826838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KbaNeW1hTJqiQyiUjsPz-Q/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      967 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KbaNeW1hTJqiQyiUjsPz-Q/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.702838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KjRoo3mLSUqYc6iRB10r6A/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.826838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KjRoo3mLSUqYc6iRB10r6A/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)    26068 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KjRoo3mLSUqYc6iRB10r6A/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KjRoo3mLSUqYc6iRB10r6A/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.826838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KjRoo3mLSUqYc6iRB10r6A/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      888 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KjRoo3mLSUqYc6iRB10r6A/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KqRwX5EUQcK1b39svcLjjw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.826838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KqRwX5EUQcK1b39svcLjjw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     4589 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KqRwX5EUQcK1b39svcLjjw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KqRwX5EUQcK1b39svcLjjw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.826838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KqRwX5EUQcK1b39svcLjjw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1007 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KqRwX5EUQcK1b39svcLjjw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/L1emPAoBROSoDSetQl5qYw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.826838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/L1emPAoBROSoDSetQl5qYw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7711 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/L1emPAoBROSoDSetQl5qYw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/L1emPAoBROSoDSetQl5qYw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.826838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/L1emPAoBROSoDSetQl5qYw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      993 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/L1emPAoBROSoDSetQl5qYw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LBuW7cjQS8-aE75qH-udRQ/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.826838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LBuW7cjQS8-aE75qH-udRQ/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7690 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LBuW7cjQS8-aE75qH-udRQ/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LBuW7cjQS8-aE75qH-udRQ/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.826838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LBuW7cjQS8-aE75qH-udRQ/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      850 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LBuW7cjQS8-aE75qH-udRQ/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LYO9FlvJQGSiffYQhMcW5Q/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.826838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LYO9FlvJQGSiffYQhMcW5Q/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)    25958 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LYO9FlvJQGSiffYQhMcW5Q/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LYO9FlvJQGSiffYQhMcW5Q/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.826838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LYO9FlvJQGSiffYQhMcW5Q/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      888 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LYO9FlvJQGSiffYQhMcW5Q/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Lelr43PoRWWgnumQRpIb8Q/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.826838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Lelr43PoRWWgnumQRpIb8Q/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     5086 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Lelr43PoRWWgnumQRpIb8Q/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Lelr43PoRWWgnumQRpIb8Q/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.830838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Lelr43PoRWWgnumQRpIb8Q/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      849 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Lelr43PoRWWgnumQRpIb8Q/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LjluSbFjS5qg3jljQ38itQ/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.830838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LjluSbFjS5qg3jljQ38itQ/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LjluSbFjS5qg3jljQ38itQ/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LjluSbFjS5qg3jljQ38itQ/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.830838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LjluSbFjS5qg3jljQ38itQ/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1107 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LjluSbFjS5qg3jljQ38itQ/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LzlIi12cQsWwfxig59k2VQ/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.830838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LzlIi12cQsWwfxig59k2VQ/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LzlIi12cQsWwfxig59k2VQ/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LzlIi12cQsWwfxig59k2VQ/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.830838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LzlIi12cQsWwfxig59k2VQ/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      972 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LzlIi12cQsWwfxig59k2VQ/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MIuWH-PkRdOQvhsM9elc5Q/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.830838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MIuWH-PkRdOQvhsM9elc5Q/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)    28473 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MIuWH-PkRdOQvhsM9elc5Q/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MIuWH-PkRdOQvhsM9elc5Q/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MIuWH-PkRdOQvhsM9elc5Q/artifacts/public/build/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.830838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MIuWH-PkRdOQvhsM9elc5Q/artifacts/public/build/en-US/
--rw-r--r--   0 worker    (1000) worker    (1000)      767 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MIuWH-PkRdOQvhsM9elc5Q/artifacts/public/build/en-US/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MJfJtItbRjmydzrvwwURrg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.830838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MJfJtItbRjmydzrvwwURrg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)    28495 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MJfJtItbRjmydzrvwwURrg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MJfJtItbRjmydzrvwwURrg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MJfJtItbRjmydzrvwwURrg/artifacts/public/build/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.830838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MJfJtItbRjmydzrvwwURrg/artifacts/public/build/en-US/
--rw-r--r--   0 worker    (1000) worker    (1000)      758 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MJfJtItbRjmydzrvwwURrg/artifacts/public/build/en-US/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.706838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MJm-0bUOR7WEyESS_3EuMg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.830838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MJm-0bUOR7WEyESS_3EuMg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7661 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MJm-0bUOR7WEyESS_3EuMg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.710838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MJm-0bUOR7WEyESS_3EuMg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.830838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MJm-0bUOR7WEyESS_3EuMg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1234 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MJm-0bUOR7WEyESS_3EuMg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.710838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MVFFVBcITlmoKD8m1Uqwkw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.830838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MVFFVBcITlmoKD8m1Uqwkw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MVFFVBcITlmoKD8m1Uqwkw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.710838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MVFFVBcITlmoKD8m1Uqwkw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.830838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MVFFVBcITlmoKD8m1Uqwkw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      975 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MVFFVBcITlmoKD8m1Uqwkw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.710838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Ma7H24MaS5GP8jZpl6R5Xw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.830838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Ma7H24MaS5GP8jZpl6R5Xw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Ma7H24MaS5GP8jZpl6R5Xw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.710838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Ma7H24MaS5GP8jZpl6R5Xw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.830838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Ma7H24MaS5GP8jZpl6R5Xw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      960 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Ma7H24MaS5GP8jZpl6R5Xw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.710838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/N491PvLhQcCSBX0gFmTKkg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.834838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/N491PvLhQcCSBX0gFmTKkg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7517 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/N491PvLhQcCSBX0gFmTKkg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.710838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/N491PvLhQcCSBX0gFmTKkg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.834838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/N491PvLhQcCSBX0gFmTKkg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1105 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/N491PvLhQcCSBX0gFmTKkg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.710838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/N7ENCbCgSvGvuiV3wM91Tg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.834838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/N7ENCbCgSvGvuiV3wM91Tg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/N7ENCbCgSvGvuiV3wM91Tg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.710838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/N7ENCbCgSvGvuiV3wM91Tg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.834838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/N7ENCbCgSvGvuiV3wM91Tg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1107 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/N7ENCbCgSvGvuiV3wM91Tg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.710838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/O2UuedRNRvSbkRXzgtfTZg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.834838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/O2UuedRNRvSbkRXzgtfTZg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7727 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/O2UuedRNRvSbkRXzgtfTZg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.710838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/O2UuedRNRvSbkRXzgtfTZg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.834838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/O2UuedRNRvSbkRXzgtfTZg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      983 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/O2UuedRNRvSbkRXzgtfTZg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.710838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/O5RMm0izRSSMLncwLUUZzA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.834838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/O5RMm0izRSSMLncwLUUZzA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7692 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/O5RMm0izRSSMLncwLUUZzA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.710838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/O5RMm0izRSSMLncwLUUZzA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.834838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/O5RMm0izRSSMLncwLUUZzA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1128 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/O5RMm0izRSSMLncwLUUZzA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.710838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Oxnm2nS5SQeujyAmxci87w/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.834838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Oxnm2nS5SQeujyAmxci87w/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Oxnm2nS5SQeujyAmxci87w/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.710838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Oxnm2nS5SQeujyAmxci87w/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.834838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Oxnm2nS5SQeujyAmxci87w/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1099 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Oxnm2nS5SQeujyAmxci87w/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.710838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PTEeGj5sQP-VOR_rereX_Q/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.834838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PTEeGj5sQP-VOR_rereX_Q/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)    28583 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PTEeGj5sQP-VOR_rereX_Q/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PTEeGj5sQP-VOR_rereX_Q/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PTEeGj5sQP-VOR_rereX_Q/artifacts/public/build/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.834838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PTEeGj5sQP-VOR_rereX_Q/artifacts/public/build/en-US/
--rw-r--r--   0 worker    (1000) worker    (1000)      764 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PTEeGj5sQP-VOR_rereX_Q/artifacts/public/build/en-US/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PU23u6VeRDWDKVUnX09Cvw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.834838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PU23u6VeRDWDKVUnX09Cvw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PU23u6VeRDWDKVUnX09Cvw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PU23u6VeRDWDKVUnX09Cvw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.834838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PU23u6VeRDWDKVUnX09Cvw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      972 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PU23u6VeRDWDKVUnX09Cvw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PUrV4bCUQ3GKWvMCV3_Bzw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.834838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PUrV4bCUQ3GKWvMCV3_Bzw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7722 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PUrV4bCUQ3GKWvMCV3_Bzw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PUrV4bCUQ3GKWvMCV3_Bzw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.834838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PUrV4bCUQ3GKWvMCV3_Bzw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      855 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PUrV4bCUQ3GKWvMCV3_Bzw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/QaS45XFwRASfCE9F9TaqCg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.834838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/QaS45XFwRASfCE9F9TaqCg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7727 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/QaS45XFwRASfCE9F9TaqCg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/QaS45XFwRASfCE9F9TaqCg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.834838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/QaS45XFwRASfCE9F9TaqCg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      927 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/QaS45XFwRASfCE9F9TaqCg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.834838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)    28825 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/artifacts/public/build/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/artifacts/public/build/en-US/
--rw-r--r--   0 worker    (1000) worker    (1000)      777 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/artifacts/public/build/en-US/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/R6b2C_MbQwWKJPjvs_PZaA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/R6b2C_MbQwWKJPjvs_PZaA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/R6b2C_MbQwWKJPjvs_PZaA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/R6b2C_MbQwWKJPjvs_PZaA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/R6b2C_MbQwWKJPjvs_PZaA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      960 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/R6b2C_MbQwWKJPjvs_PZaA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/R8E6ScjVREuVI0hLQorxwA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/R8E6ScjVREuVI0hLQorxwA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)    26068 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/R8E6ScjVREuVI0hLQorxwA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/R8E6ScjVREuVI0hLQorxwA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/R8E6ScjVREuVI0hLQorxwA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      888 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/R8E6ScjVREuVI0hLQorxwA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)    28143 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/artifacts/public/build/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/artifacts/public/build/en-US/
--rw-r--r--   0 worker    (1000) worker    (1000)      748 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/artifacts/public/build/en-US/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Rd61yPVqQ0CdZmbvuQ9YcQ/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Rd61yPVqQ0CdZmbvuQ9YcQ/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     4589 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Rd61yPVqQ0CdZmbvuQ9YcQ/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Rd61yPVqQ0CdZmbvuQ9YcQ/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Rd61yPVqQ0CdZmbvuQ9YcQ/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1001 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Rd61yPVqQ0CdZmbvuQ9YcQ/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/S1o0P_q8RM601Mq0d4urkw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/S1o0P_q8RM601Mq0d4urkw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     6983 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/S1o0P_q8RM601Mq0d4urkw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/S1o0P_q8RM601Mq0d4urkw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/S1o0P_q8RM601Mq0d4urkw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      994 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/S1o0P_q8RM601Mq0d4urkw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.714838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/SdJspoE-QROYKIlrSM5E9w/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/SdJspoE-QROYKIlrSM5E9w/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7697 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/SdJspoE-QROYKIlrSM5E9w/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/SdJspoE-QROYKIlrSM5E9w/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/SdJspoE-QROYKIlrSM5E9w/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1165 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/SdJspoE-QROYKIlrSM5E9w/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/SkWkmrKDSF2hQhnMOfS1PQ/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/SkWkmrKDSF2hQhnMOfS1PQ/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/SkWkmrKDSF2hQhnMOfS1PQ/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/SkWkmrKDSF2hQhnMOfS1PQ/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/SkWkmrKDSF2hQhnMOfS1PQ/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      972 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/SkWkmrKDSF2hQhnMOfS1PQ/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/T1ARQQKHTKu_m1EtjZv7YQ/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/T1ARQQKHTKu_m1EtjZv7YQ/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     8106 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/T1ARQQKHTKu_m1EtjZv7YQ/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/T1ARQQKHTKu_m1EtjZv7YQ/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/T1ARQQKHTKu_m1EtjZv7YQ/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      925 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/T1ARQQKHTKu_m1EtjZv7YQ/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TJD91R5LTxSyqoutUKFjtg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TJD91R5LTxSyqoutUKFjtg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)    28473 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TJD91R5LTxSyqoutUKFjtg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TJD91R5LTxSyqoutUKFjtg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TJD91R5LTxSyqoutUKFjtg/artifacts/public/build/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TJD91R5LTxSyqoutUKFjtg/artifacts/public/build/en-US/
--rw-r--r--   0 worker    (1000) worker    (1000)      768 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TJD91R5LTxSyqoutUKFjtg/artifacts/public/build/en-US/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TTYSB2nKSUWvv5rbQDLtzw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.838838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TTYSB2nKSUWvv5rbQDLtzw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TTYSB2nKSUWvv5rbQDLtzw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TTYSB2nKSUWvv5rbQDLtzw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TTYSB2nKSUWvv5rbQDLtzw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      963 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TTYSB2nKSUWvv5rbQDLtzw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TXelMo4QSxqUzn0l-PWWyg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TXelMo4QSxqUzn0l-PWWyg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7722 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TXelMo4QSxqUzn0l-PWWyg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TXelMo4QSxqUzn0l-PWWyg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TXelMo4QSxqUzn0l-PWWyg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      836 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TXelMo4QSxqUzn0l-PWWyg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ThUoABnMR12AkygRTIAcKA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ThUoABnMR12AkygRTIAcKA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7708 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ThUoABnMR12AkygRTIAcKA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ThUoABnMR12AkygRTIAcKA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ThUoABnMR12AkygRTIAcKA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1083 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ThUoABnMR12AkygRTIAcKA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TheuGGRAQEeVfrK_nIxlYA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TheuGGRAQEeVfrK_nIxlYA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     8240 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TheuGGRAQEeVfrK_nIxlYA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TheuGGRAQEeVfrK_nIxlYA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TheuGGRAQEeVfrK_nIxlYA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      841 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TheuGGRAQEeVfrK_nIxlYA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UUrwCxWRQ5OeCJEhZOQBHg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UUrwCxWRQ5OeCJEhZOQBHg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7711 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UUrwCxWRQ5OeCJEhZOQBHg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UUrwCxWRQ5OeCJEhZOQBHg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UUrwCxWRQ5OeCJEhZOQBHg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      999 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UUrwCxWRQ5OeCJEhZOQBHg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UoKNy4deRsKipcwj_CSJcA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UoKNy4deRsKipcwj_CSJcA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7521 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UoKNy4deRsKipcwj_CSJcA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UoKNy4deRsKipcwj_CSJcA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UoKNy4deRsKipcwj_CSJcA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1010 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UoKNy4deRsKipcwj_CSJcA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.718838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Ut4dGXE3RpCRQy6Pd2PpVg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Ut4dGXE3RpCRQy6Pd2PpVg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     4589 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Ut4dGXE3RpCRQy6Pd2PpVg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Ut4dGXE3RpCRQy6Pd2PpVg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Ut4dGXE3RpCRQy6Pd2PpVg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1080 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Ut4dGXE3RpCRQy6Pd2PpVg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UuWQ2KScQ3KrYF4wFkczHw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UuWQ2KScQ3KrYF4wFkczHw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)    28803 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UuWQ2KScQ3KrYF4wFkczHw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UuWQ2KScQ3KrYF4wFkczHw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UuWQ2KScQ3KrYF4wFkczHw/artifacts/public/build/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UuWQ2KScQ3KrYF4wFkczHw/artifacts/public/build/en-US/
--rw-r--r--   0 worker    (1000) worker    (1000)      787 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UuWQ2KScQ3KrYF4wFkczHw/artifacts/public/build/en-US/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/VSEShvqcSxWWtdKaO6jagQ/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/VSEShvqcSxWWtdKaO6jagQ/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/VSEShvqcSxWWtdKaO6jagQ/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/VSEShvqcSxWWtdKaO6jagQ/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/VSEShvqcSxWWtdKaO6jagQ/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1108 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/VSEShvqcSxWWtdKaO6jagQ/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/V_S-Ts-2TmmGgDExnyG6qw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/V_S-Ts-2TmmGgDExnyG6qw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     4589 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/V_S-Ts-2TmmGgDExnyG6qw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/V_S-Ts-2TmmGgDExnyG6qw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/V_S-Ts-2TmmGgDExnyG6qw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1007 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/V_S-Ts-2TmmGgDExnyG6qw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Vdir5WkdS-G7MKg1VPiWEg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.842838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Vdir5WkdS-G7MKg1VPiWEg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7711 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Vdir5WkdS-G7MKg1VPiWEg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Vdir5WkdS-G7MKg1VPiWEg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Vdir5WkdS-G7MKg1VPiWEg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      999 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Vdir5WkdS-G7MKg1VPiWEg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/VyFzvPDRSaaNnxo8A1krWg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/VyFzvPDRSaaNnxo8A1krWg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/VyFzvPDRSaaNnxo8A1krWg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/VyFzvPDRSaaNnxo8A1krWg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/VyFzvPDRSaaNnxo8A1krWg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      960 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/VyFzvPDRSaaNnxo8A1krWg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/WRq2BZCZRlCITcXJwi9VOA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/WRq2BZCZRlCITcXJwi9VOA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7880 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/WRq2BZCZRlCITcXJwi9VOA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/WRq2BZCZRlCITcXJwi9VOA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/WRq2BZCZRlCITcXJwi9VOA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1277 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/WRq2BZCZRlCITcXJwi9VOA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/XDp1D7tkQBK4u1XG4reYSA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/XDp1D7tkQBK4u1XG4reYSA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/XDp1D7tkQBK4u1XG4reYSA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/XDp1D7tkQBK4u1XG4reYSA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/XDp1D7tkQBK4u1XG4reYSA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      955 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/XDp1D7tkQBK4u1XG4reYSA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/XPfHK-vXS9uGpyq4-l6xtg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/XPfHK-vXS9uGpyq4-l6xtg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7697 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/XPfHK-vXS9uGpyq4-l6xtg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/XPfHK-vXS9uGpyq4-l6xtg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/XPfHK-vXS9uGpyq4-l6xtg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1165 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/XPfHK-vXS9uGpyq4-l6xtg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/X_XmczzYTA2l8JwACz-YBg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/X_XmczzYTA2l8JwACz-YBg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/X_XmczzYTA2l8JwACz-YBg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.722838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/X_XmczzYTA2l8JwACz-YBg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/X_XmczzYTA2l8JwACz-YBg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      967 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/X_XmczzYTA2l8JwACz-YBg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.726838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Y45GeFF7SPuy1IhX9CXMPw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Y45GeFF7SPuy1IhX9CXMPw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Y45GeFF7SPuy1IhX9CXMPw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.726838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Y45GeFF7SPuy1IhX9CXMPw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Y45GeFF7SPuy1IhX9CXMPw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      965 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Y45GeFF7SPuy1IhX9CXMPw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.726838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YE5qNXJbTuu2T2uXJhk5Nw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YE5qNXJbTuu2T2uXJhk5Nw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7723 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YE5qNXJbTuu2T2uXJhk5Nw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.726838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YE5qNXJbTuu2T2uXJhk5Nw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YE5qNXJbTuu2T2uXJhk5Nw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      995 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YE5qNXJbTuu2T2uXJhk5Nw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.726838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YGDcP8gRQPebxPg7efA7Iw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YGDcP8gRQPebxPg7efA7Iw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7690 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YGDcP8gRQPebxPg7efA7Iw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.726838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YGDcP8gRQPebxPg7efA7Iw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YGDcP8gRQPebxPg7efA7Iw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1274 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YGDcP8gRQPebxPg7efA7Iw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.726838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YWFg1gR3Rfu3LH7U6mB8EQ/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YWFg1gR3Rfu3LH7U6mB8EQ/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7500 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YWFg1gR3Rfu3LH7U6mB8EQ/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.726838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YWFg1gR3Rfu3LH7U6mB8EQ/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YWFg1gR3Rfu3LH7U6mB8EQ/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1110 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YWFg1gR3Rfu3LH7U6mB8EQ/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.726838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YWIA7hhsSCqyXKErOzGqIg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.846838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YWIA7hhsSCqyXKErOzGqIg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7703 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YWIA7hhsSCqyXKErOzGqIg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.726838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YWIA7hhsSCqyXKErOzGqIg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YWIA7hhsSCqyXKErOzGqIg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1004 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YWIA7hhsSCqyXKErOzGqIg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.726838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YYrpCCBgSSmTIrul3-dXGg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YYrpCCBgSSmTIrul3-dXGg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YYrpCCBgSSmTIrul3-dXGg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.726838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YYrpCCBgSSmTIrul3-dXGg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YYrpCCBgSSmTIrul3-dXGg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1111 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YYrpCCBgSSmTIrul3-dXGg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.726838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Yy5BKCQLSNKJmVlXUgZ-Vw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Yy5BKCQLSNKJmVlXUgZ-Vw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Yy5BKCQLSNKJmVlXUgZ-Vw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.726838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Yy5BKCQLSNKJmVlXUgZ-Vw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Yy5BKCQLSNKJmVlXUgZ-Vw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      956 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Yy5BKCQLSNKJmVlXUgZ-Vw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.726838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Z2wFgrvYQfWr4sZ_5xsJyg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Z2wFgrvYQfWr4sZ_5xsJyg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7500 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Z2wFgrvYQfWr4sZ_5xsJyg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.726838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Z2wFgrvYQfWr4sZ_5xsJyg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Z2wFgrvYQfWr4sZ_5xsJyg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1110 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Z2wFgrvYQfWr4sZ_5xsJyg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.726838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Z4Nk4adQT_KY6OB36jH7GA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Z4Nk4adQT_KY6OB36jH7GA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7711 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Z4Nk4adQT_KY6OB36jH7GA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.726838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Z4Nk4adQT_KY6OB36jH7GA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Z4Nk4adQT_KY6OB36jH7GA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      993 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Z4Nk4adQT_KY6OB36jH7GA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.726838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZHf8FbtqSZa-D8WeBBRQ9A/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZHf8FbtqSZa-D8WeBBRQ9A/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)    26068 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZHf8FbtqSZa-D8WeBBRQ9A/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.730838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZHf8FbtqSZa-D8WeBBRQ9A/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZHf8FbtqSZa-D8WeBBRQ9A/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      900 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZHf8FbtqSZa-D8WeBBRQ9A/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.730838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZKZozRyQT42x6mxaQ9LhnA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZKZozRyQT42x6mxaQ9LhnA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZKZozRyQT42x6mxaQ9LhnA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.730838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZKZozRyQT42x6mxaQ9LhnA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZKZozRyQT42x6mxaQ9LhnA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      967 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZKZozRyQT42x6mxaQ9LhnA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.730838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZcTIYEkjQO2aChxeIY6fbw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZcTIYEkjQO2aChxeIY6fbw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     6976 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZcTIYEkjQO2aChxeIY6fbw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.730838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZcTIYEkjQO2aChxeIY6fbw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZcTIYEkjQO2aChxeIY6fbw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1041 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZcTIYEkjQO2aChxeIY6fbw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.730838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZukWWPukRoqeGyztJsYEXQ/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZukWWPukRoqeGyztJsYEXQ/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZukWWPukRoqeGyztJsYEXQ/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.730838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZukWWPukRoqeGyztJsYEXQ/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZukWWPukRoqeGyztJsYEXQ/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      960 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZukWWPukRoqeGyztJsYEXQ/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.730838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aAfWVw75TbKJ9Ff4vdSdXA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aAfWVw75TbKJ9Ff4vdSdXA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aAfWVw75TbKJ9Ff4vdSdXA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.730838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aAfWVw75TbKJ9Ff4vdSdXA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aAfWVw75TbKJ9Ff4vdSdXA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      955 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aAfWVw75TbKJ9Ff4vdSdXA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.730838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aNOLmiYFSnm51F5o0EF10A/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aNOLmiYFSnm51F5o0EF10A/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aNOLmiYFSnm51F5o0EF10A/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.730838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aNOLmiYFSnm51F5o0EF10A/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.850838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aNOLmiYFSnm51F5o0EF10A/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      960 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aNOLmiYFSnm51F5o0EF10A/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.730838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aNUeGazgSEqDVyec14YaHw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aNUeGazgSEqDVyec14YaHw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7502 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aNUeGazgSEqDVyec14YaHw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.730838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aNUeGazgSEqDVyec14YaHw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aNUeGazgSEqDVyec14YaHw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1130 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aNUeGazgSEqDVyec14YaHw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.730838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ac88QqpjTJuP6ZX2Is6yEQ/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ac88QqpjTJuP6ZX2Is6yEQ/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7711 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ac88QqpjTJuP6ZX2Is6yEQ/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.730838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ac88QqpjTJuP6ZX2Is6yEQ/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ac88QqpjTJuP6ZX2Is6yEQ/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1005 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ac88QqpjTJuP6ZX2Is6yEQ/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.730838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/auiN3S92TkiF21ayWnyfkw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/auiN3S92TkiF21ayWnyfkw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/auiN3S92TkiF21ayWnyfkw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.730838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/auiN3S92TkiF21ayWnyfkw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/auiN3S92TkiF21ayWnyfkw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      960 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/auiN3S92TkiF21ayWnyfkw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.730838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bkCYr42WR-aMl0t-rO918w/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bkCYr42WR-aMl0t-rO918w/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7711 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bkCYr42WR-aMl0t-rO918w/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.730838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bkCYr42WR-aMl0t-rO918w/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bkCYr42WR-aMl0t-rO918w/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      999 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bkCYr42WR-aMl0t-rO918w/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.734838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bqTeNQLPSHqviqZ-adbEgw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bqTeNQLPSHqviqZ-adbEgw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bqTeNQLPSHqviqZ-adbEgw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.734838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bqTeNQLPSHqviqZ-adbEgw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bqTeNQLPSHqviqZ-adbEgw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1099 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bqTeNQLPSHqviqZ-adbEgw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.734838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bsfhDaUBSZ-4IPUk_eXaSA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bsfhDaUBSZ-4IPUk_eXaSA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     4209 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bsfhDaUBSZ-4IPUk_eXaSA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.734838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bsfhDaUBSZ-4IPUk_eXaSA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bsfhDaUBSZ-4IPUk_eXaSA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      850 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bsfhDaUBSZ-4IPUk_eXaSA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.734838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bwP8UBmpRRKBOstsMyYOtg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bwP8UBmpRRKBOstsMyYOtg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bwP8UBmpRRKBOstsMyYOtg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.734838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bwP8UBmpRRKBOstsMyYOtg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bwP8UBmpRRKBOstsMyYOtg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1119 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bwP8UBmpRRKBOstsMyYOtg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.734838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cEquZnIzQZKo-sHRNoWdxA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cEquZnIzQZKo-sHRNoWdxA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7727 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cEquZnIzQZKo-sHRNoWdxA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.734838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cEquZnIzQZKo-sHRNoWdxA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cEquZnIzQZKo-sHRNoWdxA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1002 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cEquZnIzQZKo-sHRNoWdxA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.734838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cf-lJNFgSsmK89NsnoUNqg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cf-lJNFgSsmK89NsnoUNqg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cf-lJNFgSsmK89NsnoUNqg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.734838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cf-lJNFgSsmK89NsnoUNqg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cf-lJNFgSsmK89NsnoUNqg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1041 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cf-lJNFgSsmK89NsnoUNqg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.734838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cfhgadFrQqGdfkUQrE8DNA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cfhgadFrQqGdfkUQrE8DNA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cfhgadFrQqGdfkUQrE8DNA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.734838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cfhgadFrQqGdfkUQrE8DNA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.854838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cfhgadFrQqGdfkUQrE8DNA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      967 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cfhgadFrQqGdfkUQrE8DNA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.734838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cxsX3JgCRt-tEsH-ouLt3Q/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cxsX3JgCRt-tEsH-ouLt3Q/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     4041 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cxsX3JgCRt-tEsH-ouLt3Q/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.734838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cxsX3JgCRt-tEsH-ouLt3Q/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cxsX3JgCRt-tEsH-ouLt3Q/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1089 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cxsX3JgCRt-tEsH-ouLt3Q/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.734838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dNgIzJgjTlyYH24pQzLBug/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dNgIzJgjTlyYH24pQzLBug/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7500 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dNgIzJgjTlyYH24pQzLBug/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.734838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dNgIzJgjTlyYH24pQzLBug/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dNgIzJgjTlyYH24pQzLBug/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1110 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dNgIzJgjTlyYH24pQzLBug/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.734838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dZl_9NHxRkSM2YzG1Y29YA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dZl_9NHxRkSM2YzG1Y29YA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dZl_9NHxRkSM2YzG1Y29YA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.734838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dZl_9NHxRkSM2YzG1Y29YA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dZl_9NHxRkSM2YzG1Y29YA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1111 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dZl_9NHxRkSM2YzG1Y29YA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.734838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dcY-KGqYTdy67l7zA9K57Q/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dcY-KGqYTdy67l7zA9K57Q/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dcY-KGqYTdy67l7zA9K57Q/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.738838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dcY-KGqYTdy67l7zA9K57Q/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dcY-KGqYTdy67l7zA9K57Q/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1108 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dcY-KGqYTdy67l7zA9K57Q/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.738838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/e-15mv-6TR2SJu3iX1dz6w/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/e-15mv-6TR2SJu3iX1dz6w/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     8106 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/e-15mv-6TR2SJu3iX1dz6w/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.738838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/e-15mv-6TR2SJu3iX1dz6w/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/e-15mv-6TR2SJu3iX1dz6w/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      933 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/e-15mv-6TR2SJu3iX1dz6w/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.738838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/e8lqN78UTRWWOtoT1U9YKw/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/e8lqN78UTRWWOtoT1U9YKw/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7727 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/e8lqN78UTRWWOtoT1U9YKw/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.738838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/e8lqN78UTRWWOtoT1U9YKw/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/e8lqN78UTRWWOtoT1U9YKw/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      919 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/e8lqN78UTRWWOtoT1U9YKw/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.738838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eEzNLZ8CRPG_rqJt94V2Jg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eEzNLZ8CRPG_rqJt94V2Jg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     4589 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eEzNLZ8CRPG_rqJt94V2Jg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.738838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eEzNLZ8CRPG_rqJt94V2Jg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eEzNLZ8CRPG_rqJt94V2Jg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1001 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eEzNLZ8CRPG_rqJt94V2Jg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.738838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eNr5UDpwSv-owhKwo5RR5w/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eNr5UDpwSv-owhKwo5RR5w/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eNr5UDpwSv-owhKwo5RR5w/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.738838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eNr5UDpwSv-owhKwo5RR5w/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eNr5UDpwSv-owhKwo5RR5w/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      972 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eNr5UDpwSv-owhKwo5RR5w/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.738838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eRpROunvQa-sZ5n-zmHFCA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eRpROunvQa-sZ5n-zmHFCA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)    28913 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eRpROunvQa-sZ5n-zmHFCA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.738838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eRpROunvQa-sZ5n-zmHFCA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.738838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eRpROunvQa-sZ5n-zmHFCA/artifacts/public/build/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eRpROunvQa-sZ5n-zmHFCA/artifacts/public/build/en-US/
--rw-r--r--   0 worker    (1000) worker    (1000)      783 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eRpROunvQa-sZ5n-zmHFCA/artifacts/public/build/en-US/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.738838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eUk3ZT1tQHmJBu06q-E-AQ/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eUk3ZT1tQHmJBu06q-E-AQ/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7880 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eUk3ZT1tQHmJBu06q-E-AQ/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.738838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eUk3ZT1tQHmJBu06q-E-AQ/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eUk3ZT1tQHmJBu06q-E-AQ/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1269 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eUk3ZT1tQHmJBu06q-E-AQ/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.738838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ebZgCLndSm2ew4fN6uM48Q/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.858838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ebZgCLndSm2ew4fN6uM48Q/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     4589 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ebZgCLndSm2ew4fN6uM48Q/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.738838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ebZgCLndSm2ew4fN6uM48Q/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.862838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ebZgCLndSm2ew4fN6uM48Q/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1019 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ebZgCLndSm2ew4fN6uM48Q/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.738838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/erjBtcr7TeaKF9WkHH3fAA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.862838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/erjBtcr7TeaKF9WkHH3fAA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7711 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/erjBtcr7TeaKF9WkHH3fAA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.738838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/erjBtcr7TeaKF9WkHH3fAA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.862838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/erjBtcr7TeaKF9WkHH3fAA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)     1005 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/erjBtcr7TeaKF9WkHH3fAA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.738838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/esk9JKa7QxyKNF-pmg5UVA/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.862838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/esk9JKa7QxyKNF-pmg5UVA/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7723 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/esk9JKa7QxyKNF-pmg5UVA/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.742838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/esk9JKa7QxyKNF-pmg5UVA/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.862838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/esk9JKa7QxyKNF-pmg5UVA/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      976 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/esk9JKa7QxyKNF-pmg5UVA/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.742838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fMxvFK8yQQqnSYNv2r8Fyg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.862838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fMxvFK8yQQqnSYNv2r8Fyg/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7722 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fMxvFK8yQQqnSYNv2r8Fyg/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.742838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fMxvFK8yQQqnSYNv2r8Fyg/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.862838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fMxvFK8yQQqnSYNv2r8Fyg/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      850 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fMxvFK8yQQqnSYNv2r8Fyg/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.742838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fcYf8jKOQ9yV6VtZtbFNJQ/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.862838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fcYf8jKOQ9yV6VtZtbFNJQ/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     4236 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fcYf8jKOQ9yV6VtZtbFNJQ/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.742838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fcYf8jKOQ9yV6VtZtbFNJQ/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.862838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fcYf8jKOQ9yV6VtZtbFNJQ/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      850 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fcYf8jKOQ9yV6VtZtbFNJQ/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.742838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ff3I1qWyRvSKVMYbEZh39g/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.862838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ff3I1qWyRvSKVMYbEZh39g/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ff3I1qWyRvSKVMYbEZh39g/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.742838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ff3I1qWyRvSKVMYbEZh39g/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.862838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ff3I1qWyRvSKVMYbEZh39g/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      960 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ff3I1qWyRvSKVMYbEZh39g/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.742838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fn7T0nqKSK-wX_RsitMQwQ/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.862838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fn7T0nqKSK-wX_RsitMQwQ/artifacts/
--rw-r--r--   0 worker    (1000) worker    (1000)     1244 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fn7T0nqKSK-wX_RsitMQwQ/artifacts/.get
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.742838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fn7T0nqKSK-wX_RsitMQwQ/artifacts/public/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.862838 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fn7T0nqKSK-wX_RsitMQwQ/artifacts/public/build/
--rw-r--r--   0 worker    (1000) worker    (1000)      100 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fn7T0nqKSK-wX_RsitMQwQ/artifacts/public/build/target.json
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.742838 fuzzfetch-6.0.0/tests/mock-hg/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.742838 fuzzfetch-6.0.0/tests/mock-hg/mozilla-central/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.862838 fuzzfetch-6.0.0/tests/mock-hg/mozilla-central/json-rev/
--rw-r--r--   0 worker    (1000) worker    (1000)   273670 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-hg/mozilla-central/json-rev/10aa74237898
--rw-r--r--   0 worker    (1000) worker    (1000)    10073 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-hg/mozilla-central/json-rev/5096e8be57730ef6902aaa8954b79aa0a21b32d6
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.742838 fuzzfetch-6.0.0/tests/mock-product-details/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-03-13 21:02:54.862838 fuzzfetch-6.0.0/tests/mock-product-details/1.0/
--rw-r--r--   0 worker    (1000) worker    (1000)      673 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/mock-product-details/1.0/firefox_versions.json
--rw-r--r--   0 worker    (1000) worker    (1000)     2621 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/test_core.py
--rw-r--r--   0 worker    (1000) worker    (1000)     2266 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/test_extract.py
--rw-r--r--   0 worker    (1000) worker    (1000)     9989 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tests/test_fetch.py
--rw-r--r--   0 worker    (1000) worker    (1000)     1301 2024-03-13 21:02:47.000000 fuzzfetch-6.0.0/tox.ini
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.341250 fuzzfetch-7.0.0/
+-rw-r--r--   0 worker    (1000) worker    (1000)       55 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/.codecov.yml
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.237249 fuzzfetch-7.0.0/.github/
+-rw-r--r--   0 worker    (1000) worker    (1000)       42 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/.github/CODEOWNERS
+-rw-r--r--   0 worker    (1000) worker    (1000)      386 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/.gitignore
+-rw-r--r--   0 worker    (1000) worker    (1000)     1784 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 worker    (1000) worker    (1000)     3600 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/.taskcluster.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      689 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 worker    (1000) worker    (1000)    15550 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/LICENSE.md
+-rw-r--r--   0 worker    (1000) worker    (1000)     5450 2024-04-30 19:48:25.341250 fuzzfetch-7.0.0/PKG-INFO
+-rw-r--r--   0 worker    (1000) worker    (1000)     4609 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/README.md
+-rw-r--r--   0 worker    (1000) worker    (1000)      891 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/pyproject.toml
+-rw-r--r--   0 worker    (1000) worker    (1000)      970 2024-04-30 19:48:25.345250 fuzzfetch-7.0.0/setup.cfg
+-rwxr-xr-x   0 worker    (1000) worker    (1000)      370 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/setup.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.189249 fuzzfetch-7.0.0/src/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.241249 fuzzfetch-7.0.0/src/fuzzfetch/
+-rw-r--r--   0 worker    (1000) worker    (1000)      586 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/src/fuzzfetch/__init__.py
+-rw-r--r--   0 worker    (1000) worker    (1000)      288 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/src/fuzzfetch/__main__.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    10049 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/src/fuzzfetch/args.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    34356 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/src/fuzzfetch/core.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     3637 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/src/fuzzfetch/download.py
+-rw-r--r--   0 worker    (1000) worker    (1000)      358 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/src/fuzzfetch/errors.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     5634 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/src/fuzzfetch/extract.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    13368 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/src/fuzzfetch/models.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     2685 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/src/fuzzfetch/path.py
+-rw-r--r--   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/src/fuzzfetch/py.typed
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.341250 fuzzfetch-7.0.0/src/fuzzfetch.egg-info/
+-rw-r--r--   0 worker    (1000) worker    (1000)     5450 2024-04-30 19:48:25.000000 fuzzfetch-7.0.0/src/fuzzfetch.egg-info/PKG-INFO
+-rw-r--r--   0 worker    (1000) worker    (1000)    54516 2024-04-30 19:48:25.000000 fuzzfetch-7.0.0/src/fuzzfetch.egg-info/SOURCES.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        1 2024-04-30 19:48:25.000000 fuzzfetch-7.0.0/src/fuzzfetch.egg-info/dependency_links.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)       53 2024-04-30 19:48:25.000000 fuzzfetch-7.0.0/src/fuzzfetch.egg-info/entry_points.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        1 2024-04-30 19:48:25.000000 fuzzfetch-7.0.0/src/fuzzfetch.egg-info/not-zip-safe
+-rw-r--r--   0 worker    (1000) worker    (1000)       36 2024-04-30 19:48:25.000000 fuzzfetch-7.0.0/src/fuzzfetch.egg-info/requires.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)       10 2024-04-30 19:48:25.000000 fuzzfetch-7.0.0/src/fuzzfetch.egg-info/top_level.txt
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.241249 fuzzfetch-7.0.0/tests/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4127 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/conftest.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.189249 fuzzfetch-7.0.0/tests/mock-firefoxci/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.189249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.189249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.189249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.245249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/
+-rw-r--r--   0 worker    (1000) worker    (1000)      351 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2022.12.31
+-rw-r--r--   0 worker    (1000) worker    (1000)      351 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2023.01.02
+-rw-r--r--   0 worker    (1000) worker    (1000)      522 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2023.01.03
+-rw-r--r--   0 worker    (1000) worker    (1000)      864 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2023.01.04
+-rw-r--r--   0 worker    (1000) worker    (1000)      693 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2023.01.05
+-rw-r--r--   0 worker    (1000) worker    (1000)      693 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2023.11.23
+-rw-r--r--   0 worker    (1000) worker    (1000)      522 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2024.01.01
+-rw-r--r--   0 worker    (1000) worker    (1000)      351 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2024.01.02
+-rw-r--r--   0 worker    (1000) worker    (1000)       23 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2024.01.03
+-rw-r--r--   0 worker    (1000) worker    (1000)      341 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2022.12.31
+-rw-r--r--   0 worker    (1000) worker    (1000)      341 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2023.01.02
+-rw-r--r--   0 worker    (1000) worker    (1000)      341 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2023.01.03
+-rw-r--r--   0 worker    (1000) worker    (1000)      341 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2023.01.04
+-rw-r--r--   0 worker    (1000) worker    (1000)      341 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2023.01.05
+-rw-r--r--   0 worker    (1000) worker    (1000)      341 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2023.11.23
+-rw-r--r--   0 worker    (1000) worker    (1000)      341 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2024.01.01
+-rw-r--r--   0 worker    (1000) worker    (1000)      341 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2024.01.02
+-rw-r--r--   0 worker    (1000) worker    (1000)       23 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2024.01.03
+-rw-r--r--   0 worker    (1000) worker    (1000)      349 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-esr115.pushdate.2023.12.30
+-rw-r--r--   0 worker    (1000) worker    (1000)      349 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-esr115.pushdate.2024.01.02
+-rw-r--r--   0 worker    (1000) worker    (1000)      339 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-esr115.shippable.2023.12.30
+-rw-r--r--   0 worker    (1000) worker    (1000)       23 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-esr115.shippable.2024.01.02
+-rw-r--r--   0 worker    (1000) worker    (1000)    11775 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2023.12.29
+-rw-r--r--   0 worker    (1000) worker    (1000)     6051 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2024.01.02
+-rw-r--r--   0 worker    (1000) worker    (1000)      317 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.shippable.2023.12.29
+-rw-r--r--   0 worker    (1000) worker    (1000)      317 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.shippable.2024.01.02
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.293250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/
+-rw-r--r--   0 worker    (1000) worker    (1000)      188 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      187 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      193 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      210 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-ccov-fuzzing-asan-nyx-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      201 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-ccov-fuzzing-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      184 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-ccov-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      190 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      205 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-asan-afl-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      205 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-asan-nyx-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      201 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      198 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      201 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      191 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-searchfox-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      193 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      210 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-aarch64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      207 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-aarch64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      191 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      202 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      199 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      202 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.sm-linux64-fuzzilli-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      188 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win32-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      196 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win32-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      196 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-aarch64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      191 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      199 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-ccov-fuzzing-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      182 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-ccov-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      188 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      196 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      193 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.mobile.android-arm-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      215 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2023.11.23.20231123095534.firefox.linux64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      216 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      221 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      229 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux64-ccov-fuzzing-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      212 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux64-ccov-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      218 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      229 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      226 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      229 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux64-fuzzing-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      216 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      221 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.linux64-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      238 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.macosx64-aarch64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      235 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.macosx64-aarch64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      219 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.macosx64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      230 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.macosx64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      227 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.macosx64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      216 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.win32-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      224 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.win32-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      224 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.win64-aarch64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      219 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.win64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      227 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.win64-ccov-fuzzing-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      210 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.win64-ccov-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      216 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.win64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      224 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.firefox.win64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      221 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.20240102095659.mobile.android-arm-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      208 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2024.01.02.latest.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      231 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.10aa7423789835a7dbd24b0b44ad1ae2ad77b59b.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      231 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      236 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      244 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux64-ccov-fuzzing-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      227 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux64-ccov-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      233 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      244 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      241 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      244 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux64-fuzzing-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      231 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      236 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux64-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      253 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.macosx64-aarch64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      250 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.macosx64-aarch64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      234 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.macosx64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      245 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.macosx64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      242 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.macosx64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      231 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win32-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      239 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win32-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      239 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win64-aarch64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      234 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      242 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win64-ccov-fuzzing-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      225 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win64-ccov-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      231 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      239 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      229 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      236 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.mobile.android-arm-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      230 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.8366d9b1b0ca63aa3b706dd53ce23f052221c11b.firefox.linux64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      231 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.9d96d2c96d8fe1d9365fdaee30d8fda048c48aa1.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      232 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.cd184ad5b96078dbc9d4251ed366d7acff965d7a.firefox.macosx64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      209 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2023.01.02.latest.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      209 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2023.01.03.latest.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      209 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2023.01.04.latest.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      209 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2023.01.05.latest.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      218 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.01.latest.firefox.macosx64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      210 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.01.latest.firefox.macosx64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      207 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.02.latest.firefox.linux-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      209 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.02.latest.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      207 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.02.latest.firefox.win32-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      215 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.02.latest.firefox.win64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      207 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.02.latest.firefox.win64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      216 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.02.latest.mobile.android-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      212 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.02.latest.mobile.android-arm-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      212 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.02.latest.mobile.android-x86-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      215 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2024.01.02.latest.mobile.android-x86_64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      196 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.linux-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      198 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      207 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.macosx64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      199 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.macosx64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      196 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.win32-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      204 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.win64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      196 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.win64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      205 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.mobile.android-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      201 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.mobile.android-arm-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      201 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.mobile.android-x86-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      204 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.mobile.android-x86_64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      239 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.linux-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      239 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win32-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      247 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.firefox.win64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      248 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.mobile.android-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      244 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.mobile.android-arm-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      244 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.mobile.android-x86-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      247 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.60c369c930dc96abae06a2e0ad6833a3574b803f.mobile.android-x86_64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      250 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.cd184ad5b96078dbc9d4251ed366d7acff965d7a.firefox.macosx64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      187 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.linux-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      192 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.linux64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      189 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.linux64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      200 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.linux64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      197 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.linux64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      190 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.macosx64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      201 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.macosx64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      198 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.macosx64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      187 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.win32-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      187 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.latest.firefox.win64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      220 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2023.12.30.20231230171938.firefox.linux64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      228 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2023.12.30.20231230171938.firefox.linux64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      218 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2023.12.30.20231230171938.firefox.macosx64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      226 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2023.12.30.20231230171938.firefox.macosx64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      215 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2024.01.02.20240102145026.firefox.linux-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      217 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2024.01.02.20240102145026.firefox.linux64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      225 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2024.01.02.20240102145026.firefox.linux64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      229 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2024.01.02.20240102145026.firefox.macosx64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      215 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2024.01.02.20240102145026.firefox.win32-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      215 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.pushdate.2024.01.02.20240102145026.firefox.win64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      230 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.636a9054f04b5c65a4fbe1b79b91f1ee32629a99.firefox.linux-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      232 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.636a9054f04b5c65a4fbe1b79b91f1ee32629a99.firefox.linux64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      240 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.636a9054f04b5c65a4fbe1b79b91f1ee32629a99.firefox.linux64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      244 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.636a9054f04b5c65a4fbe1b79b91f1ee32629a99.firefox.macosx64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      230 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.636a9054f04b5c65a4fbe1b79b91f1ee32629a99.firefox.win32-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      230 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.636a9054f04b5c65a4fbe1b79b91f1ee32629a99.firefox.win64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      235 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.b8d6f1fcefecf913f749aa0b95daeb0874bda967.firefox.linux64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      243 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.b8d6f1fcefecf913f749aa0b95daeb0874bda967.firefox.linux64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      233 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.b8d6f1fcefecf913f749aa0b95daeb0874bda967.firefox.macosx64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      241 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.b8d6f1fcefecf913f749aa0b95daeb0874bda967.firefox.macosx64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      228 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.revision.b8d6f1fcefecf913f749aa0b95daeb0874bda967.firefox.win32-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      206 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.2023.12.30.latest.firefox.linux-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      208 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.2023.12.30.latest.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      209 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.2023.12.30.latest.firefox.macosx64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      206 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.2023.12.30.latest.firefox.win32-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      206 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.2023.12.30.latest.firefox.win64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      195 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.latest.firefox.linux-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      197 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.latest.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      198 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.latest.firefox.macosx64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      195 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.latest.firefox.win32-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      195 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.latest.firefox.win64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      238 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.revision.b8d6f1fcefecf913f749aa0b95daeb0874bda967.firefox.linux-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      240 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.revision.b8d6f1fcefecf913f749aa0b95daeb0874bda967.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      241 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.revision.b8d6f1fcefecf913f749aa0b95daeb0874bda967.firefox.macosx64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      238 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr115.shippable.revision.b8d6f1fcefecf913f749aa0b95daeb0874bda967.firefox.win64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      176 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      187 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      184 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      175 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      181 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      178 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      189 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      186 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      189 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-fuzzing-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      181 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      198 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-aarch64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      195 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-aarch64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      179 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      190 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      187 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      176 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win32-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      184 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win32-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      184 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win64-aarch64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      176 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      184 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      181 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.mobile.android-arm-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      209 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2023.12.29.20231229173843.mobile.android-arm-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      215 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2023.12.29.20231229181418.firefox.linux-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      212 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2023.12.29.20231229181418.firefox.linux-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      206 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102004535.firefox.linux64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      209 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102004535.firefox.linux64-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      207 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102004535.firefox.macosx64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      204 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102004535.firefox.win32-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      204 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102004535.firefox.win64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      209 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102024042.firefox.linux64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      203 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.linux64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      217 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.linux64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      214 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.linux64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      217 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.linux64-fuzzing-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      226 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.macosx64-aarch64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      223 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.macosx64-aarch64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      218 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.macosx64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      215 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.macosx64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      212 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.win32-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      212 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.win64-aarch64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      212 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102100456.firefox.win64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      204 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2024.01.02.20240102103153.firefox.linux-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      217 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.40c9a6c168c2e2f0fd8154c4e566ed7670a08fb6.firefox.win32-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      217 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.40c9a6c168c2e2f0fd8154c4e566ed7670a08fb6.firefox.win64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      224 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.50ea3793201650ea9a2c841a7e0c4904fc45e782.firefox.linux64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      221 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.50ea3793201650ea9a2c841a7e0c4904fc45e782.firefox.linux64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      224 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.50ea3793201650ea9a2c841a7e0c4904fc45e782.firefox.linux64-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      222 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.50ea3793201650ea9a2c841a7e0c4904fc45e782.firefox.macosx64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      219 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.50ea3793201650ea9a2c841a7e0c4904fc45e782.firefox.win32-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      219 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.50ea3793201650ea9a2c841a7e0c4904fc45e782.firefox.win64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      230 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.50f00cc1d403ff2c42e97aa0ac7bf953d370fead.firefox.linux-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      227 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.50f00cc1d403ff2c42e97aa0ac7bf953d370fead.firefox.linux-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      224 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.50f00cc1d403ff2c42e97aa0ac7bf953d370fead.mobile.android-arm-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      218 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.584364cc704f114b73f6d0ecea71f4435dd0d49b.firefox.linux64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      219 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.584364cc704f114b73f6d0ecea71f4435dd0d49b.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      219 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.d0e78ab7f522d06f92bebfcd18f806a2dd1bd391.firefox.linux-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      226 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.d0e78ab7f522d06f92bebfcd18f806a2dd1bd391.mobile.android-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      232 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.linux64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      229 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.linux64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      232 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.linux64-fuzzing-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      241 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.macosx64-aarch64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      238 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.macosx64-aarch64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      233 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.macosx64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      230 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.macosx64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      227 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.win32-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      227 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.win64-aarch64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      227 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ee90eb1b490de12447f767c9d616f8e07f95ee79.firefox.win64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      195 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.firefox.linux-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      197 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      206 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.firefox.macosx64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      198 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.firefox.macosx64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      195 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.firefox.win32-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      203 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.firefox.win64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      195 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.firefox.win64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      204 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.mobile.android-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      200 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.mobile.android-arm-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      200 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.mobile.android-x86-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      203 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2024.01.02.latest.mobile.android-x86_64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      184 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.linux-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      186 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      195 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.macosx64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      187 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.macosx64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      184 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.win32-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      192 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.win64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      184 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.win64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      193 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.mobile.android-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      189 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.mobile.android-arm-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      189 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.mobile.android-x86-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      192 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.mobile.android-x86_64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      227 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.d0e78ab7f522d06f92bebfcd18f806a2dd1bd391.firefox.linux-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      238 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.d0e78ab7f522d06f92bebfcd18f806a2dd1bd391.firefox.macosx64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      230 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.d0e78ab7f522d06f92bebfcd18f806a2dd1bd391.firefox.macosx64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      235 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.d0e78ab7f522d06f92bebfcd18f806a2dd1bd391.firefox.win64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      232 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.d0e78ab7f522d06f92bebfcd18f806a2dd1bd391.mobile.android-arm-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      232 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.d0e78ab7f522d06f92bebfcd18f806a2dd1bd391.mobile.android-x86-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      235 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.d0e78ab7f522d06f92bebfcd18f806a2dd1bd391.mobile.android-x86_64-opt
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.189249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.189249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.237249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.189249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/AGuXN_zgSTa4G2cOowM6tw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.293250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/AGuXN_zgSTa4G2cOowM6tw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7502 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/AGuXN_zgSTa4G2cOowM6tw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.189249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/AGuXN_zgSTa4G2cOowM6tw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.293250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/AGuXN_zgSTa4G2cOowM6tw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1133 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/AGuXN_zgSTa4G2cOowM6tw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.189249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Agexc3H0RvCxvLshb-oAkA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.293250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Agexc3H0RvCxvLshb-oAkA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Agexc3H0RvCxvLshb-oAkA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.189249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Agexc3H0RvCxvLshb-oAkA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.293250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Agexc3H0RvCxvLshb-oAkA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      956 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Agexc3H0RvCxvLshb-oAkA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.189249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/BMzeSq6sTVyo9tPp5vXCDg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.293250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/BMzeSq6sTVyo9tPp5vXCDg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     6983 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/BMzeSq6sTVyo9tPp5vXCDg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.189249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/BMzeSq6sTVyo9tPp5vXCDg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.293250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/BMzeSq6sTVyo9tPp5vXCDg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      975 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/BMzeSq6sTVyo9tPp5vXCDg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.189249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Bs_nyxXCTNm5hMfjX7DFwg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.293250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Bs_nyxXCTNm5hMfjX7DFwg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Bs_nyxXCTNm5hMfjX7DFwg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.189249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Bs_nyxXCTNm5hMfjX7DFwg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Bs_nyxXCTNm5hMfjX7DFwg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1120 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Bs_nyxXCTNm5hMfjX7DFwg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.189249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/C7bbCHVySOCJsQ24TJvNig/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/C7bbCHVySOCJsQ24TJvNig/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7692 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/C7bbCHVySOCJsQ24TJvNig/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.189249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/C7bbCHVySOCJsQ24TJvNig/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/C7bbCHVySOCJsQ24TJvNig/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1125 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/C7bbCHVySOCJsQ24TJvNig/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.189249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/C9C2cj1aS_q_Nx4Bj8YImg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/C9C2cj1aS_q_Nx4Bj8YImg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4600 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/C9C2cj1aS_q_Nx4Bj8YImg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/C9C2cj1aS_q_Nx4Bj8YImg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/C9C2cj1aS_q_Nx4Bj8YImg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      924 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/C9C2cj1aS_q_Nx4Bj8YImg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CE-2EnNGTKSY_gd7i6nqsA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CE-2EnNGTKSY_gd7i6nqsA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7517 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CE-2EnNGTKSY_gd7i6nqsA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CE-2EnNGTKSY_gd7i6nqsA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CE-2EnNGTKSY_gd7i6nqsA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1104 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CE-2EnNGTKSY_gd7i6nqsA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CGU4FyPTS9eHQD5QApPhPA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CGU4FyPTS9eHQD5QApPhPA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7722 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CGU4FyPTS9eHQD5QApPhPA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CGU4FyPTS9eHQD5QApPhPA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CGU4FyPTS9eHQD5QApPhPA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      842 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CGU4FyPTS9eHQD5QApPhPA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CSTlwpXDRDyEUfFA22wvcQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CSTlwpXDRDyEUfFA22wvcQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CSTlwpXDRDyEUfFA22wvcQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CSTlwpXDRDyEUfFA22wvcQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CSTlwpXDRDyEUfFA22wvcQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      960 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CSTlwpXDRDyEUfFA22wvcQ/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Cyn7JDoPRwuRs_eShI9x4w/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Cyn7JDoPRwuRs_eShI9x4w/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4589 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Cyn7JDoPRwuRs_eShI9x4w/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Cyn7JDoPRwuRs_eShI9x4w/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Cyn7JDoPRwuRs_eShI9x4w/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1068 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Cyn7JDoPRwuRs_eShI9x4w/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/D12fNQbWTgCF6SYMi7fdew/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/D12fNQbWTgCF6SYMi7fdew/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7502 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/D12fNQbWTgCF6SYMi7fdew/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/D12fNQbWTgCF6SYMi7fdew/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/D12fNQbWTgCF6SYMi7fdew/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1130 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/D12fNQbWTgCF6SYMi7fdew/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/DTDhDQy_Te-8TX2GWjDyRA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/DTDhDQy_Te-8TX2GWjDyRA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7708 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/DTDhDQy_Te-8TX2GWjDyRA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/DTDhDQy_Te-8TX2GWjDyRA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/DTDhDQy_Te-8TX2GWjDyRA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1079 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/DTDhDQy_Te-8TX2GWjDyRA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Db65HT83SdCGu8IcAEMSJw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Db65HT83SdCGu8IcAEMSJw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7711 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Db65HT83SdCGu8IcAEMSJw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Db65HT83SdCGu8IcAEMSJw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Db65HT83SdCGu8IcAEMSJw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1011 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Db65HT83SdCGu8IcAEMSJw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/DvotWT9VS4---6k12rWy2g/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.297250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/DvotWT9VS4---6k12rWy2g/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/DvotWT9VS4---6k12rWy2g/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/DvotWT9VS4---6k12rWy2g/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/DvotWT9VS4---6k12rWy2g/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      972 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/DvotWT9VS4---6k12rWy2g/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/F-2XbyLdRoOWYqs1Wkz1bw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/F-2XbyLdRoOWYqs1Wkz1bw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/F-2XbyLdRoOWYqs1Wkz1bw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/F-2XbyLdRoOWYqs1Wkz1bw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/F-2XbyLdRoOWYqs1Wkz1bw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      963 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/F-2XbyLdRoOWYqs1Wkz1bw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/FK4OkxYcQWqYpmxP1ay0_A/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/FK4OkxYcQWqYpmxP1ay0_A/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7703 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/FK4OkxYcQWqYpmxP1ay0_A/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.193249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/FK4OkxYcQWqYpmxP1ay0_A/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/FK4OkxYcQWqYpmxP1ay0_A/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1007 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/FK4OkxYcQWqYpmxP1ay0_A/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/FWlvKTVwRUqznJSgpz4mSA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/FWlvKTVwRUqznJSgpz4mSA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7697 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/FWlvKTVwRUqznJSgpz4mSA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/FWlvKTVwRUqznJSgpz4mSA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/FWlvKTVwRUqznJSgpz4mSA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1161 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/FWlvKTVwRUqznJSgpz4mSA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Fy4__LJrS7yOddt0JlST1g/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Fy4__LJrS7yOddt0JlST1g/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7517 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Fy4__LJrS7yOddt0JlST1g/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Fy4__LJrS7yOddt0JlST1g/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Fy4__LJrS7yOddt0JlST1g/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1105 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Fy4__LJrS7yOddt0JlST1g/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GSN2ZF03SvGfJWTNQOR66Q/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GSN2ZF03SvGfJWTNQOR66Q/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     6803 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GSN2ZF03SvGfJWTNQOR66Q/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GSN2ZF03SvGfJWTNQOR66Q/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GSN2ZF03SvGfJWTNQOR66Q/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1148 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GSN2ZF03SvGfJWTNQOR66Q/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Glj2IKdJQ1OoKLUOshkKuw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Glj2IKdJQ1OoKLUOshkKuw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7517 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Glj2IKdJQ1OoKLUOshkKuw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Glj2IKdJQ1OoKLUOshkKuw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Glj2IKdJQ1OoKLUOshkKuw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1116 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Glj2IKdJQ1OoKLUOshkKuw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GrUeski1SfiJNpkgzaWWww/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GrUeski1SfiJNpkgzaWWww/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4600 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GrUeski1SfiJNpkgzaWWww/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GrUeski1SfiJNpkgzaWWww/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GrUeski1SfiJNpkgzaWWww/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      924 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GrUeski1SfiJNpkgzaWWww/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GxgYQf58TRaWVJ-2vy4tLg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GxgYQf58TRaWVJ-2vy4tLg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7500 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GxgYQf58TRaWVJ-2vy4tLg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GxgYQf58TRaWVJ-2vy4tLg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GxgYQf58TRaWVJ-2vy4tLg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1110 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GxgYQf58TRaWVJ-2vy4tLg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/H_rT971WQQayQyE8l4ABqA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/H_rT971WQQayQyE8l4ABqA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4589 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/H_rT971WQQayQyE8l4ABqA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/H_rT971WQQayQyE8l4ABqA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/H_rT971WQQayQyE8l4ABqA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1013 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/H_rT971WQQayQyE8l4ABqA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/I1ojS418TMeExBMFJ3LcIA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/I1ojS418TMeExBMFJ3LcIA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/I1ojS418TMeExBMFJ3LcIA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/I1ojS418TMeExBMFJ3LcIA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/I1ojS418TMeExBMFJ3LcIA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      968 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/I1ojS418TMeExBMFJ3LcIA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/I2nBckWWSRahjagcQD3aCg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.301250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/I2nBckWWSRahjagcQD3aCg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4589 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/I2nBckWWSRahjagcQD3aCg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/I2nBckWWSRahjagcQD3aCg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/I2nBckWWSRahjagcQD3aCg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1068 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/I2nBckWWSRahjagcQD3aCg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/IMcMRzZvTVyh5X4GdIMKUg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/IMcMRzZvTVyh5X4GdIMKUg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/IMcMRzZvTVyh5X4GdIMKUg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/IMcMRzZvTVyh5X4GdIMKUg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/IMcMRzZvTVyh5X4GdIMKUg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      955 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/IMcMRzZvTVyh5X4GdIMKUg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/INMgwWKtT7Kp5SH7zAfQ7w/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/INMgwWKtT7Kp5SH7zAfQ7w/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7711 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/INMgwWKtT7Kp5SH7zAfQ7w/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.197249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/INMgwWKtT7Kp5SH7zAfQ7w/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/INMgwWKtT7Kp5SH7zAfQ7w/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      993 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/INMgwWKtT7Kp5SH7zAfQ7w/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Je_Ek1ecSgidmukgi1oGjA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Je_Ek1ecSgidmukgi1oGjA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7517 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Je_Ek1ecSgidmukgi1oGjA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Je_Ek1ecSgidmukgi1oGjA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Je_Ek1ecSgidmukgi1oGjA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1104 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Je_Ek1ecSgidmukgi1oGjA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/JwuxI9J2Q5qC4D9dzziQmg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/JwuxI9J2Q5qC4D9dzziQmg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7517 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/JwuxI9J2Q5qC4D9dzziQmg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/JwuxI9J2Q5qC4D9dzziQmg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/JwuxI9J2Q5qC4D9dzziQmg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1117 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/JwuxI9J2Q5qC4D9dzziQmg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KbaNeW1hTJqiQyiUjsPz-Q/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KbaNeW1hTJqiQyiUjsPz-Q/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KbaNeW1hTJqiQyiUjsPz-Q/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KbaNeW1hTJqiQyiUjsPz-Q/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KbaNeW1hTJqiQyiUjsPz-Q/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      967 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KbaNeW1hTJqiQyiUjsPz-Q/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KjRoo3mLSUqYc6iRB10r6A/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KjRoo3mLSUqYc6iRB10r6A/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    26068 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KjRoo3mLSUqYc6iRB10r6A/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KjRoo3mLSUqYc6iRB10r6A/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KjRoo3mLSUqYc6iRB10r6A/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      888 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KjRoo3mLSUqYc6iRB10r6A/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KqRwX5EUQcK1b39svcLjjw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KqRwX5EUQcK1b39svcLjjw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4589 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KqRwX5EUQcK1b39svcLjjw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KqRwX5EUQcK1b39svcLjjw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KqRwX5EUQcK1b39svcLjjw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1007 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KqRwX5EUQcK1b39svcLjjw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/L1emPAoBROSoDSetQl5qYw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/L1emPAoBROSoDSetQl5qYw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7711 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/L1emPAoBROSoDSetQl5qYw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/L1emPAoBROSoDSetQl5qYw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/L1emPAoBROSoDSetQl5qYw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      993 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/L1emPAoBROSoDSetQl5qYw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LBuW7cjQS8-aE75qH-udRQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LBuW7cjQS8-aE75qH-udRQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7690 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LBuW7cjQS8-aE75qH-udRQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LBuW7cjQS8-aE75qH-udRQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LBuW7cjQS8-aE75qH-udRQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      850 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LBuW7cjQS8-aE75qH-udRQ/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LYO9FlvJQGSiffYQhMcW5Q/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.305250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LYO9FlvJQGSiffYQhMcW5Q/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    25958 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LYO9FlvJQGSiffYQhMcW5Q/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LYO9FlvJQGSiffYQhMcW5Q/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.309250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LYO9FlvJQGSiffYQhMcW5Q/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      888 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LYO9FlvJQGSiffYQhMcW5Q/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Lelr43PoRWWgnumQRpIb8Q/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.309250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Lelr43PoRWWgnumQRpIb8Q/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     5086 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Lelr43PoRWWgnumQRpIb8Q/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Lelr43PoRWWgnumQRpIb8Q/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.309250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Lelr43PoRWWgnumQRpIb8Q/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      849 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Lelr43PoRWWgnumQRpIb8Q/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LjluSbFjS5qg3jljQ38itQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.309250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LjluSbFjS5qg3jljQ38itQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LjluSbFjS5qg3jljQ38itQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LjluSbFjS5qg3jljQ38itQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.309250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LjluSbFjS5qg3jljQ38itQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1107 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LjluSbFjS5qg3jljQ38itQ/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.201249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LzlIi12cQsWwfxig59k2VQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.309250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LzlIi12cQsWwfxig59k2VQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LzlIi12cQsWwfxig59k2VQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LzlIi12cQsWwfxig59k2VQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.309250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LzlIi12cQsWwfxig59k2VQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      972 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LzlIi12cQsWwfxig59k2VQ/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MIuWH-PkRdOQvhsM9elc5Q/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.309250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MIuWH-PkRdOQvhsM9elc5Q/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    28473 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MIuWH-PkRdOQvhsM9elc5Q/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MIuWH-PkRdOQvhsM9elc5Q/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MIuWH-PkRdOQvhsM9elc5Q/artifacts/public/build/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.309250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MIuWH-PkRdOQvhsM9elc5Q/artifacts/public/build/en-US/
+-rw-r--r--   0 worker    (1000) worker    (1000)      767 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MIuWH-PkRdOQvhsM9elc5Q/artifacts/public/build/en-US/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MJfJtItbRjmydzrvwwURrg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.309250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MJfJtItbRjmydzrvwwURrg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    28495 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MJfJtItbRjmydzrvwwURrg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MJfJtItbRjmydzrvwwURrg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MJfJtItbRjmydzrvwwURrg/artifacts/public/build/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.309250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MJfJtItbRjmydzrvwwURrg/artifacts/public/build/en-US/
+-rw-r--r--   0 worker    (1000) worker    (1000)      758 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MJfJtItbRjmydzrvwwURrg/artifacts/public/build/en-US/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MJm-0bUOR7WEyESS_3EuMg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.309250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MJm-0bUOR7WEyESS_3EuMg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7661 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MJm-0bUOR7WEyESS_3EuMg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MJm-0bUOR7WEyESS_3EuMg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.309250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MJm-0bUOR7WEyESS_3EuMg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1234 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MJm-0bUOR7WEyESS_3EuMg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MVFFVBcITlmoKD8m1Uqwkw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.309250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MVFFVBcITlmoKD8m1Uqwkw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MVFFVBcITlmoKD8m1Uqwkw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MVFFVBcITlmoKD8m1Uqwkw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.309250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MVFFVBcITlmoKD8m1Uqwkw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      975 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MVFFVBcITlmoKD8m1Uqwkw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Ma7H24MaS5GP8jZpl6R5Xw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.309250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Ma7H24MaS5GP8jZpl6R5Xw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Ma7H24MaS5GP8jZpl6R5Xw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Ma7H24MaS5GP8jZpl6R5Xw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.309250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Ma7H24MaS5GP8jZpl6R5Xw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      960 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Ma7H24MaS5GP8jZpl6R5Xw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/N491PvLhQcCSBX0gFmTKkg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.309250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/N491PvLhQcCSBX0gFmTKkg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7517 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/N491PvLhQcCSBX0gFmTKkg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/N491PvLhQcCSBX0gFmTKkg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.309250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/N491PvLhQcCSBX0gFmTKkg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1105 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/N491PvLhQcCSBX0gFmTKkg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/N7ENCbCgSvGvuiV3wM91Tg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/N7ENCbCgSvGvuiV3wM91Tg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/N7ENCbCgSvGvuiV3wM91Tg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/N7ENCbCgSvGvuiV3wM91Tg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/N7ENCbCgSvGvuiV3wM91Tg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1107 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/N7ENCbCgSvGvuiV3wM91Tg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/O2UuedRNRvSbkRXzgtfTZg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/O2UuedRNRvSbkRXzgtfTZg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7727 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/O2UuedRNRvSbkRXzgtfTZg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/O2UuedRNRvSbkRXzgtfTZg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/O2UuedRNRvSbkRXzgtfTZg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      983 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/O2UuedRNRvSbkRXzgtfTZg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/O5RMm0izRSSMLncwLUUZzA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/O5RMm0izRSSMLncwLUUZzA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7692 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/O5RMm0izRSSMLncwLUUZzA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/O5RMm0izRSSMLncwLUUZzA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/O5RMm0izRSSMLncwLUUZzA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1128 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/O5RMm0izRSSMLncwLUUZzA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Oxnm2nS5SQeujyAmxci87w/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Oxnm2nS5SQeujyAmxci87w/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Oxnm2nS5SQeujyAmxci87w/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Oxnm2nS5SQeujyAmxci87w/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Oxnm2nS5SQeujyAmxci87w/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1099 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Oxnm2nS5SQeujyAmxci87w/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.205249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PTEeGj5sQP-VOR_rereX_Q/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PTEeGj5sQP-VOR_rereX_Q/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    28583 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PTEeGj5sQP-VOR_rereX_Q/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PTEeGj5sQP-VOR_rereX_Q/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PTEeGj5sQP-VOR_rereX_Q/artifacts/public/build/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PTEeGj5sQP-VOR_rereX_Q/artifacts/public/build/en-US/
+-rw-r--r--   0 worker    (1000) worker    (1000)      764 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PTEeGj5sQP-VOR_rereX_Q/artifacts/public/build/en-US/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PU23u6VeRDWDKVUnX09Cvw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PU23u6VeRDWDKVUnX09Cvw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PU23u6VeRDWDKVUnX09Cvw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PU23u6VeRDWDKVUnX09Cvw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PU23u6VeRDWDKVUnX09Cvw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      972 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PU23u6VeRDWDKVUnX09Cvw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PUrV4bCUQ3GKWvMCV3_Bzw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PUrV4bCUQ3GKWvMCV3_Bzw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7722 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PUrV4bCUQ3GKWvMCV3_Bzw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PUrV4bCUQ3GKWvMCV3_Bzw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PUrV4bCUQ3GKWvMCV3_Bzw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      855 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PUrV4bCUQ3GKWvMCV3_Bzw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/QaS45XFwRASfCE9F9TaqCg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/QaS45XFwRASfCE9F9TaqCg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7727 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/QaS45XFwRASfCE9F9TaqCg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/QaS45XFwRASfCE9F9TaqCg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/QaS45XFwRASfCE9F9TaqCg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      927 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/QaS45XFwRASfCE9F9TaqCg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    28825 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/artifacts/public/build/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/artifacts/public/build/en-US/
+-rw-r--r--   0 worker    (1000) worker    (1000)      777 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/artifacts/public/build/en-US/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Qsu15jVeRGeYGaPva8g7Xw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Qsu15jVeRGeYGaPva8g7Xw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Qsu15jVeRGeYGaPva8g7Xw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Qsu15jVeRGeYGaPva8g7Xw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Qsu15jVeRGeYGaPva8g7Xw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1041 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Qsu15jVeRGeYGaPva8g7Xw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/R6b2C_MbQwWKJPjvs_PZaA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.313250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/R6b2C_MbQwWKJPjvs_PZaA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/R6b2C_MbQwWKJPjvs_PZaA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/R6b2C_MbQwWKJPjvs_PZaA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/R6b2C_MbQwWKJPjvs_PZaA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      960 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/R6b2C_MbQwWKJPjvs_PZaA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/R8E6ScjVREuVI0hLQorxwA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/R8E6ScjVREuVI0hLQorxwA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    26068 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/R8E6ScjVREuVI0hLQorxwA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/R8E6ScjVREuVI0hLQorxwA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/R8E6ScjVREuVI0hLQorxwA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      888 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/R8E6ScjVREuVI0hLQorxwA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    28143 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/artifacts/public/build/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/artifacts/public/build/en-US/
+-rw-r--r--   0 worker    (1000) worker    (1000)      748 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/artifacts/public/build/en-US/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Rd61yPVqQ0CdZmbvuQ9YcQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Rd61yPVqQ0CdZmbvuQ9YcQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4589 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Rd61yPVqQ0CdZmbvuQ9YcQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Rd61yPVqQ0CdZmbvuQ9YcQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Rd61yPVqQ0CdZmbvuQ9YcQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1001 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Rd61yPVqQ0CdZmbvuQ9YcQ/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.209249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/S1o0P_q8RM601Mq0d4urkw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/S1o0P_q8RM601Mq0d4urkw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     6983 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/S1o0P_q8RM601Mq0d4urkw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/S1o0P_q8RM601Mq0d4urkw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/S1o0P_q8RM601Mq0d4urkw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      994 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/S1o0P_q8RM601Mq0d4urkw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/SdJspoE-QROYKIlrSM5E9w/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/SdJspoE-QROYKIlrSM5E9w/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7697 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/SdJspoE-QROYKIlrSM5E9w/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/SdJspoE-QROYKIlrSM5E9w/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/SdJspoE-QROYKIlrSM5E9w/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1165 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/SdJspoE-QROYKIlrSM5E9w/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/SkWkmrKDSF2hQhnMOfS1PQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/SkWkmrKDSF2hQhnMOfS1PQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/SkWkmrKDSF2hQhnMOfS1PQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/SkWkmrKDSF2hQhnMOfS1PQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/SkWkmrKDSF2hQhnMOfS1PQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      972 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/SkWkmrKDSF2hQhnMOfS1PQ/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/T1ARQQKHTKu_m1EtjZv7YQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/T1ARQQKHTKu_m1EtjZv7YQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     8106 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/T1ARQQKHTKu_m1EtjZv7YQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/T1ARQQKHTKu_m1EtjZv7YQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/T1ARQQKHTKu_m1EtjZv7YQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      925 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/T1ARQQKHTKu_m1EtjZv7YQ/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TJD91R5LTxSyqoutUKFjtg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TJD91R5LTxSyqoutUKFjtg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    28473 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TJD91R5LTxSyqoutUKFjtg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TJD91R5LTxSyqoutUKFjtg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TJD91R5LTxSyqoutUKFjtg/artifacts/public/build/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TJD91R5LTxSyqoutUKFjtg/artifacts/public/build/en-US/
+-rw-r--r--   0 worker    (1000) worker    (1000)      768 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TJD91R5LTxSyqoutUKFjtg/artifacts/public/build/en-US/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TTYSB2nKSUWvv5rbQDLtzw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TTYSB2nKSUWvv5rbQDLtzw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TTYSB2nKSUWvv5rbQDLtzw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TTYSB2nKSUWvv5rbQDLtzw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TTYSB2nKSUWvv5rbQDLtzw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      963 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TTYSB2nKSUWvv5rbQDLtzw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TXelMo4QSxqUzn0l-PWWyg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TXelMo4QSxqUzn0l-PWWyg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7722 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TXelMo4QSxqUzn0l-PWWyg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TXelMo4QSxqUzn0l-PWWyg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TXelMo4QSxqUzn0l-PWWyg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      836 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TXelMo4QSxqUzn0l-PWWyg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ThUoABnMR12AkygRTIAcKA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.317250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ThUoABnMR12AkygRTIAcKA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7708 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ThUoABnMR12AkygRTIAcKA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ThUoABnMR12AkygRTIAcKA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ThUoABnMR12AkygRTIAcKA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1083 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ThUoABnMR12AkygRTIAcKA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TheuGGRAQEeVfrK_nIxlYA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TheuGGRAQEeVfrK_nIxlYA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     8240 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TheuGGRAQEeVfrK_nIxlYA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TheuGGRAQEeVfrK_nIxlYA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TheuGGRAQEeVfrK_nIxlYA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      841 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TheuGGRAQEeVfrK_nIxlYA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UUrwCxWRQ5OeCJEhZOQBHg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UUrwCxWRQ5OeCJEhZOQBHg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7711 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UUrwCxWRQ5OeCJEhZOQBHg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UUrwCxWRQ5OeCJEhZOQBHg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UUrwCxWRQ5OeCJEhZOQBHg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      999 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UUrwCxWRQ5OeCJEhZOQBHg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.213249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UoKNy4deRsKipcwj_CSJcA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UoKNy4deRsKipcwj_CSJcA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7521 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UoKNy4deRsKipcwj_CSJcA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UoKNy4deRsKipcwj_CSJcA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UoKNy4deRsKipcwj_CSJcA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1010 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UoKNy4deRsKipcwj_CSJcA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Ut4dGXE3RpCRQy6Pd2PpVg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Ut4dGXE3RpCRQy6Pd2PpVg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4589 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Ut4dGXE3RpCRQy6Pd2PpVg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Ut4dGXE3RpCRQy6Pd2PpVg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Ut4dGXE3RpCRQy6Pd2PpVg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1080 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Ut4dGXE3RpCRQy6Pd2PpVg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UuWQ2KScQ3KrYF4wFkczHw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UuWQ2KScQ3KrYF4wFkczHw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    28803 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UuWQ2KScQ3KrYF4wFkczHw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UuWQ2KScQ3KrYF4wFkczHw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UuWQ2KScQ3KrYF4wFkczHw/artifacts/public/build/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UuWQ2KScQ3KrYF4wFkczHw/artifacts/public/build/en-US/
+-rw-r--r--   0 worker    (1000) worker    (1000)      787 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UuWQ2KScQ3KrYF4wFkczHw/artifacts/public/build/en-US/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/VSEShvqcSxWWtdKaO6jagQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/VSEShvqcSxWWtdKaO6jagQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/VSEShvqcSxWWtdKaO6jagQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/VSEShvqcSxWWtdKaO6jagQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/VSEShvqcSxWWtdKaO6jagQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1108 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/VSEShvqcSxWWtdKaO6jagQ/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/V_S-Ts-2TmmGgDExnyG6qw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/V_S-Ts-2TmmGgDExnyG6qw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4589 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/V_S-Ts-2TmmGgDExnyG6qw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/V_S-Ts-2TmmGgDExnyG6qw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/V_S-Ts-2TmmGgDExnyG6qw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1007 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/V_S-Ts-2TmmGgDExnyG6qw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Vdir5WkdS-G7MKg1VPiWEg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Vdir5WkdS-G7MKg1VPiWEg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7711 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Vdir5WkdS-G7MKg1VPiWEg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Vdir5WkdS-G7MKg1VPiWEg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Vdir5WkdS-G7MKg1VPiWEg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      999 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Vdir5WkdS-G7MKg1VPiWEg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/VyFzvPDRSaaNnxo8A1krWg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/VyFzvPDRSaaNnxo8A1krWg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/VyFzvPDRSaaNnxo8A1krWg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/VyFzvPDRSaaNnxo8A1krWg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/VyFzvPDRSaaNnxo8A1krWg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      960 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/VyFzvPDRSaaNnxo8A1krWg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/WRq2BZCZRlCITcXJwi9VOA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/WRq2BZCZRlCITcXJwi9VOA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7880 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/WRq2BZCZRlCITcXJwi9VOA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/WRq2BZCZRlCITcXJwi9VOA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/WRq2BZCZRlCITcXJwi9VOA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1277 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/WRq2BZCZRlCITcXJwi9VOA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/XDp1D7tkQBK4u1XG4reYSA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.321250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/XDp1D7tkQBK4u1XG4reYSA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/XDp1D7tkQBK4u1XG4reYSA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/XDp1D7tkQBK4u1XG4reYSA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.325250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/XDp1D7tkQBK4u1XG4reYSA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      955 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/XDp1D7tkQBK4u1XG4reYSA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/XPfHK-vXS9uGpyq4-l6xtg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.325250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/XPfHK-vXS9uGpyq4-l6xtg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7697 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/XPfHK-vXS9uGpyq4-l6xtg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.217249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/XPfHK-vXS9uGpyq4-l6xtg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.325250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/XPfHK-vXS9uGpyq4-l6xtg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1165 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/XPfHK-vXS9uGpyq4-l6xtg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/X_XmczzYTA2l8JwACz-YBg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.325250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/X_XmczzYTA2l8JwACz-YBg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/X_XmczzYTA2l8JwACz-YBg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/X_XmczzYTA2l8JwACz-YBg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.325250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/X_XmczzYTA2l8JwACz-YBg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      967 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/X_XmczzYTA2l8JwACz-YBg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Y45GeFF7SPuy1IhX9CXMPw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.325250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Y45GeFF7SPuy1IhX9CXMPw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Y45GeFF7SPuy1IhX9CXMPw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Y45GeFF7SPuy1IhX9CXMPw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.325250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Y45GeFF7SPuy1IhX9CXMPw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      965 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Y45GeFF7SPuy1IhX9CXMPw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YE5qNXJbTuu2T2uXJhk5Nw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.325250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YE5qNXJbTuu2T2uXJhk5Nw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7723 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YE5qNXJbTuu2T2uXJhk5Nw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YE5qNXJbTuu2T2uXJhk5Nw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.325250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YE5qNXJbTuu2T2uXJhk5Nw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      995 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YE5qNXJbTuu2T2uXJhk5Nw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YGDcP8gRQPebxPg7efA7Iw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.325250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YGDcP8gRQPebxPg7efA7Iw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7690 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YGDcP8gRQPebxPg7efA7Iw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YGDcP8gRQPebxPg7efA7Iw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.325250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YGDcP8gRQPebxPg7efA7Iw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1274 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YGDcP8gRQPebxPg7efA7Iw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YWFg1gR3Rfu3LH7U6mB8EQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.325250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YWFg1gR3Rfu3LH7U6mB8EQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7500 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YWFg1gR3Rfu3LH7U6mB8EQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YWFg1gR3Rfu3LH7U6mB8EQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.325250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YWFg1gR3Rfu3LH7U6mB8EQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1110 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YWFg1gR3Rfu3LH7U6mB8EQ/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YWIA7hhsSCqyXKErOzGqIg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.325250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YWIA7hhsSCqyXKErOzGqIg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7703 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YWIA7hhsSCqyXKErOzGqIg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YWIA7hhsSCqyXKErOzGqIg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.325250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YWIA7hhsSCqyXKErOzGqIg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1004 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YWIA7hhsSCqyXKErOzGqIg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YYrpCCBgSSmTIrul3-dXGg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.325250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YYrpCCBgSSmTIrul3-dXGg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YYrpCCBgSSmTIrul3-dXGg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YYrpCCBgSSmTIrul3-dXGg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.325250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YYrpCCBgSSmTIrul3-dXGg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1111 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YYrpCCBgSSmTIrul3-dXGg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Yy5BKCQLSNKJmVlXUgZ-Vw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.325250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Yy5BKCQLSNKJmVlXUgZ-Vw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Yy5BKCQLSNKJmVlXUgZ-Vw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Yy5BKCQLSNKJmVlXUgZ-Vw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.329250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Yy5BKCQLSNKJmVlXUgZ-Vw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      956 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Yy5BKCQLSNKJmVlXUgZ-Vw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Z2wFgrvYQfWr4sZ_5xsJyg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.329250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Z2wFgrvYQfWr4sZ_5xsJyg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7500 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Z2wFgrvYQfWr4sZ_5xsJyg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Z2wFgrvYQfWr4sZ_5xsJyg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.329250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Z2wFgrvYQfWr4sZ_5xsJyg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1110 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Z2wFgrvYQfWr4sZ_5xsJyg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Z4Nk4adQT_KY6OB36jH7GA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.329250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Z4Nk4adQT_KY6OB36jH7GA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7711 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Z4Nk4adQT_KY6OB36jH7GA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.221249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Z4Nk4adQT_KY6OB36jH7GA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.329250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Z4Nk4adQT_KY6OB36jH7GA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      993 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Z4Nk4adQT_KY6OB36jH7GA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZHf8FbtqSZa-D8WeBBRQ9A/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.329250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZHf8FbtqSZa-D8WeBBRQ9A/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    26068 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZHf8FbtqSZa-D8WeBBRQ9A/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZHf8FbtqSZa-D8WeBBRQ9A/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.329250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZHf8FbtqSZa-D8WeBBRQ9A/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      900 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZHf8FbtqSZa-D8WeBBRQ9A/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZKZozRyQT42x6mxaQ9LhnA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.329250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZKZozRyQT42x6mxaQ9LhnA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZKZozRyQT42x6mxaQ9LhnA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZKZozRyQT42x6mxaQ9LhnA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.329250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZKZozRyQT42x6mxaQ9LhnA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      967 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZKZozRyQT42x6mxaQ9LhnA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZcTIYEkjQO2aChxeIY6fbw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.329250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZcTIYEkjQO2aChxeIY6fbw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     6976 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZcTIYEkjQO2aChxeIY6fbw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZcTIYEkjQO2aChxeIY6fbw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.329250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZcTIYEkjQO2aChxeIY6fbw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1041 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZcTIYEkjQO2aChxeIY6fbw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZukWWPukRoqeGyztJsYEXQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.329250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZukWWPukRoqeGyztJsYEXQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZukWWPukRoqeGyztJsYEXQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZukWWPukRoqeGyztJsYEXQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.329250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZukWWPukRoqeGyztJsYEXQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      960 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZukWWPukRoqeGyztJsYEXQ/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aAfWVw75TbKJ9Ff4vdSdXA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.329250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aAfWVw75TbKJ9Ff4vdSdXA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aAfWVw75TbKJ9Ff4vdSdXA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aAfWVw75TbKJ9Ff4vdSdXA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.329250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aAfWVw75TbKJ9Ff4vdSdXA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      955 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aAfWVw75TbKJ9Ff4vdSdXA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aNOLmiYFSnm51F5o0EF10A/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.329250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aNOLmiYFSnm51F5o0EF10A/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aNOLmiYFSnm51F5o0EF10A/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aNOLmiYFSnm51F5o0EF10A/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.329250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aNOLmiYFSnm51F5o0EF10A/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      960 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aNOLmiYFSnm51F5o0EF10A/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aNUeGazgSEqDVyec14YaHw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.329250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aNUeGazgSEqDVyec14YaHw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7502 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aNUeGazgSEqDVyec14YaHw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aNUeGazgSEqDVyec14YaHw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aNUeGazgSEqDVyec14YaHw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1130 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aNUeGazgSEqDVyec14YaHw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ac88QqpjTJuP6ZX2Is6yEQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ac88QqpjTJuP6ZX2Is6yEQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7711 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ac88QqpjTJuP6ZX2Is6yEQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ac88QqpjTJuP6ZX2Is6yEQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ac88QqpjTJuP6ZX2Is6yEQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1005 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ac88QqpjTJuP6ZX2Is6yEQ/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/auiN3S92TkiF21ayWnyfkw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/auiN3S92TkiF21ayWnyfkw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/auiN3S92TkiF21ayWnyfkw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/auiN3S92TkiF21ayWnyfkw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/auiN3S92TkiF21ayWnyfkw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      960 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/auiN3S92TkiF21ayWnyfkw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bkCYr42WR-aMl0t-rO918w/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bkCYr42WR-aMl0t-rO918w/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7711 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bkCYr42WR-aMl0t-rO918w/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bkCYr42WR-aMl0t-rO918w/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bkCYr42WR-aMl0t-rO918w/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      999 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bkCYr42WR-aMl0t-rO918w/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.225249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bqTeNQLPSHqviqZ-adbEgw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bqTeNQLPSHqviqZ-adbEgw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bqTeNQLPSHqviqZ-adbEgw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bqTeNQLPSHqviqZ-adbEgw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bqTeNQLPSHqviqZ-adbEgw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1099 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bqTeNQLPSHqviqZ-adbEgw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bsfhDaUBSZ-4IPUk_eXaSA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bsfhDaUBSZ-4IPUk_eXaSA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4209 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bsfhDaUBSZ-4IPUk_eXaSA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bsfhDaUBSZ-4IPUk_eXaSA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bsfhDaUBSZ-4IPUk_eXaSA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      850 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bsfhDaUBSZ-4IPUk_eXaSA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bwP8UBmpRRKBOstsMyYOtg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bwP8UBmpRRKBOstsMyYOtg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bwP8UBmpRRKBOstsMyYOtg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bwP8UBmpRRKBOstsMyYOtg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bwP8UBmpRRKBOstsMyYOtg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1119 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bwP8UBmpRRKBOstsMyYOtg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cEquZnIzQZKo-sHRNoWdxA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cEquZnIzQZKo-sHRNoWdxA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7727 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cEquZnIzQZKo-sHRNoWdxA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cEquZnIzQZKo-sHRNoWdxA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cEquZnIzQZKo-sHRNoWdxA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1002 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cEquZnIzQZKo-sHRNoWdxA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cf-lJNFgSsmK89NsnoUNqg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cf-lJNFgSsmK89NsnoUNqg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cf-lJNFgSsmK89NsnoUNqg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cf-lJNFgSsmK89NsnoUNqg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cf-lJNFgSsmK89NsnoUNqg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1041 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cf-lJNFgSsmK89NsnoUNqg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cfhgadFrQqGdfkUQrE8DNA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cfhgadFrQqGdfkUQrE8DNA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7706 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cfhgadFrQqGdfkUQrE8DNA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cfhgadFrQqGdfkUQrE8DNA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cfhgadFrQqGdfkUQrE8DNA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      967 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cfhgadFrQqGdfkUQrE8DNA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cxsX3JgCRt-tEsH-ouLt3Q/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.333250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cxsX3JgCRt-tEsH-ouLt3Q/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4041 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cxsX3JgCRt-tEsH-ouLt3Q/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cxsX3JgCRt-tEsH-ouLt3Q/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cxsX3JgCRt-tEsH-ouLt3Q/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1089 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cxsX3JgCRt-tEsH-ouLt3Q/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dNgIzJgjTlyYH24pQzLBug/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dNgIzJgjTlyYH24pQzLBug/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7500 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dNgIzJgjTlyYH24pQzLBug/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dNgIzJgjTlyYH24pQzLBug/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dNgIzJgjTlyYH24pQzLBug/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1110 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dNgIzJgjTlyYH24pQzLBug/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dZl_9NHxRkSM2YzG1Y29YA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dZl_9NHxRkSM2YzG1Y29YA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dZl_9NHxRkSM2YzG1Y29YA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dZl_9NHxRkSM2YzG1Y29YA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dZl_9NHxRkSM2YzG1Y29YA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1111 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dZl_9NHxRkSM2YzG1Y29YA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dcY-KGqYTdy67l7zA9K57Q/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dcY-KGqYTdy67l7zA9K57Q/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7707 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dcY-KGqYTdy67l7zA9K57Q/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dcY-KGqYTdy67l7zA9K57Q/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dcY-KGqYTdy67l7zA9K57Q/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1108 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dcY-KGqYTdy67l7zA9K57Q/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/e-15mv-6TR2SJu3iX1dz6w/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/e-15mv-6TR2SJu3iX1dz6w/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     8106 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/e-15mv-6TR2SJu3iX1dz6w/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/e-15mv-6TR2SJu3iX1dz6w/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/e-15mv-6TR2SJu3iX1dz6w/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      933 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/e-15mv-6TR2SJu3iX1dz6w/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.229249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/e8lqN78UTRWWOtoT1U9YKw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/e8lqN78UTRWWOtoT1U9YKw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7727 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/e8lqN78UTRWWOtoT1U9YKw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/e8lqN78UTRWWOtoT1U9YKw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/e8lqN78UTRWWOtoT1U9YKw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      919 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/e8lqN78UTRWWOtoT1U9YKw/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eEzNLZ8CRPG_rqJt94V2Jg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eEzNLZ8CRPG_rqJt94V2Jg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4589 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eEzNLZ8CRPG_rqJt94V2Jg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eEzNLZ8CRPG_rqJt94V2Jg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eEzNLZ8CRPG_rqJt94V2Jg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1001 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eEzNLZ8CRPG_rqJt94V2Jg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eNr5UDpwSv-owhKwo5RR5w/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eNr5UDpwSv-owhKwo5RR5w/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eNr5UDpwSv-owhKwo5RR5w/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eNr5UDpwSv-owhKwo5RR5w/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eNr5UDpwSv-owhKwo5RR5w/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      972 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eNr5UDpwSv-owhKwo5RR5w/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eRpROunvQa-sZ5n-zmHFCA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eRpROunvQa-sZ5n-zmHFCA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    28913 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eRpROunvQa-sZ5n-zmHFCA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eRpROunvQa-sZ5n-zmHFCA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eRpROunvQa-sZ5n-zmHFCA/artifacts/public/build/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eRpROunvQa-sZ5n-zmHFCA/artifacts/public/build/en-US/
+-rw-r--r--   0 worker    (1000) worker    (1000)      783 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eRpROunvQa-sZ5n-zmHFCA/artifacts/public/build/en-US/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eUk3ZT1tQHmJBu06q-E-AQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eUk3ZT1tQHmJBu06q-E-AQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7880 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eUk3ZT1tQHmJBu06q-E-AQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eUk3ZT1tQHmJBu06q-E-AQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eUk3ZT1tQHmJBu06q-E-AQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1269 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eUk3ZT1tQHmJBu06q-E-AQ/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ebZgCLndSm2ew4fN6uM48Q/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ebZgCLndSm2ew4fN6uM48Q/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4589 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ebZgCLndSm2ew4fN6uM48Q/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ebZgCLndSm2ew4fN6uM48Q/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ebZgCLndSm2ew4fN6uM48Q/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1019 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ebZgCLndSm2ew4fN6uM48Q/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/erjBtcr7TeaKF9WkHH3fAA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.337250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/erjBtcr7TeaKF9WkHH3fAA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7711 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/erjBtcr7TeaKF9WkHH3fAA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/erjBtcr7TeaKF9WkHH3fAA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.341250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/erjBtcr7TeaKF9WkHH3fAA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1005 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/erjBtcr7TeaKF9WkHH3fAA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/esk9JKa7QxyKNF-pmg5UVA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.341250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/esk9JKa7QxyKNF-pmg5UVA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7723 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/esk9JKa7QxyKNF-pmg5UVA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/esk9JKa7QxyKNF-pmg5UVA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.341250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/esk9JKa7QxyKNF-pmg5UVA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      976 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/esk9JKa7QxyKNF-pmg5UVA/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fMxvFK8yQQqnSYNv2r8Fyg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.341250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fMxvFK8yQQqnSYNv2r8Fyg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7722 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fMxvFK8yQQqnSYNv2r8Fyg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fMxvFK8yQQqnSYNv2r8Fyg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.341250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fMxvFK8yQQqnSYNv2r8Fyg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      850 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fMxvFK8yQQqnSYNv2r8Fyg/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fcYf8jKOQ9yV6VtZtbFNJQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.341250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fcYf8jKOQ9yV6VtZtbFNJQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4236 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fcYf8jKOQ9yV6VtZtbFNJQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.233249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fcYf8jKOQ9yV6VtZtbFNJQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.341250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fcYf8jKOQ9yV6VtZtbFNJQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      850 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fcYf8jKOQ9yV6VtZtbFNJQ/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.237249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ff3I1qWyRvSKVMYbEZh39g/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.341250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ff3I1qWyRvSKVMYbEZh39g/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ff3I1qWyRvSKVMYbEZh39g/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.237249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ff3I1qWyRvSKVMYbEZh39g/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.341250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ff3I1qWyRvSKVMYbEZh39g/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      960 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ff3I1qWyRvSKVMYbEZh39g/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.237249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fn7T0nqKSK-wX_RsitMQwQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.341250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fn7T0nqKSK-wX_RsitMQwQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1244 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fn7T0nqKSK-wX_RsitMQwQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.237249 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fn7T0nqKSK-wX_RsitMQwQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.341250 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fn7T0nqKSK-wX_RsitMQwQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      100 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fn7T0nqKSK-wX_RsitMQwQ/artifacts/public/build/target.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.237249 fuzzfetch-7.0.0/tests/mock-hg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.237249 fuzzfetch-7.0.0/tests/mock-hg/mozilla-central/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.341250 fuzzfetch-7.0.0/tests/mock-hg/mozilla-central/json-rev/
+-rw-r--r--   0 worker    (1000) worker    (1000)   273670 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-hg/mozilla-central/json-rev/10aa74237898
+-rw-r--r--   0 worker    (1000) worker    (1000)    10073 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-hg/mozilla-central/json-rev/5096e8be57730ef6902aaa8954b79aa0a21b32d6
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.237249 fuzzfetch-7.0.0/tests/mock-product-details/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-04-30 19:48:25.341250 fuzzfetch-7.0.0/tests/mock-product-details/1.0/
+-rw-r--r--   0 worker    (1000) worker    (1000)      673 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/mock-product-details/1.0/firefox_versions.json
+-rw-r--r--   0 worker    (1000) worker    (1000)     2621 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/test_core.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     2266 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/test_extract.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    10300 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tests/test_fetch.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     1301 2024-04-30 19:48:16.000000 fuzzfetch-7.0.0/tox.ini
```

### Comparing `fuzzfetch-6.0.0/.pre-commit-config.yaml` & `fuzzfetch-7.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/.taskcluster.yml` & `fuzzfetch-7.0.0/.taskcluster.yml`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/CODE_OF_CONDUCT.md` & `fuzzfetch-7.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/LICENSE.md` & `fuzzfetch-7.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/PKG-INFO` & `fuzzfetch-7.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzfetch
-Version: 6.0.0
+Version: 7.0.0
 Summary: Downloader for firefox/jsshell builds.
 Home-page: https://github.com/MozillaSecurity/fuzzfetch
 Maintainer: Mozilla Fuzzing Team
 Maintainer-email: fuzzing@mozilla.com
 License: MPL 2.0
 Keywords: fuzz fuzzing security test testing
 Platform: any
```

### Comparing `fuzzfetch-6.0.0/README.md` & `fuzzfetch-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/pyproject.toml` & `fuzzfetch-7.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/setup.cfg` & `fuzzfetch-7.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/src/fuzzfetch/__init__.py` & `fuzzfetch-7.0.0/src/fuzzfetch/__init__.py`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/src/fuzzfetch/args.py` & `fuzzfetch-7.0.0/src/fuzzfetch/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,17 @@
         build_group.add_argument(
             "-a",
             "--asan",
             action="store_true",
             help="Download AddressSanitizer builds.",
         )
         build_group.add_argument(
+            "--afl", action="store_true", help="Download AFL++ builds."
+        )
+        build_group.add_argument(
             "-t", "--tsan", action="store_true", help="Download ThreadSanitizer builds."
         )
         build_group.add_argument(
             "--fuzzing", action="store_true", help="Download --enable-fuzzing builds."
         )
         build_group.add_argument(
             "--fuzzilli",
```

### Comparing `fuzzfetch-6.0.0/src/fuzzfetch/core.py` & `fuzzfetch-7.0.0/src/fuzzfetch/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         """
         Arguments:
             branch: a valid gecko branch, eg. 'central', 'autoland', 'beta',
                     'release', 'esr52', etc.
             build: build identifier. acceptable identifiers are: TaskCluster
                    namespace, hg changeset, date, 'latest'
             flags: ('asan', 'debug', 'fuzzing', 'coverage', 'valgrind', 'tsan',
-                    'no_opt', 'fuzzilli', 'nyx'),
+                    'no_opt', 'fuzzilli', 'nyx', 'searchfox', 'afl'),
                    each a bool, not all combinations exist in TaskCluster
             platform: force platform if different than current system
             nearest: Search for nearest build, not exact
         """
         self._memo: Dict[str, Any] = {}
         "memorized values for @properties"
         self._branch = branch
@@ -111,19 +111,22 @@
                     coverage,
                     valgrind,
                     tsan,
                     no_opt,
                     fuzzilli,
                     nyx,
                     searchfox,
+                    afl,
                 ) = self._flags
                 if not debug:
                     debug = "-debug" in build or "-dbg" in build
                 if not asan:
                     asan = "-asan" in build
+                if not afl:
+                    afl = "-afl" in build
                 if not tsan:
                     tsan = "-tsan" in build
                 if not fuzzing:
                     fuzzing = "-fuzzing" in build
                 if not coverage:
                     coverage = "-ccov" in build
                 if not valgrind:
@@ -132,26 +135,29 @@
                     no_opt = "-noopt" in build
                 if not fuzzilli:
                     fuzzilli = "-fuzzilli" in build
                 if not nyx:
                     nyx = "-nyx" in build
                 if not searchfox:
                     searchfox = "-searchfox" in build
+                if not afl:
+                    afl = "-afl" in build
 
                 self._flags = BuildFlags(
                     asan,
                     tsan,
                     debug,
                     fuzzing,
                     coverage,
                     valgrind,
                     no_opt,
                     fuzzilli,
                     nyx,
                     searchfox,
+                    afl,
                 )
 
                 # Validate flags
                 if self._flags.asan and "-asan" not in build:
                     raise FetcherException(
                         "'build' is not an asan build, but asan=True given "
                         f"(build={build})"
@@ -197,14 +203,19 @@
                         f"(build={build})"
                     )
                 if self._flags.searchfox and "-searchfox" not in build:
                     raise FetcherException(
                         "'build' is not a searchfox build, but searchfox=True given "
                         f"(build={build})"
                     )
+                if self._flags.afl and "-afl" not in build:
+                    raise FetcherException(
+                        "'build' is not an AFL++ build, but afl=True given "
+                        f"(build={build})"
+                    )
 
             # Attempt to fetch the build.  If it fails and nearest is set, try and find
             # the nearest build that matches
             now = datetime.now(timezone("UTC"))
 
             try:
                 self._task = BuildTask(build, branch, self._flags, self._platform)
@@ -791,14 +802,15 @@
             args.fuzzing,
             args.coverage,
             args.valgrind,
             args.no_opt,
             args.fuzzilli,
             args.nyx,
             args.searchfox,
+            args.afl,
         )
         obj = cls(
             args.branch,
             args.build,
             flags,
             args.target,
             Platform(args.os, args.cpu),
```

### Comparing `fuzzfetch-6.0.0/src/fuzzfetch/download.py` & `fuzzfetch-7.0.0/src/fuzzfetch/download.py`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/src/fuzzfetch/extract.py` & `fuzzfetch-7.0.0/src/fuzzfetch/extract.py`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/src/fuzzfetch/models.py` & `fuzzfetch-7.0.0/src/fuzzfetch/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
             "fuzzing",
             "coverage",
             "valgrind",
             "no_opt",
             "fuzzilli",
             "nyx",
             "searchfox",
+            "afl",
         ),
     )
 ):
     """Class for storing TaskCluster build flags"""
 
     def build_string(self) -> str:
         """
@@ -49,14 +50,15 @@
         """
         return (
             ("-ccov" if self.coverage else "")
             + ("-fuzzilli" if self.fuzzilli else "")
             + ("-fuzzing" if self.fuzzing else "")
             + ("-asan" if self.asan else "")
             + ("-tsan" if self.tsan else "")
+            + ("-afl" if self.afl else "")
             + ("-nyx" if self.nyx else "")
             + ("-valgrind" if self.valgrind else "")
             + ("-noopt" if self.no_opt else "")
             + ("-searchfox" if self.searchfox else "")
             + ("-debug" if self.debug else "")
             + ("-opt" if not self.no_opt and not self.debug else "")
         )
```

### Comparing `fuzzfetch-6.0.0/src/fuzzfetch/path.py` & `fuzzfetch-7.0.0/src/fuzzfetch/path.py`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/src/fuzzfetch.egg-info/PKG-INFO` & `fuzzfetch-7.0.0/src/fuzzfetch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzfetch
-Version: 6.0.0
+Version: 7.0.0
 Summary: Downloader for firefox/jsshell builds.
 Home-page: https://github.com/MozillaSecurity/fuzzfetch
 Maintainer: Mozilla Fuzzing Team
 Maintainer-email: fuzzing@mozilla.com
 License: MPL 2.0
 Keywords: fuzz fuzzing security test testing
 Platform: any
```

### Comparing `fuzzfetch-6.0.0/src/fuzzfetch.egg-info/SOURCES.txt` & `fuzzfetch-7.0.0/src/fuzzfetch.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux-debug
 tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-aarch64-opt
 tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-asan-opt
 tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-ccov-fuzzing-asan-nyx-opt
 tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-ccov-fuzzing-opt
 tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-ccov-opt
 tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-debug
+tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-asan-afl-opt
 tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-asan-nyx-opt
 tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-asan-opt
 tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-debug
 tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-tsan-opt
 tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-searchfox-debug
 tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-tsan-opt
 tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-aarch64-fuzzing-asan-opt
@@ -417,14 +418,16 @@
 tests/mock-firefoxci/api/queue/v1/task/PU23u6VeRDWDKVUnX09Cvw/artifacts/public/build/target.json
 tests/mock-firefoxci/api/queue/v1/task/PUrV4bCUQ3GKWvMCV3_Bzw/artifacts/.get
 tests/mock-firefoxci/api/queue/v1/task/PUrV4bCUQ3GKWvMCV3_Bzw/artifacts/public/build/target.json
 tests/mock-firefoxci/api/queue/v1/task/QaS45XFwRASfCE9F9TaqCg/artifacts/.get
 tests/mock-firefoxci/api/queue/v1/task/QaS45XFwRASfCE9F9TaqCg/artifacts/public/build/target.json
 tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/artifacts/.get
 tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/artifacts/public/build/en-US/target.json
+tests/mock-firefoxci/api/queue/v1/task/Qsu15jVeRGeYGaPva8g7Xw/artifacts/.get
+tests/mock-firefoxci/api/queue/v1/task/Qsu15jVeRGeYGaPva8g7Xw/artifacts/public/build/target.json
 tests/mock-firefoxci/api/queue/v1/task/R6b2C_MbQwWKJPjvs_PZaA/artifacts/.get
 tests/mock-firefoxci/api/queue/v1/task/R6b2C_MbQwWKJPjvs_PZaA/artifacts/public/build/target.json
 tests/mock-firefoxci/api/queue/v1/task/R8E6ScjVREuVI0hLQorxwA/artifacts/.get
 tests/mock-firefoxci/api/queue/v1/task/R8E6ScjVREuVI0hLQorxwA/artifacts/public/build/target.json
 tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/artifacts/.get
 tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/artifacts/public/build/en-US/target.json
 tests/mock-firefoxci/api/queue/v1/task/Rd61yPVqQ0CdZmbvuQ9YcQ/artifacts/.get
```

### Comparing `fuzzfetch-6.0.0/tests/conftest.py` & `fuzzfetch-7.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2023.01.03` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2023.01.03`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2023.01.04` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2023.01.04`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2023.01.05` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2023.01.05`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2023.11.23` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2023.11.23`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2024.01.01` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2024.01.01`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2023.12.29` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2023.12.29`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2024.01.02` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2024.01.02`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/AGuXN_zgSTa4G2cOowM6tw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/AGuXN_zgSTa4G2cOowM6tw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/AGuXN_zgSTa4G2cOowM6tw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/AGuXN_zgSTa4G2cOowM6tw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Agexc3H0RvCxvLshb-oAkA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Agexc3H0RvCxvLshb-oAkA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Agexc3H0RvCxvLshb-oAkA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Agexc3H0RvCxvLshb-oAkA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/BMzeSq6sTVyo9tPp5vXCDg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/BMzeSq6sTVyo9tPp5vXCDg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/BMzeSq6sTVyo9tPp5vXCDg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/BMzeSq6sTVyo9tPp5vXCDg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Bs_nyxXCTNm5hMfjX7DFwg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Bs_nyxXCTNm5hMfjX7DFwg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Bs_nyxXCTNm5hMfjX7DFwg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Bs_nyxXCTNm5hMfjX7DFwg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/C7bbCHVySOCJsQ24TJvNig/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/C7bbCHVySOCJsQ24TJvNig/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/C7bbCHVySOCJsQ24TJvNig/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/C7bbCHVySOCJsQ24TJvNig/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/C9C2cj1aS_q_Nx4Bj8YImg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/C9C2cj1aS_q_Nx4Bj8YImg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/C9C2cj1aS_q_Nx4Bj8YImg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/C9C2cj1aS_q_Nx4Bj8YImg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CE-2EnNGTKSY_gd7i6nqsA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CE-2EnNGTKSY_gd7i6nqsA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CE-2EnNGTKSY_gd7i6nqsA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CE-2EnNGTKSY_gd7i6nqsA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CGU4FyPTS9eHQD5QApPhPA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CGU4FyPTS9eHQD5QApPhPA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CGU4FyPTS9eHQD5QApPhPA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CGU4FyPTS9eHQD5QApPhPA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CSTlwpXDRDyEUfFA22wvcQ/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CSTlwpXDRDyEUfFA22wvcQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/CSTlwpXDRDyEUfFA22wvcQ/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/CSTlwpXDRDyEUfFA22wvcQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Cyn7JDoPRwuRs_eShI9x4w/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Cyn7JDoPRwuRs_eShI9x4w/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Cyn7JDoPRwuRs_eShI9x4w/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Cyn7JDoPRwuRs_eShI9x4w/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/D12fNQbWTgCF6SYMi7fdew/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/D12fNQbWTgCF6SYMi7fdew/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/D12fNQbWTgCF6SYMi7fdew/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/D12fNQbWTgCF6SYMi7fdew/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/DTDhDQy_Te-8TX2GWjDyRA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/DTDhDQy_Te-8TX2GWjDyRA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/DTDhDQy_Te-8TX2GWjDyRA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/DTDhDQy_Te-8TX2GWjDyRA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Db65HT83SdCGu8IcAEMSJw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Db65HT83SdCGu8IcAEMSJw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Db65HT83SdCGu8IcAEMSJw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Db65HT83SdCGu8IcAEMSJw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/DvotWT9VS4---6k12rWy2g/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/DvotWT9VS4---6k12rWy2g/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/DvotWT9VS4---6k12rWy2g/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/DvotWT9VS4---6k12rWy2g/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/F-2XbyLdRoOWYqs1Wkz1bw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/F-2XbyLdRoOWYqs1Wkz1bw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/F-2XbyLdRoOWYqs1Wkz1bw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/F-2XbyLdRoOWYqs1Wkz1bw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/FK4OkxYcQWqYpmxP1ay0_A/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/FK4OkxYcQWqYpmxP1ay0_A/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/FK4OkxYcQWqYpmxP1ay0_A/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/FK4OkxYcQWqYpmxP1ay0_A/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/FWlvKTVwRUqznJSgpz4mSA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/FWlvKTVwRUqznJSgpz4mSA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/FWlvKTVwRUqznJSgpz4mSA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/FWlvKTVwRUqznJSgpz4mSA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Fy4__LJrS7yOddt0JlST1g/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Fy4__LJrS7yOddt0JlST1g/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Fy4__LJrS7yOddt0JlST1g/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Fy4__LJrS7yOddt0JlST1g/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GSN2ZF03SvGfJWTNQOR66Q/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GSN2ZF03SvGfJWTNQOR66Q/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GSN2ZF03SvGfJWTNQOR66Q/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GSN2ZF03SvGfJWTNQOR66Q/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Glj2IKdJQ1OoKLUOshkKuw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Glj2IKdJQ1OoKLUOshkKuw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Glj2IKdJQ1OoKLUOshkKuw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Glj2IKdJQ1OoKLUOshkKuw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GrUeski1SfiJNpkgzaWWww/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GrUeski1SfiJNpkgzaWWww/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GrUeski1SfiJNpkgzaWWww/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GrUeski1SfiJNpkgzaWWww/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GxgYQf58TRaWVJ-2vy4tLg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GxgYQf58TRaWVJ-2vy4tLg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/GxgYQf58TRaWVJ-2vy4tLg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/GxgYQf58TRaWVJ-2vy4tLg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/H_rT971WQQayQyE8l4ABqA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/H_rT971WQQayQyE8l4ABqA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/H_rT971WQQayQyE8l4ABqA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/H_rT971WQQayQyE8l4ABqA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/I1ojS418TMeExBMFJ3LcIA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/I1ojS418TMeExBMFJ3LcIA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/I1ojS418TMeExBMFJ3LcIA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/I1ojS418TMeExBMFJ3LcIA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/I2nBckWWSRahjagcQD3aCg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/I2nBckWWSRahjagcQD3aCg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/I2nBckWWSRahjagcQD3aCg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/I2nBckWWSRahjagcQD3aCg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/IMcMRzZvTVyh5X4GdIMKUg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/IMcMRzZvTVyh5X4GdIMKUg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/IMcMRzZvTVyh5X4GdIMKUg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/IMcMRzZvTVyh5X4GdIMKUg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/INMgwWKtT7Kp5SH7zAfQ7w/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/INMgwWKtT7Kp5SH7zAfQ7w/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/INMgwWKtT7Kp5SH7zAfQ7w/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/INMgwWKtT7Kp5SH7zAfQ7w/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Je_Ek1ecSgidmukgi1oGjA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Je_Ek1ecSgidmukgi1oGjA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Je_Ek1ecSgidmukgi1oGjA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Je_Ek1ecSgidmukgi1oGjA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/JwuxI9J2Q5qC4D9dzziQmg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/JwuxI9J2Q5qC4D9dzziQmg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/JwuxI9J2Q5qC4D9dzziQmg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/JwuxI9J2Q5qC4D9dzziQmg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KbaNeW1hTJqiQyiUjsPz-Q/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KbaNeW1hTJqiQyiUjsPz-Q/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KbaNeW1hTJqiQyiUjsPz-Q/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KbaNeW1hTJqiQyiUjsPz-Q/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KjRoo3mLSUqYc6iRB10r6A/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KjRoo3mLSUqYc6iRB10r6A/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KjRoo3mLSUqYc6iRB10r6A/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KjRoo3mLSUqYc6iRB10r6A/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KqRwX5EUQcK1b39svcLjjw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KqRwX5EUQcK1b39svcLjjw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/KqRwX5EUQcK1b39svcLjjw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/KqRwX5EUQcK1b39svcLjjw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/L1emPAoBROSoDSetQl5qYw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/L1emPAoBROSoDSetQl5qYw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/L1emPAoBROSoDSetQl5qYw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/L1emPAoBROSoDSetQl5qYw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LBuW7cjQS8-aE75qH-udRQ/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LBuW7cjQS8-aE75qH-udRQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LBuW7cjQS8-aE75qH-udRQ/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LBuW7cjQS8-aE75qH-udRQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LYO9FlvJQGSiffYQhMcW5Q/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LYO9FlvJQGSiffYQhMcW5Q/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LYO9FlvJQGSiffYQhMcW5Q/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LYO9FlvJQGSiffYQhMcW5Q/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Lelr43PoRWWgnumQRpIb8Q/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Lelr43PoRWWgnumQRpIb8Q/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Lelr43PoRWWgnumQRpIb8Q/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Lelr43PoRWWgnumQRpIb8Q/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LjluSbFjS5qg3jljQ38itQ/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LjluSbFjS5qg3jljQ38itQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LjluSbFjS5qg3jljQ38itQ/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LjluSbFjS5qg3jljQ38itQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LzlIi12cQsWwfxig59k2VQ/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LzlIi12cQsWwfxig59k2VQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/LzlIi12cQsWwfxig59k2VQ/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/LzlIi12cQsWwfxig59k2VQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MIuWH-PkRdOQvhsM9elc5Q/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MIuWH-PkRdOQvhsM9elc5Q/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MIuWH-PkRdOQvhsM9elc5Q/artifacts/public/build/en-US/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MIuWH-PkRdOQvhsM9elc5Q/artifacts/public/build/en-US/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MJfJtItbRjmydzrvwwURrg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MJfJtItbRjmydzrvwwURrg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MJfJtItbRjmydzrvwwURrg/artifacts/public/build/en-US/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MJfJtItbRjmydzrvwwURrg/artifacts/public/build/en-US/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MJm-0bUOR7WEyESS_3EuMg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MJm-0bUOR7WEyESS_3EuMg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MJm-0bUOR7WEyESS_3EuMg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MJm-0bUOR7WEyESS_3EuMg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MVFFVBcITlmoKD8m1Uqwkw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MVFFVBcITlmoKD8m1Uqwkw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/MVFFVBcITlmoKD8m1Uqwkw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/MVFFVBcITlmoKD8m1Uqwkw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Ma7H24MaS5GP8jZpl6R5Xw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Ma7H24MaS5GP8jZpl6R5Xw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Ma7H24MaS5GP8jZpl6R5Xw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Ma7H24MaS5GP8jZpl6R5Xw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/N491PvLhQcCSBX0gFmTKkg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/N491PvLhQcCSBX0gFmTKkg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/N491PvLhQcCSBX0gFmTKkg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/N491PvLhQcCSBX0gFmTKkg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/N7ENCbCgSvGvuiV3wM91Tg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/N7ENCbCgSvGvuiV3wM91Tg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/N7ENCbCgSvGvuiV3wM91Tg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/N7ENCbCgSvGvuiV3wM91Tg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/O2UuedRNRvSbkRXzgtfTZg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/O2UuedRNRvSbkRXzgtfTZg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/O2UuedRNRvSbkRXzgtfTZg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/O2UuedRNRvSbkRXzgtfTZg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/O5RMm0izRSSMLncwLUUZzA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/O5RMm0izRSSMLncwLUUZzA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/O5RMm0izRSSMLncwLUUZzA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/O5RMm0izRSSMLncwLUUZzA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Oxnm2nS5SQeujyAmxci87w/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Oxnm2nS5SQeujyAmxci87w/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Oxnm2nS5SQeujyAmxci87w/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Oxnm2nS5SQeujyAmxci87w/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PTEeGj5sQP-VOR_rereX_Q/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PTEeGj5sQP-VOR_rereX_Q/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PTEeGj5sQP-VOR_rereX_Q/artifacts/public/build/en-US/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PTEeGj5sQP-VOR_rereX_Q/artifacts/public/build/en-US/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PU23u6VeRDWDKVUnX09Cvw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PU23u6VeRDWDKVUnX09Cvw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PU23u6VeRDWDKVUnX09Cvw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PU23u6VeRDWDKVUnX09Cvw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PUrV4bCUQ3GKWvMCV3_Bzw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PUrV4bCUQ3GKWvMCV3_Bzw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/PUrV4bCUQ3GKWvMCV3_Bzw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/PUrV4bCUQ3GKWvMCV3_Bzw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/QaS45XFwRASfCE9F9TaqCg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/QaS45XFwRASfCE9F9TaqCg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/QaS45XFwRASfCE9F9TaqCg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/QaS45XFwRASfCE9F9TaqCg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/artifacts/public/build/en-US/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/QoL9iVgCTmWQWNa8jJzbew/artifacts/public/build/en-US/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/R6b2C_MbQwWKJPjvs_PZaA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/R6b2C_MbQwWKJPjvs_PZaA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/R6b2C_MbQwWKJPjvs_PZaA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/R6b2C_MbQwWKJPjvs_PZaA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/R8E6ScjVREuVI0hLQorxwA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/R8E6ScjVREuVI0hLQorxwA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/R8E6ScjVREuVI0hLQorxwA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/R8E6ScjVREuVI0hLQorxwA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/artifacts/public/build/en-US/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/RKe6CgRPThe8fr4L-oOTCQ/artifacts/public/build/en-US/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Rd61yPVqQ0CdZmbvuQ9YcQ/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Rd61yPVqQ0CdZmbvuQ9YcQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Rd61yPVqQ0CdZmbvuQ9YcQ/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Rd61yPVqQ0CdZmbvuQ9YcQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/S1o0P_q8RM601Mq0d4urkw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/S1o0P_q8RM601Mq0d4urkw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/S1o0P_q8RM601Mq0d4urkw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/S1o0P_q8RM601Mq0d4urkw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/SdJspoE-QROYKIlrSM5E9w/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/SdJspoE-QROYKIlrSM5E9w/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/SdJspoE-QROYKIlrSM5E9w/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/SdJspoE-QROYKIlrSM5E9w/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/SkWkmrKDSF2hQhnMOfS1PQ/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/SkWkmrKDSF2hQhnMOfS1PQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/SkWkmrKDSF2hQhnMOfS1PQ/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/SkWkmrKDSF2hQhnMOfS1PQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/T1ARQQKHTKu_m1EtjZv7YQ/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/T1ARQQKHTKu_m1EtjZv7YQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/T1ARQQKHTKu_m1EtjZv7YQ/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/T1ARQQKHTKu_m1EtjZv7YQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TJD91R5LTxSyqoutUKFjtg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TJD91R5LTxSyqoutUKFjtg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TJD91R5LTxSyqoutUKFjtg/artifacts/public/build/en-US/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TJD91R5LTxSyqoutUKFjtg/artifacts/public/build/en-US/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TTYSB2nKSUWvv5rbQDLtzw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TTYSB2nKSUWvv5rbQDLtzw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TTYSB2nKSUWvv5rbQDLtzw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TTYSB2nKSUWvv5rbQDLtzw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TXelMo4QSxqUzn0l-PWWyg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TXelMo4QSxqUzn0l-PWWyg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TXelMo4QSxqUzn0l-PWWyg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TXelMo4QSxqUzn0l-PWWyg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ThUoABnMR12AkygRTIAcKA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ThUoABnMR12AkygRTIAcKA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ThUoABnMR12AkygRTIAcKA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ThUoABnMR12AkygRTIAcKA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TheuGGRAQEeVfrK_nIxlYA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TheuGGRAQEeVfrK_nIxlYA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/TheuGGRAQEeVfrK_nIxlYA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/TheuGGRAQEeVfrK_nIxlYA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UUrwCxWRQ5OeCJEhZOQBHg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UUrwCxWRQ5OeCJEhZOQBHg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UUrwCxWRQ5OeCJEhZOQBHg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UUrwCxWRQ5OeCJEhZOQBHg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UoKNy4deRsKipcwj_CSJcA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UoKNy4deRsKipcwj_CSJcA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UoKNy4deRsKipcwj_CSJcA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UoKNy4deRsKipcwj_CSJcA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Ut4dGXE3RpCRQy6Pd2PpVg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Ut4dGXE3RpCRQy6Pd2PpVg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Ut4dGXE3RpCRQy6Pd2PpVg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Ut4dGXE3RpCRQy6Pd2PpVg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UuWQ2KScQ3KrYF4wFkczHw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UuWQ2KScQ3KrYF4wFkczHw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/UuWQ2KScQ3KrYF4wFkczHw/artifacts/public/build/en-US/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/UuWQ2KScQ3KrYF4wFkczHw/artifacts/public/build/en-US/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/VSEShvqcSxWWtdKaO6jagQ/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/VSEShvqcSxWWtdKaO6jagQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/VSEShvqcSxWWtdKaO6jagQ/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/VSEShvqcSxWWtdKaO6jagQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/V_S-Ts-2TmmGgDExnyG6qw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/V_S-Ts-2TmmGgDExnyG6qw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/V_S-Ts-2TmmGgDExnyG6qw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/V_S-Ts-2TmmGgDExnyG6qw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Vdir5WkdS-G7MKg1VPiWEg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Vdir5WkdS-G7MKg1VPiWEg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Vdir5WkdS-G7MKg1VPiWEg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Vdir5WkdS-G7MKg1VPiWEg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/VyFzvPDRSaaNnxo8A1krWg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/VyFzvPDRSaaNnxo8A1krWg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/VyFzvPDRSaaNnxo8A1krWg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/VyFzvPDRSaaNnxo8A1krWg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/WRq2BZCZRlCITcXJwi9VOA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/WRq2BZCZRlCITcXJwi9VOA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/WRq2BZCZRlCITcXJwi9VOA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/WRq2BZCZRlCITcXJwi9VOA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/XDp1D7tkQBK4u1XG4reYSA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/XDp1D7tkQBK4u1XG4reYSA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/XDp1D7tkQBK4u1XG4reYSA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/XDp1D7tkQBK4u1XG4reYSA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/XPfHK-vXS9uGpyq4-l6xtg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/XPfHK-vXS9uGpyq4-l6xtg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/XPfHK-vXS9uGpyq4-l6xtg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/XPfHK-vXS9uGpyq4-l6xtg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/X_XmczzYTA2l8JwACz-YBg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/X_XmczzYTA2l8JwACz-YBg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/X_XmczzYTA2l8JwACz-YBg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/X_XmczzYTA2l8JwACz-YBg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Y45GeFF7SPuy1IhX9CXMPw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Y45GeFF7SPuy1IhX9CXMPw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Y45GeFF7SPuy1IhX9CXMPw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Y45GeFF7SPuy1IhX9CXMPw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YE5qNXJbTuu2T2uXJhk5Nw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YE5qNXJbTuu2T2uXJhk5Nw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YE5qNXJbTuu2T2uXJhk5Nw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YE5qNXJbTuu2T2uXJhk5Nw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YGDcP8gRQPebxPg7efA7Iw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YGDcP8gRQPebxPg7efA7Iw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YGDcP8gRQPebxPg7efA7Iw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YGDcP8gRQPebxPg7efA7Iw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YWFg1gR3Rfu3LH7U6mB8EQ/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YWFg1gR3Rfu3LH7U6mB8EQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YWFg1gR3Rfu3LH7U6mB8EQ/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YWFg1gR3Rfu3LH7U6mB8EQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YWIA7hhsSCqyXKErOzGqIg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YWIA7hhsSCqyXKErOzGqIg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YWIA7hhsSCqyXKErOzGqIg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YWIA7hhsSCqyXKErOzGqIg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YYrpCCBgSSmTIrul3-dXGg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YYrpCCBgSSmTIrul3-dXGg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/YYrpCCBgSSmTIrul3-dXGg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/YYrpCCBgSSmTIrul3-dXGg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Yy5BKCQLSNKJmVlXUgZ-Vw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Yy5BKCQLSNKJmVlXUgZ-Vw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Yy5BKCQLSNKJmVlXUgZ-Vw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Yy5BKCQLSNKJmVlXUgZ-Vw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Z2wFgrvYQfWr4sZ_5xsJyg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Z2wFgrvYQfWr4sZ_5xsJyg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Z2wFgrvYQfWr4sZ_5xsJyg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Z2wFgrvYQfWr4sZ_5xsJyg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Z4Nk4adQT_KY6OB36jH7GA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Z4Nk4adQT_KY6OB36jH7GA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/Z4Nk4adQT_KY6OB36jH7GA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/Z4Nk4adQT_KY6OB36jH7GA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZHf8FbtqSZa-D8WeBBRQ9A/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZHf8FbtqSZa-D8WeBBRQ9A/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZHf8FbtqSZa-D8WeBBRQ9A/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZHf8FbtqSZa-D8WeBBRQ9A/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZKZozRyQT42x6mxaQ9LhnA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZKZozRyQT42x6mxaQ9LhnA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZKZozRyQT42x6mxaQ9LhnA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZKZozRyQT42x6mxaQ9LhnA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZcTIYEkjQO2aChxeIY6fbw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZcTIYEkjQO2aChxeIY6fbw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZcTIYEkjQO2aChxeIY6fbw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZcTIYEkjQO2aChxeIY6fbw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZukWWPukRoqeGyztJsYEXQ/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZukWWPukRoqeGyztJsYEXQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ZukWWPukRoqeGyztJsYEXQ/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ZukWWPukRoqeGyztJsYEXQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aAfWVw75TbKJ9Ff4vdSdXA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aAfWVw75TbKJ9Ff4vdSdXA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aAfWVw75TbKJ9Ff4vdSdXA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aAfWVw75TbKJ9Ff4vdSdXA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aNOLmiYFSnm51F5o0EF10A/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aNOLmiYFSnm51F5o0EF10A/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aNOLmiYFSnm51F5o0EF10A/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aNOLmiYFSnm51F5o0EF10A/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aNUeGazgSEqDVyec14YaHw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aNUeGazgSEqDVyec14YaHw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/aNUeGazgSEqDVyec14YaHw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/aNUeGazgSEqDVyec14YaHw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ac88QqpjTJuP6ZX2Is6yEQ/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ac88QqpjTJuP6ZX2Is6yEQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ac88QqpjTJuP6ZX2Is6yEQ/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ac88QqpjTJuP6ZX2Is6yEQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/auiN3S92TkiF21ayWnyfkw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/auiN3S92TkiF21ayWnyfkw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/auiN3S92TkiF21ayWnyfkw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/auiN3S92TkiF21ayWnyfkw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bkCYr42WR-aMl0t-rO918w/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bkCYr42WR-aMl0t-rO918w/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bkCYr42WR-aMl0t-rO918w/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bkCYr42WR-aMl0t-rO918w/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bqTeNQLPSHqviqZ-adbEgw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bqTeNQLPSHqviqZ-adbEgw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bqTeNQLPSHqviqZ-adbEgw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bqTeNQLPSHqviqZ-adbEgw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bsfhDaUBSZ-4IPUk_eXaSA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bsfhDaUBSZ-4IPUk_eXaSA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bsfhDaUBSZ-4IPUk_eXaSA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bsfhDaUBSZ-4IPUk_eXaSA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bwP8UBmpRRKBOstsMyYOtg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bwP8UBmpRRKBOstsMyYOtg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/bwP8UBmpRRKBOstsMyYOtg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/bwP8UBmpRRKBOstsMyYOtg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cEquZnIzQZKo-sHRNoWdxA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cEquZnIzQZKo-sHRNoWdxA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cEquZnIzQZKo-sHRNoWdxA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cEquZnIzQZKo-sHRNoWdxA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cf-lJNFgSsmK89NsnoUNqg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cf-lJNFgSsmK89NsnoUNqg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cf-lJNFgSsmK89NsnoUNqg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cf-lJNFgSsmK89NsnoUNqg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cfhgadFrQqGdfkUQrE8DNA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cfhgadFrQqGdfkUQrE8DNA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cfhgadFrQqGdfkUQrE8DNA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cfhgadFrQqGdfkUQrE8DNA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cxsX3JgCRt-tEsH-ouLt3Q/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cxsX3JgCRt-tEsH-ouLt3Q/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/cxsX3JgCRt-tEsH-ouLt3Q/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/cxsX3JgCRt-tEsH-ouLt3Q/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dNgIzJgjTlyYH24pQzLBug/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dNgIzJgjTlyYH24pQzLBug/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dNgIzJgjTlyYH24pQzLBug/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dNgIzJgjTlyYH24pQzLBug/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dZl_9NHxRkSM2YzG1Y29YA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dZl_9NHxRkSM2YzG1Y29YA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dZl_9NHxRkSM2YzG1Y29YA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dZl_9NHxRkSM2YzG1Y29YA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dcY-KGqYTdy67l7zA9K57Q/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dcY-KGqYTdy67l7zA9K57Q/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/dcY-KGqYTdy67l7zA9K57Q/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/dcY-KGqYTdy67l7zA9K57Q/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/e-15mv-6TR2SJu3iX1dz6w/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/e-15mv-6TR2SJu3iX1dz6w/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/e-15mv-6TR2SJu3iX1dz6w/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/e-15mv-6TR2SJu3iX1dz6w/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/e8lqN78UTRWWOtoT1U9YKw/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/e8lqN78UTRWWOtoT1U9YKw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/e8lqN78UTRWWOtoT1U9YKw/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/e8lqN78UTRWWOtoT1U9YKw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eEzNLZ8CRPG_rqJt94V2Jg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eEzNLZ8CRPG_rqJt94V2Jg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eEzNLZ8CRPG_rqJt94V2Jg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eEzNLZ8CRPG_rqJt94V2Jg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eNr5UDpwSv-owhKwo5RR5w/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eNr5UDpwSv-owhKwo5RR5w/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eNr5UDpwSv-owhKwo5RR5w/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eNr5UDpwSv-owhKwo5RR5w/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eRpROunvQa-sZ5n-zmHFCA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eRpROunvQa-sZ5n-zmHFCA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eRpROunvQa-sZ5n-zmHFCA/artifacts/public/build/en-US/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eRpROunvQa-sZ5n-zmHFCA/artifacts/public/build/en-US/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eUk3ZT1tQHmJBu06q-E-AQ/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eUk3ZT1tQHmJBu06q-E-AQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/eUk3ZT1tQHmJBu06q-E-AQ/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/eUk3ZT1tQHmJBu06q-E-AQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ebZgCLndSm2ew4fN6uM48Q/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ebZgCLndSm2ew4fN6uM48Q/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ebZgCLndSm2ew4fN6uM48Q/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ebZgCLndSm2ew4fN6uM48Q/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/erjBtcr7TeaKF9WkHH3fAA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/erjBtcr7TeaKF9WkHH3fAA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/erjBtcr7TeaKF9WkHH3fAA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/erjBtcr7TeaKF9WkHH3fAA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/esk9JKa7QxyKNF-pmg5UVA/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/esk9JKa7QxyKNF-pmg5UVA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/esk9JKa7QxyKNF-pmg5UVA/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/esk9JKa7QxyKNF-pmg5UVA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fMxvFK8yQQqnSYNv2r8Fyg/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fMxvFK8yQQqnSYNv2r8Fyg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fMxvFK8yQQqnSYNv2r8Fyg/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fMxvFK8yQQqnSYNv2r8Fyg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fcYf8jKOQ9yV6VtZtbFNJQ/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fcYf8jKOQ9yV6VtZtbFNJQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fcYf8jKOQ9yV6VtZtbFNJQ/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fcYf8jKOQ9yV6VtZtbFNJQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ff3I1qWyRvSKVMYbEZh39g/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ff3I1qWyRvSKVMYbEZh39g/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/ff3I1qWyRvSKVMYbEZh39g/artifacts/public/build/target.json` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/ff3I1qWyRvSKVMYbEZh39g/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-firefoxci/api/queue/v1/task/fn7T0nqKSK-wX_RsitMQwQ/artifacts/.get` & `fuzzfetch-7.0.0/tests/mock-firefoxci/api/queue/v1/task/fn7T0nqKSK-wX_RsitMQwQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-hg/mozilla-central/json-rev/10aa74237898` & `fuzzfetch-7.0.0/tests/mock-hg/mozilla-central/json-rev/10aa74237898`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-hg/mozilla-central/json-rev/5096e8be57730ef6902aaa8954b79aa0a21b32d6` & `fuzzfetch-7.0.0/tests/mock-hg/mozilla-central/json-rev/5096e8be57730ef6902aaa8954b79aa0a21b32d6`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/mock-product-details/1.0/firefox_versions.json` & `fuzzfetch-7.0.0/tests/mock-product-details/1.0/firefox_versions.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/test_core.py` & `fuzzfetch-7.0.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/test_extract.py` & `fuzzfetch-7.0.0/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `fuzzfetch-6.0.0/tests/test_fetch.py` & `fuzzfetch-7.0.0/tests/test_fetch.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,7 +296,20 @@
     """
     Fetcher(
         "central",
         "latest",
         build_flags_factory(searchfox=True, debug=True),
         ["searchfox"],
     )
+
+
+@pytest.mark.usefixtures("fetcher_mock_resolve_targets", "requests_mock_cache")
+def test_afl_builds():
+    """
+    Test for retrieving AFL++ enabled builds
+    """
+    Fetcher(
+        "central",
+        "latest",
+        build_flags_factory(asan=True, fuzzing=True, afl=True),
+        DEFAULT_TARGETS,
+    )
```

### Comparing `fuzzfetch-6.0.0/tox.ini` & `fuzzfetch-7.0.0/tox.ini`

 * *Files identical despite different names*

