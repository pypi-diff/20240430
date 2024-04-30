# Comparing `tmp/cheap_pie-1.0.8.tar.gz` & `tmp/cheap_pie-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheap_pie-1.0.8.tar", last modified: Wed Nov 15 21:57:54 2023, max compression
+gzip compressed data, was "cheap_pie-1.0.9.tar", last modified: Mon Jan  1 22:34:44 2024, max compression
```

## Comparing `cheap_pie-1.0.8.tar` & `cheap_pie-1.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0 eink      (1002) eink      (1002)        0 2023-11-15 21:57:54.811900 cheap_pie-1.0.8/
--rwxrwxrwx   0 eink      (1002) eink      (1002)    11357 2022-12-10 01:01:26.000000 cheap_pie-1.0.8/LICENSE
--rwxrwxrwx   0 eink      (1002) eink      (1002)     8121 2023-11-15 21:57:54.812310 cheap_pie-1.0.8/PKG-INFO
--rwxrwxrwx   0 eink      (1002) eink      (1002)     7780 2023-05-24 22:06:57.000000 cheap_pie-1.0.8/README.md
--rwxrwxrwx   0 eink      (1002) eink      (1002)      103 2023-11-15 21:57:54.812978 cheap_pie-1.0.8/setup.cfg
--rwxrwxrwx   0 eink      (1002) eink      (1002)     1263 2023-11-15 21:25:53.000000 cheap_pie-1.0.8/setup.py
-drwxrwxrwx   0 eink      (1002) eink      (1002)        0 2023-11-15 21:57:54.765275 cheap_pie-1.0.8/src/
-drwxrwxrwx   0 eink      (1002) eink      (1002)        0 2023-11-15 21:57:54.769675 cheap_pie-1.0.8/src/cheap_pie/
--rwxrwxrwx   0 eink      (1002) eink      (1002)      207 2023-05-22 21:21:25.000000 cheap_pie-1.0.8/src/cheap_pie/__init__.py
-drwxrwxrwx   0 eink      (1002) eink      (1002)        0 2023-11-15 21:57:54.795294 cheap_pie-1.0.8/src/cheap_pie/cheap_pie_core/
--rwxrwxrwx   0 eink      (1002) eink      (1002)      213 2023-09-05 19:27:17.000000 cheap_pie-1.0.8/src/cheap_pie/cheap_pie_core/__init__.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     7659 2023-09-05 19:27:17.000000 cheap_pie-1.0.8/src/cheap_pie/cheap_pie_core/cbitfield.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     2795 2023-09-05 19:27:17.000000 cheap_pie-1.0.8/src/cheap_pie/cheap_pie_core/cheap_pie_main.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     3355 2023-09-05 19:27:17.000000 cheap_pie-1.0.8/src/cheap_pie/cheap_pie_core/cp_banner.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     3434 2023-09-05 19:27:17.000000 cheap_pie-1.0.8/src/cheap_pie/cheap_pie_core/cp_builder.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     2675 2023-09-05 19:27:17.000000 cheap_pie-1.0.8/src/cheap_pie/cheap_pie_core/cp_cli.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)    14441 2023-11-15 21:11:13.000000 cheap_pie-1.0.8/src/cheap_pie/cheap_pie_core/cp_hal.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)    16476 2023-11-15 21:13:49.000000 cheap_pie-1.0.8/src/cheap_pie/cheap_pie_core/cp_register.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     3670 2023-09-09 20:02:15.000000 cheap_pie-1.0.8/src/cheap_pie/cheap_pie_core/test.py
-drwxrwxrwx   0 eink      (1002) eink      (1002)        0 2023-11-15 21:57:54.803658 cheap_pie-1.0.8/src/cheap_pie/parsers/
--rwxrwxrwx   0 eink      (1002) eink      (1002)      163 2023-05-22 20:56:30.000000 cheap_pie-1.0.8/src/cheap_pie/parsers/__init__.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     2441 2023-09-05 19:27:17.000000 cheap_pie-1.0.8/src/cheap_pie/parsers/cp_parsers_wrapper.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     3212 2023-09-05 19:46:05.000000 cheap_pie-1.0.8/src/cheap_pie/parsers/ipxact_parse.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     2636 2023-09-05 19:27:17.000000 cheap_pie-1.0.8/src/cheap_pie/parsers/ipyxact_parse.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     1174 2023-09-05 19:27:17.000000 cheap_pie-1.0.8/src/cheap_pie/parsers/rdl_parse.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     3165 2023-09-05 19:58:57.000000 cheap_pie-1.0.8/src/cheap_pie/parsers/svd_parse.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     3198 2023-09-05 19:27:17.000000 cheap_pie-1.0.8/src/cheap_pie/parsers/svd_parse_repo.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     2504 2023-09-05 19:47:55.000000 cheap_pie-1.0.8/src/cheap_pie/parsers/xml_xslt.py
-drwxrwxrwx   0 eink      (1002) eink      (1002)        0 2023-11-15 21:57:54.806344 cheap_pie-1.0.8/src/cheap_pie/tools/
--rwxrwxrwx   0 eink      (1002) eink      (1002)       92 2023-05-21 15:55:01.000000 cheap_pie-1.0.8/src/cheap_pie/tools/__init__.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     4633 2023-09-05 19:52:30.000000 cheap_pie-1.0.8/src/cheap_pie/tools/hal2doc.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     2695 2023-11-15 21:30:39.000000 cheap_pie-1.0.8/src/cheap_pie/tools/rdl2any.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     2662 2023-09-05 19:27:17.000000 cheap_pie-1.0.8/src/cheap_pie/tools/search.py
-drwxrwxrwx   0 eink      (1002) eink      (1002)        0 2023-11-15 21:57:54.811023 cheap_pie-1.0.8/src/cheap_pie/transport/
--rwxrwxrwx   0 eink      (1002) eink      (1002)      225 2023-09-05 19:27:17.000000 cheap_pie-1.0.8/src/cheap_pie/transport/__init__.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     2417 2023-09-09 20:02:15.000000 cheap_pie-1.0.8/src/cheap_pie/transport/cp_dummy_transport.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     2255 2023-11-15 20:50:23.000000 cheap_pie-1.0.8/src/cheap_pie/transport/cp_esptool_transport.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     1772 2023-09-05 19:27:17.000000 cheap_pie-1.0.8/src/cheap_pie/transport/cp_jlink_transport.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     1794 2023-09-05 19:27:17.000000 cheap_pie-1.0.8/src/cheap_pie/transport/cp_pyocd_transport.py
--rwxrwxrwx   0 eink      (1002) eink      (1002)     5682 2023-09-05 19:27:17.000000 cheap_pie-1.0.8/src/cheap_pie/transport/cp_pyverilator_transport.py
-drwxrwxrwx   0 eink      (1002) eink      (1002)        0 2023-11-15 21:57:54.773298 cheap_pie-1.0.8/src/cheap_pie.egg-info/
--rwxrwxrwx   0 eink      (1002) eink      (1002)     8121 2023-11-15 21:57:54.000000 cheap_pie-1.0.8/src/cheap_pie.egg-info/PKG-INFO
--rwxrwxrwx   0 eink      (1002) eink      (1002)     1317 2023-11-15 21:57:54.000000 cheap_pie-1.0.8/src/cheap_pie.egg-info/SOURCES.txt
--rwxrwxrwx   0 eink      (1002) eink      (1002)        1 2023-11-15 21:57:54.000000 cheap_pie-1.0.8/src/cheap_pie.egg-info/dependency_links.txt
--rwxrwxrwx   0 eink      (1002) eink      (1002)      128 2023-11-15 21:57:54.000000 cheap_pie-1.0.8/src/cheap_pie.egg-info/requires.txt
--rwxrwxrwx   0 eink      (1002) eink      (1002)       10 2023-11-15 21:57:54.000000 cheap_pie-1.0.8/src/cheap_pie.egg-info/top_level.txt
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-01-01 22:34:44.349322 cheap_pie-1.0.9/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    11357 2022-12-10 01:01:26.000000 cheap_pie-1.0.9/LICENSE
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     8121 2024-01-01 22:34:44.349855 cheap_pie-1.0.9/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     7780 2023-05-24 22:06:57.000000 cheap_pie-1.0.9/README.md
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      103 2024-01-01 22:34:44.351306 cheap_pie-1.0.9/setup.cfg
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1263 2024-01-01 21:40:22.000000 cheap_pie-1.0.9/setup.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-01-01 22:34:44.274921 cheap_pie-1.0.9/src/
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-01-01 22:34:44.283830 cheap_pie-1.0.9/src/cheap_pie/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      207 2023-05-22 21:21:25.000000 cheap_pie-1.0.9/src/cheap_pie/__init__.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-01-01 22:34:44.306817 cheap_pie-1.0.9/src/cheap_pie/cheap_pie_core/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      213 2023-09-05 19:27:17.000000 cheap_pie-1.0.9/src/cheap_pie/cheap_pie_core/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     7659 2023-09-05 19:27:17.000000 cheap_pie-1.0.9/src/cheap_pie/cheap_pie_core/cbitfield.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3161 2024-01-01 21:40:22.000000 cheap_pie-1.0.9/src/cheap_pie/cheap_pie_core/cheap_pie_main.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3355 2023-09-05 19:27:17.000000 cheap_pie-1.0.9/src/cheap_pie/cheap_pie_core/cp_banner.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3434 2023-09-05 19:27:17.000000 cheap_pie-1.0.9/src/cheap_pie/cheap_pie_core/cp_builder.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3043 2024-01-01 21:40:23.000000 cheap_pie-1.0.9/src/cheap_pie/cheap_pie_core/cp_cli.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    14441 2023-11-15 21:11:13.000000 cheap_pie-1.0.9/src/cheap_pie/cheap_pie_core/cp_hal.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    16476 2023-11-15 21:13:49.000000 cheap_pie-1.0.9/src/cheap_pie/cheap_pie_core/cp_register.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3670 2023-09-09 20:02:15.000000 cheap_pie-1.0.9/src/cheap_pie/cheap_pie_core/test.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-01-01 22:34:44.320665 cheap_pie-1.0.9/src/cheap_pie/parsers/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      163 2023-05-22 20:56:30.000000 cheap_pie-1.0.9/src/cheap_pie/parsers/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2441 2023-09-05 19:27:17.000000 cheap_pie-1.0.9/src/cheap_pie/parsers/cp_parsers_wrapper.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3212 2023-09-05 19:46:05.000000 cheap_pie-1.0.9/src/cheap_pie/parsers/ipxact_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2636 2023-09-05 19:27:17.000000 cheap_pie-1.0.9/src/cheap_pie/parsers/ipyxact_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1174 2023-09-05 19:27:17.000000 cheap_pie-1.0.9/src/cheap_pie/parsers/rdl_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3165 2023-09-05 19:58:57.000000 cheap_pie-1.0.9/src/cheap_pie/parsers/svd_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     5045 2024-01-01 21:58:32.000000 cheap_pie-1.0.9/src/cheap_pie/parsers/svd_parse_repo.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2504 2023-09-05 19:47:55.000000 cheap_pie-1.0.9/src/cheap_pie/parsers/xml_xslt.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-01-01 22:34:44.336356 cheap_pie-1.0.9/src/cheap_pie/tools/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       92 2023-05-21 15:55:01.000000 cheap_pie-1.0.9/src/cheap_pie/tools/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4633 2023-09-05 19:52:30.000000 cheap_pie-1.0.9/src/cheap_pie/tools/hal2doc.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2695 2023-11-15 21:30:39.000000 cheap_pie-1.0.9/src/cheap_pie/tools/rdl2any.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2662 2023-09-05 19:27:17.000000 cheap_pie-1.0.9/src/cheap_pie/tools/search.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-01-01 22:34:44.348032 cheap_pie-1.0.9/src/cheap_pie/transport/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      225 2023-09-05 19:27:17.000000 cheap_pie-1.0.9/src/cheap_pie/transport/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2417 2023-09-09 20:02:15.000000 cheap_pie-1.0.9/src/cheap_pie/transport/cp_dummy_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2255 2023-11-15 20:50:23.000000 cheap_pie-1.0.9/src/cheap_pie/transport/cp_esptool_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1772 2023-09-05 19:27:17.000000 cheap_pie-1.0.9/src/cheap_pie/transport/cp_jlink_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1794 2023-09-05 19:27:17.000000 cheap_pie-1.0.9/src/cheap_pie/transport/cp_pyocd_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     5682 2023-09-05 19:27:17.000000 cheap_pie-1.0.9/src/cheap_pie/transport/cp_pyverilator_transport.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2024-01-01 22:34:44.289647 cheap_pie-1.0.9/src/cheap_pie.egg-info/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     8121 2024-01-01 22:34:44.000000 cheap_pie-1.0.9/src/cheap_pie.egg-info/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1317 2024-01-01 22:34:44.000000 cheap_pie-1.0.9/src/cheap_pie.egg-info/SOURCES.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2024-01-01 22:34:44.000000 cheap_pie-1.0.9/src/cheap_pie.egg-info/dependency_links.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      128 2024-01-01 22:34:44.000000 cheap_pie-1.0.9/src/cheap_pie.egg-info/requires.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       10 2024-01-01 22:34:44.000000 cheap_pie-1.0.9/src/cheap_pie.egg-info/top_level.txt
```

### Comparing `cheap_pie-1.0.8/LICENSE` & `cheap_pie-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/PKG-INFO` & `cheap_pie-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheap_pie
-Version: 1.0.8
+Version: 1.0.9
 Summary: A python tool for silicon validation.
 Home-page: https://github.com/bat52/cheap_pie
 Author: Marco Merlin
 Author-email: marcomerli@gmail.com
 License: Apache 2.0
 Keywords: python silicon validation
 Platform: UNKNOWN
