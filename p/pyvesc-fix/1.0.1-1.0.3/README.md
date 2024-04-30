# Comparing `tmp/pyvesc_fix-1.0.1.tar.gz` & `tmp/pyvesc_fix-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvesc_fix-1.0.1.tar", last modified: Tue Apr 30 13:56:39 2024, max compression
+gzip compressed data, was "pyvesc_fix-1.0.3.tar", last modified: Tue Apr 30 13:51:21 2024, max compression
```

## Comparing `pyvesc_fix-1.0.1.tar` & `pyvesc_fix-1.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:56:39.660024 pyvesc_fix-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-30 13:56:26.000000 pyvesc_fix-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-30 13:56:39.660024 pyvesc_fix-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-30 13:56:26.000000 pyvesc_fix-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:56:39.656024 pyvesc_fix-1.0.1/pyvesc_fix/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:56:39.656024 pyvesc_fix-1.0.1/pyvesc_fix/VESC/
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-30 13:56:26.000000 pyvesc_fix-1.0.1/pyvesc_fix/VESC/VESC.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-30 13:56:26.000000 pyvesc_fix-1.0.1/pyvesc_fix/VESC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:56:39.656024 pyvesc_fix-1.0.1/pyvesc_fix/VESC/messages/
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-30 13:56:26.000000 pyvesc_fix-1.0.1/pyvesc_fix/VESC/messages/Vedder_BLDC_Commands.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-30 13:56:26.000000 pyvesc_fix-1.0.1/pyvesc_fix/VESC/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-30 13:56:26.000000 pyvesc_fix-1.0.1/pyvesc_fix/VESC/messages/getters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-30 13:56:26.000000 pyvesc_fix-1.0.1/pyvesc_fix/VESC/messages/setters.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-30 13:56:27.000000 pyvesc_fix-1.0.1/pyvesc_fix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-30 13:56:26.000000 pyvesc_fix-1.0.1/pyvesc_fix/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:56:39.656024 pyvesc_fix-1.0.1/pyvesc_fix/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-30 13:56:26.000000 pyvesc_fix-1.0.1/pyvesc_fix/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-30 13:56:26.000000 pyvesc_fix-1.0.1/pyvesc_fix/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-30 13:56:26.000000 pyvesc_fix-1.0.1/pyvesc_fix/protocol/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:56:39.660024 pyvesc_fix-1.0.1/pyvesc_fix/protocol/packet/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-30 13:56:26.000000 pyvesc_fix-1.0.1/pyvesc_fix/protocol/packet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-04-30 13:56:26.000000 pyvesc_fix-1.0.1/pyvesc_fix/protocol/packet/codec.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 13:56:26.000000 pyvesc_fix-1.0.1/pyvesc_fix/protocol/packet/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-30 13:56:26.000000 pyvesc_fix-1.0.1/pyvesc_fix/protocol/packet/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:56:39.660024 pyvesc_fix-1.0.1/pyvesc_fix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-30 13:56:39.000000 pyvesc_fix-1.0.1/pyvesc_fix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-30 13:56:39.000000 pyvesc_fix-1.0.1/pyvesc_fix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:56:39.000000 pyvesc_fix-1.0.1/pyvesc_fix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 13:56:39.000000 pyvesc_fix-1.0.1/pyvesc_fix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 13:56:39.000000 pyvesc_fix-1.0.1/pyvesc_fix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:56:39.660024 pyvesc_fix-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-30 13:56:27.000000 pyvesc_fix-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:56:39.660024 pyvesc_fix-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:56:26.000000 pyvesc_fix-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16208 2024-04-30 13:56:26.000000 pyvesc_fix-1.0.1/tests/test_vesc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:51:21.753367 pyvesc_fix-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-30 13:51:07.000000 pyvesc_fix-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-30 13:51:21.753367 pyvesc_fix-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-30 13:51:07.000000 pyvesc_fix-1.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:51:21.749366 pyvesc_fix-1.0.3/pyvesc_fix/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:51:21.749366 pyvesc_fix-1.0.3/pyvesc_fix/VESC/
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-30 13:51:07.000000 pyvesc_fix-1.0.3/pyvesc_fix/VESC/VESC.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-30 13:51:07.000000 pyvesc_fix-1.0.3/pyvesc_fix/VESC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:51:21.749366 pyvesc_fix-1.0.3/pyvesc_fix/VESC/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-30 13:51:07.000000 pyvesc_fix-1.0.3/pyvesc_fix/VESC/messages/Vedder_BLDC_Commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-30 13:51:07.000000 pyvesc_fix-1.0.3/pyvesc_fix/VESC/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-30 13:51:07.000000 pyvesc_fix-1.0.3/pyvesc_fix/VESC/messages/getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-30 13:51:07.000000 pyvesc_fix-1.0.3/pyvesc_fix/VESC/messages/setters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-30 13:51:08.000000 pyvesc_fix-1.0.3/pyvesc_fix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-30 13:51:07.000000 pyvesc_fix-1.0.3/pyvesc_fix/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:51:21.749366 pyvesc_fix-1.0.3/pyvesc_fix/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-30 13:51:07.000000 pyvesc_fix-1.0.3/pyvesc_fix/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-30 13:51:07.000000 pyvesc_fix-1.0.3/pyvesc_fix/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-30 13:51:07.000000 pyvesc_fix-1.0.3/pyvesc_fix/protocol/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:51:21.753367 pyvesc_fix-1.0.3/pyvesc_fix/protocol/packet/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-30 13:51:07.000000 pyvesc_fix-1.0.3/pyvesc_fix/protocol/packet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-04-30 13:51:07.000000 pyvesc_fix-1.0.3/pyvesc_fix/protocol/packet/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 13:51:07.000000 pyvesc_fix-1.0.3/pyvesc_fix/protocol/packet/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-30 13:51:07.000000 pyvesc_fix-1.0.3/pyvesc_fix/protocol/packet/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:51:21.753367 pyvesc_fix-1.0.3/pyvesc_fix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-30 13:51:21.000000 pyvesc_fix-1.0.3/pyvesc_fix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-30 13:51:21.000000 pyvesc_fix-1.0.3/pyvesc_fix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:51:21.000000 pyvesc_fix-1.0.3/pyvesc_fix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 13:51:21.000000 pyvesc_fix-1.0.3/pyvesc_fix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 13:51:21.000000 pyvesc_fix-1.0.3/pyvesc_fix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:51:21.753367 pyvesc_fix-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-30 13:51:08.000000 pyvesc_fix-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:51:21.753367 pyvesc_fix-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:51:07.000000 pyvesc_fix-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16208 2024-04-30 13:51:07.000000 pyvesc_fix-1.0.3/tests/test_vesc.py
```

### Comparing `pyvesc_fix-1.0.1/LICENSE.txt` & `pyvesc_fix-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyvesc_fix-1.0.1/PKG-INFO` & `pyvesc_fix-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyvesc_fix
-Version: 1.0.1
+Version: 1.0.3
 Summary: This is a repackagin of a fork from the pyvesc library.
 Home-page: https://github.com/Hanra-s-work/PyVESC
