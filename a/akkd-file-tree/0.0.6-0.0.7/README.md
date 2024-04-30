# Comparing `tmp/akkd_file_tree-0.0.6.tar.gz` & `tmp/akkd_file_tree-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akkd_file_tree-0.0.6.tar", last modified: Sat Apr 27 21:29:01 2024, max compression
+gzip compressed data, was "akkd_file_tree-0.0.7.tar", last modified: Tue Apr 30 06:32:52 2024, max compression
```

## Comparing `akkd_file_tree-0.0.6.tar` & `akkd_file_tree-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 21:29:01.157032 akkd_file_tree-0.0.6/
--rw-rw-rw-   0        0        0       89 2024-04-27 20:20:29.000000 akkd_file_tree-0.0.6/AUTHORS.md
--rw-rw-rw-   0        0        0     1102 2024-04-27 20:20:29.000000 akkd_file_tree-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0      748 2024-04-27 21:29:01.157032 akkd_file_tree-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       56 2024-04-27 21:16:39.000000 akkd_file_tree-0.0.6/README.md
--rw-rw-rw-   0        0        0     1443 2024-04-27 21:29:01.158033 akkd_file_tree-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      659 2024-04-27 21:28:44.000000 akkd_file_tree-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 21:29:01.141443 akkd_file_tree-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-27 21:29:01.156025 akkd_file_tree-0.0.6/src/akkd_file_tree.egg-info/
--rw-rw-rw-   0        0        0      748 2024-04-27 21:29:01.000000 akkd_file_tree-0.0.6/src/akkd_file_tree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2024-04-27 21:29:01.000000 akkd_file_tree-0.0.6/src/akkd_file_tree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 21:29:01.000000 akkd_file_tree-0.0.6/src/akkd_file_tree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-27 21:29:01.000000 akkd_file_tree-0.0.6/src/akkd_file_tree.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-27 20:53:13.000000 akkd_file_tree-0.0.6/src/akkd_file_tree.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       86 2024-04-27 21:29:01.000000 akkd_file_tree-0.0.6/src/akkd_file_tree.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-27 21:29:01.000000 akkd_file_tree-0.0.6/src/akkd_file_tree.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-27 21:29:01.156025 akkd_file_tree-0.0.6/src/file_tree/
--rw-rw-rw-   0        0        0       72 2024-04-27 20:25:40.000000 akkd_file_tree-0.0.6/src/file_tree/__init__.py
--rw-rw-rw-   0        0        0    33851 2024-04-27 20:20:29.000000 akkd_file_tree-0.0.6/src/file_tree/_file_tree.py
--rw-rw-rw-   0        0        0     1013 2024-04-27 20:20:29.000000 akkd_file_tree-0.0.6/src/file_tree/utils.py
--rw-rw-rw-   0        0        0       22 2024-04-27 21:28:51.000000 akkd_file_tree-0.0.6/src/file_tree/version.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:32:52.282780 akkd_file_tree-0.0.7/
+-rw-rw-rw-   0        0        0       60 2024-04-30 06:31:19.000000 akkd_file_tree-0.0.7/AUTHORS.md
+-rw-rw-rw-   0        0        0     1102 2024-04-27 20:20:29.000000 akkd_file_tree-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      981 2024-04-30 06:32:52.282780 akkd_file_tree-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2024-04-27 21:16:39.000000 akkd_file_tree-0.0.7/README.md
+-rw-rw-rw-   0        0        0     1609 2024-04-30 06:32:52.284779 akkd_file_tree-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      659 2024-04-27 21:28:44.000000 akkd_file_tree-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:32:52.268781 akkd_file_tree-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-30 06:32:52.281780 akkd_file_tree-0.0.7/src/akkd_file_tree.egg-info/
+-rw-rw-rw-   0        0        0      981 2024-04-30 06:32:52.000000 akkd_file_tree-0.0.7/src/akkd_file_tree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2024-04-30 06:32:52.000000 akkd_file_tree-0.0.7/src/akkd_file_tree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 06:32:52.000000 akkd_file_tree-0.0.7/src/akkd_file_tree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-30 06:32:52.000000 akkd_file_tree-0.0.7/src/akkd_file_tree.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-27 20:53:13.000000 akkd_file_tree-0.0.7/src/akkd_file_tree.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       75 2024-04-30 06:32:52.000000 akkd_file_tree-0.0.7/src/akkd_file_tree.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-30 06:32:52.000000 akkd_file_tree-0.0.7/src/akkd_file_tree.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 06:32:52.280782 akkd_file_tree-0.0.7/src/file_tree/
+-rw-rw-rw-   0        0        0      122 2024-04-30 06:31:19.000000 akkd_file_tree-0.0.7/src/file_tree/__init__.py
+-rw-rw-rw-   0        0        0    31497 2024-04-30 06:31:19.000000 akkd_file_tree-0.0.7/src/file_tree/_file_tree.py
+-rw-rw-rw-   0        0        0       22 2024-04-30 06:31:19.000000 akkd_file_tree-0.0.7/src/file_tree/version.py
```

### Comparing `akkd_file_tree-0.0.6/LICENSE.txt` & `akkd_file_tree-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `akkd_file_tree-0.0.6/setup.cfg` & `akkd_file_tree-0.0.7/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -9,83 +9,93 @@
 00000080: 0d0a 6175 7468 6f72 203d 204d 6963 6861  ..author = Micha
 00000090: 656c 2042 6172 726f 730d 0a61 7574 686f  el Barros..autho
 000000a0: 725f 656d 6169 6c20 3d20 6d69 6368 6165  r_email = michae
 000000b0: 6c63 6261 7272 6f73 4067 6d61 696c 2e63  lcbarros@gmail.c
 000000c0: 6f6d 0d0a 6c69 6365 6e73 6520 3d20 4d49  om..license = MI
 000000d0: 540d 0a6c 6f6e 675f 6465 7363 7269 7074  T..long_descript
 000000e0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
-000000f0: 4d45 2e72 7374 0d0a 6c6f 6e67 5f64 6573  ME.rst..long_des
-00000100: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
-00000110: 5f74 7970 6520 3d20 7465 7874 2f78 2d72  _type = text/x-r
-00000120: 7374 3b20 6368 6172 7365 743d 5554 462d  st; charset=UTF-
-00000130: 380d 0a75 726c 203d 2068 7474 7073 3a2f  8..url = https:/
-00000140: 2f67 6974 6875 622e 636f 6d2f 7079 7363  /github.com/pysc
-00000150: 6166 666f 6c64 2f70 7973 6361 6666 6f6c  affold/pyscaffol
-00000160: 642f 0d0a 7072 6f6a 6563 745f 7572 6c73  d/..project_urls
-00000170: 203d 200d 0a09 446f 6375 6d65 6e74 6174   = ...Documentat
-00000180: 696f 6e20 3d20 6874 7470 733a 2f2f 7079  ion = https://py
-00000190: 7363 6166 666f 6c64 2e6f 7267 2f0d 0a70  scaffold.org/..p
-000001a0: 6c61 7466 6f72 6d73 203d 2061 6e79 0d0a  latforms = any..
-000001b0: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-000001c0: 0944 6576 656c 6f70 6d65 6e74 2053 7461  .Development Sta
-000001d0: 7475 7320 3a3a 2034 202d 2042 6574 610d  tus :: 4 - Beta.
-000001e0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000001f0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000200: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a7a  ....[options]..z
-00000210: 6970 5f73 6166 6520 3d20 4661 6c73 650d  ip_safe = False.
-00000220: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
-00000230: 5f6e 616d 6573 7061 6365 3a0d 0a69 6e63  _namespace:..inc
-00000240: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
-00000250: 6120 3d20 5472 7565 0d0a 7061 636b 6167  a = True..packag
-00000260: 655f 6469 7220 3d20 0d0a 093d 7372 630d  e_dir = ...=src.
-00000270: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-00000280: 203d 203e 3d33 2e36 0d0a 696e 7374 616c   = >=3.6..instal
-00000290: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
-000002a0: 696d 706f 7274 6c69 622d 6d65 7461 6461  importlib-metada
-000002b0: 7461 3b20 7079 7468 6f6e 5f76 6572 7369  ta; python_versi
-000002c0: 6f6e 3c22 332e 3822 0d0a 0963 6c69 636b  on<"3.8"...click
-000002d0: 0d0a 0963 6f6c 720d 0a0d 0a5b 6f70 7469  ...colr....[opti
-000002e0: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
-000002f0: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
-00000300: 0a65 7863 6c75 6465 203d 200d 0a09 7465  .exclude = ...te
-00000310: 7374 730d 0a0d 0a5b 6f70 7469 6f6e 732e  sts....[options.
-00000320: 6578 7472 6173 5f72 6571 7569 7265 5d0d  extras_require].
-00000330: 0a74 6573 7469 6e67 203d 200d 0a09 7079  .testing = ...py
-00000340: 7465 7374 0d0a 0970 7974 6573 742d 636f  test...pytest-co
-00000350: 760d 0a0d 0a5b 6f70 7469 6f6e 732e 656e  v....[options.en
-00000360: 7472 795f 706f 696e 7473 5d0d 0a63 6f6e  try_points]..con
-00000370: 736f 6c65 5f73 6372 6970 7473 203d 200d  sole_scripts = .
-00000380: 0a09 6669 6c65 2d74 7265 6520 3d20 6669  ..file-tree = fi
-00000390: 6c65 5f74 7265 652e 5f66 696c 655f 7472  le_tree._file_tr
-000003a0: 6565 3a72 756e 0d0a 0d0a 5b74 6f6f 6c3a  ee:run....[tool:
-000003b0: 7079 7465 7374 5d0d 0a61 6464 6f70 7473  pytest]..addopts
-000003c0: 203d 200d 0a09 2d2d 636f 7620 6669 6c65   = ...--cov file
-000003d0: 5f74 7265 6520 2d2d 636f 762d 7265 706f  _tree --cov-repo
-000003e0: 7274 2074 6572 6d2d 6d69 7373 696e 670d  rt term-missing.
-000003f0: 0a09 2d2d 7665 7262 6f73 650d 0a6e 6f72  ..--verbose..nor
-00000400: 6563 7572 7365 6469 7273 203d 200d 0a09  ecursedirs = ...
-00000410: 6469 7374 0d0a 0962 7569 6c64 0d0a 092e  dist...build....
-00000420: 746f 780d 0a74 6573 7470 6174 6873 203d  tox..testpaths =
-00000430: 2074 6573 7473 0d0a 0d0a 5b61 6c69 6173   tests....[alias
-00000440: 6573 5d0d 0a64 6973 7473 203d 2073 6469  es]..dists = sdi
-00000450: 7374 2062 6469 7374 5f77 6865 656c 0d0a  st bdist_wheel..
-00000460: 0d0a 5b64 6576 7069 3a75 706c 6f61 645d  ..[devpi:upload]
-00000470: 0d0a 6e6f 2d76 6373 203d 2031 0d0a 666f  ..no-vcs = 1..fo
-00000480: 726d 6174 7320 3d20 6264 6973 745f 7768  rmats = bdist_wh
-00000490: 6565 6c0d 0a0d 0a5b 666c 616b 6538 5d0d  eel....[flake8].
-000004a0: 0a6d 6178 2d6c 696e 652d 6c65 6e67 7468  .max-line-length
-000004b0: 203d 2038 380d 0a65 7874 656e 642d 6967   = 88..extend-ig
-000004c0: 6e6f 7265 203d 2045 3230 332c 2057 3530  nore = E203, W50
-000004d0: 330d 0a65 7863 6c75 6465 203d 200d 0a09  3..exclude = ...
-000004e0: 2e74 6f78 0d0a 0962 7569 6c64 0d0a 0964  .tox...build...d
-000004f0: 6973 740d 0a09 2e65 6767 730d 0a09 646f  ist....eggs...do
-00000500: 6373 2f63 6f6e 662e 7079 0d0a 0d0a 5b70  cs/conf.py....[p
-00000510: 7973 6361 6666 6f6c 645d 0d0a 7665 7273  yscaffold]..vers
-00000520: 696f 6e20 3d20 342e 3061 330d 0a70 6163  ion = 4.0a3..pac
-00000530: 6b61 6765 203d 2066 696c 655f 7472 6565  kage = file_tree
-00000540: 0d0a 6578 7465 6e73 696f 6e73 203d 200d  ..extensions = .
-00000550: 0a09 6e6f 5f70 7970 726f 6a65 6374 0d0a  ..no_pyproject..
-00000560: 096e 6f5f 736b 656c 6574 6f6e 0d0a 096e  .no_skeleton...n
-00000570: 6f5f 746f 780d 0a0d 0a5b 6567 675f 696e  o_tox....[egg_in
-00000580: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-00000590: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-000005a0: 0a0d 0a                                  ...
+000000f0: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
+00000100: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+00000110: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
+00000120: 646f 776e 3b20 6368 6172 7365 743d 5554  down; charset=UT
+00000130: 462d 380d 0a75 726c 203d 2068 7474 7073  F-8..url = https
+00000140: 3a2f 2f67 6974 6875 622e 636f 6d2f 3933  ://github.com/93
+00000150: 416b 6b6f 7264 2f66 696c 652d 7472 6565  Akkord/file-tree
+00000160: 2f0d 0a70 726f 6a65 6374 5f75 726c 7320  /..project_urls 
+00000170: 3d20 0d0a 0944 6f63 756d 656e 7461 7469  = ...Documentati
+00000180: 6f6e 203d 2068 7474 7073 3a2f 2f67 6974  on = https://git
+00000190: 6875 622e 636f 6d2f 3933 416b 6b6f 7264  hub.com/93Akkord
+000001a0: 2f66 696c 652d 7472 6565 2f0d 0a09 536f  /file-tree/...So
+000001b0: 7572 6365 203d 2068 7474 7073 3a2f 2f67  urce = https://g
+000001c0: 6974 6875 622e 636f 6d2f 3933 416b 6b6f  ithub.com/93Akko
+000001d0: 7264 2f66 696c 652d 7472 6565 2f0d 0a09  rd/file-tree/...
+000001e0: 5472 6163 6b65 7220 3d20 6874 7470 733a  Tracker = https:
+000001f0: 2f2f 6769 7468 7562 2e63 6f6d 2f39 3341  //github.com/93A
+00000200: 6b6b 6f72 642f 6669 6c65 2d74 7265 652f  kkord/file-tree/
+00000210: 6973 7375 6573 0d0a 0944 6f77 6e6c 6f61  issues...Downloa
+00000220: 6420 3d20 6874 7470 733a 2f2f 7079 7069  d = https://pypi
+00000230: 2e6f 7267 2f70 726f 6a65 6374 2f61 6b6b  .org/project/akk
+00000240: 642d 6669 6c65 2d74 7265 652f 2366 696c  d-file-tree/#fil
+00000250: 6573 0d0a 706c 6174 666f 726d 7320 3d20  es..platforms = 
+00000260: 616e 790d 0a63 6c61 7373 6966 6965 7273  any..classifiers
+00000270: 203d 200d 0a09 4465 7665 6c6f 706d 656e   = ...Developmen
+00000280: 7420 5374 6174 7573 203a 3a20 3420 2d20  t Status :: 4 - 
+00000290: 4265 7461 0d0a 0950 726f 6772 616d 6d69  Beta...Programmi
+000002a0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000002b0: 7974 686f 6e0d 0a0d 0a5b 6f70 7469 6f6e  ython....[option
+000002c0: 735d 0d0a 7a69 705f 7361 6665 203d 2046  s]..zip_safe = F
+000002d0: 616c 7365 0d0a 7061 636b 6167 6573 203d  alse..packages =
+000002e0: 2066 696e 645f 6e61 6d65 7370 6163 653a   find_namespace:
+000002f0: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
+00000300: 655f 6461 7461 203d 2054 7275 650d 0a70  e_data = True..p
+00000310: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
+00000320: 3d73 7263 0d0a 7079 7468 6f6e 5f72 6571  =src..python_req
+00000330: 7569 7265 7320 3d20 3e3d 332e 380d 0a69  uires = >=3.8..i
+00000340: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
+00000350: 3d20 0d0a 0969 6d70 6f72 746c 6962 2d6d  = ...importlib-m
+00000360: 6574 6164 6174 613b 2070 7974 686f 6e5f  etadata; python_
+00000370: 7665 7273 696f 6e3c 2233 2e38 220d 0a0d  version<"3.8"...
+00000380: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+00000390: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
+000003a0: 3d20 7372 630d 0a65 7863 6c75 6465 203d  = src..exclude =
+000003b0: 200d 0a09 7465 7374 730d 0a0d 0a5b 6f70   ...tests....[op
+000003c0: 7469 6f6e 732e 6578 7472 6173 5f72 6571  tions.extras_req
+000003d0: 7569 7265 5d0d 0a74 6573 7469 6e67 203d  uire]..testing =
+000003e0: 200d 0a09 7079 7465 7374 0d0a 0970 7974   ...pytest...pyt
+000003f0: 6573 742d 636f 760d 0a0d 0a5b 6f70 7469  est-cov....[opti
+00000400: 6f6e 732e 656e 7472 795f 706f 696e 7473  ons.entry_points
+00000410: 5d0d 0a63 6f6e 736f 6c65 5f73 6372 6970  ]..console_scrip
+00000420: 7473 203d 200d 0a09 6669 6c65 2d74 7265  ts = ...file-tre
+00000430: 6520 3d20 6669 6c65 5f74 7265 652e 5f66  e = file_tree._f
+00000440: 696c 655f 7472 6565 3a72 756e 0d0a 0d0a  ile_tree:run....
+00000450: 5b74 6f6f 6c3a 7079 7465 7374 5d0d 0a61  [tool:pytest]..a
+00000460: 6464 6f70 7473 203d 200d 0a09 2d2d 636f  ddopts = ...--co
+00000470: 7620 6669 6c65 5f74 7265 6520 2d2d 636f  v file_tree --co
+00000480: 762d 7265 706f 7274 2074 6572 6d2d 6d69  v-report term-mi
+00000490: 7373 696e 670d 0a09 2d2d 7665 7262 6f73  ssing...--verbos
+000004a0: 650d 0a6e 6f72 6563 7572 7365 6469 7273  e..norecursedirs
+000004b0: 203d 200d 0a09 6469 7374 0d0a 0962 7569   = ...dist...bui
+000004c0: 6c64 0d0a 092e 746f 780d 0a74 6573 7470  ld....tox..testp
+000004d0: 6174 6873 203d 2074 6573 7473 0d0a 0d0a  aths = tests....
+000004e0: 5b61 6c69 6173 6573 5d0d 0a64 6973 7473  [aliases]..dists
+000004f0: 203d 2073 6469 7374 2062 6469 7374 5f77   = sdist bdist_w
+00000500: 6865 656c 0d0a 0d0a 5b64 6576 7069 3a75  heel....[devpi:u
+00000510: 706c 6f61 645d 0d0a 6e6f 2d76 6373 203d  pload]..no-vcs =
+00000520: 2031 0d0a 666f 726d 6174 7320 3d20 6264   1..formats = bd
+00000530: 6973 745f 7768 6565 6c0d 0a0d 0a5b 666c  ist_wheel....[fl
+00000540: 616b 6538 5d0d 0a6d 6178 2d6c 696e 652d  ake8]..max-line-
+00000550: 6c65 6e67 7468 203d 2038 380d 0a65 7874  length = 88..ext
+00000560: 656e 642d 6967 6e6f 7265 203d 2045 3230  end-ignore = E20
+00000570: 332c 2057 3530 330d 0a65 7863 6c75 6465  3, W503..exclude
+00000580: 203d 200d 0a09 2e74 6f78 0d0a 0962 7569   = ....tox...bui
+00000590: 6c64 0d0a 0964 6973 740d 0a09 2e65 6767  ld...dist....egg
+000005a0: 730d 0a09 646f 6373 2f63 6f6e 662e 7079  s...docs/conf.py
+000005b0: 0d0a 0d0a 5b70 7973 6361 6666 6f6c 645d  ....[pyscaffold]
+000005c0: 0d0a 7665 7273 696f 6e20 3d20 342e 3061  ..version = 4.0a
+000005d0: 330d 0a70 6163 6b61 6765 203d 2066 696c  3..package = fil
+000005e0: 655f 7472 6565 0d0a 6578 7465 6e73 696f  e_tree..extensio
+000005f0: 6e73 203d 200d 0a09 6e6f 5f70 7970 726f  ns = ...no_pypro
+00000600: 6a65 6374 0d0a 096e 6f5f 736b 656c 6574  ject...no_skelet
+00000610: 6f6e 0d0a 096e 6f5f 746f 780d 0a0d 0a5b  on...no_tox....[
+00000620: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+00000630: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+00000640: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `akkd_file_tree-0.0.6/setup.py` & `akkd_file_tree-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `akkd_file_tree-0.0.6/src/file_tree/_file_tree.py` & `akkd_file_tree-0.0.7/src/file_tree/_file_tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# !/home/rda_admin/portable/python/install/bin/python3
+#!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 '''file-tree.py: ...'''
 
 from __future__ import annotations
 
 import copy
@@ -21,14 +21,21 @@
 from typing import Any, Callable, Dict, Generator, Iterator, List, Tuple, Type, TypeVar, Union
 
 import six
 
 from _collections_abc import dict_items, dict_keys, dict_values
 
 
+__all__ = [
+    'File',
+    'Folder',
+    'FileTreeMaker',
+    'print_file_tree',
+]
+
 faulthandler.enable()
 
 
 __author__ = 'michaelcbarros@gmail.com'
 
 
 getcwd = os.getcwd if hasattr(os, 'getcwd') else os.getcwd
@@ -40,44 +47,26 @@
 
 T = TypeVar('T')
 
 
 # region Icons
 
 
-class IconsMeta(type):
-    def __new__(cls: Type['IconsMeta'], name: str, bases: Tuple[type, ...], attrs: Dict[str, Any]) -> 'IconsMeta':
-        for attr_name, attr_value in attrs.items():
-            if not callable(attr_value) and not attr_name.startswith('__'):
-                # emoji = '\uFE0F'
-                # text = '\uFE0E'
-                attrs[attr_name] = attr_value.lower() + '\0'
-
-        return super().__new__(cls, name, bases, attrs)
-
-
-class Icons:  # (metaclass=IconsMeta)
+class Icons:
     FOLDER = b'\xf0\x9f\x93\x81'.decode('utf-8')
     OPEN_FOLDER = b'\xf0\x9f\x93\x82'.decode('utf-8')
     FILE = b'\xf0\x9f\x93\x84'.decode('utf-8')
     LINK = b'\xf0\x9f\x94\x97'.decode('utf-8')
 
 
 # endregion Icons
 
 # region utils.py
 
 
-def is_admin():
-    try:
-        return ctypes.windll.shell32.IsUserAnAdmin()
-    except:
-        return False
-
-
 def bytes_2_human_readable(number_of_bytes: int | float, si=False, decimals=1) -> str:
     thresh = 1000 if si else 1024
 
     if math.fabs(number_of_bytes) < thresh:
         return str(number_of_bytes) + ' B'
 
     units = ['kB', 'MB', 'GB', 'TB', 'PB', 'EB', 'ZB', 'YB'] if si else ['KiB', 'MiB', 'GiB', 'TiB', 'PiB', 'EiB', 'ZiB', 'YiB']
@@ -256,19 +245,15 @@
             error = ctypes.WinError()
 
             error_files.append({
                 'filename': filename,
                 'error': str(error)
             })
 
-            print('filename:', filename)
-            print('\n' * 3)
-
             raise error
-
         try:
             while True:
                 if data.cFileName not in ('.', '..'):
                     st = find_data_to_stat(data)
                     is_symlink = stat.S_ISLNK(st.st_mode)
 
                     # yield (data.cFileName, st, is_symlink)
@@ -415,42 +400,14 @@
         return -1
 
     def remove(self):
         self.parent.children.pop(self.index)
 
         self.parent = None
 
-    # region Old Code
-
-    # def get_key_path_old(self) -> List[int]:
-    #     key_path = []
-
-    #     temp_self = self
-
-    #     while temp_self.parent is not None:
-    #         print(temp_self.path)
-
-    #         index = get_obj_index(temp_self.parent.children, temp_self)
-
-    #         key_path.append(index)
-
-    #         temp_self = temp_self.parent
-
-    #     return reversed(key_path)
-
-    # def remove_path_old(self, key_path: List[int]):
-    #     temp_self = self
-
-    #     for i in key_path:
-    #         temp_self = temp_self.children[i]
-
-    #     temp_self.parent.children.remove(temp_self)
-
-    # endregion Old Code
-
     def __setitem__(self, key: Any, item: Any) -> None:
         self.__dict__[key] = item
 
     def __getitem__(self, key: Any) -> Any:
         return self.__dict__[key]
 
     def __repr__(self) -> str:
@@ -525,51 +482,14 @@
 
         return sum(file_sizes)
 
     @size.setter
     def size(self, value: int):
         pass
 
-    # @property
-    # def nested_child_count(self) -> int:
-    #     child_counts: List[int] = []
-    #     first_run = True
-
-    #     def cb(item: File | Folder, level: int, is_last: bool, is_mid_child: bool) -> File | Folder:
-    #         if type(item) == Folder:
-    #             # count = len(item.children)
-                
-    #             # print(f'count: {count}')
-
-    #             child_counts.append(item.nested_child_count)
-
-    #         return item
-
-    #     while first_run:
-    #         first_run = False
-
-    #         self.walk(cb)
-
-    #     if self.path == 'C:\\Users\\mbarros\\development\\big_data\\entity_resolution\\spark-node-dev\\scripts\\python\\tools\\glue_jobs_backups':
-    #         print('Here01')
-
-    #     return sum(child_counts)
-
-    # @property
-    # def nested_child_count(self) -> int:
-    #     queue = [self]
-    #     count = 0
-
-    #     while queue:
-    #         current_folder = queue.pop(0)
-    #         count += len(current_folder.children)
-    #         queue.extend(child for child in current_folder.children if isinstance(child, Folder))
-
-    #     return count
-
     @property
     def nested_child_count(self) -> Tuple[int, int]:
         queue: List[Folder] = [self]
         folder_count = 0
         file_count = 0
 
         while queue:
@@ -625,27 +545,27 @@
                 child.walk(callback=callback, level=level + 1)
             else:
                 self.children[idx] = callback(child, level, is_last, is_mid_child)
 
 
 class FileTreeMaker(object):
     def __init__(self,
-                 root: str | bytes,
-                 max_level: int,
-                 remove_pipe: bool,
-                 exclude_folder: List[str] | List[bytes],
-                 exclude_name: List[str] | List[bytes],
-                 exclude_regex: List[str],
-                 include_regex: List[str],
-                 size_limit: int,
-                 exclude_empty_files: bool,
-                 later_than_date: str,
-                 links: bool,
-                 show_size: bool,
-                 show_counts: bool):
+                 root: str | bytes = '.',
+                 max_level: int = -1,
+                 remove_pipe: bool = False,
+                 exclude_folder: List[str] | List[bytes] = [],
+                 exclude_name: List[str] | List[bytes] = [],
+                 exclude_regex: List[str] | List[bytes] = [],
+                 include_regex: List[str] | List[bytes] = [],
+                 size_limit: int = -1,
+                 exclude_empty_files: bool = False,
+                 later_than_date: str = None,
+                 links: bool = False,
+                 show_size: bool = False,
+                 show_counts: bool = False) -> None:
         global error_files
 
         error_files = []
 
         self.root = os.path.abspath(root)
         self.exclude_folder = exclude_folder
         self.exclude_name = exclude_name
@@ -804,19 +724,19 @@
                 name = '{name}'.format(name=create_file_link_str(item_path, item_name, color_file_type)) if item.type == 'Folder' else create_file_link_str(item_path, item_name, color_file_type)
             else:
                 name = '{name}'.format(name=create_colored_str(item_name, color_file_type)) if item.type == 'Folder' else create_colored_str(item_name, color_file_type)
 
             size_count_str = get_size_count_str(self, item)
 
             output = '{prefix}{idc}{space}{icon} {name}{size_count_str}'.format(prefix=prefix,
-                                                                      idc=idc,
-                                                                      space='' if type(item) == Folder and item.is_root else ' ',
-                                                                      icon=icon,
-                                                                      name=name,
-                                                                      size_count_str=size_count_str)
+                                                                                idc=idc,
+                                                                                space='' if type(item) == Folder and item.is_root else ' ',
+                                                                                icon=icon,
+                                                                                name=name,
+                                                                                size_count_str=size_count_str)
 
             lines.append(output)
 
         self.root_dir_tree.walk_create_output_str(cb, remove_pipe=self.remove_pipe)
 
         output_str = '\n'.join(lines)
 
@@ -863,38 +783,39 @@
     return size_count_str
 
 
 def sigint_handler(signum: int, frame: Any):
     sys.exit(0)
 
 
+signal.signal(signal.SIGINT, sigint_handler)
+
+
 def run() -> None:
     res = parse_args()
 
-    __run(**res.__dict__)
+    print_file_tree(**res.__dict__)
 
 
-def __run(root: str,
-          output: str,
-          max_level: int,
-          flat: bool,
-          remove_pipe: bool,
-          exclude_folder: Tuple[str, ...] | List[str],
-          exclude_name: Tuple[str, ...] | List[str],
-          exclude_regex: Tuple[str, ...] | List[str],
-          include_regex: Tuple[str, ...] | List[str],
-          size_limit: int,
-          exclude_empty_files: bool,
-          later_than_date: str,
-          links: bool,
-          show_size: bool,
-          show_counts: bool,
-          errors: bool) -> None:
-    signal.signal(signal.SIGINT, sigint_handler)
-
+def print_file_tree(root: str | bytes = '.',
+                    output: str = None,
+                    max_level: int = -1,
+                    flat: bool = False,
+                    remove_pipe: bool = False,
+                    exclude_folder: List[str] | List[bytes] = [],
+                    exclude_name: List[str] | List[bytes] = [],
+                    exclude_regex: List[str] | List[bytes] = [],
+                    include_regex: List[str] | List[bytes] = [],
+                    size_limit: int = -1,
+                    exclude_empty_files: bool = False,
+                    later_than_date: str = None,
+                    links: bool = False,
+                    show_size: bool = False,
+                    show_counts: bool = False,
+                    errors: bool = False) -> None:
     exclude_folder = list(exclude_folder)
     exclude_name = list(exclude_name)
     exclude_regex = list(exclude_regex)
     include_regex = list(include_regex)
 
     root = os.path.abspath(root)
 
@@ -1009,35 +930,15 @@
 
     return args
 
 
 if __name__ == '__main__':
     # args = [
     #     '-r',
-    #     r'C:\Users\mbarros\development\big_data\entity_resolution\spark-node-dev',
-    #     '-xf',
-    #     '"node_modules"',
-    #     # '-l',
-    #     # '-f',
-    #     # '-e',
-    #     '-ir',
-    #     r'"(\.py|\.js)$"',
+    #     'C:\\Users\\mbarros\\development\\big_data\\entity_resolution\\spark-node-dev\\scripts\\python\\tools',
+    #     '-s',
+    #     '-c',
     # ]
 
-    # args = [
-    #     '-r',
-    #     r'C:\Program Files (x86)\Microsoft Visual Studio\2017',
-    #     # '-rp',
-    #     '-l',
-    #     '-s'
-    # ]
-
-    args = [
-        '-r',
-        'C:\\Users\\mbarros\\development\\big_data\\entity_resolution\\spark-node-dev\\scripts\\python\\tools',
-        '-s',
-        '-c',
-    ]
-
-    sys.argv = sys.argv + args
+    # sys.argv = sys.argv + args
 
     run()
```