```

### Comparing `cheap_pie-1.0.8/README.md` & `cheap_pie-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/setup.py` & `cheap_pie-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setup(
     name='cheap_pie',
-    version='1.0.8',
+    version='1.0.9',
     license='Apache 2.0',
     author="Marco Merlin",
     author_email='marcomerli@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description="A python tool for silicon validation.",
     long_description=long_description,
```

### Comparing `cheap_pie-1.0.8/src/cheap_pie/cheap_pie_core/cbitfield.py` & `cheap_pie-1.0.9/src/cheap_pie/cheap_pie_core/cbitfield.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie/cheap_pie_core/cheap_pie_main.py` & `cheap_pie-1.0.9/src/cheap_pie/cheap_pie_core/cheap_pie_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-#!/usr/bin/python3
+#!/usr/bin/env python3
 """
 This file is part of cheap_pie, a python tool for chip validation
  author: Marco Merlin
  email: marcomerli@gmail.com
 """
 
 if __name__ == '__main__':
     # needed if cheap_pie not installed
     import os
     import sys
     sys.path.append(os.path.join(os.path.dirname(__file__), '../..'))
 
 from cheap_pie.parsers.cp_parsers_wrapper import cp_parsers_wrapper  # pylint: disable=C0413,E0401
+from cheap_pie.parsers.svd_parse_repo import svd_repo_print_vendors, svd_repo_print_vendor_devices # pylint: disable=C0413,E0401
 from cheap_pie.cheap_pie_core.cp_banner import cp_banner            # pylint: disable=C0413,E0401
 from cheap_pie.cheap_pie_core.cp_cli import cp_cli                  # pylint: disable=C0413,E0401
 from cheap_pie.transport.cp_dummy_transport import CpDummyTransport  # pylint: disable=C0413,E0401
 
 # Ipython autoreload
 # %load_ext autoreload
 # %autoreload 2
@@ -30,14 +31,21 @@
     ## banner #######################################################################
     cp_banner()
     #
     ## input parameters ###########################################################
     print('Parsing input arguments...')
     prms = cp_cli(argv)
 
+    ## helper functions ###########################################################
+
+    if prms.vendors:
+        return svd_repo_print_vendors()
+    if prms.devices:
+        return svd_repo_print_vendor_devices(vendor=prms.vendor)
+
     # transport hif interface %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
     print('Initialising Host Interface...')
 
     # init jlink transport: importing under if case allows not installing all transport libraries
     if prms.transport == 'dummy':
         hif = CpDummyTransport()
     elif prms.transport == 'jlink':  # disable jlink for testing
```

### Comparing `cheap_pie-1.0.8/src/cheap_pie/cheap_pie_core/cp_banner.py` & `cheap_pie-1.0.9/src/cheap_pie/cheap_pie_core/cp_banner.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie/cheap_pie_core/cp_builder.py` & `cheap_pie-1.0.9/src/cheap_pie/cheap_pie_core/cp_builder.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie/cheap_pie_core/cp_cli.py` & `cheap_pie-1.0.9/src/cheap_pie/cheap_pie_core/cp_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/python3
+#!/usr/bin/env python3
 """
 Cheap Pie Command Line Interface
 """
 # this file is part of cheap_pie, a python tool for chip validation
 # author: Marco Merlin
 # email: marcomerli@gmail.com
 
@@ -45,14 +45,20 @@
                         )
     parser.add_argument("-fmt", "--format", help="device description format",
                         action='store', type=str, default="cmsis-svd",
                         choices=["svd", "cmsis-svd", "ipxact", "ipyxact", "rdl"])
     parser.add_argument("-ve", "--vendor",
                         help="device vendor. if specified parses svd file from github repository.",
                         action='store', type=str, default=None)