-Download-URL: https://github.com/Hanra-s-work/PyVESC1.0.1
+Download-URL: https://github.com/Hanra-s-work/PyVESC1.0.3
 Author: Henry Letellier
 Author-email: henrysoftwarehouse@protonmail.com
 Keywords: vesc,VESC,communication,protocol,packet
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `pyvesc_fix-1.0.1/pyvesc_fix/VESC/VESC.py` & `pyvesc_fix-1.0.3/pyvesc_fix/VESC/VESC.py`

 * *Files identical despite different names*

### Comparing `pyvesc_fix-1.0.1/pyvesc_fix/VESC/messages/Vedder_BLDC_Commands.py` & `pyvesc_fix-1.0.3/pyvesc_fix/VESC/messages/Vedder_BLDC_Commands.py`

 * *Files identical despite different names*

### Comparing `pyvesc_fix-1.0.1/pyvesc_fix/VESC/messages/getters.py` & `pyvesc_fix-1.0.3/pyvesc_fix/VESC/messages/getters.py`

 * *Files identical despite different names*

### Comparing `pyvesc_fix-1.0.1/pyvesc_fix/VESC/messages/setters.py` & `pyvesc_fix-1.0.3/pyvesc_fix/VESC/messages/setters.py`

 * *Files identical despite different names*

### Comparing `pyvesc_fix-1.0.1/pyvesc_fix/protocol/base.py` & `pyvesc_fix-1.0.3/pyvesc_fix/protocol/base.py`

 * *Files identical despite different names*

### Comparing `pyvesc_fix-1.0.1/pyvesc_fix/protocol/interface.py` & `pyvesc_fix-1.0.3/pyvesc_fix/protocol/interface.py`

 * *Files identical despite different names*

### Comparing `pyvesc_fix-1.0.1/pyvesc_fix/protocol/packet/codec.py` & `pyvesc_fix-1.0.3/pyvesc_fix/protocol/packet/codec.py`

 * *Files identical despite different names*

### Comparing `pyvesc_fix-1.0.1/pyvesc_fix/protocol/packet/structure.py` & `pyvesc_fix-1.0.3/pyvesc_fix/protocol/packet/structure.py`

 * *Files identical despite different names*

### Comparing `pyvesc_fix-1.0.1/pyvesc_fix.egg-info/PKG-INFO` & `pyvesc_fix-1.0.3/pyvesc_fix.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyvesc_fix
-Version: 1.0.1
+Version: 1.0.3
 Summary: This is a repackagin of a fork from the pyvesc library.
 Home-page: https://github.com/Hanra-s-work/PyVESC
-Download-URL: https://github.com/Hanra-s-work/PyVESC1.0.1
+Download-URL: https://github.com/Hanra-s-work/PyVESC1.0.3
 Author: Henry Letellier
 Author-email: henrysoftwarehouse@protonmail.com
 Keywords: vesc,VESC,communication,protocol,packet
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `pyvesc_fix-1.0.1/pyvesc_fix.egg-info/SOURCES.txt` & `pyvesc_fix-1.0.3/pyvesc_fix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvesc_fix-1.0.1/setup.py` & `pyvesc_fix-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 ## License
 
 Just like VESC, PyVESC is distributed under a
 [Creative Commons ShareALike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/).
 """
 
-VERSION = '1.0.1'
+VERSION = '1.0.3'
 
 setuptools.setup(
     name='pyvesc_fix',
     version=VERSION,
     packages=setuptools.find_packages(),
     install_requires=[
         'pyserial==3.5',
```

### Comparing `pyvesc_fix-1.0.1/tests/test_vesc.py` & `pyvesc_fix-1.0.3/tests/test_vesc.py`

 * *Files identical despite different names*

