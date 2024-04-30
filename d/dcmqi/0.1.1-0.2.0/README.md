# Comparing `tmp/dcmqi-0.1.1.tar.gz` & `tmp/dcmqi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcmqi-0.1.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "dcmqi-0.2.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `dcmqi-0.1.1.tar` & `dcmqi-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      426 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.copier-answers.yml
--rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.git_archival.txt
--rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.gitattributes
--rw-r--r--   0        0        0     2390 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.github/matchers/pylint.json
--rw-r--r--   0        0        0     3296 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.github/workflows/cd.yml
--rw-r--r--   0        0        0     2634 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2258 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.gitignore
--rw-r--r--   0        0        0     2591 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2022-11-09 12:37:21.000000 dcmqi-0.1.1/.readthedocs.yaml
--rw-r--r--   0        0        0     2103 2022-11-09 12:37:21.000000 dcmqi-0.1.1/CMakeLists.txt
--rw-r--r--   0        0        0     1057 2022-11-09 12:37:21.000000 dcmqi-0.1.1/LICENSE
--rw-r--r--   0        0        0     2323 2022-11-09 12:37:21.000000 dcmqi-0.1.1/README.md
--rw-r--r--   0        0        0     1304 2022-11-09 12:37:21.000000 dcmqi-0.1.1/dcmqiUrls.cmake
--rw-r--r--   0        0        0      837 2022-11-09 12:37:21.000000 dcmqi-0.1.1/docs/conf.py
--rw-r--r--   0        0        0      192 2022-11-09 12:37:21.000000 dcmqi-0.1.1/docs/index.md
--rw-r--r--   0        0        0     2738 2022-11-09 12:37:21.000000 dcmqi-0.1.1/noxfile.py
--rw-r--r--   0        0        0     4549 2022-11-09 12:37:21.000000 dcmqi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2194 2022-11-09 12:37:21.000000 dcmqi-0.1.1/src/dcmqi/__init__.py
--rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 dcmqi-0.1.1/src/dcmqi/_version.py
--rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 dcmqi-0.1.1/src/dcmqi/_version.pyi
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 dcmqi-0.1.1/src/dcmqi/py.typed
--rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 dcmqi-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2115 2022-11-09 12:37:21.000000 dcmqi-0.1.1/tests/test_executable.py
--rw-r--r--   0        0        0      167 2022-11-09 12:37:21.000000 dcmqi-0.1.1/tests/test_package.py
--rw-r--r--   0        0        0     5453 2022-11-09 12:37:21.000000 dcmqi-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      426 2022-11-09 12:37:21.000000 dcmqi-0.2.0/.copier-answers.yml
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 dcmqi-0.2.0/.git_archival.txt
+-rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 dcmqi-0.2.0/.gitattributes
+-rw-r--r--   0        0        0     2390 2022-11-09 12:37:21.000000 dcmqi-0.2.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 dcmqi-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2022-11-09 12:37:21.000000 dcmqi-0.2.0/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     3296 2022-11-09 12:37:21.000000 dcmqi-0.2.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2634 2022-11-09 12:37:21.000000 dcmqi-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2258 2022-11-09 12:37:21.000000 dcmqi-0.2.0/.gitignore
+-rw-r--r--   0        0        0     2591 2022-11-09 12:37:21.000000 dcmqi-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2022-11-09 12:37:21.000000 dcmqi-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     2103 2022-11-09 12:37:21.000000 dcmqi-0.2.0/CMakeLists.txt
+-rw-r--r--   0        0        0     1057 2022-11-09 12:37:21.000000 dcmqi-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2323 2022-11-09 12:37:21.000000 dcmqi-0.2.0/README.md
+-rw-r--r--   0        0        0     1304 2022-11-09 12:37:21.000000 dcmqi-0.2.0/dcmqiUrls.cmake
+-rw-r--r--   0        0        0      837 2022-11-09 12:37:21.000000 dcmqi-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0      192 2022-11-09 12:37:21.000000 dcmqi-0.2.0/docs/index.md
+-rw-r--r--   0        0        0     2738 2022-11-09 12:37:21.000000 dcmqi-0.2.0/noxfile.py
+-rw-r--r--   0        0        0     4549 2022-11-09 12:37:21.000000 dcmqi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2194 2022-11-09 12:37:21.000000 dcmqi-0.2.0/src/dcmqi/__init__.py
+-rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 dcmqi-0.2.0/src/dcmqi/_version.py
+-rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 dcmqi-0.2.0/src/dcmqi/_version.pyi
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 dcmqi-0.2.0/src/dcmqi/py.typed
+-rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 dcmqi-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     2115 2022-11-09 12:37:21.000000 dcmqi-0.2.0/tests/test_executable.py
+-rw-r--r--   0        0        0      167 2022-11-09 12:37:21.000000 dcmqi-0.2.0/tests/test_package.py
+-rw-r--r--   0        0        0     5453 2022-11-09 12:37:21.000000 dcmqi-0.2.0/PKG-INFO
```

### Comparing `dcmqi-0.1.1/.github/CONTRIBUTING.md` & `dcmqi-0.2.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.1/.github/matchers/pylint.json` & `dcmqi-0.2.0/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.1/.github/workflows/cd.yml` & `dcmqi-0.2.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.1/.github/workflows/ci.yml` & `dcmqi-0.2.0/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -97,13 +97,13 @@
             test-skip: "*-win_arm64"
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
-      - uses: pypa/cibuildwheel@v2.16.5
+      - uses: pypa/cibuildwheel@v2.17.0
         env:
           CIBW_BUILD: "${{ matrix.python-version }}-*"
           CIBW_ARCHS: "${{ matrix.arch }}"
           CIBW_TEST_SKIP: "${{ matrix.test-skip }}"
           CIBW_SKIP: "*musllinux*"