+    parser.add_argument("-vendors", "--vendors",
+                        help="Available device vendors from cmsis-svd package.",
+                        action='store_true')
+    parser.add_argument("-devices", "--devices",
+                        help="Available devices for specified vendor from cmsis-svd package.",
+                        action='store_true')
     # transport options
     parser.add_argument("-d", "--device", help="jlink/ocd device name", action='store',
                         type=str, default="CORTEX-M4")
     parser.add_argument("-t", "--transport", help="transport", action='store', type=str,
                         default="dummy", choices=["jlink", "dummy", "ocd", "esptool", "verilator"])
     parser.add_argument("-p", "--port", help="esptool serial port", action='store', type=str,
                         default="/dev/ttyUSB0")
```

### Comparing `cheap_pie-1.0.8/src/cheap_pie/cheap_pie_core/cp_hal.py` & `cheap_pie-1.0.9/src/cheap_pie/cheap_pie_core/cp_hal.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie/cheap_pie_core/cp_register.py` & `cheap_pie-1.0.9/src/cheap_pie/cheap_pie_core/cp_register.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie/cheap_pie_core/test.py` & `cheap_pie-1.0.9/src/cheap_pie/cheap_pie_core/test.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie/parsers/cp_parsers_wrapper.py` & `cheap_pie-1.0.9/src/cheap_pie/parsers/cp_parsers_wrapper.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie/parsers/ipxact_parse.py` & `cheap_pie-1.0.9/src/cheap_pie/parsers/ipxact_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie/parsers/ipyxact_parse.py` & `cheap_pie-1.0.9/src/cheap_pie/parsers/ipyxact_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie/parsers/rdl_parse.py` & `cheap_pie-1.0.9/src/cheap_pie/parsers/rdl_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie/parsers/svd_parse.py` & `cheap_pie-1.0.9/src/cheap_pie/parsers/svd_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie/parsers/xml_xslt.py` & `cheap_pie-1.0.9/src/cheap_pie/parsers/xml_xslt.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie/tools/hal2doc.py` & `cheap_pie-1.0.9/src/cheap_pie/tools/hal2doc.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie/tools/rdl2any.py` & `cheap_pie-1.0.9/src/cheap_pie/tools/rdl2any.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie/tools/search.py` & `cheap_pie-1.0.9/src/cheap_pie/tools/search.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie/transport/cp_dummy_transport.py` & `cheap_pie-1.0.9/src/cheap_pie/transport/cp_dummy_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie/transport/cp_esptool_transport.py` & `cheap_pie-1.0.9/src/cheap_pie/transport/cp_esptool_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie/transport/cp_jlink_transport.py` & `cheap_pie-1.0.9/src/cheap_pie/transport/cp_jlink_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie/transport/cp_pyocd_transport.py` & `cheap_pie-1.0.9/src/cheap_pie/transport/cp_pyocd_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie/transport/cp_pyverilator_transport.py` & `cheap_pie-1.0.9/src/cheap_pie/transport/cp_pyverilator_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.8/src/cheap_pie.egg-info/PKG-INFO` & `cheap_pie-1.0.9/src/cheap_pie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheap-pie
-Version: 1.0.8
+Version: 1.0.9
 Summary: A python tool for silicon validation.
 Home-page: https://github.com/bat52/cheap_pie
 Author: Marco Merlin
 Author-email: marcomerli@gmail.com
 License: Apache 2.0
 Keywords: python silicon validation
 Platform: UNKNOWN
```

### Comparing `cheap_pie-1.0.8/src/cheap_pie.egg-info/SOURCES.txt` & `cheap_pie-1.0.9/src/cheap_pie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

