# Comparing `tmp/advanced_input-0.1.1.tar.gz` & `tmp/advanced_input-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advanced_input-0.1.1.tar", last modified: Tue Apr 30 06:20:26 2024, max compression
+gzip compressed data, was "advanced_input-0.1.2.tar", last modified: Tue Apr 30 06:34:16 2024, max compression
```

## Comparing `advanced_input-0.1.1.tar` & `advanced_input-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 06:20:26.860340 advanced_input-0.1.1/
--rw-rw-rw-   0        0        0     1235 2020-07-21 09:29:29.000000 advanced_input-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1691 2024-04-30 06:20:26.860340 advanced_input-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1144 2024-04-26 06:22:56.000000 advanced_input-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 06:20:26.825369 advanced_input-0.1.1/advanced_input/
--rw-rw-rw-   0        0        0      415 2024-04-26 06:35:29.000000 advanced_input-0.1.1/advanced_input/__init__.py
--rw-rw-rw-   0        0        0      316 2024-04-25 10:42:38.000000 advanced_input-0.1.1/advanced_input/constants.py
--rw-rw-rw-   0        0        0     2914 2024-04-30 06:19:39.000000 advanced_input-0.1.1/advanced_input/input.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:20:26.859342 advanced_input-0.1.1/advanced_input.egg-info/
--rw-rw-rw-   0        0        0     1691 2024-04-30 06:20:26.000000 advanced_input-0.1.1/advanced_input.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-04-30 06:20:26.000000 advanced_input-0.1.1/advanced_input.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 06:20:26.000000 advanced_input-0.1.1/advanced_input.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-30 06:20:26.000000 advanced_input-0.1.1/advanced_input.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-12-08 11:06:28.000000 advanced_input-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      611 2024-04-30 06:20:26.861340 advanced_input-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 06:34:16.455799 advanced_input-0.1.2/
+-rw-rw-rw-   0        0        0     1235 2020-07-21 09:29:29.000000 advanced_input-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1691 2024-04-30 06:34:16.455278 advanced_input-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1144 2024-04-26 06:22:56.000000 advanced_input-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 06:34:16.441362 advanced_input-0.1.2/advanced_input/
+-rw-rw-rw-   0        0        0      415 2024-04-26 06:35:29.000000 advanced_input-0.1.2/advanced_input/__init__.py
+-rw-rw-rw-   0        0        0      316 2024-04-25 10:42:38.000000 advanced_input-0.1.2/advanced_input/constants.py
+-rw-rw-rw-   0        0        0     2914 2024-04-30 06:19:39.000000 advanced_input-0.1.2/advanced_input/input.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:34:16.454714 advanced_input-0.1.2/advanced_input.egg-info/
+-rw-rw-rw-   0        0        0     1691 2024-04-30 06:34:16.000000 advanced_input-0.1.2/advanced_input.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-04-30 06:34:16.000000 advanced_input-0.1.2/advanced_input.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 06:34:16.000000 advanced_input-0.1.2/advanced_input.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-30 06:34:16.000000 advanced_input-0.1.2/advanced_input.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-12-08 11:06:28.000000 advanced_input-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      640 2024-04-30 06:34:16.456796 advanced_input-0.1.2/setup.cfg
```

### Comparing `advanced_input-0.1.1/LICENSE` & `advanced_input-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `advanced_input-0.1.1/PKG-INFO` & `advanced_input-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advanced_input
-Version: 0.1.1
+Version: 0.1.2
 Summary: IO Extention
 Home-page: https://github.com/NightKey/advanced-input
 Author: Janthó Dávid
 Author-email: davidjantho@gmail.com
 Project-URL: Bug Tracker, https://github.com/NightKey/advanced-input/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `advanced_input-0.1.1/README.md` & `advanced_input-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `advanced_input-0.1.1/advanced_input/input.py` & `advanced_input-0.1.2/advanced_input/input.py`

 * *Files identical despite different names*

### Comparing `advanced_input-0.1.1/advanced_input.egg-info/PKG-INFO` & `advanced_input-0.1.2/advanced_input.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advanced_input
-Version: 0.1.1
+Version: 0.1.2
 Summary: IO Extention
 Home-page: https://github.com/NightKey/advanced-input
 Author: Janthó Dávid
 Author-email: davidjantho@gmail.com
 Project-URL: Bug Tracker, https://github.com/NightKey/advanced-input/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `advanced_input-0.1.1/setup.cfg` & `advanced_input-0.1.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6476 616e 6365 645f 696e 7075   = advanced_inpu
 00000020: 740d 0a76 6572 7369 6f6e 203d 2030 2e31  t..version = 0.1
-00000030: 2e31 0d0a 6175 7468 6f72 203d 204a 616e  .1..author = Jan
+00000030: 2e32 0d0a 6175 7468 6f72 203d 204a 616e  .2..author = Jan
 00000040: 7468 c3b3 2044 c3a1 7669 640d 0a61 7574  th.. D..vid..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6461 7669  hor_email = davi
 00000060: 646a 616e 7468 6f40 676d 6169 6c2e 636f  djantho@gmail.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2049 4f20 4578 7465 6e74 696f 6e0d 0a6c   IO Extention..l
 00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 000000a0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
@@ -27,13 +27,14 @@
 000001a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
 000001b0: 2050 7974 686f 6e20 3a3a 2033 0d0a 094c   Python :: 3...L
 000001c0: 6963 656e 7365 203a 3a20 4672 6565 7761  icense :: Freewa
 000001d0: 7265 0d0a 094f 7065 7261 7469 6e67 2053  re...Operating S
 000001e0: 7973 7465 6d20 3a3a 204d 6963 726f 736f  ystem :: Microso
 000001f0: 6674 203a 3a20 5769 6e64 6f77 730d 0a0d  ft :: Windows...
 00000200: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
-00000210: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
-00000220: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-00000230: 3e3d 332e 370d 0a0d 0a5b 6567 675f 696e  >=3.7....[egg_in
-00000240: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-00000250: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-00000260: 0a0d 0a                                  ...
+00000210: 6167 6573 203d 2066 696e 643a 0d0a 696e  ages = find:..in
+00000220: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
+00000230: 6120 3d20 5472 7565 2c0d 0a70 7974 686f  a = True,..pytho
+00000240: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
+00000250: 2e37 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  .7....[egg_info]
+00000260: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+00000270: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

