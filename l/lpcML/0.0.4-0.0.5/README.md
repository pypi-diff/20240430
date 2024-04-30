# Comparing `tmp/lpcML-0.0.4.tar.gz` & `tmp/lpcML-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpcML-0.0.4.tar", last modified: Tue Apr 30 09:59:19 2024, max compression
+gzip compressed data, was "lpcML-0.0.5.tar", last modified: Tue Apr 30 10:00:41 2024, max compression
```

## Comparing `lpcML-0.0.4.tar` & `lpcML-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:59:19.881209 lpcML-0.0.4/
--rw-rw-rw-   0 root         (0) root         (0)    35165 2024-04-30 09:59:07.000000 lpcML-0.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1646 2024-04-30 09:59:19.881209 lpcML-0.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      900 2024-04-30 09:59:07.000000 lpcML-0.0.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 09:59:19.881209 lpcML-0.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-30 09:59:07.000000 lpcML-0.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:59:19.877209 lpcML-0.0.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:59:19.881209 lpcML-0.0.4/src/lpcML/
--rw-rw-rw-   0 root         (0) root         (0)       97 2024-04-30 09:59:07.000000 lpcML-0.0.4/src/lpcML/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6594 2024-04-30 09:59:07.000000 lpcML-0.0.4/src/lpcML/data_processing.py
--rw-rw-rw-   0 root         (0) root         (0)     4012 2024-04-30 09:59:07.000000 lpcML-0.0.4/src/lpcML/model.py
--rw-rw-rw-   0 root         (0) root         (0)     4175 2024-04-30 09:59:07.000000 lpcML-0.0.4/src/lpcML/model_fitting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:59:19.881209 lpcML-0.0.4/src/lpcML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1646 2024-04-30 09:59:19.000000 lpcML-0.0.4/src/lpcML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      287 2024-04-30 09:59:19.000000 lpcML-0.0.4/src/lpcML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 09:59:19.000000 lpcML-0.0.4/src/lpcML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-30 09:59:19.000000 lpcML-0.0.4/src/lpcML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-30 09:59:19.000000 lpcML-0.0.4/src/lpcML.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:00:41.653283 lpcML-0.0.5/
+-rw-rw-rw-   0 root         (0) root         (0)    35165 2024-04-30 10:00:28.000000 lpcML-0.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1646 2024-04-30 10:00:41.653283 lpcML-0.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      900 2024-04-30 10:00:28.000000 lpcML-0.0.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 10:00:41.653283 lpcML-0.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-30 10:00:28.000000 lpcML-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:00:41.649283 lpcML-0.0.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:00:41.653283 lpcML-0.0.5/src/lpcML/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-04-30 10:00:28.000000 lpcML-0.0.5/src/lpcML/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6594 2024-04-30 10:00:28.000000 lpcML-0.0.5/src/lpcML/data_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4012 2024-04-30 10:00:28.000000 lpcML-0.0.5/src/lpcML/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4175 2024-04-30 10:00:28.000000 lpcML-0.0.5/src/lpcML/model_fitting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 10:00:41.653283 lpcML-0.0.5/src/lpcML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1646 2024-04-30 10:00:41.000000 lpcML-0.0.5/src/lpcML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      287 2024-04-30 10:00:41.000000 lpcML-0.0.5/src/lpcML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 10:00:41.000000 lpcML-0.0.5/src/lpcML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-30 10:00:41.000000 lpcML-0.0.5/src/lpcML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-30 10:00:41.000000 lpcML-0.0.5/src/lpcML.egg-info/top_level.txt
```

### Comparing `lpcML-0.0.4/LICENSE` & `lpcML-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lpcML-0.0.4/PKG-INFO` & `lpcML-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpcML
-Version: 0.0.4
+Version: 0.0.5
 Summary: LPC ML is a machine learning workflow developed to optimize and analyze the impact of different design parameters on laser power converters (LPCs) solar cells
 Home-page: https://gitlab.citius.usc.es/julian.garcia.fernandez/lpcML
 Author: Julian Garcia Fernandez 
 Author-email: julian.garcia.fernandez2@usc.es
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `lpcML-0.0.4/README.md` & `lpcML-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `lpcML-0.0.4/setup.py` & `lpcML-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description=''
     with open(Path(Path(__file__).parent,'README.md'), 'r') as fh:
         long_description=fh.read()
     return long_description
 
 setuptools.setup(
     name='lpcML',
-    version='0.0.4',
+    version='0.0.5',
     description='LPC ML is a machine learning workflow developed to optimize and analyze the impact of different design parameters on laser power converters (LPCs) solar cells',
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
     author='Julian Garcia Fernandez ',
     author_email='julian.garcia.fernandez2@usc.es',
     url='https://gitlab.citius.usc.es/julian.garcia.fernandez/lpcML',
     setup_requires=['setuptools'],
```

### Comparing `lpcML-0.0.4/src/lpcML/data_processing.py` & `lpcML-0.0.5/src/lpcML/data_processing.py`

 * *Files identical despite different names*

### Comparing `lpcML-0.0.4/src/lpcML/model.py` & `lpcML-0.0.5/src/lpcML/model.py`

 * *Files identical despite different names*

### Comparing `lpcML-0.0.4/src/lpcML/model_fitting.py` & `lpcML-0.0.5/src/lpcML/model_fitting.py`

 * *Files identical despite different names*

### Comparing `lpcML-0.0.4/src/lpcML.egg-info/PKG-INFO` & `lpcML-0.0.5/src/lpcML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpcML
-Version: 0.0.4
+Version: 0.0.5
 Summary: LPC ML is a machine learning workflow developed to optimize and analyze the impact of different design parameters on laser power converters (LPCs) solar cells
 Home-page: https://gitlab.citius.usc.es/julian.garcia.fernandez/lpcML
 Author: Julian Garcia Fernandez 
 Author-email: julian.garcia.fernandez2@usc.es
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