```

### Comparing `dcmqi-0.1.1/.gitignore` & `dcmqi-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.1/.pre-commit-config.yaml` & `dcmqi-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.1/CMakeLists.txt` & `dcmqi-0.2.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.1/LICENSE` & `dcmqi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.1/README.md` & `dcmqi-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.1/dcmqiUrls.cmake` & `dcmqi-0.2.0/dcmqiUrls.cmake`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Checksum copied from "dcmqi_checksums.txt" associated with the dcmqi GitHub release
 
-set(version "1.3.1")
+set(version "1.3.2")
 
 set(linux_filename    "dcmqi-${version}-linux.tar.gz")
-set(linux_sha256      "b119f1d292f3214203e5812fadbc527282400eed8342431539411d62fcc91c89")
+set(linux_sha256      "bdeb99a05465e568629a7e9f72903e3f3c108ab756856f4f5e1c1a714df7c609")
 
 set(macos_filename    "dcmqi-${version}-mac.tar.gz")
-set(macos_sha256      "24ed2dcce2cfe918e17c889e22505c679c73263eab247ad291e19ab8b26ebf5a")
+set(macos_sha256      "07f785318c3b73af73fed5919080481ef1580dbfdbde2a1aec272736848cc417")
 
 set(win64_filename    "dcmqi-${version}-win64.zip")
-set(win64_sha256      "141a3f713ace11bc956818d34af6a923f92d3dcaaf0675c1c88db75f2ac221f4")
+set(win64_sha256      "e5a5328743f8128517f21b0ea1e20fd68b2844908f7349a5b40d7b0aa9af7374")
 
 
 cmake_host_system_information(RESULT is_64bit QUERY IS_64BIT)
 
 set(archive "linux")
 
 if(APPLE)
```

### Comparing `dcmqi-0.1.1/docs/conf.py` & `dcmqi-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.1/noxfile.py` & `dcmqi-0.2.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.1/pyproject.toml` & `dcmqi-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.1/src/dcmqi/__init__.py` & `dcmqi-0.2.0/src/dcmqi/__init__.py`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.1/tests/test_executable.py` & `dcmqi-0.2.0/tests/test_executable.py`

 * *Files identical despite different names*

### Comparing `dcmqi-0.1.1/PKG-INFO` & `dcmqi-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcmqi
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python distribution of the DCMQI library collection.
 Author-Email: =?utf-8?q?Leonard_N=C3=BCrnberg?= <lnuernberg@bwh.harvard.edu>
 License: Copyright 2024 Leonard Nürnberg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

