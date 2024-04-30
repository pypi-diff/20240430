# Comparing `tmp/ckanext-unfold-1.0.0.tar.gz` & `tmp/ckanext_unfold-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-unfold-1.0.0.tar", last modified: Mon Sep  4 06:01:25 2023, max compression
+gzip compressed data, was "ckanext_unfold-1.0.1.tar", last modified: Tue Apr 30 08:26:48 2024, max compression
```

## Comparing `ckanext-unfold-1.0.0.tar` & `ckanext_unfold-1.0.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-09-04 06:01:25.358640 ckanext-unfold-1.0.0/
--rw-r--r--   0 berry     (1000) berry     (1000)    34500 2023-08-30 17:41:49.000000 ckanext-unfold-1.0.0/LICENSE
--rw-r--r--   0 berry     (1000) berry     (1000)      197 2023-08-30 17:41:49.000000 ckanext-unfold-1.0.0/MANIFEST.in
--rw-r--r--   0 berry     (1000) berry     (1000)     3096 2023-09-04 06:01:25.358640 ckanext-unfold-1.0.0/PKG-INFO
--rw-r--r--   0 berry     (1000) berry     (1000)     2490 2023-09-03 13:12:53.000000 ckanext-unfold-1.0.0/README.md
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-09-04 06:01:25.358640 ckanext-unfold-1.0.0/ckanext/
--rw-r--r--   0 berry     (1000) berry     (1000)      221 2023-09-01 09:01:09.000000 ckanext-unfold-1.0.0/ckanext/__init__.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-09-04 06:01:25.358640 ckanext-unfold-1.0.0/ckanext/unfold/
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2023-08-30 17:41:49.000000 ckanext-unfold-1.0.0/ckanext/unfold/__init__.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-09-04 06:01:25.358640 ckanext-unfold-1.0.0/ckanext/unfold/adapters/
--rw-r--r--   0 berry     (1000) berry     (1000)     2869 2023-09-03 15:27:29.000000 ckanext-unfold-1.0.0/ckanext/unfold/adapters/_7z.py
--rw-r--r--   0 berry     (1000) berry     (1000)      666 2023-09-03 14:25:45.000000 ckanext-unfold-1.0.0/ckanext/unfold/adapters/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)     1125 2023-09-02 06:42:25.000000 ckanext-unfold-1.0.0/ckanext/unfold/adapters/gzip.py
--rw-r--r--   0 berry     (1000) berry     (1000)     3179 2023-09-03 15:27:21.000000 ckanext-unfold-1.0.0/ckanext/unfold/adapters/rar.py
--rw-r--r--   0 berry     (1000) berry     (1000)     3309 2023-09-03 15:21:13.000000 ckanext-unfold-1.0.0/ckanext/unfold/adapters/rpm.py
--rw-r--r--   0 berry     (1000) berry     (1000)     2878 2023-09-03 15:20:46.000000 ckanext-unfold-1.0.0/ckanext/unfold/adapters/tar.py
--rw-r--r--   0 berry     (1000) berry     (1000)     3129 2023-09-03 15:21:20.000000 ckanext-unfold-1.0.0/ckanext/unfold/adapters/zip.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-09-04 06:01:25.358640 ckanext-unfold-1.0.0/ckanext/unfold/assets/
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-09-04 06:01:25.358640 ckanext-unfold-1.0.0/ckanext/unfold/assets/css/
--rw-r--r--   0 berry     (1000) berry     (1000)      705 2023-09-03 15:27:45.000000 ckanext-unfold-1.0.0/ckanext/unfold/assets/css/unfold.css
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-09-04 06:01:25.358640 ckanext-unfold-1.0.0/ckanext/unfold/assets/js/
--rw-r--r--   0 berry     (1000) berry     (1000)     2247 2023-09-03 15:27:04.000000 ckanext-unfold-1.0.0/ckanext/unfold/assets/js/unfold-init-jstree.js
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-09-04 06:01:25.358640 ckanext-unfold-1.0.0/ckanext/unfold/assets/vendor/
--rw-r--r--   0 berry     (1000) berry     (1000)    41414 2023-09-01 10:57:10.000000 ckanext-unfold-1.0.0/ckanext/unfold/assets/vendor/jstree-table.js
--rw-r--r--   0 berry     (1000) berry     (1000)    32380 2023-08-31 14:14:28.000000 ckanext-unfold-1.0.0/ckanext/unfold/assets/vendor/jstree.min.css
--rw-r--r--   0 berry     (1000) berry     (1000)   141916 2023-09-03 14:16:06.000000 ckanext-unfold-1.0.0/ckanext/unfold/assets/vendor/jstree.min.js
--rw-r--r--   0 berry     (1000) berry     (1000)      357 2023-09-02 06:45:37.000000 ckanext-unfold-1.0.0/ckanext/unfold/assets/webassets.yml
--rw-r--r--   0 berry     (1000) berry     (1000)       39 2023-09-01 18:44:30.000000 ckanext-unfold-1.0.0/ckanext/unfold/exception.py
--rw-r--r--   0 berry     (1000) berry     (1000)     2102 2023-09-02 06:44:59.000000 ckanext-unfold-1.0.0/ckanext/unfold/plugin.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-09-04 06:01:25.358640 ckanext-unfold-1.0.0/ckanext/unfold/templates/
--rw-r--r--   0 berry     (1000) berry     (1000)      261 2023-08-30 17:50:43.000000 ckanext-unfold-1.0.0/ckanext/unfold/templates/unfold_form.html
--rw-r--r--   0 berry     (1000) berry     (1000)     1346 2023-09-03 15:26:46.000000 ckanext-unfold-1.0.0/ckanext/unfold/templates/unfold_preview.html
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-09-04 06:01:25.358640 ckanext-unfold-1.0.0/ckanext/unfold/tests/
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2023-08-30 17:41:49.000000 ckanext-unfold-1.0.0/ckanext/unfold/tests/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)      298 2023-09-02 06:57:51.000000 ckanext-unfold-1.0.0/ckanext/unfold/tests/test_unfold.py
--rw-r--r--   0 berry     (1000) berry     (1000)      331 2023-09-03 14:59:44.000000 ckanext-unfold-1.0.0/ckanext/unfold/types.py
--rw-r--r--   0 berry     (1000) berry     (1000)     4130 2023-09-03 15:28:15.000000 ckanext-unfold-1.0.0/ckanext/unfold/utils.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-09-04 06:01:25.358640 ckanext-unfold-1.0.0/ckanext_unfold.egg-info/
--rw-r--r--   0 berry     (1000) berry     (1000)     3096 2023-09-04 06:01:25.000000 ckanext-unfold-1.0.0/ckanext_unfold.egg-info/PKG-INFO
--rw-r--r--   0 berry     (1000) berry     (1000)     1136 2023-09-04 06:01:25.000000 ckanext-unfold-1.0.0/ckanext_unfold.egg-info/SOURCES.txt
--rw-r--r--   0 berry     (1000) berry     (1000)        1 2023-09-04 06:01:25.000000 ckanext-unfold-1.0.0/ckanext_unfold.egg-info/dependency_links.txt
--rw-r--r--   0 berry     (1000) berry     (1000)      116 2023-09-04 06:01:25.000000 ckanext-unfold-1.0.0/ckanext_unfold.egg-info/entry_points.txt
--rw-r--r--   0 berry     (1000) berry     (1000)        8 2023-09-04 06:01:25.000000 ckanext-unfold-1.0.0/ckanext_unfold.egg-info/namespace_packages.txt
--rw-r--r--   0 berry     (1000) berry     (1000)       58 2023-09-04 06:01:25.000000 ckanext-unfold-1.0.0/ckanext_unfold.egg-info/requires.txt
--rw-r--r--   0 berry     (1000) berry     (1000)        8 2023-09-04 06:01:25.000000 ckanext-unfold-1.0.0/ckanext_unfold.egg-info/top_level.txt
--rw-r--r--   0 berry     (1000) berry     (1000)     2973 2023-09-01 14:16:06.000000 ckanext-unfold-1.0.0/pyproject.toml
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2023-08-30 17:41:49.000000 ckanext-unfold-1.0.0/requirements.txt
--rw-r--r--   0 berry     (1000) berry     (1000)     1627 2023-09-04 06:01:25.358640 ckanext-unfold-1.0.0/setup.cfg
--rw-r--r--   0 berry     (1000) berry     (1000)      528 2023-09-01 09:01:09.000000 ckanext-unfold-1.0.0/setup.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-30 08:26:48.912354 ckanext_unfold-1.0.1/
+-rw-r--r--   0 berry     (1000) berry     (1000)    34500 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/LICENSE
+-rw-r--r--   0 berry     (1000) berry     (1000)      197 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/MANIFEST.in
+-rw-r--r--   0 berry     (1000) berry     (1000)     3095 2024-04-30 08:26:48.912354 ckanext_unfold-1.0.1/PKG-INFO
+-rw-r--r--   0 berry     (1000) berry     (1000)     2371 2024-04-30 08:26:15.000000 ckanext_unfold-1.0.1/README.md
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-30 08:26:48.912354 ckanext_unfold-1.0.1/ckanext/
+-rw-r--r--   0 berry     (1000) berry     (1000)      221 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/__init__.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-30 08:26:48.912354 ckanext_unfold-1.0.1/ckanext/unfold/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/__init__.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-30 08:26:48.912354 ckanext_unfold-1.0.1/ckanext/unfold/adapters/
+-rw-r--r--   0 berry     (1000) berry     (1000)     2906 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/adapters/_7z.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      666 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/adapters/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1162 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/adapters/gzip.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     3523 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/adapters/rar.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     3346 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/adapters/rpm.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2922 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/adapters/tar.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     3160 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/adapters/zip.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-30 08:26:48.912354 ckanext_unfold-1.0.1/ckanext/unfold/assets/
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-30 08:26:48.912354 ckanext_unfold-1.0.1/ckanext/unfold/assets/css/
+-rw-r--r--   0 berry     (1000) berry     (1000)     1446 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/assets/css/unfold.css
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-30 08:26:48.912354 ckanext_unfold-1.0.1/ckanext/unfold/assets/js/
+-rw-r--r--   0 berry     (1000) berry     (1000)     2586 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/assets/js/unfold-init-jstree.js
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-30 08:26:48.912354 ckanext_unfold-1.0.1/ckanext/unfold/assets/vendor/
+-rw-r--r--   0 berry     (1000) berry     (1000)    41414 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/assets/vendor/jstree-table.js
+-rw-r--r--   0 berry     (1000) berry     (1000)    23108 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/assets/vendor/jstree.min.css
+-rw-r--r--   0 berry     (1000) berry     (1000)   141970 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/assets/vendor/jstree.min.js
+-rw-r--r--   0 berry     (1000) berry     (1000)      357 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/assets/webassets.yml
+-rw-r--r--   0 berry     (1000) berry     (1000)       39 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/exception.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2137 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/plugin.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-30 08:26:48.912354 ckanext_unfold-1.0.1/ckanext/unfold/templates/
+-rw-r--r--   0 berry     (1000) berry     (1000)      359 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/templates/unfold_form.html
+-rw-r--r--   0 berry     (1000) berry     (1000)     1401 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/templates/unfold_preview.html
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-30 08:26:48.912354 ckanext_unfold-1.0.1/ckanext/unfold/tests/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/tests/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      298 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/tests/test_unfold.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      331 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/types.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4066 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/ckanext/unfold/utils.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-30 08:26:48.912354 ckanext_unfold-1.0.1/ckanext_unfold.egg-info/
+-rw-r--r--   0 berry     (1000) berry     (1000)     3095 2024-04-30 08:26:48.000000 ckanext_unfold-1.0.1/ckanext_unfold.egg-info/PKG-INFO
+-rw-r--r--   0 berry     (1000) berry     (1000)     1136 2024-04-30 08:26:48.000000 ckanext_unfold-1.0.1/ckanext_unfold.egg-info/SOURCES.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)        1 2024-04-30 08:26:48.000000 ckanext_unfold-1.0.1/ckanext_unfold.egg-info/dependency_links.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)      116 2024-04-30 08:26:48.000000 ckanext_unfold-1.0.1/ckanext_unfold.egg-info/entry_points.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)        8 2024-04-30 08:26:48.000000 ckanext_unfold-1.0.1/ckanext_unfold.egg-info/namespace_packages.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)       58 2024-04-30 08:26:48.000000 ckanext_unfold-1.0.1/ckanext_unfold.egg-info/requires.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)        8 2024-04-30 08:26:48.000000 ckanext_unfold-1.0.1/ckanext_unfold.egg-info/top_level.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)     2973 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/pyproject.toml
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/requirements.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)     1627 2024-04-30 08:26:48.912354 ckanext_unfold-1.0.1/setup.cfg
+-rw-r--r--   0 berry     (1000) berry     (1000)      528 2024-04-16 14:04:43.000000 ckanext_unfold-1.0.1/setup.py
```

### Comparing `ckanext-unfold-1.0.0/LICENSE` & `ckanext_unfold-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-unfold-1.0.0/PKG-INFO` & `ckanext_unfold-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: ckanext-unfold
-Version: 1.0.0
+Version: 1.0.1
 Summary: Provides previews for multiple archive formats
 Home-page: https://github.com//ckanext-unfold
 Author: Oleksandr Cherniavskyi
 Author-email: mutantsan@gmail.com
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: rarfile==4.0
+Requires-Dist: py7zr==0.20.6
+Requires-Dist: rpmfile==1.1.1
+Requires-Dist: pydantic==2.3.0
 
 [![Tests](https://github.com/mutantsan/ckanext-unfold/workflows/Tests/badge.svg?branch=master)](https://github.com/mutantsan/ckanext-unfold/actions)
 
 # ckanext-unfold
 
-Preview for different archive formats
-### TODO
- - ~~implement remote support for tar, 7z~~
- - ~~add password support for all adapters~~
- - ~~refactor to show an error to user if something went wrong (no pass, request exp, corrupted or empty archive)~~
+Enhance your CKAN experience with our extension that enables seamless previews of various archive formats, ensuring easy access and efficient data management.
 
 
 ## What are the dependencies?
 
 Working with different archive formats requires different tools:
 
 ### RAR, CBR
@@ -63,14 +63,10 @@
 
 ### RPM
 
 We are using [`rpmfile`](https://github.com/srossross/rpmfile) library.
 
 If you want to use rpmfile with zstd compressed rpms, you'll need to install the [`zstandard`](https://pypi.org/project/zstandard/) module.
 
-## Config settings
-
-TODO
-
 ## License
 
 [AGPL](https://www.gnu.org/licenses/agpl-3.0.en.html)
```

### Comparing `ckanext-unfold-1.0.0/README.md` & `ckanext_unfold-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 [![Tests](https://github.com/mutantsan/ckanext-unfold/workflows/Tests/badge.svg?branch=master)](https://github.com/mutantsan/ckanext-unfold/actions)
 
 # ckanext-unfold
 
-Preview for different archive formats
-### TODO
- - ~~implement remote support for tar, 7z~~
- - ~~add password support for all adapters~~
- - ~~refactor to show an error to user if something went wrong (no pass, request exp, corrupted or empty archive)~~
+Enhance your CKAN experience with our extension that enables seamless previews of various archive formats, ensuring easy access and efficient data management.
 
 
 ## What are the dependencies?
 
 Working with different archive formats requires different tools:
 
 ### RAR, CBR
@@ -46,14 +42,10 @@
 
 ### RPM
 
 We are using [`rpmfile`](https://github.com/srossross/rpmfile) library.
 
 If you want to use rpmfile with zstd compressed rpms, you'll need to install the [`zstandard`](https://pypi.org/project/zstandard/) module.
 
-## Config settings
-
-TODO
-
 ## License
 
 [AGPL](https://www.gnu.org/licenses/agpl-3.0.en.html)
```

### Comparing `ckanext-unfold-1.0.0/ckanext/unfold/adapters/_7z.py` & `ckanext_unfold-1.0.1/ckanext/unfold/adapters/_7z.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 import ckanext.unfold.exception as unf_exception
 import ckanext.unfold.types as unf_types
 import ckanext.unfold.utils as unf_utils
 
 log = logging.getLogger(__name__)
 
 
-def build_directory_tree(filepath: str, remote: Optional[bool] = False):
+def build_directory_tree(
+    filepath: str, resource_view: dict[str, Any], remote: Optional[bool] = False
+):
     try:
         if remote:
             file_list = get7zlist_from_url(filepath)
         else:
             with py7zr.SevenZipFile(filepath) as archive:
                 if archive.needs_password():
                     raise unf_exception.UnfoldError(
```

### Comparing `ckanext-unfold-1.0.0/ckanext/unfold/adapters/__init__.py` & `ckanext_unfold-1.0.1/ckanext/unfold/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-unfold-1.0.0/ckanext/unfold/adapters/gzip.py` & `ckanext_unfold-1.0.1/ckanext/unfold/adapters/gzip.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 from ckan import model as model
 
 import ckanext.unfold.types as unf_types
 import ckanext.unfold.utils as unf_utils
 
 
-def build_directory_tree(filepath: str, remote: Optional[bool] = False):
+def build_directory_tree(
+    filepath: str, resource_view: dict[str, Any], remote: Optional[bool] = False
+):
     resource = _get_resource(filepath)
     return [_build_node(resource)]
 
 
 def _get_resource(filepath: str) -> model.Resource:
     """We don't have a solution for gzip preview yet..."""
     parts = filepath.split("/")
```

### Comparing `ckanext-unfold-1.0.0/ckanext/unfold/adapters/rar.py` & `ckanext_unfold-1.0.1/ckanext/unfold/adapters/rar.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,32 +16,39 @@
 import ckanext.unfold.types as unf_types
 import ckanext.unfold.utils as unf_utils
 
 log = logging.getLogger(__name__)
 
 
 def build_directory_tree(
-    filepath: str, remote: Optional[bool] = False
+    filepath: str, resource_view: dict[str, Any], remote: Optional[bool] = False
 ) -> list[unf_types.Node]:
     try:
         if remote:
             file_list = get_rarlist_from_url(filepath)
         else:
             with rarfile.RarFile(filepath) as archive:
-                if archive.needs_password():
+                if archive.needs_password() and not resource_view.get("archive_pass"):
                     raise unf_exception.UnfoldError(
                         "Error. Archive is protected with password"
                     )
+                elif archive.needs_password():
+                    archive.setpassword(resource_view["archive_pass"])
 
                 file_list: list[RarInfo] = archive.infolist()
     except RarError as e:
         raise unf_exception.UnfoldError(f"Error openning archive: {e}")
     except requests.RequestException as e:
         raise unf_exception.UnfoldError(f"Error fetching remote archive: {e}")
 
+    if not file_list:
+        raise unf_exception.UnfoldError(
+            "Error. The archive is either empty or the password is incorrect."
+        )
+
     nodes: list[unf_types.Node] = []
 
     for entry in file_list:
         nodes.append(_build_node(entry))
 
     return nodes
```

### Comparing `ckanext-unfold-1.0.0/ckanext/unfold/adapters/rpm.py` & `ckanext_unfold-1.0.1/ckanext/unfold/adapters/rpm.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 import ckanext.unfold.exception as unf_exception
 import ckanext.unfold.types as unf_types
 import ckanext.unfold.utils as unf_utils
 
 log = logging.getLogger(__name__)
 
 
-def build_directory_tree(filepath: str, remote: Optional[bool] = False):
+def build_directory_tree(
+    filepath: str, resource_view: dict[str, Any], remote: Optional[bool] = False
+):
     try:
         if remote:
             file_list = get_rpmlist_from_url(filepath)
         else:
             with RPMFile(filepath, "rb") as archive:
                 file_list: list[RPMInfo] = archive.getmembers()
     except (NotImplementedError, KeyError) as e:
```

### Comparing `ckanext-unfold-1.0.0/ckanext/unfold/adapters/tar.py` & `ckanext_unfold-1.0.1/ckanext/unfold/adapters/tar.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 import ckanext.unfold.types as unf_types
 import ckanext.unfold.utils as unf_utils
 
 log = logging.getLogger(__name__)
 
 
 def build_directory_tree(
-    filepath: str, remote: Optional[bool] = False, compression: Optional[str] = None
+    filepath: str,
+    resource_view: dict[str, Any],
+    remote: Optional[bool] = False,
+    compression: Optional[str] = None,
 ):
     mode = "r" if not compression else f"r:{compression}"
 
     try:
         if remote:
             file_list = get_tarlist_from_url(filepath)
         else:
```

### Comparing `ckanext-unfold-1.0.0/ckanext/unfold/adapters/zip.py` & `ckanext_unfold-1.0.1/ckanext/unfold/adapters/zip.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import ckanext.unfold.types as unf_types
 import ckanext.unfold.utils as unf_utils
 
 log = logging.getLogger(__name__)
 
 
 def build_directory_tree(
-    filepath: str, remote: Optional[bool] = False
+    filepath: str, resource_view: dict[str, Any], remote: Optional[bool] = False
 ) -> list[unf_types.Node]:
     try:
         if remote:
             file_list = get_ziplist_from_url(filepath)
         else:
             with ZipFile(filepath) as archive:
                 # zip format do not support encrypted filenames so we don't have
```

### Comparing `ckanext-unfold-1.0.0/ckanext/unfold/assets/js/unfold-init-jstree.js` & `ckanext_unfold-1.0.1/ckanext/unfold/assets/js/unfold-init-jstree.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,28 +1,30 @@
 ckan.module("unfold-init-jstree", function($, _) {
     "use strict";
     return {
         options: {
             data: null,
             resourceId: null,
+            resourceViewId: null
         },
 
         initialize: function() {
             $.proxyAll(this, /_/);
 
             this.tree = $(this.el)
             this.errorBlock = $("#archive-tree-error");
 
             $("#jstree-search").on("change", this._onSearch);
             $("#jstree-search-clear").click(this._onClearSearch);
 
             $.ajax({
                 url: this.sandbox.url("/api/action/get_archive_structure"),
                 data: {
-                    "id": this.options.resourceId
+                    "id": this.options.resourceId,
+                    "view_id": this.options.resourceViewId
                 },
                 success: this._onSuccessRequest
             });
         },
 
         _onSearch: function(e) {
             this.tree.jstree("search", $(e.target).val())
@@ -54,33 +56,42 @@
                         dots: false
                     }
                 },
                 search: {
                     show_only_matches: true,
                 },
                 table: {
+                    columnWidth: "200px",
                     columns: [{
                         width: 400,
                         header: "Name"
                     }, {
                         width: 100,
                         header: "Size",
-                        value: "size"
+                        value: "size",
+                        cellClass: "js-tree-col",
+                        wideCellClass: "js-tree-col"
                     }, {
                         width: 100,
                         header: "Type",
-                        value: "type"
+                        value: "type",
+                        cellClass: "js-tree-col",
+                        wideCellClass: "js-tree-col"
                     }, {
                         width: 100,
                         header: "Format",
-                        value: "format"
+                        value: "format",
+                        cellClass: "js-tree-col",
+                        wideCellClass: "js-tree-col"
                     }, {
-                        width: 100,
+                        width: 200,
                         header: "Modified at",
-                        value: "modified_at"
+                        value: "modified_at",
+                        cellClass: "js-tree-col",
+                        wideCellClass: "js-tree-col"
                     }],
                     height: 700,
                 },
                 plugins: [
                     "search", "table", "sort"
                 ]
             });
```

### Comparing `ckanext-unfold-1.0.0/ckanext/unfold/assets/vendor/jstree-table.js` & `ckanext_unfold-1.0.1/ckanext/unfold/assets/vendor/jstree-table.js`

 * *Files identical despite different names*

### Comparing `ckanext-unfold-1.0.0/ckanext/unfold/assets/vendor/jstree.min.js` & `ckanext_unfold-1.0.1/ckanext/unfold/assets/vendor/jstree.min.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,28 +1,28 @@
-/*! jsTree - v3.3.15 - 2023-02-20 - (MIT) */
+/*! jsTree - v3.3.16 - 2023-09-19 - (MIT) */
 
 ! function(e) {
     "use strict";
     "function" == typeof define && define.amd ? define(["jquery"], e) : "undefined" != typeof module && module.exports ? module.exports = e(require("jquery")) : e(jQuery)
 }(function(E, P) {
     "use strict";
     if (!E.jstree) {
         var s = 0,
             a = !1,
             n = !1,
-            d = !1,
+            o = !1,
             r = [],
             e = E("script:last").attr("src"),
             b = window.document,
             c = window.setImmediate,
             i = window.Promise;
         !c && i && (c = function(e, t) {
             i.resolve(t).then(e)
         }), E.jstree = {
-            version: "3.3.15",
+            version: "3.3.16",
             defaults: {
                 plugins: []
             },
             plugins: {},
             path: e && -1 !== e.indexOf("/") ? e.replace(/\/[^\/]+$/, "") : "",
             idregex: /[\\:&!^|()\[\]<>@*'+~#";.,=\- \/${}%?`]/g,
             root: "#"
@@ -138,15 +138,16 @@
                 },
                 end: function(e) {
                     e.preventDefault(), this.element.find(".jstree-anchor").filter(":visible").last().trigger("focus")
                 },
                 f2: function(e) {
                     e.preventDefault(), this.edit(e.currentTarget)
                 }
-            }
+            },
+            allow_reselect: !1
         }, E.jstree.core.prototype = {
             plugin: function(e, t) {
                 var i = E.jstree.plugins[e];
                 return i ? (this._data[e] = {}, i.prototype = this, new i(t, this)) : this
             },
             init: function(e, t) {
                 this._model = {
@@ -513,19 +514,19 @@
             },
             is_closed: function(e) {
                 return (e = this.get_node(e)) && this.is_parent(e) && !e.state.opened
             },
             is_leaf: function(e) {
                 return !this.is_parent(e)
             },
-            load_node: function(n, d) {
+            load_node: function(n, o) {
                 var e = this.get_node(n, !0),
                     t, i, r, s, a;
-                if (E.vakata.is_array(n)) return this._load_nodes(n.slice(), d), !0;
-                if (!(n = this.get_node(n))) return d && d.call(this, n, !1), !1;
+                if (E.vakata.is_array(n)) return this._load_nodes(n.slice(), o), !0;
+                if (!(n = this.get_node(n))) return o && o.call(this, n, !1), !1;
                 if (n.state.loaded) {
                     for (n.state.loaded = !1, r = 0, s = n.parents.length; r < s; r++) this._model.data[n.parents[r]].children_d = E.vakata.array_filter(this._model.data[n.parents[r]].children_d, function(e) {
                         return -1 === E.inArray(e, n.children_d)
                     });
                     for (t = 0, i = n.children_d.length; t < i; t++) this._model.data[n.children_d[t]].state.selected && (a = !0), delete this._model.data[n.children_d[t]];
                     a && (this._data.core.selected = E.vakata.array_filter(this._data.core.selected, function(e) {
                         return -1 === E.inArray(e, n.children_d)
@@ -540,23 +541,23 @@
                     for (var t = this.get_node(n, !0), i = 0, r = 0, s = this._model.data, a = !1, i = 0, r = n.children.length; i < r; i++)
                         if (s[n.children[i]] && !s[n.children[i]].state.hidden) {
                             a = !0;
                             break
                         } n.state.loaded && t && t.length && (t.removeClass("jstree-closed jstree-open jstree-leaf"), a ? "#" !== n.id && t.addClass(n.state.opened ? "jstree-open" : "jstree-closed") : t.addClass("jstree-leaf")), (n.id !== E.jstree.root ? t.children(".jstree-anchor") : t).attr("aria-busy", !1), t.removeClass("jstree-loading"), this.trigger("load_node", {
                         node: n,
                         status: e
-                    }), d && d.call(this, n, e)
+                    }), o && o.call(this, n, e)
                 }.bind(this)), !0
             },
             _load_nodes: function(e, t, i, r) {
                 for (var s = !0, a = function() {
                         this._load_nodes(e, t, !0)
-                    }, n = this._model.data, d, o, c = [], d = 0, o = e.length; d < o; d++) n[e[d]] && (!n[e[d]].state.loaded && !n[e[d]].state.failed || !i && r) && (this.is_loading(e[d]) || this.load_node(e[d], a), s = !1);
+                    }, n = this._model.data, o, d, c = [], o = 0, d = e.length; o < d; o++) n[e[o]] && (!n[e[o]].state.loaded && !n[e[o]].state.failed || !i && r) && (this.is_loading(e[o]) || this.load_node(e[o], a), s = !1);
                 if (s) {
-                    for (d = 0, o = e.length; d < o; d++) n[e[d]] && n[e[d]].state.loaded && c.push(e[d]);
+                    for (o = 0, d = e.length; o < d; o++) n[e[o]] && n[e[o]].state.loaded && c.push(e[o]);
                     t && !t.done && (t.call(this, c), t.done = !0)
                 }
             },
             load_all: function(e, t) {
                 if (e = e || E.jstree.root, !(e = this.get_node(e))) return !1;
                 var i = [],
                     r = this._model.data,
@@ -635,29 +636,29 @@
             _append_html_data: function(e, t, i) {
                 (e = this.get_node(e)).children = [], e.children_d = [];
                 var t = t.is("ul") ? t.children() : t,
                     r = e.id,
                     s = [],
                     a = [],
                     n = this._model.data,
-                    d = n[r],
+                    o = n[r],
                     e = this._data.core.selected.length,
-                    o, c, l;
+                    d, c, l;
                 for (t.each(function(e, t) {
-                        (o = this._parse_model_from_html(E(t), r, d.parents.concat())) && (s.push(o), a.push(o), n[o].children_d.length && (a = a.concat(n[o].children_d)))
-                    }.bind(this)), d.children = s, d.children_d = a, c = 0, l = d.parents.length; c < l; c++) n[d.parents[c]].children_d = n[d.parents[c]].children_d.concat(a);
+                        (d = this._parse_model_from_html(E(t), r, o.parents.concat())) && (s.push(d), a.push(d), n[d].children_d.length && (a = a.concat(n[d].children_d)))
+                    }.bind(this)), o.children = s, o.children_d = a, c = 0, l = o.parents.length; c < l; c++) n[o.parents[c]].children_d = n[o.parents[c]].children_d.concat(a);
                 this.trigger("model", {
                     nodes: a,
                     parent: r
                 }), r !== E.jstree.root ? (this._node_changed(r), this.redraw()) : (this.get_container_ul().children(".jstree-initial-node").remove(), this.redraw(!0)), this._data.core.selected.length !== e && this.trigger("changed", {
                     action: "model",
                     selected: this._data.core.selected
                 }), i.call(this, !0)
             },
-            _append_json_data: function(e, t, o, i) {
+            _append_json_data: function(e, t, d, i) {
                 if (null !== this.element) {
                     (e = this.get_node(e)).children = [], e.children_d = [], t.d && "string" == typeof(t = t.d) && (t = JSON.parse(t)), E.vakata.is_array(t) || (t = [t]);
                     var r = null,
                         s = {
                             df: this._model.default_state,
                             dat: t,
                             par: e.id,
@@ -675,18 +676,18 @@
                                 l = [],
                                 h = e.df,
                                 _ = e.t_id,
                                 g = e.t_cnt,
                                 u = e.m,
                                 a = u[i],
                                 e = e.sel,
-                                n, d, o, f, p = function(e, t, i) {
+                                n, o, d, f, p = function(e, t, i) {
                                     i = i ? i.concat() : [], t && i.unshift(t);
                                     var r = e.id.toString(),
-                                        s, a, n, d, o = {
+                                        s, a, n, o, d = {
                                             id: r,
                                             text: e.text || "",
                                             icon: e.icon === c || e.icon,
                                             parent: t,
                                             parents: i,
                                             children: e.children || [],
                                             children_d: e.children_d || [],
@@ -696,34 +697,34 @@
                                                 id: !1
                                             },
                                             a_attr: {
                                                 href: "#"
                                             },
                                             original: !1
                                         };
-                                    for (s in h) h.hasOwnProperty(s) && (o.state[s] = h[s]);
-                                    if (e && e.data && e.data.jstree && e.data.jstree.icon && (o.icon = e.data.jstree.icon), o.icon !== c && null !== o.icon && "" !== o.icon || (o.icon = !0), e && e.data && (o.data = e.data, e.data.jstree))
-                                        for (s in e.data.jstree) e.data.jstree.hasOwnProperty(s) && (o.state[s] = e.data.jstree[s]);
+                                    for (s in h) h.hasOwnProperty(s) && (d.state[s] = h[s]);
+                                    if (e && e.data && e.data.jstree && e.data.jstree.icon && (d.icon = e.data.jstree.icon), d.icon !== c && null !== d.icon && "" !== d.icon || (d.icon = !0), e && e.data && (d.data = e.data, e.data.jstree))
+                                        for (s in e.data.jstree) e.data.jstree.hasOwnProperty(s) && (d.state[s] = e.data.jstree[s]);
                                     if (e && "object" == typeof e.state)
-                                        for (s in e.state) e.state.hasOwnProperty(s) && (o.state[s] = e.state[s]);
+                                        for (s in e.state) e.state.hasOwnProperty(s) && (d.state[s] = e.state[s]);
                                     if (e && "object" == typeof e.li_attr)
-                                        for (s in e.li_attr) e.li_attr.hasOwnProperty(s) && (o.li_attr[s] = e.li_attr[s]);
-                                    if (o.li_attr.id || (o.li_attr.id = r), e && "object" == typeof e.a_attr)
-                                        for (s in e.a_attr) e.a_attr.hasOwnProperty(s) && (o.a_attr[s] = e.a_attr[s]);
-                                    for (e && e.children && !0 === e.children && (o.state.loaded = !1, o.children = [], o.children_d = []), s = 0, a = (u[o.id] = o).children.length; s < a; s++) n = p(u[o.children[s]], o.id, i), d = u[n], o.children_d.push(n), d.children_d.length && (o.children_d = o.children_d.concat(d.children_d));
-                                    return delete e.data, delete e.children, u[o.id].original = e, o.state.selected && l.push(o.id), o.id
+                                        for (s in e.li_attr) e.li_attr.hasOwnProperty(s) && (d.li_attr[s] = e.li_attr[s]);
+                                    if (d.li_attr.id || (d.li_attr.id = r), e && "object" == typeof e.a_attr)
+                                        for (s in e.a_attr) e.a_attr.hasOwnProperty(s) && (d.a_attr[s] = e.a_attr[s]);
+                                    for (e && e.children && !0 === e.children && (d.state.loaded = !1, d.children = [], d.children_d = []), s = 0, a = (u[d.id] = d).children.length; s < a; s++) n = p(u[d.children[s]], d.id, i), o = u[n], d.children_d.push(n), o.children_d.length && (d.children_d = d.children_d.concat(o.children_d));
+                                    return delete e.data, delete e.children, u[d.id].original = e, d.state.selected && l.push(d.id), d.id
                                 },
                                 m = function(e, t, i) {
                                     i = i ? i.concat() : [], t && i.unshift(t);
                                     var r = !1,
-                                        s, a, n, d, o;
+                                        s, a, n, o, d;
                                     do {
                                         r = "j" + _ + "_" + ++g
                                     } while (u[r]);
-                                    for (s in o = {
+                                    for (s in d = {
                                             id: !1,
                                             text: "string" == typeof e ? e : "",
                                             icon: "object" != typeof e || e.icon === c || e.icon,
                                             parent: t,
                                             parents: i,
                                             children: [],
                                             children_d: [],
@@ -732,54 +733,54 @@
                                             li_attr: {
                                                 id: !1
                                             },
                                             a_attr: {
                                                 href: "#"
                                             },
                                             original: !1
-                                        }, h) h.hasOwnProperty(s) && (o.state[s] = h[s]);
-                                    if (e && (e.id || 0 === e.id) && (o.id = e.id.toString()), e && e.text && (o.text = e.text), e && e.data && e.data.jstree && e.data.jstree.icon && (o.icon = e.data.jstree.icon), o.icon !== c && null !== o.icon && "" !== o.icon || (o.icon = !0), e && e.data && (o.data = e.data, e.data.jstree))
-                                        for (s in e.data.jstree) e.data.jstree.hasOwnProperty(s) && (o.state[s] = e.data.jstree[s]);
+                                        }, h) h.hasOwnProperty(s) && (d.state[s] = h[s]);
+                                    if (e && (e.id || 0 === e.id) && (d.id = e.id.toString()), e && e.text && (d.text = e.text), e && e.data && e.data.jstree && e.data.jstree.icon && (d.icon = e.data.jstree.icon), d.icon !== c && null !== d.icon && "" !== d.icon || (d.icon = !0), e && e.data && (d.data = e.data, e.data.jstree))
+                                        for (s in e.data.jstree) e.data.jstree.hasOwnProperty(s) && (d.state[s] = e.data.jstree[s]);
                                     if (e && "object" == typeof e.state)
-                                        for (s in e.state) e.state.hasOwnProperty(s) && (o.state[s] = e.state[s]);
+                                        for (s in e.state) e.state.hasOwnProperty(s) && (d.state[s] = e.state[s]);
                                     if (e && "object" == typeof e.li_attr)
-                                        for (s in e.li_attr) e.li_attr.hasOwnProperty(s) && (o.li_attr[s] = e.li_attr[s]);
-                                    if (o.li_attr.id && !o.id && 0 !== o.id && (o.id = o.li_attr.id.toString()), o.id || 0 === o.id || (o.id = r), o.li_attr.id || (o.li_attr.id = o.id), e && "object" == typeof e.a_attr)
-                                        for (s in e.a_attr) e.a_attr.hasOwnProperty(s) && (o.a_attr[s] = e.a_attr[s]);
+                                        for (s in e.li_attr) e.li_attr.hasOwnProperty(s) && (d.li_attr[s] = e.li_attr[s]);
+                                    if (d.li_attr.id && !d.id && 0 !== d.id && (d.id = d.li_attr.id.toString()), d.id || 0 === d.id || (d.id = r), d.li_attr.id || (d.li_attr.id = d.id), e && "object" == typeof e.a_attr)
+                                        for (s in e.a_attr) e.a_attr.hasOwnProperty(s) && (d.a_attr[s] = e.a_attr[s]);
                                     if (e && e.children && e.children.length) {
-                                        for (s = 0, a = e.children.length; s < a; s++) n = m(e.children[s], o.id, i), d = u[n], o.children.push(n), d.children_d.length && (o.children_d = o.children_d.concat(d.children_d));
-                                        o.children_d = o.children_d.concat(o.children)
+                                        for (s = 0, a = e.children.length; s < a; s++) n = m(e.children[s], d.id, i), o = u[n], d.children.push(n), o.children_d.length && (d.children_d = d.children_d.concat(o.children_d));
+                                        d.children_d = d.children_d.concat(d.children)
                                     }
-                                    return e && e.children && !0 === e.children && (o.state.loaded = !1, o.children = [], o.children_d = []), delete e.data, delete e.children, o.original = e, (u[o.id] = o).state.selected && l.push(o.id), o.id
+                                    return e && e.children && !0 === e.children && (d.state.loaded = !1, d.children = [], d.children_d = []), delete e.data, delete e.children, d.original = e, (u[d.id] = d).state.selected && l.push(d.id), d.id
                                 };
                             if (t.length && t[0].id !== c && t[0].parent !== c) {
-                                for (d = 0, o = t.length; d < o; d++) t[d].children || (t[d].children = []), t[d].state || (t[d].state = {}), u[t[d].id.toString()] = t[d];
-                                for (d = 0, o = t.length; d < o; d++) u[t[d].parent.toString()] ? (u[t[d].parent.toString()].children.push(t[d].id.toString()), a.children_d.push(t[d].id.toString())) : void 0 !== v && (v._data.core.last_error = {
+                                for (o = 0, d = t.length; o < d; o++) t[o].children || (t[o].children = []), t[o].state || (t[o].state = {}), u[t[o].id.toString()] = t[o];
+                                for (o = 0, d = t.length; o < d; o++) u[t[o].parent.toString()] ? (u[t[o].parent.toString()].children.push(t[o].id.toString()), a.children_d.push(t[o].id.toString())) : void 0 !== v && (v._data.core.last_error = {
                                     error: "parse",
                                     plugin: "core",
                                     id: "core_07",
                                     reason: "Node with invalid parent",
                                     data: JSON.stringify({
-                                        id: t[d].id.toString(),
-                                        parent: t[d].parent.toString()
+                                        id: t[o].id.toString(),
+                                        parent: t[o].parent.toString()
                                     })
                                 }, v.settings.core.error.call(v, v._data.core.last_error));
-                                for (d = 0, o = a.children.length; d < o; d++) n = p(u[a.children[d]], i, a.parents.concat()), s.push(n), u[n].children_d.length && (s = s.concat(u[n].children_d));
-                                for (d = 0, o = a.parents.length; d < o; d++) u[a.parents[d]].children_d = u[a.parents[d]].children_d.concat(s);
+                                for (o = 0, d = a.children.length; o < d; o++) n = p(u[a.children[o]], i, a.parents.concat()), s.push(n), u[n].children_d.length && (s = s.concat(u[n].children_d));
+                                for (o = 0, d = a.parents.length; o < d; o++) u[a.parents[o]].children_d = u[a.parents[o]].children_d.concat(s);
                                 f = {
                                     cnt: g,
                                     mod: u,
                                     sel: e,
                                     par: i,
                                     dpc: s,
                                     add: l
                                 }
                             } else {
-                                for (d = 0, o = t.length; d < o; d++)(n = m(t[d], i, a.parents.concat())) && (r.push(n), s.push(n), u[n].children_d.length && (s = s.concat(u[n].children_d)));
-                                for (a.children = r, a.children_d = s, d = 0, o = a.parents.length; d < o; d++) u[a.parents[d]].children_d = u[a.parents[d]].children_d.concat(s);
+                                for (o = 0, d = t.length; o < d; o++)(n = m(t[o], i, a.parents.concat())) && (r.push(n), s.push(n), u[n].children_d.length && (s = s.concat(u[n].children_d)));
+                                for (a.children = r, a.children_d = s, o = 0, d = a.parents.length; o < d; o++) u[a.parents[o]].children_d = u[a.parents[o]].children_d.concat(s);
                                 f = {
                                     cnt: g,
                                     mod: u,
                                     sel: e,
                                     par: i,
                                     dpc: s,
                                     add: l
@@ -791,44 +792,44 @@
                         n = function(e, t) {
                             if (null !== this.element) {
                                 var i, r;
                                 for (i in this._cnt = e.cnt, r = this._model.data) r.hasOwnProperty(i) && r[i].state && r[i].state.loading && e.mod[i] && (e.mod[i].state.loading = !0);
                                 if (this._model.data = e.mod, t) {
                                     var s, a = e.add,
                                         n = e.sel,
-                                        d = this._data.core.selected.slice(),
+                                        o = this._data.core.selected.slice(),
                                         r = this._model.data;
-                                    if (n.length !== d.length || E.vakata.array_unique(n.concat(d)).length !== n.length) {
-                                        for (i = 0, s = n.length; i < s; i++) - 1 === E.inArray(n[i], a) && -1 === E.inArray(n[i], d) && (r[n[i]].state.selected = !1);
-                                        for (i = 0, s = d.length; i < s; i++) - 1 === E.inArray(d[i], n) && (r[d[i]].state.selected = !0)
+                                    if (n.length !== o.length || E.vakata.array_unique(n.concat(o)).length !== n.length) {
+                                        for (i = 0, s = n.length; i < s; i++) - 1 === E.inArray(n[i], a) && -1 === E.inArray(n[i], o) && (r[n[i]].state.selected = !1);
+                                        for (i = 0, s = o.length; i < s; i++) - 1 === E.inArray(o[i], n) && (r[o[i]].state.selected = !0)
                                     }
                                 }
                                 e.add.length && (this._data.core.selected = this._data.core.selected.concat(e.add)), this.trigger("model", {
                                     nodes: e.dpc,
                                     parent: e.par
                                 }), e.par !== E.jstree.root ? (this._node_changed(e.par), this.redraw()) : this.redraw(!0), e.add.length && this.trigger("changed", {
                                     action: "model",
                                     selected: this._data.core.selected
                                 }), !t && c ? c(function() {
-                                    o.call(v, !0)
-                                }) : o.call(v, !0)
+                                    d.call(v, !0)
+                                }) : d.call(v, !0)
                             }
                         };
                     if (this.settings.core.worker && window.Blob && window.URL && window.Worker) try {
                         null === this._wrk && (this._wrk = window.URL.createObjectURL(new window.Blob(["self.onmessage = " + a.toString()], {
                             type: "text/javascript"
                         }))), !this._data.core.working || i ? (this._data.core.working = !0, (r = new window.Worker(this._wrk)).onmessage = function(e) {
                             n.call(this, e.data, !0);
                             try {
                                 r.terminate(), r = null
                             } catch (e) {}
                             this._data.core.worker_queue.length ? this._append_json_data.apply(this, this._data.core.worker_queue.shift()) : this._data.core.working = !1
                         }.bind(this), r.onerror = function(e) {
                             n.call(this, a(s), !1), this._data.core.worker_queue.length ? this._append_json_data.apply(this, this._data.core.worker_queue.shift()) : this._data.core.working = !1
-                        }.bind(this), s.par ? r.postMessage(s) : this._data.core.worker_queue.length ? this._append_json_data.apply(this, this._data.core.worker_queue.shift()) : this._data.core.working = !1) : this._data.core.worker_queue.push([e, t, o, !0])
+                        }.bind(this), s.par ? r.postMessage(s) : this._data.core.worker_queue.length ? this._append_json_data.apply(this, this._data.core.worker_queue.shift()) : this._data.core.working = !1) : this._data.core.worker_queue.push([e, t, d, !0])
                     } catch (e) {
                         n.call(this, a(s), !1), this._data.core.worker_queue.length ? this._append_json_data.apply(this, this._data.core.worker_queue.shift()) : this._data.core.working = !1
                     } else n.call(this, a(s), !1)
                 }
             },
             _parse_model_from_html: function(e, t, i) {
                 i = i ? [].concat(i) : [], t && i.unshift(t);
@@ -847,36 +848,36 @@
                             id: !1
                         },
                         a_attr: {
                             href: "#"
                         },
                         original: !1
                     },
-                    d, t, o;
-                for (d in this._model.default_state) this._model.default_state.hasOwnProperty(d) && (n.state[d] = this._model.default_state[d]);
+                    o, t, d;
+                for (o in this._model.default_state) this._model.default_state.hasOwnProperty(o) && (n.state[o] = this._model.default_state[o]);
                 if (t = E.vakata.attributes(e, !0), E.each(t, function(e, t) {
                         return !(t = E.vakata.trim(t)).length || (n.li_attr[e] = t, void("id" === e && (n.id = t.toString())))
                     }), (t = e.children("a").first()).length && (t = E.vakata.attributes(t, !0), E.each(t, function(e, t) {
                         (t = E.vakata.trim(t)).length && (n.a_attr[e] = t)
                     })), (t = (e.children("a").first().length ? e.children("a").first() : e).clone()).children("ins, i, ul").remove(), t = t.html(), t = E("<div></div>").html(t), n.text = this.settings.core.force_text ? t.text() : t.html(), t = e.data(), n.data = t ? E.extend(!0, {}, t) : null, n.state.opened = e.hasClass("jstree-open"), n.state.selected = e.children("a").hasClass("jstree-clicked"), n.state.disabled = e.children("a").hasClass("jstree-disabled"), n.data && n.data.jstree)
-                    for (d in n.data.jstree) n.data.jstree.hasOwnProperty(d) && (n.state[d] = n.data.jstree[d]);
+                    for (o in n.data.jstree) n.data.jstree.hasOwnProperty(o) && (n.state[o] = n.data.jstree[o]);
                 (t = e.children("a").children(".jstree-themeicon")).length && (n.icon = !t.hasClass("jstree-themeicon-hidden") && t.attr("rel")), n.state.icon !== P && (n.icon = n.state.icon), n.icon !== P && null !== n.icon && "" !== n.icon || (n.icon = !0), t = e.children("ul").children("li");
                 do {
-                    o = "j" + this._id + "_" + ++this._cnt
-                } while (a[o]);
-                return n.id = n.li_attr.id ? n.li_attr.id.toString() : o, t.length ? (t.each(function(e, t) {
+                    d = "j" + this._id + "_" + ++this._cnt
+                } while (a[d]);
+                return n.id = n.li_attr.id ? n.li_attr.id.toString() : d, t.length ? (t.each(function(e, t) {
                     r = this._parse_model_from_html(E(t), n.id, i), s = this._model.data[r], n.children.push(r), s.children_d.length && (n.children_d = n.children_d.concat(s.children_d))
                 }.bind(this)), n.children_d = n.children_d.concat(n.children)) : e.hasClass("jstree-closed") && (n.state.loaded = !1), n.li_attr.class && (n.li_attr.class = n.li_attr.class.replace("jstree-closed", "").replace("jstree-open", "")), n.a_attr.class && (n.a_attr.class = n.a_attr.class.replace("jstree-clicked", "").replace("jstree-disabled", "")), (a[n.id] = n).state.selected && this._data.core.selected.push(n.id), n.id
             },
             _parse_model_from_flat_json: function(e, t, i) {
                 i = i ? i.concat() : [], t && i.unshift(t);
                 var r = e.id.toString(),
                     s = this._model.data,
                     a = this._model.default_state,
-                    n, d, o, c, l = {
+                    n, o, d, c, l = {
                         id: r,
                         text: e.text || "",
                         icon: e.icon === P || e.icon,
                         parent: t,
                         parents: i,
                         children: e.children || [],
                         children_d: e.children_d || [],
@@ -895,26 +896,26 @@
                     for (n in e.data.jstree) e.data.jstree.hasOwnProperty(n) && (l.state[n] = e.data.jstree[n]);
                 if (e && "object" == typeof e.state)
                     for (n in e.state) e.state.hasOwnProperty(n) && (l.state[n] = e.state[n]);
                 if (e && "object" == typeof e.li_attr)
                     for (n in e.li_attr) e.li_attr.hasOwnProperty(n) && (l.li_attr[n] = e.li_attr[n]);
                 if (l.li_attr.id || (l.li_attr.id = r), e && "object" == typeof e.a_attr)
                     for (n in e.a_attr) e.a_attr.hasOwnProperty(n) && (l.a_attr[n] = e.a_attr[n]);
-                for (e && e.children && !0 === e.children && (l.state.loaded = !1, l.children = [], l.children_d = []), n = 0, d = (s[l.id] = l).children.length; n < d; n++) c = s[o = this._parse_model_from_flat_json(s[l.children[n]], l.id, i)], l.children_d.push(o), c.children_d.length && (l.children_d = l.children_d.concat(c.children_d));
+                for (e && e.children && !0 === e.children && (l.state.loaded = !1, l.children = [], l.children_d = []), n = 0, o = (s[l.id] = l).children.length; n < o; n++) c = s[d = this._parse_model_from_flat_json(s[l.children[n]], l.id, i)], l.children_d.push(d), c.children_d.length && (l.children_d = l.children_d.concat(c.children_d));
                 return delete e.data, delete e.children, s[l.id].original = e, l.state.selected && this._data.core.selected.push(l.id), l.id
             },
             _parse_model_from_json: function(e, t, i) {
                 i = i ? i.concat() : [], t && i.unshift(t);
                 var r = !1,
-                    s, a, n, d, o = this._model.data,
+                    s, a, n, o, d = this._model.data,
                     c = this._model.default_state,
                     l;
                 do {
                     r = "j" + this._id + "_" + ++this._cnt
-                } while (o[r]);
+                } while (d[r]);
                 for (s in l = {
                         id: !1,
                         text: "string" == typeof e ? e : "",
                         icon: "object" != typeof e || e.icon === P || e.icon,
                         parent: t,
                         parents: i,
                         children: [],
@@ -934,18 +935,18 @@
                 if (e && "object" == typeof e.state)
                     for (s in e.state) e.state.hasOwnProperty(s) && (l.state[s] = e.state[s]);
                 if (e && "object" == typeof e.li_attr)
                     for (s in e.li_attr) e.li_attr.hasOwnProperty(s) && (l.li_attr[s] = e.li_attr[s]);
                 if (l.li_attr.id && !l.id && 0 !== l.id && (l.id = l.li_attr.id.toString()), l.id || 0 === l.id || (l.id = r), l.li_attr.id || (l.li_attr.id = l.id), e && "object" == typeof e.a_attr)
                     for (s in e.a_attr) e.a_attr.hasOwnProperty(s) && (l.a_attr[s] = e.a_attr[s]);
                 if (e && e.children && e.children.length) {
-                    for (s = 0, a = e.children.length; s < a; s++) d = o[n = this._parse_model_from_json(e.children[s], l.id, i)], l.children.push(n), d.children_d.length && (l.children_d = l.children_d.concat(d.children_d));
+                    for (s = 0, a = e.children.length; s < a; s++) o = d[n = this._parse_model_from_json(e.children[s], l.id, i)], l.children.push(n), o.children_d.length && (l.children_d = l.children_d.concat(o.children_d));
                     l.children_d = l.children.concat(l.children_d)
                 }
-                return e && e.children && !0 === e.children && (l.state.loaded = !1, l.children = [], l.children_d = []), delete e.data, delete e.children, l.original = e, (o[l.id] = l).state.selected && this._data.core.selected.push(l.id), l.id
+                return e && e.children && !0 === e.children && (l.state.loaded = !1, l.children = [], l.children_d = []), delete e.data, delete e.children, l.original = e, (d[l.id] = l).state.selected && this._data.core.selected.push(l.id), l.id
             },
             _redraw: function() {
                 for (var e = (this._model.force_full_redraw ? this._model.data[E.jstree.root].children : this._model.changed).concat([]), t = b.createElement("UL"), i, r, s, a = this._data.core.focused, r = 0, s = e.length; r < s; r++)(i = this.redraw_node(e[r], !0, this._model.force_full_redraw)) && this._model.force_full_redraw && t.appendChild(i);
                 this._model.force_full_redraw && (t.className = this.get_container_ul()[0].className, t.setAttribute("role", "presentation"), this.element.empty().append(t)), null !== a && this.settings.core.restore_focus && ((i = this.get_node(a, !0)) && i.length && i.children(".jstree-anchor")[0] !== b.activeElement ? i.children(".jstree-anchor").trigger("focus") : this._data.core.focused = null), this._model.force_full_redraw = !1, this._model.changed = [], this.trigger("redraw", {
                     nodes: e
                 })
             },
@@ -966,52 +967,52 @@
                     e.appendChild(s)
                 }
             },
             redraw_node: function(e, t, i, r) {
                 var s = this.get_node(e),
                     a = !1,
                     n = !1,
-                    d = !1,
                     o = !1,
+                    d = !1,
                     c = !1,
                     l = !1,
                     h = "",
                     _ = b,
                     g = this._model.data,
                     u = !1,
                     f = !1,
                     p = null,
                     m = 0,
                     v = 0,
                     j = !1,
                     k = !1;
                 if (!s) return !1;
                 if (s.id === E.jstree.root) return this.redraw(!0);
-                if (t = t || 0 === s.children.length, e = b.querySelector ? this.element[0].querySelector("#" + (-1 !== "0123456789".indexOf(s.id[0]) ? "\\3" + s.id[0] + " " + s.id.substr(1).replace(E.jstree.idregex, "\\$&") : s.id.replace(E.jstree.idregex, "\\$&"))) : b.getElementById(s.id)) e = E(e), i || ((a = e.parent().parent()[0]) === this.element[0] && (a = null), n = e.index()), (t = !t && s.children.length && !e.children(".jstree-children").length ? !0 : t) || (d = e.children(".jstree-children")[0]), u = e.children(".jstree-anchor")[0] === b.activeElement, e.remove();
+                if (t = t || 0 === s.children.length, e = b.querySelector ? this.element[0].querySelector("#" + (-1 !== "0123456789".indexOf(s.id[0]) ? "\\3" + s.id[0] + " " + s.id.substr(1).replace(E.jstree.idregex, "\\$&") : s.id.replace(E.jstree.idregex, "\\$&"))) : b.getElementById(s.id)) e = E(e), i || ((a = e.parent().parent()[0]) === this.element[0] && (a = null), n = e.index()), (t = !t && s.children.length && !e.children(".jstree-children").length ? !0 : t) || (o = e.children(".jstree-children")[0]), u = e.children(".jstree-anchor")[0] === b.activeElement, e.remove();
                 else if (t = !0, !i) {
                     if (!(null === (a = s.parent !== E.jstree.root ? E("#" + s.parent.replace(E.jstree.idregex, "\\$&"), this.element)[0] : null) || a && g[s.parent].state.opened)) return !1;
                     n = E.inArray(s.id, (null === a ? g[E.jstree.root] : g[s.parent]).children)
                 }
-                for (o in e = this._data.core.node.cloneNode(!0), h = "jstree-node ", s.li_attr) s.li_attr.hasOwnProperty(o) && "id" !== o && ("class" !== o ? e.setAttribute(o, s.li_attr[o]) : h += s.li_attr[o]);
-                for (s.a_attr.id || (s.a_attr.id = s.id + "_anchor"), e.childNodes[1].setAttribute("aria-selected", !!s.state.selected), e.childNodes[1].setAttribute("aria-level", s.parents.length), this.settings.core.compute_elements_positions && (e.childNodes[1].setAttribute("aria-setsize", g[s.parent].children.length), e.childNodes[1].setAttribute("aria-posinset", g[s.parent].children.indexOf(s.id) + 1)), s.state.disabled && e.childNodes[1].setAttribute("aria-disabled", !0), o = 0, c = s.children.length; o < c; o++)
-                    if (!g[s.children[o]].state.hidden) {
+                for (d in e = this._data.core.node.cloneNode(!0), h = "jstree-node ", s.li_attr) s.li_attr.hasOwnProperty(d) && "id" !== d && ("class" !== d ? e.setAttribute(d, s.li_attr[d]) : h += s.li_attr[d]);
+                for (s.a_attr.id || (s.a_attr.id = s.id + "_anchor"), e.childNodes[1].setAttribute("aria-selected", !!s.state.selected), e.childNodes[1].setAttribute("aria-level", s.parents.length), this.settings.core.compute_elements_positions && (e.childNodes[1].setAttribute("aria-setsize", g[s.parent].children.length), e.childNodes[1].setAttribute("aria-posinset", g[s.parent].children.indexOf(s.id) + 1)), s.state.disabled && e.childNodes[1].setAttribute("aria-disabled", !0), d = 0, c = s.children.length; d < c; d++)
+                    if (!g[s.children[d]].state.hidden) {
                         j = !0;
                         break
-                    } if (null !== s.parent && g[s.parent] && !s.state.hidden && (o = E.inArray(s.id, g[s.parent].children), k = s.id, -1 !== o))
-                    for (o++, c = g[s.parent].children.length; o < c; o++)
-                        if ((k = !g[g[s.parent].children[o]].state.hidden ? g[s.parent].children[o] : k) !== s.id) break;
+                    } if (null !== s.parent && g[s.parent] && !s.state.hidden && (d = E.inArray(s.id, g[s.parent].children), k = s.id, -1 !== d))
+                    for (d++, c = g[s.parent].children.length; d < c; d++)
+                        if ((k = !g[g[s.parent].children[d]].state.hidden ? g[s.parent].children[d] : k) !== s.id) break;
                 for (c in s.state.hidden && (h += " jstree-hidden"), s.state.loading && (h += " jstree-loading"), s.state.loaded && !j ? h += " jstree-leaf" : (h += s.state.opened && s.state.loaded ? " jstree-open" : " jstree-closed", e.childNodes[1].setAttribute("aria-expanded", s.state.opened && s.state.loaded)), k === s.id && (h += " jstree-last"), e.id = s.id, e.className = h, h = (s.state.selected ? " jstree-clicked" : "") + (s.state.disabled ? " jstree-disabled" : ""), s.a_attr) s.a_attr.hasOwnProperty(c) && ("href" === c && "#" === s.a_attr[c] || ("class" !== c ? e.childNodes[1].setAttribute(c, s.a_attr[c]) : h += " " + s.a_attr[c]));
                 if (h.length && (e.childNodes[1].className = "jstree-anchor " + h), (s.icon && !0 !== s.icon || !1 === s.icon) && (!1 === s.icon ? e.childNodes[1].childNodes[0].className += " jstree-themeicon-hidden" : -1 === s.icon.indexOf("/") && -1 === s.icon.indexOf(".") ? e.childNodes[1].childNodes[0].className += " " + s.icon + " jstree-themeicon-custom" : (e.childNodes[1].childNodes[0].style.backgroundImage = 'url("' + s.icon + '")', e.childNodes[1].childNodes[0].style.backgroundPosition = "center center", e.childNodes[1].childNodes[0].style.backgroundSize = "auto", e.childNodes[1].childNodes[0].className += " jstree-themeicon-custom")), this.settings.core.force_text ? e.childNodes[1].appendChild(_.createTextNode(s.text)) : e.childNodes[1].innerHTML += s.text, t && s.children.length && (s.state.opened || r) && s.state.loaded) {
-                    for ((l = _.createElement("UL")).setAttribute("role", "group"), l.className = "jstree-children", o = 0, c = s.children.length; o < c; o++) l.appendChild(this.redraw_node(s.children[o], t, !0));
+                    for ((l = _.createElement("UL")).setAttribute("role", "group"), l.className = "jstree-children", d = 0, c = s.children.length; d < c; d++) l.appendChild(this.redraw_node(s.children[d], t, !0));
                     e.appendChild(l)
                 }
-                if (d && e.appendChild(d), !i) {
-                    for (o = 0, c = (a = a || this.element[0]).childNodes.length; o < c; o++)
-                        if (a.childNodes[o] && a.childNodes[o].className && -1 !== a.childNodes[o].className.indexOf("jstree-children")) {
-                            p = a.childNodes[o];
+                if (o && e.appendChild(o), !i) {
+                    for (d = 0, c = (a = a || this.element[0]).childNodes.length; d < c; d++)
+                        if (a.childNodes[d] && a.childNodes[d].className && -1 !== a.childNodes[d].className.indexOf("jstree-children")) {
+                            p = a.childNodes[d];
                             break
                         } p || ((p = _.createElement("UL")).setAttribute("role", "group"), p.className = "jstree-children", a.appendChild(p)), n < (a = p).childNodes.length ? a.insertBefore(e, a.childNodes[n]) : a.appendChild(e), u && (m = this.element[0].scrollTop, v = this.element[0].scrollLeft, e.childNodes[1].focus(), this.element[0].scrollTop = m, this.element[0].scrollLeft = v)
                 }
                 return s.state.opened && !s.state.loaded && (s.state.opened = !1, setTimeout(function() {
                     this.open_node(s.id, !1, 0)
                 }.bind(this), 0)), e
             },
@@ -1168,23 +1169,23 @@
                     nodes: r
                 }), r
             },
             activate_node: function(e, t) {
                 if (this.is_disabled(e)) return !1;
                 if (t && "object" == typeof t || (t = {}), this._data.core.last_clicked = this._data.core.last_clicked && this._data.core.last_clicked.id !== P ? this.get_node(this._data.core.last_clicked.id) : null, this._data.core.last_clicked && !this._data.core.last_clicked.state.selected && (this._data.core.last_clicked = null), !this._data.core.last_clicked && this._data.core.selected.length && (this._data.core.last_clicked = this.get_node(this._data.core.selected[this._data.core.selected.length - 1])), this.settings.core.multiple && (t.metaKey || t.ctrlKey || t.shiftKey) && (!t.shiftKey || this._data.core.last_clicked && this.get_parent(e) && this.get_parent(e) === this._data.core.last_clicked.parent))
                     if (t.shiftKey) {
-                        for (var i = this.get_node(e).id, r = this._data.core.last_clicked.id, s = this.get_node(this._data.core.last_clicked.parent).children, a = !1, n, d, n = 0, d = s.length; n < d; n += 1) s[n] === i && (a = !a), s[n] === r && (a = !a), this.is_disabled(s[n]) || !a && s[n] !== i && s[n] !== r ? t.ctrlKey || this.deselect_node(s[n], !0, t) : this.is_hidden(s[n]) || this.select_node(s[n], !0, !1, t);
+                        for (var i = this.get_node(e).id, r = this._data.core.last_clicked.id, s = this.get_node(this._data.core.last_clicked.parent).children, a = !1, n, o, n = 0, o = s.length; n < o; n += 1) s[n] === i && (a = !a), s[n] === r && (a = !a), this.is_disabled(s[n]) || !a && s[n] !== i && s[n] !== r ? t.ctrlKey || this.deselect_node(s[n], !0, t) : this.is_hidden(s[n]) || this.select_node(s[n], !0, !1, t);
                         this.trigger("changed", {
                             action: "select_node",
                             node: this.get_node(e),
                             selected: this._data.core.selected,
                             event: t
                         })
                     } else this.is_selected(e) ? this.deselect_node(e, !1, t) : (t.ctrlKey && (this._data.core.last_clicked = this.get_node(e)), this.select_node(e, !1, !1, t));
-                else !this.settings.core.multiple && (t.metaKey || t.ctrlKey || t.shiftKey) && this.is_selected(e) ? this.deselect_node(e, !1, t) : (this.is_selected(e) && 1 === this._data.core.selected.length || (this.deselect_all(!0), this.select_node(e, !1, !1, t)), this._data.core.last_clicked = this.get_node(e));
+                else !this.settings.core.multiple && (t.metaKey || t.ctrlKey || t.shiftKey) && this.is_selected(e) ? this.deselect_node(e, !1, t) : (!this.settings.core.allow_reselect && this.is_selected(e) && 1 === this._data.core.selected.length || (this.deselect_all(!0), this.select_node(e, !1, !1, t)), this._data.core.last_clicked = this.get_node(e));
                 this.trigger("activate_node", {
                     node: this.get_node(e),
                     event: t
                 })
             },
             hover_node: function(e) {
                 if (!(e = this.get_node(e, !0)) || !e.length || e.children(".jstree-hovered").length) return !1;
@@ -1199,15 +1200,15 @@
             dehover_node: function(e) {
                 if (!(e = this.get_node(e, !0)) || !e.length || !e.children(".jstree-hovered").length) return !1;
                 e.children(".jstree-anchor").removeClass("jstree-hovered"), this.trigger("dehover_node", {
                     node: this.get_node(e)
                 })
             },
             select_node: function(e, t, i, r) {
-                var s, a, n, d;
+                var s, a, n, o;
                 if (E.vakata.is_array(e)) {
                     for (a = 0, n = (e = e.slice()).length; a < n; a++) this.select_node(e[a], t, i, r);
                     return !0
                 }
                 if (!(e = this.get_node(e)) || e.id === E.jstree.root) return !1;
                 s = this.get_node(e, !0), e.state.selected || (e.state.selected = !0, this._data.core.selected.push(e.id), (s = !i ? this._open_to(e) : s) && s.length && s.children(".jstree-anchor").addClass("jstree-clicked").attr("aria-selected", !0), this.trigger("select_node", {
                     node: e,
@@ -1401,15 +1402,15 @@
                 return t && t.flat ? i : e.id === E.jstree.root ? r.children : r
             },
             create_node: function(e, t, i, r, s) {
                 if (null === e && (e = E.jstree.root), !(e = this.get_node(e))) return !1;
                 if (!(i = i === P ? "last" : i).toString().match(/^(before|after)$/) && !s && !this.is_loaded(e)) return this.load_node(e, function() {
                     this.create_node(e, t, i, r, !0)
                 });
-                var a, n, d, o;
+                var a, n, o, d;
                 switch ((t = "string" == typeof(t = t || {
                         text: this.get_string("New node")
                     }) ? {
                         text: t
                     } : E.extend(!0, {}, t)).text === P && (t.text = this.get_string("New node")), i = e.id === E.jstree.root && "after" === (i = "before" === i ? "first" : i) ? "last" : i) {
                     case "before":
                         a = this.get_node(e.parent), i = E.inArray(e.id, a.children), e = a;
@@ -1428,16 +1429,16 @@
                         i = i || 0
                 }
                 if (i > e.children.length && (i = e.children.length), t.id === P && (t.id = !0), !this.check("create_node", t, e, i)) return this.settings.core.error.call(this, this._data.core.last_error), !1;
                 if (!0 === t.id && delete t.id, !(t = this._parse_model_from_json(t, e.id, e.parents.concat()))) return !1;
                 for (a = this.get_node(t), (n = []).push(t), n = n.concat(a.children_d), this.trigger("model", {
                         nodes: n,
                         parent: e.id
-                    }), e.children_d = e.children_d.concat(n), d = 0, o = e.parents.length; d < o; d++) this._model.data[e.parents[d]].children_d = this._model.data[e.parents[d]].children_d.concat(n);
-                for (t = a, a = [], d = 0, o = e.children.length; d < o; d++) a[i <= d ? d + 1 : d] = e.children[d];
+                    }), e.children_d = e.children_d.concat(n), o = 0, d = e.parents.length; o < d; o++) this._model.data[e.parents[o]].children_d = this._model.data[e.parents[o]].children_d.concat(n);
+                for (t = a, a = [], o = 0, d = e.children.length; o < d; o++) a[i <= o ? o + 1 : o] = e.children[o];
                 return a[i] = t.id, e.children = a, this.redraw_node(e, !0), this.trigger("create_node", {
                     node: this.get_node(t),
                     parent: e.id,
                     position: i
                 }), r && r.call(this, this.get_node(t)), t.id
             },
             rename_node: function(e, t) {
@@ -1449,39 +1450,39 @@
                 return !(!(e = this.get_node(e)) || e.id === E.jstree.root) && (s = e.text, this.check("rename_node", e, this.get_parent(e), t) ? (this.set_text(e, t), this.trigger("rename_node", {
                     node: e,
                     text: t,
                     old: s
                 }), !0) : (this.settings.core.error.call(this, this._data.core.last_error), !1))
             },
             delete_node: function(e) {
-                var t, i, r, s, a, n, d, o, c, l, h, s;
+                var t, i, r, s, a, n, o, d, c, l, h, s;
                 if (E.vakata.is_array(e)) {
                     for (t = 0, i = (e = e.slice()).length; t < i; t++) this.delete_node(e[t]);
                     return !0
                 }
                 if (!(e = this.get_node(e)) || e.id === E.jstree.root) return !1;
                 if (r = this.get_node(e.parent), s = E.inArray(e.id, r.children), l = !1, !this.check("delete_node", e, r, s)) return this.settings.core.error.call(this, this._data.core.last_error), !1;
-                for (-1 !== s && (r.children = E.vakata.array_remove(r.children, s)), (a = e.children_d.concat([])).push(e.id), n = 0, d = e.parents.length; n < d; n++) this._model.data[e.parents[n]].children_d = E.vakata.array_filter(this._model.data[e.parents[n]].children_d, function(e) {
+                for (-1 !== s && (r.children = E.vakata.array_remove(r.children, s)), (a = e.children_d.concat([])).push(e.id), n = 0, o = e.parents.length; n < o; n++) this._model.data[e.parents[n]].children_d = E.vakata.array_filter(this._model.data[e.parents[n]].children_d, function(e) {
                     return -1 === E.inArray(e, a)
                 });
-                for (o = 0, c = a.length; o < c; o++)
-                    if (this._model.data[a[o]].state.selected) {
+                for (d = 0, c = a.length; d < c; d++)
+                    if (this._model.data[a[d]].state.selected) {
                         l = !0;
                         break
                     } for (l && (this._data.core.selected = E.vakata.array_filter(this._data.core.selected, function(e) {
                         return -1 === E.inArray(e, a)
                     })), this.trigger("delete_node", {
                         node: e,
                         parent: r.id
                     }), l && this.trigger("changed", {
                         action: "delete_node",
                         node: e,
                         selected: this._data.core.selected,
                         parent: r.id
-                    }), o = 0, c = a.length; o < c; o++) delete this._model.data[a[o]];
+                    }), d = 0, c = a.length; d < c; d++) delete this._model.data[a[d]];
                 return -1 !== E.inArray(this._data.core.focused, a) && (this._data.core.focused = null, h = this.element[0].scrollTop, s = this.element[0].scrollLeft, r.id === E.jstree.root ? this._model.data[E.jstree.root].children[0] && this.get_node(this._model.data[E.jstree.root].children[0], !0).children(".jstree-anchor").trigger("focus") : this.get_node(r, !0).children(".jstree-anchor").trigger("focus"), this.element[0].scrollTop = h, this.element[0].scrollLeft = s), this.redraw_node(r, !0), !0
             },
             check: function(e, t, i, r, s) {
                 t = t && t.id ? t : this.get_node(t), i = i && i.id ? i : this.get_node(i);
                 var a = e.match(/^(move_node|copy_node|create_node)$/i) ? i : t,
                     n = this.settings.core.check_callback;
                 if ("move_node" === e || "copy_node" === e) {
@@ -1534,22 +1535,22 @@
                     })
                 })
             },
             last_error: function() {
                 return this._data.core.last_error
             },
             move_node: function(e, t, i, r, s, a, n) {
-                var d, o, c, l, h, _, g, u, f, p, m, v, j, k;
+                var o, d, c, l, h, _, g, u, f, p, m, v, j, k;
                 if (t = this.get_node(t), i = i === P ? 0 : i, !t) return !1;
                 if (!i.toString().match(/^(before|after)$/) && !s && !this.is_loaded(t)) return this.load_node(t, function() {
                     this.move_node(e, t, i, r, !0, !1, n)
                 });
                 if (E.vakata.is_array(e)) {
                     if (1 !== e.length) {
-                        for (d = 0, o = e.length; d < o; d++)(f = this.move_node(e[d], t, i, r, s, !1, n)) && (t = f, i = "after");
+                        for (o = 0, d = e.length; o < d; o++)(f = this.move_node(e[o], t, i, r, s, !1, n)) && (t = f, i = "after");
                         return this.redraw(), !0
                     }
                     e = e[0]
                 }
                 if (!(e = e && e.id !== P ? e : this.get_node(e)) || e.id === E.jstree.root) return !1;
                 if (c = (e.parent || E.jstree.root).toString(), h = i.toString().match(/^(before|after)$/) && t.id !== E.jstree.root ? this.get_node(t.parent) : t, g = !(_ = n || (this._model.data[e.id] ? this : E.jstree.reference(e.id))) || !_._id || this._id !== _._id, l = _ && _._id && c && _._model.data[c] && _._model.data[c].children ? E.inArray(e.id, _._model.data[c].children) : -1, _ && _._id && (e = _._model.data[e.id]), g) return !!(f = this.copy_node(e, t, i, r, s, !1, n)) && (_ && _.delete_node(e), f);
                 switch (i = t.id === E.jstree.root && "after" === (i = "before" === i ? "first" : i) ? "last" : i) {
@@ -1597,22 +1598,22 @@
                     is_multi: _ && _._id && _._id !== this._id,
                     is_foreign: !_ || !_._id,
                     old_instance: _,
                     new_instance: this
                 }), e.id
             },
             copy_node: function(e, t, i, r, s, a, n) {
-                var d, o, c, l, h, _, g, u, f, p, m;
+                var o, d, c, l, h, _, g, u, f, p, m;
                 if (t = this.get_node(t), i = i === P ? 0 : i, !t) return !1;
                 if (!i.toString().match(/^(before|after)$/) && !s && !this.is_loaded(t)) return this.load_node(t, function() {
                     this.copy_node(e, t, i, r, !0, !1, n)
                 });
                 if (E.vakata.is_array(e)) {
                     if (1 !== e.length) {
-                        for (d = 0, o = e.length; d < o; d++)(l = this.copy_node(e[d], t, i, r, s, !0, n)) && (t = l, i = "after");
+                        for (o = 0, d = e.length; o < d; o++)(l = this.copy_node(e[o], t, i, r, s, !0, n)) && (t = l, i = "after");
                         return this.redraw(), !0
                     }
                     e = e[0]
                 }
                 if (!(e = e && e.id !== P ? e : this.get_node(e)) || e.id === E.jstree.root) return !1;
                 switch (u = (e.parent || E.jstree.root).toString(), f = i.toString().match(/^(before|after)$/) && t.id !== E.jstree.root ? this.get_node(t.parent) : t, m = !(p = n || (this._model.data[e.id] ? this : E.jstree.reference(e.id))) || !p._id || this._id !== p._id, p && p._id && (e = p._model.data[e.id]), i = t.id === E.jstree.root && "after" === (i = "before" === i ? "first" : i) ? "last" : i) {
                     case "before":
@@ -1661,58 +1662,58 @@
                     new_instance: this
                 }), l.id
             },
             cut: function(e) {
                 if (e = e || this._data.core.selected.concat(), !(e = !E.vakata.is_array(e) ? [e] : e).length) return !1;
                 for (var t = [], i, r, s, r = 0, s = e.length; r < s; r++)(i = this.get_node(e[r])) && (i.id || 0 === i.id) && i.id !== E.jstree.root && t.push(i);
                 if (!t.length) return !1;
-                a = t, n = "move_node", (d = this).trigger("cut", {
+                a = t, n = "move_node", (o = this).trigger("cut", {
                     node: e
                 })
             },
             copy: function(e) {
                 if (e = e || this._data.core.selected.concat(), !(e = !E.vakata.is_array(e) ? [e] : e).length) return !1;
                 for (var t = [], i, r, s, r = 0, s = e.length; r < s; r++)(i = this.get_node(e[r])) && i.id !== P && i.id !== E.jstree.root && t.push(i);
                 if (!t.length) return !1;
-                a = t, n = "copy_node", (d = this).trigger("copy", {
+                a = t, n = "copy_node", (o = this).trigger("copy", {
                     node: e
                 })
             },
             get_buffer: function() {
                 return {
                     mode: n,
                     node: a,
-                    inst: d
+                    inst: o
                 }
             },
             can_paste: function() {
                 return !1 !== n && !1 !== a
             },
             paste: function(e, t) {
                 if (!((e = this.get_node(e)) && n && n.match(/^(copy_node|move_node)$/) && a)) return !1;
-                this[n](a, e, t, !1, !1, !1, d) && this.trigger("paste", {
+                this[n](a, e, t, !1, !1, !1, o) && this.trigger("paste", {
                     parent: e.id,
                     node: a,
                     mode: n
-                }), d = n = a = !1
+                }), o = n = a = !1
             },
             clear_buffer: function() {
-                d = n = a = !1, this.trigger("clear_buffer")
+                o = n = a = !1, this.trigger("clear_buffer")
             },
             edit: function(r, e, s) {
-                var t, i, a, n, d, o, c, t, l, h = !1;
-                return !!(r = this.get_node(r)) && (this.check("edit", r, this.get_parent(r)) ? (l = r, e = "string" == typeof e ? e : r.text, this.set_text(r, ""), r = this._open_to(r), l.text = e, t = this._data.core.rtl, i = this.element.width(), this._data.core.focused = l.id, a = r.children(".jstree-anchor").trigger("focus"), n = E("<span></span>"), d = e, o = E("<div></div>", {
+                var t, i, a, n, o, d, c, t, l, h = !1;
+                return !!(r = this.get_node(r)) && (this.check("edit", r, this.get_parent(r)) ? (l = r, e = "string" == typeof e ? e : r.text, this.set_text(r, ""), r = this._open_to(r), l.text = e, t = this._data.core.rtl, i = this.element.width(), this._data.core.focused = l.id, a = r.children(".jstree-anchor").trigger("focus"), n = E("<span></span>"), o = e, d = E("<div></div>", {
                     css: {
                         position: "absolute",
                         top: "-200px",
                         left: t ? "0px" : "-1000px",
                         visibility: "hidden"
                     }
                 }).appendTo(b.body), c = E("<input />", {
-                    value: d,
+                    value: o,
                     class: "jstree-rename-input",
                     css: {
                         padding: "0",
                         border: "1px solid silver",
                         "box-sizing": "border-box",
                         display: "inline-block",
                         height: this._data.core.li_height + "px",
@@ -1720,45 +1721,45 @@
                         width: "150px"
                     },
                     blur: function(e) {
                         e.stopImmediatePropagation(), e.preventDefault();
                         var t, i = n.children(".jstree-rename-input").val(),
                             e = this.settings.core.force_text,
                             e;
-                        "" === i && (i = d), o.remove(), n.replaceWith(a), n.remove(), d = e ? d : E("<div></div>").append(E.parseHTML(d)).html(), r = this.get_node(r), this.set_text(r, d), (e = !!this.rename_node(r, e ? E("<div></div>").text(i).text() : E("<div></div>").append(E.parseHTML(i)).html())) || this.set_text(r, d), this._data.core.focused = l.id, setTimeout(function() {
+                        "" === i && (i = o), d.remove(), n.replaceWith(a), n.remove(), o = e ? o : E("<div></div>").append(E.parseHTML(o)).html(), r = this.get_node(r), this.set_text(r, o), (e = !!this.rename_node(r, e ? E("<div></div>").text(i).text() : E("<div></div>").append(E.parseHTML(i)).html())) || this.set_text(r, o), this._data.core.focused = l.id, setTimeout(function() {
                             var e = this.get_node(l.id, !0);
                             e.length && (this._data.core.focused = l.id, e.children(".jstree-anchor").trigger("focus"))
                         }.bind(this), 0), s && s.call(this, l, e, h, i), c = null
                     }.bind(this),
                     keydown: function(e) {
                         var t = e.which;
-                        27 === t && (h = !0, this.value = d), 27 !== t && 13 !== t && 37 !== t && 38 !== t && 39 !== t && 40 !== t && 32 !== t || e.stopImmediatePropagation(), 27 !== t && 13 !== t || (e.preventDefault(), this.blur())
+                        27 === t && (h = !0, this.value = o), 27 !== t && 13 !== t && 37 !== t && 38 !== t && 39 !== t && 40 !== t && 32 !== t || e.stopImmediatePropagation(), 27 !== t && 13 !== t || (e.preventDefault(), this.blur())
                     },
                     click: function(e) {
                         e.stopImmediatePropagation()
                     },
                     mousedown: function(e) {
                         e.stopImmediatePropagation()
                     },
                     keyup: function(e) {
-                        c.width(Math.min(o.text("pW" + this.value).width(), i))
+                        c.width(Math.min(d.text("pW" + this.value).width(), i))
                     },
                     keypress: function(e) {
                         if (13 === e.which) return !1
                     }
                 }), t = {
                     fontFamily: a.css("fontFamily") || "",
                     fontSize: a.css("fontSize") || "",
                     fontWeight: a.css("fontWeight") || "",
                     fontStyle: a.css("fontStyle") || "",
                     fontStretch: a.css("fontStretch") || "",
                     fontVariant: a.css("fontVariant") || "",
                     letterSpacing: a.css("letterSpacing") || "",
                     wordSpacing: a.css("wordSpacing") || ""
-                }, n.attr("class", a.attr("class")).append(a.contents().clone()).append(c), a.replaceWith(n), o.css(t), c.css(t).width(Math.min(o.text("pW" + c[0].value).width(), i))[0].select(), void E(b).one("mousedown.jstree touchstart.jstree dnd_start.vakata", function(e) {
+                }, n.attr("class", a.attr("class")).append(a.contents().clone()).append(c), a.replaceWith(n), d.css(t), c.css(t).width(Math.min(d.text("pW" + c[0].value).width(), i))[0].select(), void E(b).one("mousedown.jstree touchstart.jstree dnd_start.vakata", function(e) {
                     c && e.target !== c && E(c).trigger("blur")
                 })) : (this.settings.core.error.call(this, this._data.core.last_error), !1))
             },
             set_theme: function(e, t) {
                 if (!e) return !1;
                 var i, i;
                 (t = !0 === t ? (i = (i = this.settings.core.themes.dir) || E.jstree.path + "/themes") + "/" + e + "/style.css" : t) && -1 === E.inArray(t, r) && (E("head").append('<link rel="stylesheet" href="' + t + '" type="text/css" />'), r.push(t)), this._data.core.themes.name && this.element.removeClass("jstree-" + this._data.core.themes.name), this._data.core.themes.name = e, this.element.addClass("jstree-" + e), this.element[this.settings.core.themes.responsive ? "addClass" : "removeClass"]("jstree-" + e + "-responsive"), this.trigger("set_theme", {
@@ -1886,171 +1887,171 @@
                 }
                 a.trigger.call(this, e, t)
             }, this.refresh = function(e, t) {
                 return n = [], a.refresh.apply(this, arguments)
             }
         };
         var l = b.createElement("I"),
-            h, _, g, o, u, f, p, w;
+            h, _, g, d, u, f, p, w;
         l.className = "jstree-icon jstree-checkbox", l.setAttribute("role", "presentation"), E.jstree.defaults.checkbox = {
             visible: !0,
             three_state: !0,
             whole_node: !0,
             keep_selected_style: !0,
             cascade: "",
             tie_selection: !0,
             cascade_to_disabled: !0,
             cascade_to_hidden: !0
-        }, E.jstree.plugins.checkbox = function(e, o) {
+        }, E.jstree.plugins.checkbox = function(e, d) {
             this.bind = function() {
-                o.bind.call(this), this._data.checkbox.uto = !1, this._data.checkbox.selected = [], this.settings.checkbox.three_state && (this.settings.checkbox.cascade = "up+down+undetermined"), this.element.on("init.jstree", function() {
+                d.bind.call(this), this._data.checkbox.uto = !1, this._data.checkbox.selected = [], this.settings.checkbox.three_state && (this.settings.checkbox.cascade = "up+down+undetermined"), this.element.on("init.jstree", function() {
                     this._data.checkbox.visible = this.settings.checkbox.visible, this.settings.checkbox.keep_selected_style || this.element.addClass("jstree-checkbox-no-clicked"), this.settings.checkbox.tie_selection && this.element.addClass("jstree-checkbox-selection")
                 }.bind(this)).on("loading.jstree", function() {
                     this[this._data.checkbox.visible ? "show_checkboxes" : "hide_checkboxes"]()
                 }.bind(this)), -1 !== this.settings.checkbox.cascade.indexOf("undetermined") && this.element.on("changed.jstree uncheck_node.jstree check_node.jstree uncheck_all.jstree check_all.jstree move_node.jstree copy_node.jstree redraw.jstree open_node.jstree", function() {
                     this._data.checkbox.uto && clearTimeout(this._data.checkbox.uto), this._data.checkbox.uto = setTimeout(this._undetermined.bind(this), 50)
                 }.bind(this)), this.settings.checkbox.tie_selection || this.element.on("model.jstree", function(e, t) {
                     for (var i = this._model.data, r = i[t.parent], s = t.nodes, a, n, a = 0, n = s.length; a < n; a++) i[s[a]].state.checked = i[s[a]].state.checked || i[s[a]].original && i[s[a]].original.state && i[s[a]].original.state.checked, i[s[a]].state.checked && this._data.checkbox.selected.push(s[a])
                 }.bind(this)), -1 === this.settings.checkbox.cascade.indexOf("up") && -1 === this.settings.checkbox.cascade.indexOf("down") || this.element.on("model.jstree", function(e, t) {
                     var i = this._model.data,
                         r = i[t.parent],
                         s = t.nodes,
                         a = [],
-                        n, d, o, c, l, h, t = this.settings.checkbox.cascade,
+                        n, o, d, c, l, h, t = this.settings.checkbox.cascade,
                         _ = this.settings.checkbox.tie_selection;
                     if (-1 !== t.indexOf("down"))
                         if (r.state[_ ? "selected" : "checked"]) {
-                            for (d = 0, o = s.length; d < o; d++) i[s[d]].state[_ ? "selected" : "checked"] = !0;
+                            for (o = 0, d = s.length; o < d; o++) i[s[o]].state[_ ? "selected" : "checked"] = !0;
                             this._data[_ ? "core" : "checkbox"].selected = this._data[_ ? "core" : "checkbox"].selected.concat(s)
                         } else
-                            for (d = 0, o = s.length; d < o; d++)
-                                if (i[s[d]].state[_ ? "selected" : "checked"]) {
-                                    for (c = 0, l = i[s[d]].children_d.length; c < l; c++) i[i[s[d]].children_d[c]].state[_ ? "selected" : "checked"] = !0;
-                                    this._data[_ ? "core" : "checkbox"].selected = this._data[_ ? "core" : "checkbox"].selected.concat(i[s[d]].children_d)
+                            for (o = 0, d = s.length; o < d; o++)
+                                if (i[s[o]].state[_ ? "selected" : "checked"]) {
+                                    for (c = 0, l = i[s[o]].children_d.length; c < l; c++) i[i[s[o]].children_d[c]].state[_ ? "selected" : "checked"] = !0;
+                                    this._data[_ ? "core" : "checkbox"].selected = this._data[_ ? "core" : "checkbox"].selected.concat(i[s[o]].children_d)
                                 } if (-1 !== t.indexOf("up")) {
-                        for (d = 0, o = r.children_d.length; d < o; d++) i[r.children_d[d]].children.length || a.push(i[r.children_d[d]].parent);
+                        for (o = 0, d = r.children_d.length; o < d; o++) i[r.children_d[o]].children.length || a.push(i[r.children_d[o]].parent);
                         for (c = 0, l = (a = E.vakata.array_unique(a)).length; c < l; c++) {
                             r = i[a[c]];
                             while (r && r.id !== E.jstree.root) {
-                                for (d = n = 0, o = r.children.length; d < o; d++) n += i[r.children[d]].state[_ ? "selected" : "checked"];
-                                if (n !== o) break;
+                                for (o = n = 0, d = r.children.length; o < d; o++) n += i[r.children[o]].state[_ ? "selected" : "checked"];
+                                if (n !== d) break;
                                 r.state[_ ? "selected" : "checked"] = !0, this._data[_ ? "core" : "checkbox"].selected.push(r.id), (h = this.get_node(r, !0)) && h.length && h.children(".jstree-anchor").attr("aria-selected", !0).addClass(_ ? "jstree-clicked" : "jstree-checked"), r = this.get_node(r.parent)
                             }
                         }
                     }
                     this._data[_ ? "core" : "checkbox"].selected = E.vakata.array_unique(this._data[_ ? "core" : "checkbox"].selected)
                 }.bind(this)).on(this.settings.checkbox.tie_selection ? "select_node.jstree" : "check_node.jstree", function(e, t) {
                     var i = this,
                         r = t.node,
                         s = this._model.data,
                         a = this.get_node(r.parent),
-                        n, d, o, c, t = this.settings.checkbox.cascade,
+                        n, o, d, c, t = this.settings.checkbox.cascade,
                         l = this.settings.checkbox.tie_selection,
                         h = {},
                         _ = this._data[l ? "core" : "checkbox"].selected;
-                    for (n = 0, d = _.length; n < d; n++) h[_[n]] = !0;
+                    for (n = 0, o = _.length; n < o; n++) h[_[n]] = !0;
                     if (-1 !== t.indexOf("down"))
-                        for (var g = this._cascade_new_checked_state(r.id, !0), u = r.children_d.concat(r.id), n = 0, d = u.length; n < d; n++) - 1 < g.indexOf(u[n]) ? h[u[n]] = !0 : delete h[u[n]];
+                        for (var g = this._cascade_new_checked_state(r.id, !0), u = r.children_d.concat(r.id), n = 0, o = u.length; n < o; n++) - 1 < g.indexOf(u[n]) ? h[u[n]] = !0 : delete h[u[n]];
                     if (-1 !== t.indexOf("up"))
                         while (a && a.id !== E.jstree.root) {
-                            for (n = o = 0, d = a.children.length; n < d; n++) o += s[a.children[n]].state[l ? "selected" : "checked"];
-                            if (o !== d) break;
+                            for (n = d = 0, o = a.children.length; n < o; n++) d += s[a.children[n]].state[l ? "selected" : "checked"];
+                            if (d !== o) break;
                             a.state[l ? "selected" : "checked"] = !0, h[a.id] = !0, (c = this.get_node(a, !0)) && c.length && c.children(".jstree-anchor").attr("aria-selected", !0).addClass(l ? "jstree-clicked" : "jstree-checked"), a = this.get_node(a.parent)
                         }
                     for (n in _ = [], h) h.hasOwnProperty(n) && _.push(n);
                     this._data[l ? "core" : "checkbox"].selected = _
                 }.bind(this)).on(this.settings.checkbox.tie_selection ? "deselect_all.jstree" : "uncheck_all.jstree", function(e, t) {
                     for (var i = this.get_node(E.jstree.root), r = this._model.data, s, a, n, s = 0, a = i.children_d.length; s < a; s++)(n = r[i.children_d[s]]) && n.original && n.original.state && n.original.state.undetermined && (n.original.state.undetermined = !1)
                 }.bind(this)).on(this.settings.checkbox.tie_selection ? "deselect_node.jstree" : "uncheck_node.jstree", function(e, t) {
                     var i = this,
                         r = t.node,
                         s = this.get_node(r, !0),
-                        a, n, d, o = this.settings.checkbox.cascade,
+                        a, n, o, d = this.settings.checkbox.cascade,
                         c = this.settings.checkbox.tie_selection,
                         t = this._data[c ? "core" : "checkbox"].selected,
                         l = {},
                         h = [],
                         _ = r.children_d.concat(r.id),
                         g, t;
-                    if (-1 !== o.indexOf("down") && (g = this._cascade_new_checked_state(r.id, !1), t = E.vakata.array_filter(t, function(e) {
+                    if (-1 !== d.indexOf("down") && (g = this._cascade_new_checked_state(r.id, !1), t = E.vakata.array_filter(t, function(e) {
                             return -1 === _.indexOf(e) || -1 < g.indexOf(e)
-                        })), -1 !== o.indexOf("up") && -1 === t.indexOf(r.id)) {
-                        for (a = 0, n = r.parents.length; a < n; a++)(d = this._model.data[r.parents[a]]).state[c ? "selected" : "checked"] = !1, d && d.original && d.original.state && d.original.state.undetermined && (d.original.state.undetermined = !1), (d = this.get_node(r.parents[a], !0)) && d.length && d.children(".jstree-anchor").attr("aria-selected", !1).removeClass(c ? "jstree-clicked" : "jstree-checked");
+                        })), -1 !== d.indexOf("up") && -1 === t.indexOf(r.id)) {
+                        for (a = 0, n = r.parents.length; a < n; a++)(o = this._model.data[r.parents[a]]).state[c ? "selected" : "checked"] = !1, o && o.original && o.original.state && o.original.state.undetermined && (o.original.state.undetermined = !1), (o = this.get_node(r.parents[a], !0)) && o.length && o.children(".jstree-anchor").attr("aria-selected", !1).removeClass(c ? "jstree-clicked" : "jstree-checked");
                         t = E.vakata.array_filter(t, function(e) {
                             return -1 === r.parents.indexOf(e)
                         })
                     }
                     this._data[c ? "core" : "checkbox"].selected = t
                 }.bind(this)), -1 !== this.settings.checkbox.cascade.indexOf("up") && this.element.on("delete_node.jstree", function(e, t) {
                     var i = this.get_node(t.parent),
                         r = this._model.data,
-                        s, a, n, d, o = this.settings.checkbox.tie_selection;
-                    while (i && i.id !== E.jstree.root && !i.state[o ? "selected" : "checked"]) {
-                        for (s = n = 0, a = i.children.length; s < a; s++) n += r[i.children[s]].state[o ? "selected" : "checked"];
+                        s, a, n, o, d = this.settings.checkbox.tie_selection;
+                    while (i && i.id !== E.jstree.root && !i.state[d ? "selected" : "checked"]) {
+                        for (s = n = 0, a = i.children.length; s < a; s++) n += r[i.children[s]].state[d ? "selected" : "checked"];
                         if (!(0 < a && n === a)) break;
-                        i.state[o ? "selected" : "checked"] = !0, this._data[o ? "core" : "checkbox"].selected.push(i.id), (d = this.get_node(i, !0)) && d.length && d.children(".jstree-anchor").attr("aria-selected", !0).addClass(o ? "jstree-clicked" : "jstree-checked"), i = this.get_node(i.parent)
+                        i.state[d ? "selected" : "checked"] = !0, this._data[d ? "core" : "checkbox"].selected.push(i.id), (o = this.get_node(i, !0)) && o.length && o.children(".jstree-anchor").attr("aria-selected", !0).addClass(d ? "jstree-clicked" : "jstree-checked"), i = this.get_node(i.parent)
                     }
                 }.bind(this)).on("move_node.jstree", function(e, t) {
                     var i = t.is_multi,
                         r = t.old_parent,
                         t = this.get_node(t.parent),
                         s = this._model.data,
-                        a, n, d, o, c, l = this.settings.checkbox.tie_selection;
+                        a, n, o, d, c, l = this.settings.checkbox.tie_selection;
                     if (!i) {
                         a = this.get_node(r);
                         while (a && a.id !== E.jstree.root && !a.state[l ? "selected" : "checked"]) {
-                            for (d = n = 0, o = a.children.length; d < o; d++) n += s[a.children[d]].state[l ? "selected" : "checked"];
-                            if (!(0 < o && n === o)) break;
+                            for (o = n = 0, d = a.children.length; o < d; o++) n += s[a.children[o]].state[l ? "selected" : "checked"];
+                            if (!(0 < d && n === d)) break;
                             a.state[l ? "selected" : "checked"] = !0, this._data[l ? "core" : "checkbox"].selected.push(a.id), (c = this.get_node(a, !0)) && c.length && c.children(".jstree-anchor").attr("aria-selected", !0).addClass(l ? "jstree-clicked" : "jstree-checked"), a = this.get_node(a.parent)
                         }
                     }
                     a = t;
                     while (a && a.id !== E.jstree.root) {
-                        for (d = n = 0, o = a.children.length; d < o; d++) n += s[a.children[d]].state[l ? "selected" : "checked"];
-                        if (n === o) a.state[l ? "selected" : "checked"] || (a.state[l ? "selected" : "checked"] = !0, this._data[l ? "core" : "checkbox"].selected.push(a.id), (c = this.get_node(a, !0)) && c.length && c.children(".jstree-anchor").attr("aria-selected", !0).addClass(l ? "jstree-clicked" : "jstree-checked"));
+                        for (o = n = 0, d = a.children.length; o < d; o++) n += s[a.children[o]].state[l ? "selected" : "checked"];
+                        if (n === d) a.state[l ? "selected" : "checked"] || (a.state[l ? "selected" : "checked"] = !0, this._data[l ? "core" : "checkbox"].selected.push(a.id), (c = this.get_node(a, !0)) && c.length && c.children(".jstree-anchor").attr("aria-selected", !0).addClass(l ? "jstree-clicked" : "jstree-checked"));
                         else {
                             if (!a.state[l ? "selected" : "checked"]) break;
                             a.state[l ? "selected" : "checked"] = !1, this._data[l ? "core" : "checkbox"].selected = E.vakata.array_remove_item(this._data[l ? "core" : "checkbox"].selected, a.id), (c = this.get_node(a, !0)) && c.length && c.children(".jstree-anchor").attr("aria-selected", !1).removeClass(l ? "jstree-clicked" : "jstree-checked")
                         }
                         a = this.get_node(a.parent)
                     }
                 }.bind(this))
             }, this.get_undetermined = function(e) {
                 if (-1 === this.settings.checkbox.cascade.indexOf("undetermined")) return [];
-                for (var i, r, s, a, n = {}, d = this._model.data, t = this.settings.checkbox.tie_selection, o = this._data[t ? "core" : "checkbox"].selected, c = [], l = this, h = [], i = 0, r = o.length; i < r; i++)
-                    if (d[o[i]] && d[o[i]].parents)
-                        for (s = 0, a = d[o[i]].parents.length; s < a; s++) {
-                            if (n[d[o[i]].parents[s]] !== P) break;
-                            d[o[i]].parents[s] !== E.jstree.root && (n[d[o[i]].parents[s]] = !0, c.push(d[o[i]].parents[s]))
+                for (var i, r, s, a, n = {}, o = this._model.data, t = this.settings.checkbox.tie_selection, d = this._data[t ? "core" : "checkbox"].selected, c = [], l = this, h = [], i = 0, r = d.length; i < r; i++)
+                    if (o[d[i]] && o[d[i]].parents)
+                        for (s = 0, a = o[d[i]].parents.length; s < a; s++) {
+                            if (n[o[d[i]].parents[s]] !== P) break;
+                            o[d[i]].parents[s] !== E.jstree.root && (n[o[d[i]].parents[s]] = !0, c.push(o[d[i]].parents[s]))
                         }
                 for (this.element.find(".jstree-closed").not(":has(.jstree-children)").each(function() {
                         var e = l.get_node(this),
                             t;
                         if (e)
                             if (e.state.loaded) {
                                 for (i = 0, r = e.children_d.length; i < r; i++)
-                                    if (!(t = d[e.children_d[i]]).state.loaded && t.original && t.original.state && t.original.state.undetermined && !0 === t.original.state.undetermined)
+                                    if (!(t = o[e.children_d[i]]).state.loaded && t.original && t.original.state && t.original.state.undetermined && !0 === t.original.state.undetermined)
                                         for (n[t.id] === P && t.id !== E.jstree.root && (n[t.id] = !0, c.push(t.id)), s = 0, a = t.parents.length; s < a; s++) n[t.parents[s]] === P && t.parents[s] !== E.jstree.root && (n[t.parents[s]] = !0, c.push(t.parents[s]))
                             } else if (e.original && e.original.state && e.original.state.undetermined && !0 === e.original.state.undetermined)
                             for (n[e.id] === P && e.id !== E.jstree.root && (n[e.id] = !0, c.push(e.id)), s = 0, a = e.parents.length; s < a; s++) n[e.parents[s]] === P && e.parents[s] !== E.jstree.root && (n[e.parents[s]] = !0, c.push(e.parents[s]))
-                    }), i = 0, r = c.length; i < r; i++) d[c[i]].state[t ? "selected" : "checked"] || h.push(e ? d[c[i]] : c[i]);
+                    }), i = 0, r = c.length; i < r; i++) o[c[i]].state[t ? "selected" : "checked"] || h.push(e ? o[c[i]] : c[i]);
                 return h
             }, this._undetermined = function() {
                 if (null !== this.element) {
                     var e = this.get_undetermined(!1),
                         t, i, r;
                     for (this.element.find(".jstree-undetermined").removeClass("jstree-undetermined"), t = 0, i = e.length; t < i; t++)(r = this.get_node(e[t], !0)) && r.length && r.children(".jstree-anchor").children(".jstree-checkbox").addClass("jstree-undetermined")
                 }
             }, this.redraw_node = function(e, t, i, r) {
-                if (e = o.redraw_node.apply(this, arguments)) {
-                    for (var s, a, n = null, d = null, s = 0, a = e.childNodes.length; s < a; s++)
+                if (e = d.redraw_node.apply(this, arguments)) {
+                    for (var s, a, n = null, o = null, s = 0, a = e.childNodes.length; s < a; s++)
                         if (e.childNodes[s] && e.childNodes[s].className && -1 !== e.childNodes[s].className.indexOf("jstree-anchor")) {
                             n = e.childNodes[s];
                             break
-                        } n && (!this.settings.checkbox.tie_selection && this._model.data[e.id].state.checked && (n.className += " jstree-checked"), d = l.cloneNode(!1), this._model.data[e.id].state.checkbox_disabled && (d.className += " jstree-checkbox-disabled"), n.insertBefore(d, n.childNodes[0]))
+                        } n && (!this.settings.checkbox.tie_selection && this._model.data[e.id].state.checked && (n.className += " jstree-checked"), o = l.cloneNode(!1), this._model.data[e.id].state.checkbox_disabled && (o.className += " jstree-checkbox-disabled"), n.insertBefore(o, n.childNodes[0]))
                 }
                 return i || -1 === this.settings.checkbox.cascade.indexOf("undetermined") || (this._data.checkbox.uto && clearTimeout(this._data.checkbox.uto), this._data.checkbox.uto = setTimeout(this._undetermined.bind(this), 50)), e
             }, this.show_checkboxes = function() {
                 this._data.core.themes.checkboxes = !0, this.get_container_ul().removeClass("jstree-no-checkboxes")
             }, this.hide_checkboxes = function() {
                 this._data.core.themes.checkboxes = !1, this.get_container_ul().addClass("jstree-no-checkboxes")
             }, this.toggle_checkboxes = function() {
@@ -2083,40 +2084,40 @@
                     return !0
                 }
                 if (!(e = this.get_node(e)) || e.id === E.jstree.root) return !1;
                 r = this.get_node(e, !0), e.state.checkbox_disabled && (e.state.checkbox_disabled = !1, r && r.length && r.children(".jstree-anchor").children(".jstree-checkbox").removeClass("jstree-checkbox-disabled"), this.trigger("enable_checkbox", {
                     node: e
                 }))
             }, this.activate_node = function(e, t) {
-                return !E(t.target).hasClass("jstree-checkbox-disabled") && (this.settings.checkbox.tie_selection && (this.settings.checkbox.whole_node || E(t.target).hasClass("jstree-checkbox")) && (t.ctrlKey = !0), this.settings.checkbox.tie_selection || !this.settings.checkbox.whole_node && !E(t.target).hasClass("jstree-checkbox") ? o.activate_node.call(this, e, t) : !this.is_disabled(e) && (this.is_checked(e) ? this.uncheck_node(e, t) : this.check_node(e, t), void this.trigger("activate_node", {
+                return !E(t.target).hasClass("jstree-checkbox-disabled") && (this.settings.checkbox.tie_selection && (this.settings.checkbox.whole_node || E(t.target).hasClass("jstree-checkbox")) && (t.ctrlKey = !0), this.settings.checkbox.tie_selection || !this.settings.checkbox.whole_node && !E(t.target).hasClass("jstree-checkbox") ? d.activate_node.call(this, e, t) : !this.is_disabled(e) && (this.is_checked(e) ? this.uncheck_node(e, t) : this.check_node(e, t), void this.trigger("activate_node", {
                     node: this.get_node(e)
                 })))
             }, this.delete_node = function(e) {
-                if (this.settings.checkbox.tie_selection || E.vakata.is_array(e)) return o.delete_node.call(this, e);
+                if (this.settings.checkbox.tie_selection || E.vakata.is_array(e)) return d.delete_node.call(this, e);
                 var t, i, r, s = !1;
                 if (!(e = this.get_node(e)) || e.id === E.jstree.root) return !1;
                 for ((t = e.children_d.concat([])).push(e.id), i = 0, r = t.length; i < r; i++)
                     if (this._model.data[t[i]].state.checked) {
                         s = !0;
                         break
                     } return s && (this._data.checkbox.selected = E.vakata.array_filter(this._data.checkbox.selected, function(e) {
                     return -1 === E.inArray(e, t)
-                })), o.delete_node.call(this, e)
+                })), d.delete_node.call(this, e)
             }, this._cascade_new_checked_state = function(e, t) {
                 var i = this,
                     r = this.settings.checkbox.tie_selection,
                     s = this._model.data[e],
                     a = [],
                     n = [],
-                    d, o, c;
+                    o, d, c;
                 if (!this.settings.checkbox.cascade_to_disabled && s.state.disabled || !this.settings.checkbox.cascade_to_hidden && s.state.hidden) c = this.get_checked_descendants(e), s.state[r ? "selected" : "checked"] && c.push(s.id), a = a.concat(c);
                 else {
                     if (s.children)
-                        for (d = 0, o = s.children.length; d < o; d++) {
-                            var l = s.children[d],
+                        for (o = 0, d = s.children.length; o < d; o++) {
+                            var l = s.children[o],
                                 c = i._cascade_new_checked_state(l, t),
                                 a = a.concat(c); - 1 < c.indexOf(l) && n.push(l)
                         }
                     var h = i.get_node(s, !0),
                         e = 0 < n.length && n.length < s.children.length;
                     s.original && s.original.state && s.original.state.undetermined && (s.original.state.undetermined = e), !e && t && n.length === s.children.length ? (s.state[r ? "selected" : "checked"] = t, a.push(s.id), h.children(".jstree-anchor").attr("aria-selected", !0).addClass(r ? "jstree-clicked" : "jstree-checked")) : (s.state[r ? "selected" : "checked"] = !1, h.children(".jstree-anchor").attr("aria-selected", !1).removeClass(r ? "jstree-clicked" : "jstree-checked"))
                 }
@@ -2187,29 +2188,29 @@
             }, this.get_bottom_checked = function(e) {
                 if (this.settings.checkbox.tie_selection) return this.get_bottom_selected(e);
                 for (var t = this.get_checked(!0), i = [], r, s, r = 0, s = t.length; r < s; r++) t[r].children.length || i.push(t[r].id);
                 return e ? E.map(i, function(e) {
                     return this.get_node(e)
                 }.bind(this)) : i
             }, this.load_node = function(e, t) {
-                var i, r, s, a, n, d;
-                if (!E.vakata.is_array(e) && !this.settings.checkbox.tie_selection && (d = this.get_node(e)) && d.state.loaded)
-                    for (i = 0, r = d.children_d.length; i < r; i++) this._model.data[d.children_d[i]].state.checked && (this._data.checkbox.selected = E.vakata.array_remove_item(this._data.checkbox.selected, d.children_d[i]));
-                return o.load_node.apply(this, arguments)
+                var i, r, s, a, n, o;
+                if (!E.vakata.is_array(e) && !this.settings.checkbox.tie_selection && (o = this.get_node(e)) && o.state.loaded)
+                    for (i = 0, r = o.children_d.length; i < r; i++) this._model.data[o.children_d[i]].state.checked && (this._data.checkbox.selected = E.vakata.array_remove_item(this._data.checkbox.selected, o.children_d[i]));
+                return d.load_node.apply(this, arguments)
             }, this.get_state = function() {
-                var e = o.get_state.apply(this, arguments);
+                var e = d.get_state.apply(this, arguments);
                 return this.settings.checkbox.tie_selection || (e.checkbox = this._data.checkbox.selected.slice()), e
             }, this.set_state = function(e, t) {
-                var i = o.set_state.apply(this, arguments),
+                var i = d.set_state.apply(this, arguments),
                     r;
                 return i && e.checkbox ? (this.settings.checkbox.tie_selection || (this.uncheck_all(), r = this, E.each(e.checkbox, function(e, t) {
                     r.check_node(t)
                 })), delete e.checkbox, this.set_state(e, t), !1) : i
             }, this.refresh = function(e, t) {
-                return this.settings.checkbox.tie_selection && (this._data.checkbox.selected = []), o.refresh.apply(this, arguments)
+                return this.settings.checkbox.tie_selection && (this._data.checkbox.selected = []), d.refresh.apply(this, arguments)
             }
         }, E.jstree.defaults.conditionalselect = function() {
             return !0
         }, E.jstree.plugins.conditionalselect = function(e, i) {
             this.activate_node = function(e, t) {
                 if (this.settings.conditionalselect.call(this, this.get_node(e), t)) return i.activate_node.call(this, e, t)
             }
@@ -2331,19 +2332,19 @@
                 }.bind(this))
             }, this.teardown = function() {
                 this._data.contextmenu.visible && E.vakata.context.hide(), E(b).off("context_hide.vakata.jstree"), a.teardown.call(this)
             }, this.show_contextmenu = function(t, i, r, e) {
                 if (!(t = this.get_node(t)) || t.id === E.jstree.root) return !1;
                 var s = this.settings.contextmenu,
                     a, n = this.get_node(t, !0).children(".jstree-anchor"),
-                    d = !1,
-                    o = !1;
-                !s.show_at_node && i !== P && r !== P || (d = n.offset(), i = d.left, r = d.top + this._data.core.li_height), this.settings.contextmenu.select_node && !this.is_selected(t) && this.activate_node(t, e), o = s.items, E.vakata.is_function(o) && (o = o.call(this, t, function(e) {
+                    o = !1,
+                    d = !1;
+                !s.show_at_node && i !== P && r !== P || (o = n.offset(), i = o.left, r = o.top + this._data.core.li_height), this.settings.contextmenu.select_node && !this.is_selected(t) && this.activate_node(t, e), d = s.items, E.vakata.is_function(d) && (d = d.call(this, t, function(e) {
                     this._show_contextmenu(t, i, r, e)
-                }.bind(this))), E.isPlainObject(o) && this._show_contextmenu(t, i, r, o)
+                }.bind(this))), E.isPlainObject(d) && this._show_contextmenu(t, i, r, d)
             }, this._show_contextmenu = function(e, t, i, r) {
                 var s, a = this.get_node(e, !0).children(".jstree-anchor");
                 E(b).one("context_show.vakata.jstree", function(e, t) {
                     var i = "jstree-contextmenu jstree-" + this.get_theme() + "-contextmenu";
                     E(t.element).addClass(i), a.addClass("jstree-context")
                 }.bind(this)), this._data.contextmenu.visible = !0, E.vakata.context.show(a, {
                     x: t,
@@ -2407,34 +2408,34 @@
                         item: e,
                         reference: g.reference,
                         element: g.element
                     }) : t.label) + (t.shortcut ? ' <span class="vakata-contextmenu-shortcut vakata-contextmenu-shortcut-' + t.shortcut + '">' + (t.shortcut_label || "") + "</span>" : "") + "</a>", t.submenu && (s = h.vakata.context._parse(t.submenu, !0)) && (i += s), i += "</li>", void(t.separator_after && (i += "<li class='vakata-context-separator'><a href='#' " + (h.vakata.context.settings.icons ? "" : 'class="vakata-context-no-icons"') + ">&#160;</a></li>", r = !0)))
                 }), i = i.replace(/<li class\='vakata-context-separator'\><\/li\>$/, ""), t && (i += "</ul>"), t || (g.html = i, h.vakata.context._trigger("parse")), 10 < i.length && i
             },
             _show_submenu: function(e) {
-                var t, i, r, s, a, n, d, o;
-                (e = h(e)).length && e.children("ul").length && (t = e.children("ul"), r = (i = e.offset().left) + e.outerWidth(), s = e.offset().top, a = t.width(), n = t.height(), d = h(window).width() + h(window).scrollLeft(), o = h(window).height() + h(window).scrollTop(), _ ? e[r - (a + 10 + e.outerWidth()) < 0 ? "addClass" : "removeClass"]("vakata-context-left") : e[d < r + a && d - r < i ? "addClass" : "removeClass"]("vakata-context-right"), o < s + n + 10 && t.css("bottom", "-1px"), e.hasClass("vakata-context-right") ? i < a && t.css("margin-right", i - a) : d - r < a && t.css("margin-left", d - r - a), t.show())
+                var t, i, r, s, a, n, o, d;
+                (e = h(e)).length && e.children("ul").length && (t = e.children("ul"), r = (i = e.offset().left) + e.outerWidth(), s = e.offset().top, a = t.width(), n = t.height(), o = h(window).width() + h(window).scrollLeft(), d = h(window).height() + h(window).scrollTop(), _ ? e[r - (a + 10 + e.outerWidth()) < 0 ? "addClass" : "removeClass"]("vakata-context-left") : e[o < r + a && o - r < i ? "addClass" : "removeClass"]("vakata-context-right"), d < s + n + 10 && t.css("bottom", "-1px"), e.hasClass("vakata-context-right") ? i < a && t.css("margin-right", i - a) : o - r < a && t.css("margin-left", o - r - a), t.show())
             },
             show: function(e, t, i) {
-                var r, s, a, n, d, o, c, i, l = !0;
+                var r, s, a, n, o, d, c, i, l = !0;
                 switch (g.element && g.element.length && g.element.width(""), !0) {
                     case !t && !e:
                         return !1;
                     case !!t && !!e:
                         g.reference = e, g.position_x = t.x, g.position_y = t.y;
                         break;
                     case !t && !!e:
                         r = (g.reference = e).offset(), g.position_x = r.left + e.outerHeight(), g.position_y = r.top;
                         break;
                     case !!t && !e:
                         g.position_x = t.x, g.position_y = t.y
                 }
-                e && !i && h(e).data("vakata_contextmenu") && (i = h(e).data("vakata_contextmenu")), h.vakata.context._parse(i) && g.element.html(g.html), g.items.length && (g.element.appendTo(b.body), s = g.element, a = g.position_x, n = g.position_y, d = s.width(), o = s.height(), c = h(window).width() + h(window).scrollLeft(), i = h(window).height() + h(window).scrollTop(), _ && (a -= s.outerWidth() - h(e).outerWidth()) < h(window).scrollLeft() + 20 && (a = h(window).scrollLeft() + 20), g.element.css({
-                    left: a = c < a + d + 20 ? c - (d + 20) : a,
-                    top: n = i < n + o + 20 ? i - (o + 20) : n
+                e && !i && h(e).data("vakata_contextmenu") && (i = h(e).data("vakata_contextmenu")), h.vakata.context._parse(i) && g.element.html(g.html), g.items.length && (g.element.appendTo(b.body), s = g.element, a = g.position_x, n = g.position_y, o = s.width(), d = s.height(), c = h(window).width() + h(window).scrollLeft(), i = h(window).height() + h(window).scrollTop(), _ && (a -= s.outerWidth() - h(e).outerWidth()) < h(window).scrollLeft() + 20 && (a = h(window).scrollLeft() + 20), g.element.css({
+                    left: a = c < a + o + 20 ? c - (o + 20) : a,
+                    top: n = i < n + d + 20 ? i - (d + 20) : n
                 }).show().find("a").first().trigger("focus").parent().addClass("vakata-context-hover"), g.is_visible = !0, h.vakata.context._trigger("show"))
             },
             hide: function() {
                 g.is_visible && (g.element.hide().find("ul").hide().end().find(":focus").trigger("blur").end().detach(), g.is_visible = !1, h.vakata.context._trigger("hide"))
             }
         }, h(function() {
             _ = "rtl" === h(b.body).css("direction");
@@ -2490,52 +2491,52 @@
             inside_pos: 0,
             drag_selection: !0,
             touch: !0,
             large_drop_target: !1,
             large_drag_target: !1,
             use_html5: !1,
             blank_space_drop: !1
-        }, E.jstree.plugins.dnd = function(e, d) {
+        }, E.jstree.plugins.dnd = function(e, o) {
             this.init = function(e, t) {
-                d.init.call(this, e, t), this.settings.dnd.use_html5 = this.settings.dnd.use_html5 && "draggable" in b.createElement("span")
+                o.init.call(this, e, t), this.settings.dnd.use_html5 = this.settings.dnd.use_html5 && "draggable" in b.createElement("span")
             }, this.bind = function() {
-                d.bind.call(this), this.element.on(this.settings.dnd.use_html5 ? "dragstart.jstree" : "mousedown.jstree touchstart.jstree", this.settings.dnd.large_drag_target ? ".jstree-node" : ".jstree-anchor", function(e) {
+                o.bind.call(this), this.element.on(this.settings.dnd.use_html5 ? "dragstart.jstree" : "mousedown.jstree touchstart.jstree", this.settings.dnd.large_drag_target ? ".jstree-node" : ".jstree-anchor", function(e) {
                     if (this.settings.dnd.large_drag_target && E(e.target).closest(".jstree-node")[0] !== e.currentTarget) return !0;
                     if ("touchstart" === e.type && (!this.settings.dnd.touch || "selected" === this.settings.dnd.touch && !E(e.currentTarget).closest(".jstree-node").children(".jstree-anchor").hasClass("jstree-clicked"))) return !0;
                     var t = this.get_node(e.target),
                         i = this.is_selected(t) && this.settings.dnd.drag_selection ? this.get_top_selected().length : 1,
                         r = 1 < i ? i + " " + this.get_string("nodes") : this.get_text(e.currentTarget);
                     if (this.settings.core.force_text && (r = E.vakata.html.escape(r)), t && (t.id || 0 === t.id) && t.id !== E.jstree.root && (1 === e.which || "touchstart" === e.type || "dragstart" === e.type) && (!0 === this.settings.dnd.is_draggable || E.vakata.is_function(this.settings.dnd.is_draggable) && this.settings.dnd.is_draggable.call(this, 1 < i ? this.get_top_selected(!0) : [t], e))) {
-                        if (o = {
+                        if (d = {
                                 jstree: !0,
                                 origin: this,
                                 obj: this.get_node(t, !0),
                                 nodes: 1 < i ? this.get_top_selected() : [t.id]
-                            }, u = e.currentTarget, !this.settings.dnd.use_html5) return this.element.trigger("mousedown.jstree"), E.vakata.dnd.start(e, o, '<div id="jstree-dnd" class="jstree-' + this.get_theme() + " jstree-" + this.get_theme() + "-" + this.get_theme_variant() + " " + (this.settings.core.themes.responsive ? " jstree-dnd-responsive" : "") + '"><i class="jstree-icon jstree-er"></i>' + r + '<ins class="jstree-copy">+</ins></div>');
+                            }, u = e.currentTarget, !this.settings.dnd.use_html5) return this.element.trigger("mousedown.jstree"), E.vakata.dnd.start(e, d, '<div id="jstree-dnd" class="jstree-' + this.get_theme() + " jstree-" + this.get_theme() + "-" + this.get_theme_variant() + " " + (this.settings.core.themes.responsive ? " jstree-dnd-responsive" : "") + '"><i class="jstree-icon jstree-er"></i>' + r + '<ins class="jstree-copy">+</ins></div>');
                         E.vakata.dnd._trigger("start", e, {
                             helper: E(),
                             element: u,
-                            data: o
+                            data: d
                         })
                     }
                 }.bind(this)), this.settings.dnd.use_html5 && this.element.on("dragover.jstree", function(e) {
                     return e.preventDefault(), E.vakata.dnd._trigger("move", e, {
                         helper: E(),
                         element: u,
-                        data: o
+                        data: d
                     }), !1
                 }).on("drop.jstree", function(e) {
                     return e.preventDefault(), E.vakata.dnd._trigger("stop", e, {
                         helper: E(),
                         element: u,
-                        data: o
+                        data: d
                     }), !1
                 }.bind(this))
             }, this.redraw_node = function(e, t, i, r) {
-                if ((e = d.redraw_node.apply(this, arguments)) && this.settings.dnd.use_html5)
+                if ((e = o.redraw_node.apply(this, arguments)) && this.settings.dnd.use_html5)
                     if (this.settings.dnd.large_drag_target) e.setAttribute("draggable", !0);
                     else {
                         for (var s, a, n = null, s = 0, a = e.childNodes.length; s < a; s++)
                             if (e.childNodes[s] && e.childNodes[s].className && -1 !== e.childNodes[s].className.indexOf("jstree-anchor")) {
                                 n = e.childNodes[s];
                                 break
                             } n && n.setAttribute("draggable", !0)
@@ -2547,59 +2548,59 @@
                 O = !1,
                 A = !1,
                 S = E('<div id="jstree-marker">&#160;</div>').hide();
             E(b).on("dragover.vakata.jstree", function(e) {
                 u && E.vakata.dnd._trigger("move", e, {
                     helper: E(),
                     element: u,
-                    data: o
+                    data: d
                 })
             }).on("drop.vakata.jstree", function(e) {
                 u && (E.vakata.dnd._trigger("stop", e, {
                     helper: E(),
                     element: u,
-                    data: o
-                }), o = u = null)
+                    data: d
+                }), d = u = null)
             }).on("dnd_start.vakata.jstree", function(e, t) {
                 O = N = !1, t && t.data && t.data.jstree && S.appendTo(b.body)
             }).on("dnd_move.vakata.jstree", function(e, s) {
                 var a = s.event.target !== O.target;
                 if (A && (s.event && "dragover" === s.event.type && !a || clearTimeout(A)), s && s.data && s.data.jstree && (!s.event.target.id || "jstree-marker" !== s.event.target.id)) {
                     O = s.event;
                     var n = E.jstree.reference(s.event.target),
-                        d = !1,
                         o = !1,
+                        d = !1,
                         t = !1,
                         i, c, l, h, _, g, u, f, p, m, v, j, k, b, y, x, w, C;
                     if (n && n._data && n._data.dnd)
                         if (S.attr("class", "jstree-" + n.get_theme() + (n.settings.core.themes.responsive ? " jstree-dnd-responsive" : "")), x = s.data.origin && (s.data.origin.settings.dnd.always_copy || s.data.origin.settings.dnd.copy && (s.event.metaKey || s.event.ctrlKey)), s.helper.children().attr("class", "jstree-" + n.get_theme() + " jstree-" + n.get_theme() + "-" + n.get_theme_variant() + " " + (n.settings.core.themes.responsive ? " jstree-dnd-responsive" : "")).find(".jstree-copy").first()[x ? "show" : "hide"](), s.event.target !== n.element[0] && s.event.target !== n.get_container_ul()[0] || 0 !== n.get_container_ul().children().length && !n.settings.dnd.blank_space_drop) {
-                            if ((d = n.settings.dnd.large_drop_target ? E(s.event.target).closest(".jstree-node").children(".jstree-anchor") : E(s.event.target).closest(".jstree-anchor")) && d.length && d.parent().is(".jstree-closed, .jstree-open, .jstree-leaf") && (o = d.offset(), t = (s.event.pageY !== P ? s.event : s.event.originalEvent).pageY - o.top, h = d.outerHeight(), u = t < h / 3 ? ["b", "i", "a"] : h - h / 3 < t ? ["a", "i", "b"] : h / 2 < t ? ["i", "a", "b"] : ["i", "b", "a"], E.each(u, function(e, t) {
+                            if ((o = n.settings.dnd.large_drop_target ? E(s.event.target).closest(".jstree-node").children(".jstree-anchor") : E(s.event.target).closest(".jstree-anchor")) && o.length && o.parent().is(".jstree-closed, .jstree-open, .jstree-leaf") && (d = o.offset(), t = (s.event.pageY !== P ? s.event : s.event.originalEvent).pageY - d.top, h = o.outerHeight(), u = t < h / 3 ? ["b", "i", "a"] : h - h / 3 < t ? ["a", "i", "b"] : h / 2 < t ? ["i", "a", "b"] : ["i", "b", "a"], E.each(u, function(e, t) {
                                     switch (t) {
                                         case "b":
-                                            c = o.left - 6, l = o.top, _ = n.get_parent(d), g = d.parent().index(), C = "jstree-below";
+                                            c = d.left - 6, l = d.top, _ = n.get_parent(o), g = o.parent().index(), C = "jstree-below";
                                             break;
                                         case "i":
-                                            b = n.settings.dnd.inside_pos, y = n.get_node(d.parent()), c = o.left - 2, l = o.top + h / 2 + 1, _ = y.id, g = "first" === b ? 0 : "last" === b ? y.children.length : Math.min(b, y.children.length), C = "jstree-inside";
+                                            b = n.settings.dnd.inside_pos, y = n.get_node(o.parent()), c = d.left - 2, l = d.top + h / 2 + 1, _ = y.id, g = "first" === b ? 0 : "last" === b ? y.children.length : Math.min(b, y.children.length), C = "jstree-inside";
                                             break;
                                         case "a":
-                                            c = o.left - 6, l = o.top + h, _ = n.get_parent(d), g = d.parent().index() + 1, C = "jstree-above"
+                                            c = d.left - 6, l = d.top + h, _ = n.get_parent(o), g = o.parent().index() + 1, C = "jstree-above"
                                     }
                                     for (f = !0, p = 0, m = s.data.nodes.length; p < m; p++)
                                         if (v = s.data.origin && (s.data.origin.settings.dnd.always_copy || s.data.origin.settings.dnd.copy && (s.event.metaKey || s.event.ctrlKey)) ? "copy_node" : "move_node", j = g, "move_node" == v && "a" === t && s.data.origin && s.data.origin === n && _ === n.get_parent(s.data.nodes[p]) && (k = n.get_node(_), j > E.inArray(s.data.nodes[p], k.children) && --j), !(f = f && (n && n.settings && n.settings.dnd && !1 === n.settings.dnd.check_while_dragging || n.check(v, s.data.origin && s.data.origin !== n ? s.data.origin.get_node(s.data.nodes[p]) : s.data.nodes[p], _, j, {
                                                 dnd: !0,
-                                                ref: n.get_node(d.parent()),
+                                                ref: n.get_node(o.parent()),
                                                 pos: t,
                                                 origin: s.data.origin,
                                                 is_multi: s.data.origin && s.data.origin !== n,
                                                 is_foreign: !s.data.origin
                                             })))) {
                                             n && n.last_error && (T = n.last_error());
                                             break
                                         } var i, r;
-                                    if ("i" === t && d.parent().is(".jstree-closed") && n.settings.dnd.open_timeout && (s.event && "dragover" === s.event.type && !a || (A && clearTimeout(A), A = setTimeout((r = d, function() {
+                                    if ("i" === t && o.parent().is(".jstree-closed") && n.settings.dnd.open_timeout && (s.event && "dragover" === s.event.type && !a || (A && clearTimeout(A), A = setTimeout((r = o, function() {
                                             i.open_node(r)
                                         }), (i = n).settings.dnd.open_timeout))), f) return (w = n.get_node(_, !0)).hasClass(".jstree-dnd-parent") || (E(".jstree-dnd-parent").removeClass("jstree-dnd-parent"), w.addClass("jstree-dnd-parent")), N = {
                                         ins: n,
                                         par: _,
                                         pos: "i" !== t || "last" !== b || 0 !== g || n.is_loaded(y) ? g : "last"
                                     }, S.css({
                                         left: c + "px",
@@ -2731,25 +2732,25 @@
                     }
                     var e = !1,
                         t = !1,
                         r = !1,
                         s = !1,
                         a = !1,
                         n = !1,
-                        d = !1,
                         o = !1,
+                        d = !1,
                         c = !1,
                         l = !1;
                     return p.scroll_t = 0, p.scroll_l = 0, p.scroll_e = !1, f(f(i.target).parentsUntil("body").addBack().get().reverse()).filter(function() {
                         return this.ownerDocument && /^auto|scroll$/.test(f(this).css("overflow")) && (this.scrollHeight > this.offsetHeight || this.scrollWidth > this.offsetWidth)
                     }).each(function() {
                         var e = f(this),
                             t = e.offset();
                         if (this.scrollHeight > this.offsetHeight && (t.top + e.height() - i.pageY < f.vakata.dnd.settings.scroll_proximity && (p.scroll_t = 1), i.pageY - t.top < f.vakata.dnd.settings.scroll_proximity && (p.scroll_t = -1)), this.scrollWidth > this.offsetWidth && (t.left + e.width() - i.pageX < f.vakata.dnd.settings.scroll_proximity && (p.scroll_l = 1), i.pageX - t.left < f.vakata.dnd.settings.scroll_proximity && (p.scroll_l = -1)), p.scroll_t || p.scroll_l) return p.scroll_e = f(this), !1
-                    }), p.scroll_e || (e = f(b), t = f(window), r = e.height(), s = t.height(), a = e.width(), n = t.width(), d = e.scrollTop(), o = e.scrollLeft(), s < r && i.pageY - d < f.vakata.dnd.settings.scroll_proximity && (p.scroll_t = -1), s < r && s - (i.pageY - d) < f.vakata.dnd.settings.scroll_proximity && (p.scroll_t = 1), n < a && i.pageX - o < f.vakata.dnd.settings.scroll_proximity && (p.scroll_l = -1), n < a && n - (i.pageX - o) < f.vakata.dnd.settings.scroll_proximity && (p.scroll_l = 1), (p.scroll_t || p.scroll_l) && (p.scroll_e = e)), p.scroll_e && f.vakata.dnd._scroll(!0), p.helper && (c = parseInt(i.pageY + f.vakata.dnd.settings.helper_top, 10), l = parseInt(i.pageX + f.vakata.dnd.settings.helper_left, 10), a && l + p.helper_w > a && (l = a - (p.helper_w + 2)), p.helper.css({
+                    }), p.scroll_e || (e = f(b), t = f(window), r = e.height(), s = t.height(), a = e.width(), n = t.width(), o = e.scrollTop(), d = e.scrollLeft(), s < r && i.pageY - o < f.vakata.dnd.settings.scroll_proximity && (p.scroll_t = -1), s < r && s - (i.pageY - o) < f.vakata.dnd.settings.scroll_proximity && (p.scroll_t = 1), n < a && i.pageX - d < f.vakata.dnd.settings.scroll_proximity && (p.scroll_l = -1), n < a && n - (i.pageX - d) < f.vakata.dnd.settings.scroll_proximity && (p.scroll_l = 1), (p.scroll_t || p.scroll_l) && (p.scroll_e = e)), p.scroll_e && f.vakata.dnd._scroll(!0), p.helper && (c = parseInt(i.pageY + f.vakata.dnd.settings.helper_top, 10), l = parseInt(i.pageX + f.vakata.dnd.settings.helper_left, 10), a && l + p.helper_w > a && (l = a - (p.helper_w + 2)), p.helper.css({
                         left: l + "px",
                         top: (c = r && r < c + 25 ? r - 50 : c) + "px"
                     })), f.vakata.dnd._trigger("move", i), !1
                 }
             },
             stop: function(e) {
                 var t;
@@ -2758,41 +2759,41 @@
                 }, 100), f(e.target).one("click", function() {
                     t && clearTimeout(t)
                 })), f.vakata.dnd._clean(), !1
             }
         }, E.jstree.defaults.massload = null, E.jstree.plugins.massload = function(e, l) {
             this.init = function(e, t) {
                 this._data.massload = {}, l.init.call(this, e, t)
-            }, this._load_nodes = function(a, n, d, o) {
+            }, this._load_nodes = function(a, n, o, d) {
                 var e = this.settings.massload,
                     t = [],
                     i = this._model.data,
                     r, s, c;
-                if (!d) {
-                    for (r = 0, s = a.length; r < s; r++) i[a[r]] && (i[a[r]].state.loaded || i[a[r]].state.failed) && !o || (t.push(a[r]), (c = this.get_node(a[r], !0)) && c.length && c.addClass("jstree-loading").attr("aria-busy", !0));
+                if (!o) {
+                    for (r = 0, s = a.length; r < s; r++) i[a[r]] && (i[a[r]].state.loaded || i[a[r]].state.failed) && !d || (t.push(a[r]), (c = this.get_node(a[r], !0)) && c.length && c.addClass("jstree-loading").attr("aria-busy", !0));
                     if (this._data.massload = {}, t.length) {
                         if (E.vakata.is_function(e)) return e.call(this, t, function(e) {
                             var t, i;
                             if (e)
                                 for (t in e) e.hasOwnProperty(t) && (this._data.massload[t] = e[t]);
                             for (t = 0, i = a.length; t < i; t++)(c = this.get_node(a[t], !0)) && c.length && c.removeClass("jstree-loading").attr("aria-busy", !1);
-                            l._load_nodes.call(this, a, n, d, o)
+                            l._load_nodes.call(this, a, n, o, d)
                         }.bind(this));
                         if ("object" == typeof e && e && e.url) return e = E.extend(!0, {}, e), E.vakata.is_function(e.url) && (e.url = e.url.call(this, t)), E.vakata.is_function(e.data) && (e.data = e.data.call(this, t)), E.ajax(e).done(function(e, t, i) {
                             var r, s;
                             if (e)
                                 for (r in e) e.hasOwnProperty(r) && (this._data.massload[r] = e[r]);
                             for (r = 0, s = a.length; r < s; r++)(c = this.get_node(a[r], !0)) && c.length && c.removeClass("jstree-loading").attr("aria-busy", !1);
-                            l._load_nodes.call(this, a, n, d, o)
+                            l._load_nodes.call(this, a, n, o, d)
                         }.bind(this)).fail(function(e) {
-                            l._load_nodes.call(this, a, n, d, o)
+                            l._load_nodes.call(this, a, n, o, d)
                         }.bind(this))
                     }
                 }
-                return l._load_nodes.call(this, a, n, d, o)
+                return l._load_nodes.call(this, a, n, o, d)
             }, this._load_node = function(e, t) {
                 var i = this._data.massload[e.id],
                     r = null,
                     i;
                 return i ? (r = this["string" == typeof i ? "_append_html_data" : "_append_json_data"](e, "string" == typeof i ? E(E.parseHTML(i)).filter(function() {
                     return 3 !== this.nodeType
                 }) : i, function(e) {
@@ -2804,61 +2805,61 @@
             fuzzy: !1,
             case_sensitive: !1,
             show_only_matches: !1,
             show_only_matches_children: !1,
             close_opened_onclear: !0,
             search_leaves_only: !1,
             search_callback: !1
-        }, E.jstree.plugins.search = function(e, d) {
+        }, E.jstree.plugins.search = function(e, o) {
             this.bind = function() {
-                d.bind.call(this), this._data.search.str = "", this._data.search.dom = E(), this._data.search.res = [], this._data.search.opn = [], this._data.search.som = !1, this._data.search.smc = !1, this._data.search.hdn = [], this.element.on("search.jstree", function(e, t) {
+                o.bind.call(this), this._data.search.str = "", this._data.search.dom = E(), this._data.search.res = [], this._data.search.opn = [], this._data.search.som = !1, this._data.search.smc = !1, this._data.search.hdn = [], this.element.on("search.jstree", function(e, t) {
                     if (this._data.search.som && t.res.length) {
-                        for (var i = this._model.data, r, s, a = [], n, d, r = 0, s = t.res.length; r < s; r++)
+                        for (var i = this._model.data, r, s, a = [], n, o, r = 0, s = t.res.length; r < s; r++)
                             if (i[t.res[r]] && !i[t.res[r]].state.hidden && (a.push(t.res[r]), a = a.concat(i[t.res[r]].parents), this._data.search.smc))
-                                for (n = 0, d = i[t.res[r]].children_d.length; n < d; n++) i[i[t.res[r]].children_d[n]] && !i[i[t.res[r]].children_d[n]].state.hidden && a.push(i[t.res[r]].children_d[n]);
+                                for (n = 0, o = i[t.res[r]].children_d.length; n < o; n++) i[i[t.res[r]].children_d[n]] && !i[i[t.res[r]].children_d[n]].state.hidden && a.push(i[t.res[r]].children_d[n]);
                         a = E.vakata.array_remove_item(E.vakata.array_unique(a), E.jstree.root), this._data.search.hdn = this.hide_all(!0), this.show_node(a, !0), this.redraw(!0)
                     }
                 }.bind(this)).on("clear_search.jstree", function(e, t) {
                     this._data.search.som && t.res.length && (this.show_node(this._data.search.hdn, !0), this.redraw(!0))
                 }.bind(this))
             }, this.search = function(r, e, t, i, s, a) {
                 if (!1 === r || "" === E.vakata.trim(r.toString())) return this.clear_search();
                 i = (i = this.get_node(i)) && (i.id || 0 === i.id) ? i.id : null, r = r.toString();
                 var n = this.settings.search,
-                    d = n.ajax || !1,
-                    o = this._model.data,
+                    o = n.ajax || !1,
+                    d = this._model.data,
                     c = null,
                     l = [],
                     h = [],
                     _, g;
-                if (this._data.search.res.length && !s && this.clear_search(), t === P && (t = n.show_only_matches), a === P && (a = n.show_only_matches_children), !e && !1 !== d) return E.vakata.is_function(d) ? d.call(this, r, function(e) {
+                if (this._data.search.res.length && !s && this.clear_search(), t === P && (t = n.show_only_matches), a === P && (a = n.show_only_matches_children), !e && !1 !== o) return E.vakata.is_function(o) ? o.call(this, r, function(e) {
                     e && e.d && (e = e.d), this._load_nodes(E.vakata.is_array(e) ? E.vakata.array_unique(e) : [], function() {
                         this.search(r, !0, t, i, s, a)
                     })
-                }.bind(this), i) : ((d = E.extend({}, d)).data || (d.data = {}), d.data.str = r, i && (d.data.inside = i), this._data.search.lastRequest && this._data.search.lastRequest.abort(), this._data.search.lastRequest = E.ajax(d).fail(function() {
+                }.bind(this), i) : ((o = E.extend({}, o)).data || (o.data = {}), o.data.str = r, i && (o.data.inside = i), this._data.search.lastRequest && this._data.search.lastRequest.abort(), this._data.search.lastRequest = E.ajax(o).fail(function() {
                     this._data.core.last_error = {
                         error: "ajax",
                         plugin: "search",
                         id: "search_01",
                         reason: "Could not load search parents",
-                        data: JSON.stringify(d)
+                        data: JSON.stringify(o)
                     }, this.settings.core.error.call(this, this._data.core.last_error)
                 }.bind(this)).done(function(e) {
                     e && e.d && (e = e.d), this._load_nodes(E.vakata.is_array(e) ? E.vakata.array_unique(e) : [], function() {
                         this.search(r, !0, t, i, s, a)
                     })
                 }.bind(this)), this._data.search.lastRequest);
                 if (s || (this._data.search.str = r, this._data.search.dom = E(), this._data.search.res = [], this._data.search.opn = [], this._data.search.som = t, this._data.search.smc = a), c = new E.vakata.search(r, !0, {
                         caseSensitive: n.case_sensitive,
                         fuzzy: n.fuzzy
-                    }), E.each(o[i || E.jstree.root].children_d, function(e, t) {
-                        var i = o[t];
+                    }), E.each(d[i || E.jstree.root].children_d, function(e, t) {
+                        var i = d[t];
                         i.text && !i.state.hidden && (!n.search_leaves_only || i.state.loaded && 0 === i.children.length) && (n.search_callback && n.search_callback.call(this, r, i) || !n.search_callback && c.search(i.text).isMatch) && (l.push(t), h = h.concat(i.parents))
                     }), l.length) {
-                    for (_ = 0, g = (h = E.vakata.array_unique(h)).length; _ < g; _++) h[_] !== E.jstree.root && o[h[_]] && !0 === this.open_node(h[_], null, 0) && this._data.search.opn.push(h[_]);
+                    for (_ = 0, g = (h = E.vakata.array_unique(h)).length; _ < g; _++) h[_] !== E.jstree.root && d[h[_]] && !0 === this.open_node(h[_], null, 0) && this._data.search.opn.push(h[_]);
                     s ? (this._data.search.dom = this._data.search.dom.add(E(this.element[0].querySelectorAll("#" + E.map(l, function(e) {
                         return -1 !== "0123456789".indexOf(e[0]) ? "\\3" + e[0] + " " + e.substr(1).replace(E.jstree.idregex, "\\$&") : e.replace(E.jstree.idregex, "\\$&")
                     }).join(", #")))), this._data.search.res = E.vakata.array_unique(this._data.search.res.concat(l))) : (this._data.search.dom = E(this.element[0].querySelectorAll("#" + E.map(l, function(e) {
                         return -1 !== "0123456789".indexOf(e[0]) ? "\\3" + e[0] + " " + e.substr(1).replace(E.jstree.idregex, "\\$&") : e.replace(E.jstree.idregex, "\\$&")
                     }).join(", #"))), this._data.search.res = l), this._data.search.dom.children(".jstree-anchor").addClass("jstree-search")
                 }
                 this.trigger("search", {
@@ -2872,15 +2873,15 @@
                     nodes: this._data.search.dom,
                     str: this._data.search.str,
                     res: this._data.search.res
                 }), this._data.search.res.length && (this._data.search.dom = E(this.element[0].querySelectorAll("#" + E.map(this._data.search.res, function(e) {
                     return -1 !== "0123456789".indexOf(e[0]) ? "\\3" + e[0] + " " + e.substr(1).replace(E.jstree.idregex, "\\$&") : e.replace(E.jstree.idregex, "\\$&")
                 }).join(", #"))), this._data.search.dom.children(".jstree-anchor").removeClass("jstree-search")), this._data.search.str = "", this._data.search.res = [], this._data.search.opn = [], this._data.search.dom = E()
             }, this.redraw_node = function(e, t, i, r) {
-                if ((e = d.redraw_node.apply(this, arguments)) && -1 !== E.inArray(e.id, this._data.search.res)) {
+                if ((e = o.redraw_node.apply(this, arguments)) && -1 !== E.inArray(e.id, this._data.search.res)) {
                     for (var s, a, n = null, s = 0, a = e.childNodes.length; s < a; s++)
                         if (e.childNodes[s] && e.childNodes[s].className && -1 !== e.childNodes[s].className.indexOf("jstree-anchor")) {
                             n = e.childNodes[s];
                             break
                         } n && (n.className += " jstree-search")
                 }
                 return e
@@ -2908,21 +2909,21 @@
                 if (!m.fuzzy) return {
                     isMatch: !1,
                     score: 1
                 };
                 var t, i, r = e.length,
                     s = j,
                     a = e.indexOf(p, v),
-                    n, d, o = k + r,
+                    n, o, d = k + r,
                     c, l, h, _, g, u = 1,
                     f = [];
                 for (-1 !== a && (s = Math.min(x(0, a), s), -1 !== (a = e.lastIndexOf(p, v + k)) && (s = Math.min(x(0, a), s))), a = -1, t = 0; t < k; t++) {
-                    n = 0, d = o;
-                    while (n < d) x(t, v + d) <= s ? n = d : o = d, d = Math.floor((o - n) / 2 + n);
-                    for (o = d, l = Math.max(1, v - d + 1), h = Math.min(v + d, r) + k, (_ = new Array(h + 2))[h + 1] = (1 << t) - 1, i = h; l <= i; i--)
+                    n = 0, o = d;
+                    while (n < o) x(t, v + o) <= s ? n = o : d = o, o = Math.floor((d - n) / 2 + n);
+                    for (d = o, l = Math.max(1, v - o + 1), h = Math.min(v + o, r) + k, (_ = new Array(h + 2))[h + 1] = (1 << t) - 1, i = h; l <= i; i--)
                         if (g = y[e.charAt(i - 1)], _[i] = 0 === t ? (_[i + 1] << 1 | 1) & g : (_[i + 1] << 1 | 1) & g | (c[i + 1] | c[i]) << 1 | 1 | c[i + 1], _[i] & b && (u = x(t, i - 1)) <= s) {
                             if (s = u, f.push(a = i - 1), !(v < a)) break;
                             l = Math.max(1, 2 * v - a)
                         } if (x(t + 1, v) > s) break;
                     c = _
                 }
                 return {
@@ -3020,43 +3021,43 @@
                         if ("default" !== i && i !== E.jstree.root && t.types.hasOwnProperty(i))
                             for (r in t.types.default) t.types.default.hasOwnProperty(r) && t.types[i][r] === P && (t.types[i][r] = t.types.default[r]);
                 l.init.call(this, e, t), this._model.data[E.jstree.root].type = E.jstree.root
             }, this.refresh = function(e, t) {
                 l.refresh.call(this, e, t), this._model.data[E.jstree.root].type = E.jstree.root
             }, this.bind = function() {
                 this.element.on("model.jstree", function(e, t) {
-                    for (var i = this._model.data, r = t.nodes, s = this.settings.types, a, n, d = "default", o, a = 0, n = r.length; a < n; a++) {
-                        if (d = "default", i[r[a]].original && i[r[a]].original.type && s[i[r[a]].original.type] && (d = i[r[a]].original.type), i[r[a]].data && i[r[a]].data.jstree && i[r[a]].data.jstree.type && s[i[r[a]].data.jstree.type] && (d = i[r[a]].data.jstree.type), i[r[a]].type = d, !0 === i[r[a]].icon && s[d].icon !== P && (i[r[a]].icon = s[d].icon), s[d].li_attr !== P && "object" == typeof s[d].li_attr)
-                            for (o in s[d].li_attr) s[d].li_attr.hasOwnProperty(o) && "id" !== o && (i[r[a]].li_attr[o] === P ? i[r[a]].li_attr[o] = s[d].li_attr[o] : "class" === o && (i[r[a]].li_attr.class = s[d].li_attr.class + " " + i[r[a]].li_attr.class));
-                        if (s[d].a_attr !== P && "object" == typeof s[d].a_attr)
-                            for (o in s[d].a_attr) s[d].a_attr.hasOwnProperty(o) && "id" !== o && (i[r[a]].a_attr[o] === P ? i[r[a]].a_attr[o] = s[d].a_attr[o] : "href" === o && "#" === i[r[a]].a_attr[o] ? i[r[a]].a_attr.href = s[d].a_attr.href : "class" === o && (i[r[a]].a_attr.class = s[d].a_attr.class + " " + i[r[a]].a_attr.class))
+                    for (var i = this._model.data, r = t.nodes, s = this.settings.types, a, n, o = "default", d, a = 0, n = r.length; a < n; a++) {
+                        if (o = "default", i[r[a]].original && i[r[a]].original.type && s[i[r[a]].original.type] && (o = i[r[a]].original.type), i[r[a]].data && i[r[a]].data.jstree && i[r[a]].data.jstree.type && s[i[r[a]].data.jstree.type] && (o = i[r[a]].data.jstree.type), i[r[a]].type = o, !0 === i[r[a]].icon && s[o].icon !== P && (i[r[a]].icon = s[o].icon), s[o].li_attr !== P && "object" == typeof s[o].li_attr)
+                            for (d in s[o].li_attr) s[o].li_attr.hasOwnProperty(d) && "id" !== d && (i[r[a]].li_attr[d] === P ? i[r[a]].li_attr[d] = s[o].li_attr[d] : "class" === d && (i[r[a]].li_attr.class = s[o].li_attr.class + " " + i[r[a]].li_attr.class));
+                        if (s[o].a_attr !== P && "object" == typeof s[o].a_attr)
+                            for (d in s[o].a_attr) s[o].a_attr.hasOwnProperty(d) && "id" !== d && (i[r[a]].a_attr[d] === P ? i[r[a]].a_attr[d] = s[o].a_attr[d] : "href" === d && "#" === i[r[a]].a_attr[d] ? i[r[a]].a_attr.href = s[o].a_attr.href : "class" === d && (i[r[a]].a_attr.class = s[o].a_attr.class + " " + i[r[a]].a_attr.class))
                     }
                     i[E.jstree.root].type = E.jstree.root
                 }.bind(this)), l.bind.call(this)
             }, this.get_json = function(e, t, i) {
                 var r, s, a = this._model.data,
                     n = t ? E.extend(!0, {}, t, {
                         no_id: !1
                     }) : {},
-                    d = l.get_json.call(this, e, n, i);
-                if (!1 === d) return !1;
-                if (E.vakata.is_array(d))
-                    for (r = 0, s = d.length; r < s; r++) d[r].type = (d[r].id || 0 === d[r].id) && a[d[r].id] && a[d[r].id].type ? a[d[r].id].type : "default", t && t.no_id && (delete d[r].id, d[r].li_attr && d[r].li_attr.id && delete d[r].li_attr.id, d[r].a_attr && d[r].a_attr.id && delete d[r].a_attr.id);
-                else d.type = (d.id || 0 === d.id) && a[d.id] && a[d.id].type ? a[d.id].type : "default", t && t.no_id && (d = this._delete_ids(d));
-                return d
+                    o = l.get_json.call(this, e, n, i);
+                if (!1 === o) return !1;
+                if (E.vakata.is_array(o))
+                    for (r = 0, s = o.length; r < s; r++) o[r].type = (o[r].id || 0 === o[r].id) && a[o[r].id] && a[o[r].id].type ? a[o[r].id].type : "default", t && t.no_id && (delete o[r].id, o[r].li_attr && o[r].li_attr.id && delete o[r].li_attr.id, o[r].a_attr && o[r].a_attr.id && delete o[r].a_attr.id);
+                else o.type = (o.id || 0 === o.id) && a[o.id] && a[o.id].type ? a[o.id].type : "default", t && t.no_id && (o = this._delete_ids(o));
+                return o
             }, this._delete_ids = function(e) {
                 if (E.vakata.is_array(e)) {
                     for (var t = 0, i = e.length; t < i; t++) e[t] = this._delete_ids(e[t]);
                     return e
                 }
                 return delete e.id, e.li_attr && e.li_attr.id && delete e.li_attr.id, e.a_attr && e.a_attr.id && delete e.a_attr.id, e.children && E.vakata.is_array(e.children) && (e.children = this._delete_ids(e.children)), e
             }, this.check = function(e, t, i, r, s) {
                 if (!1 === l.check.call(this, e, t, i, r, s)) return !1;
                 t = t && (t.id || 0 === t.id) ? t : this.get_node(t), i = i && (i.id || 0 === i.id) ? i : this.get_node(i);
-                var a, n, d, o, c, a = (a = t && (t.id || 0 === t.id) ? s && s.origin ? s.origin : E.jstree.reference(t.id) : null) && a._model && a._model.data ? a._model.data : null;
+                var a, n, o, d, c, a = (a = t && (t.id || 0 === t.id) ? s && s.origin ? s.origin : E.jstree.reference(t.id) : null) && a._model && a._model.data ? a._model.data : null;
                 switch (e) {
                     case "create_node":
                     case "move_node":
                     case "copy_node":
                         if ("move_node" !== e || -1 === E.inArray(t.id, i.children)) {
                             if ((n = this.get_rules(i)).max_children !== P && -1 !== n.max_children && n.max_children === i.children.length) return !(this._data.core.last_error = {
                                 error: "check",
@@ -3079,77 +3080,77 @@
                                     chk: e,
                                     pos: r,
                                     obj: !(!t || !t.id && 0 !== t.id) && t.id,
                                     par: !(!i || !i.id && 0 !== i.id) && i.id
                                 })
                             });
                             if (a && t.children_d && t.parents) {
-                                for (o = d = 0, c = t.children_d.length; o < c; o++) d = Math.max(d, a[t.children_d[o]].parents.length);
-                                d = d - t.parents.length + 1
-                            }(d <= 0 || d === P) && (d = 1);
+                                for (d = o = 0, c = t.children_d.length; d < c; d++) o = Math.max(o, a[t.children_d[d]].parents.length);
+                                o = o - t.parents.length + 1
+                            }(o <= 0 || o === P) && (o = 1);
                             do {
-                                if (n.max_depth !== P && -1 !== n.max_depth && n.max_depth < d) return !(this._data.core.last_error = {
+                                if (n.max_depth !== P && -1 !== n.max_depth && n.max_depth < o) return !(this._data.core.last_error = {
                                     error: "check",
                                     plugin: "types",
                                     id: "types_03",
                                     reason: "max_depth prevents function: " + e,
                                     data: JSON.stringify({
                                         chk: e,
                                         pos: r,
                                         obj: !(!t || !t.id && 0 !== t.id) && t.id,
                                         par: !(!i || !i.id && 0 !== i.id) && i.id
                                     })
                                 });
-                                i = this.get_node(i.parent), n = this.get_rules(i), d++
+                                i = this.get_node(i.parent), n = this.get_rules(i), o++
                             } while (i)
                         }
                 }
                 return !0
             }, this.get_rules = function(e) {
                 if (!(e = this.get_node(e))) return !1;
                 var e = this.get_type(e, !0);
                 return e.max_depth === P && (e.max_depth = -1), e.max_children === P && (e.max_children = -1), e.valid_children === P && (e.valid_children = -1), e
             }, this.get_type = function(e, t) {
                 return !!(e = this.get_node(e)) && (t ? E.extend({
                     type: e.type
                 }, this.settings.types[e.type]) : e.type)
             }, this.set_type = function(e, t) {
                 var i = this._model.data,
-                    r, s, a, n, d, o, c, l;
+                    r, s, a, n, o, d, c, l;
                 if (E.vakata.is_array(e)) {
                     for (s = 0, a = (e = e.slice()).length; s < a; s++) this.set_type(e[s], t);
                     return !0
                 }
                 if (r = this.settings.types, e = this.get_node(e), !r[t] || !e) return !1;
-                if ((c = this.get_node(e, !0)) && c.length && (l = c.children(".jstree-anchor")), n = e.type, d = this.get_icon(e), e.type = t, !0 !== d && r[n] && (r[n].icon === P || d !== r[n].icon) || this.set_icon(e, r[t].icon === P || r[t].icon), r[n] && r[n].li_attr !== P && "object" == typeof r[n].li_attr)
-                    for (o in r[n].li_attr) r[n].li_attr.hasOwnProperty(o) && "id" !== o && ("class" === o ? (i[e.id].li_attr.class = (i[e.id].li_attr.class || "").replace(r[n].li_attr[o], ""), c && c.removeClass(r[n].li_attr[o])) : i[e.id].li_attr[o] === r[n].li_attr[o] && (i[e.id].li_attr[o] = null, c && c.removeAttr(o)));
+                if ((c = this.get_node(e, !0)) && c.length && (l = c.children(".jstree-anchor")), n = e.type, o = this.get_icon(e), e.type = t, !0 !== o && r[n] && (r[n].icon === P || o !== r[n].icon) || this.set_icon(e, r[t].icon === P || r[t].icon), r[n] && r[n].li_attr !== P && "object" == typeof r[n].li_attr)
+                    for (d in r[n].li_attr) r[n].li_attr.hasOwnProperty(d) && "id" !== d && ("class" === d ? (i[e.id].li_attr.class = (i[e.id].li_attr.class || "").replace(r[n].li_attr[d], ""), c && c.removeClass(r[n].li_attr[d])) : i[e.id].li_attr[d] === r[n].li_attr[d] && (i[e.id].li_attr[d] = null, c && c.removeAttr(d)));
                 if (r[n] && r[n].a_attr !== P && "object" == typeof r[n].a_attr)
-                    for (o in r[n].a_attr) r[n].a_attr.hasOwnProperty(o) && "id" !== o && ("class" === o ? (i[e.id].a_attr.class = (i[e.id].a_attr.class || "").replace(r[n].a_attr[o], ""), l && l.removeClass(r[n].a_attr[o])) : i[e.id].a_attr[o] === r[n].a_attr[o] && ("href" === o ? (i[e.id].a_attr[o] = "#", l && l.attr("href", "#")) : (delete i[e.id].a_attr[o], l && l.removeAttr(o))));
+                    for (d in r[n].a_attr) r[n].a_attr.hasOwnProperty(d) && "id" !== d && ("class" === d ? (i[e.id].a_attr.class = (i[e.id].a_attr.class || "").replace(r[n].a_attr[d], ""), l && l.removeClass(r[n].a_attr[d])) : i[e.id].a_attr[d] === r[n].a_attr[d] && ("href" === d ? (i[e.id].a_attr[d] = "#", l && l.attr("href", "#")) : (delete i[e.id].a_attr[d], l && l.removeAttr(d))));
                 if (r[t].li_attr !== P && "object" == typeof r[t].li_attr)
-                    for (o in r[t].li_attr) r[t].li_attr.hasOwnProperty(o) && "id" !== o && (i[e.id].li_attr[o] === P ? (i[e.id].li_attr[o] = r[t].li_attr[o], c && ("class" === o ? c.addClass(r[t].li_attr[o]) : c.attr(o, r[t].li_attr[o]))) : "class" === o && (i[e.id].li_attr.class = r[t].li_attr[o] + " " + i[e.id].li_attr.class, c && c.addClass(r[t].li_attr[o])));
+                    for (d in r[t].li_attr) r[t].li_attr.hasOwnProperty(d) && "id" !== d && (i[e.id].li_attr[d] === P ? (i[e.id].li_attr[d] = r[t].li_attr[d], c && ("class" === d ? c.addClass(r[t].li_attr[d]) : c.attr(d, r[t].li_attr[d]))) : "class" === d && (i[e.id].li_attr.class = r[t].li_attr[d] + " " + i[e.id].li_attr.class, c && c.addClass(r[t].li_attr[d])));
                 if (r[t].a_attr !== P && "object" == typeof r[t].a_attr)
-                    for (o in r[t].a_attr) r[t].a_attr.hasOwnProperty(o) && "id" !== o && (i[e.id].a_attr[o] === P ? (i[e.id].a_attr[o] = r[t].a_attr[o], l && ("class" === o ? l.addClass(r[t].a_attr[o]) : l.attr(o, r[t].a_attr[o]))) : "href" === o && "#" === i[e.id].a_attr[o] ? (i[e.id].a_attr.href = r[t].a_attr.href, l && l.attr("href", r[t].a_attr.href)) : "class" === o && (i[e.id].a_attr.class = r[t].a_attr.class + " " + i[e.id].a_attr.class, l && l.addClass(r[t].a_attr[o])));
+                    for (d in r[t].a_attr) r[t].a_attr.hasOwnProperty(d) && "id" !== d && (i[e.id].a_attr[d] === P ? (i[e.id].a_attr[d] = r[t].a_attr[d], l && ("class" === d ? l.addClass(r[t].a_attr[d]) : l.attr(d, r[t].a_attr[d]))) : "href" === d && "#" === i[e.id].a_attr[d] ? (i[e.id].a_attr.href = r[t].a_attr.href, l && l.attr("href", r[t].a_attr.href)) : "class" === d && (i[e.id].a_attr.class = r[t].a_attr.class + " " + i[e.id].a_attr.class, l && l.addClass(r[t].a_attr[d])));
                 return !0
             }
         }, E.jstree.defaults.unique = {
             case_sensitive: !1,
             trim_whitespace: !1,
             duplicate: function(e, t) {
                 return e + " (" + t + ")"
             }
         }, E.jstree.plugins.unique = function(e, f) {
             this.check = function(e, t, i, r, s) {
                 if (!1 === f.check.call(this, e, t, i, r, s)) return !1;
                 if (t = t && (t.id || 0 === t.id) ? t : this.get_node(t), !(i = i && (i.id || 0 === i.id) ? i : this.get_node(i)) || !i.children) return !0;
-                for (var a = "rename_node" === e ? r : t.text, n = [], d = this.settings.unique.case_sensitive, o = this.settings.unique.trim_whitespace, c = this._model.data, l, h, _, l = 0, h = i.children.length; l < h; l++) _ = c[i.children[l]].text, d || (_ = _.toLowerCase()), o && (_ = _.replace(/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g, "")), n.push(_);
-                switch (d || (a = a.toLowerCase()), o && (a = a.replace(/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g, "")), e) {
+                for (var a = "rename_node" === e ? r : t.text, n = [], o = this.settings.unique.case_sensitive, d = this.settings.unique.trim_whitespace, c = this._model.data, l, h, _, l = 0, h = i.children.length; l < h; l++) _ = c[i.children[l]].text, o || (_ = _.toLowerCase()), d && (_ = _.replace(/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g, "")), n.push(_);
+                switch (o || (a = a.toLowerCase()), d && (a = a.replace(/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g, "")), e) {
                     case "delete_node":
                         return !0;
                     case "rename_node":
-                        return _ = t.text || "", d || (_ = _.toLowerCase()), o && (_ = _.replace(/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g, "")), (l = -1 === E.inArray(a, n) || t.text && _ === a) || (this._data.core.last_error = {
+                        return _ = t.text || "", o || (_ = _.toLowerCase()), d && (_ = _.replace(/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g, "")), (l = -1 === E.inArray(a, n) || t.text && _ === a) || (this._data.core.last_error = {
                             error: "check",
                             plugin: "unique",
                             id: "unique_01",
                             reason: "Child with name " + a + " already exists. Preventing: " + e,
                             data: JSON.stringify({
                                 chk: e,
                                 pos: r,
@@ -3199,17 +3200,17 @@
                 }
                 return !0
             }, this.create_node = function(e, t, i, r, s) {
                 if (!t || "object" == typeof t && t.text === P) {
                     if (null === e && (e = E.jstree.root), !(e = this.get_node(e))) return f.create_node.call(this, e, t, i, r, s);
                     if (!(i = i === P ? "last" : i).toString().match(/^(before|after)$/) && !s && !this.is_loaded(e)) return f.create_node.call(this, e, t, i, r, s);
                     t = t || {};
-                    for (var a, n, d, o, c, l = this._model.data, h = this.settings.unique.case_sensitive, _ = this.settings.unique.trim_whitespace, g = this.settings.unique.duplicate, u, n = a = this.get_string("New node"), d = [], o = 0, c = e.children.length; o < c; o++) u = l[e.children[o]].text, h || (u = u.toLowerCase()), _ && (u = u.replace(/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g, "")), d.push(u);
-                    o = 1, u = n, h || (u = u.toLowerCase()), _ && (u = u.replace(/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g, ""));
-                    while (-1 !== E.inArray(u, d)) u = n = g.call(this, a, ++o).toString(), h || (u = u.toLowerCase()), _ && (u = u.replace(/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g, ""));
+                    for (var a, n, o, d, c, l = this._model.data, h = this.settings.unique.case_sensitive, _ = this.settings.unique.trim_whitespace, g = this.settings.unique.duplicate, u, n = a = this.get_string("New node"), o = [], d = 0, c = e.children.length; d < c; d++) u = l[e.children[d]].text, h || (u = u.toLowerCase()), _ && (u = u.replace(/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g, "")), o.push(u);
+                    d = 1, u = n, h || (u = u.toLowerCase()), _ && (u = u.replace(/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g, ""));
+                    while (-1 !== E.inArray(u, o)) u = n = g.call(this, a, ++d).toString(), h || (u = u.toLowerCase()), _ && (u = u.replace(/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g, ""));
                     t.text = n
                 }
                 return f.create_node.call(this, e, t, i, r, s)
             }
         };
         var j = b.createElement("DIV");
         if (j.setAttribute("unselectable", "on"), j.setAttribute("role", "presentation"), j.className = "jstree-wholerow", j.innerHTML = "&#160;", E.jstree.plugins.wholerow = function(e, a) {
```

### Comparing `ckanext-unfold-1.0.0/ckanext/unfold/plugin.py` & `ckanext_unfold-1.0.1/ckanext/unfold/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import ckanext.unfold.adapters as unf_adapters
 import ckanext.unfold.utils as unf_utils
 from ckanext.unfold.logic.schema import get_preview_schema
 
 
 @tk.blanket.actions
+@tk.blanket.validators
 class UnfoldPlugin(plugins.SingletonPlugin):
     plugins.implements(plugins.IConfigurer)
     plugins.implements(plugins.IResourceView, inherit=True)
     plugins.implements(plugins.IResourceController, inherit=True)
 
     # IConfigurer
 
@@ -47,18 +48,18 @@
         return "unfold_form.html"
 
     # IResourceController
 
     def before_resource_update(
         self, context: Context, current: dict[str, Any], resource: dict[str, Any]
     ) -> None:
-        if resource["url_type"] == "upload" and not resource["upload"]:
+        if resource.get("url_type") == "upload" and not resource.get("upload"):
             return
 
-        if resource["url_type"] == "url" and current["url"] == resource["url"]:
+        if resource.get("url_type") == "url" and current["url"] == resource["url"]:
             return
 
         unf_utils.delete_archive_structure(resource["id"])
 
     def before_resource_delete(
         self,
         context: Context,
```

### Comparing `ckanext-unfold-1.0.0/ckanext/unfold/templates/unfold_preview.html` & `ckanext_unfold-1.0.1/ckanext/unfold/templates/unfold_preview.html`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             <button class="btn btn-primary" id="jstree-search-clear">
                 <i class="fa fa-close"></i>
                 {{ _("Clear") }}
             </button>
         </div>
     </div>
 
-    <div id="archive-tree" data-module="unfold-init-jstree" data-module-resource-id="{{ resource.id }}">
+    <div id="archive-tree" data-module="unfold-init-jstree" data-module-resource-id="{{ resource.id }}" data-module-resource-view-id="{{ resource_view.id }}" >
         <div class="archive-tree--spinner">
             <img src="{{ h.url_for_static('/spinner.gif') }}" width="20">
             {{ _("The archive tree is currently being initialized. Please wait...") }}
         </div>
     </div>
 
     <div id="archive-tree-error" style="display: none">
```

### Comparing `ckanext-unfold-1.0.0/ckanext/unfold/utils.py` & `ckanext_unfold-1.0.1/ckanext/unfold/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import json
 import logging
 import math
 import pathlib
-from typing import Any, Optional
+from typing import Any
 
 import ckan.lib.uploader as uploader
 from ckan.lib.redis import connect_to_redis
 
 import ckanext.unfold.adapters as unf_adapters
 import ckanext.unfold.types as unf_types
 
@@ -120,15 +120,15 @@
     """Delete an archive structure from redis. Called on resource delete/update"""
     conn = connect_to_redis()
     conn.delete(f"ckanext:unfold:tree:{resource_id}")
     conn.close()
 
 
 def get_archive_tree(
-    resource: dict[str, Any]
+    resource: dict[str, Any], resource_view: dict[str, Any]
 ) -> list[unf_types.Node] | list[dict[str, Any]]:
     remote = False
 
     if resource.get("url_type") == "upload":
         upload = uploader.get_resource_uploader(resource)
         filepath = upload.get_path(resource["id"])
     else:
@@ -137,20 +137,17 @@
 
         filepath = resource["url"]
         remote = True
 
     tree = get_archive_structure(resource["id"])
 
     if not tree:
-        tree = parse_archive(resource["format"].lower(), filepath, remote)
-        save_archive_structure(tree, resource["id"])
+        res_format = resource["format"].lower()
 
-    return tree
+        if res_format not in unf_adapters.ADAPTERS:
+            raise TypeError(f"No adapter for `{res_format}` archives")
 
+        tree = unf_adapters.ADAPTERS[res_format](filepath, resource_view, remote=remote)
 
-def parse_archive(
-    fmt: str, filepath: str, remote: Optional[bool] = False
-) -> list[unf_types.Node]:
-    if fmt not in unf_adapters.ADAPTERS:
-        raise TypeError(f"No adapter for `{fmt}` archives")
+        save_archive_structure(tree, resource["id"])
 
-    return unf_adapters.ADAPTERS[fmt](filepath, remote=remote)
+    return tree
```

### Comparing `ckanext-unfold-1.0.0/ckanext_unfold.egg-info/PKG-INFO` & `ckanext_unfold-1.0.1/ckanext_unfold.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: ckanext-unfold
-Version: 1.0.0
+Version: 1.0.1
 Summary: Provides previews for multiple archive formats
 Home-page: https://github.com//ckanext-unfold
 Author: Oleksandr Cherniavskyi
 Author-email: mutantsan@gmail.com
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: rarfile==4.0
+Requires-Dist: py7zr==0.20.6
+Requires-Dist: rpmfile==1.1.1
+Requires-Dist: pydantic==2.3.0
 
 [![Tests](https://github.com/mutantsan/ckanext-unfold/workflows/Tests/badge.svg?branch=master)](https://github.com/mutantsan/ckanext-unfold/actions)
 
 # ckanext-unfold
 
-Preview for different archive formats
-### TODO
- - ~~implement remote support for tar, 7z~~
- - ~~add password support for all adapters~~
- - ~~refactor to show an error to user if something went wrong (no pass, request exp, corrupted or empty archive)~~
+Enhance your CKAN experience with our extension that enables seamless previews of various archive formats, ensuring easy access and efficient data management.
 
 
 ## What are the dependencies?
 
 Working with different archive formats requires different tools:
 
 ### RAR, CBR
@@ -63,14 +63,10 @@
 
 ### RPM
 
 We are using [`rpmfile`](https://github.com/srossross/rpmfile) library.
 
 If you want to use rpmfile with zstd compressed rpms, you'll need to install the [`zstandard`](https://pypi.org/project/zstandard/) module.
 
-## Config settings
-
-TODO
-
 ## License
 
 [AGPL](https://www.gnu.org/licenses/agpl-3.0.en.html)
```

### Comparing `ckanext-unfold-1.0.0/ckanext_unfold.egg-info/SOURCES.txt` & `ckanext_unfold-1.0.1/ckanext_unfold.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-unfold-1.0.0/pyproject.toml` & `ckanext_unfold-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-unfold-1.0.0/setup.cfg` & `ckanext_unfold-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-unfold
-version = 1.0.0
+version = 1.0.1
 description = Provides previews for multiple archive formats
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com//ckanext-unfold
 author = Oleksandr Cherniavskyi
 author_email = mutantsan@gmail.com
 license = AGPL
```

### Comparing `ckanext-unfold-1.0.0/setup.py` & `ckanext_unfold-1.0.1/setup.py`

 * *Files identical despite different names*

