# Comparing `tmp/lpcML-0.0.2.tar.gz` & `tmp/lpcML-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpcML-0.0.2.tar", last modified: Mon Apr 29 11:26:17 2024, max compression
+gzip compressed data, was "lpcML-0.0.3.tar", last modified: Tue Apr 30 09:31:56 2024, max compression
```

## Comparing `lpcML-0.0.2.tar` & `lpcML-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:26:17.954879 lpcML-0.0.2/
--rw-rw-rw-   0 root         (0) root         (0)    35165 2024-04-29 11:26:05.000000 lpcML-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1628 2024-04-29 11:26:17.954879 lpcML-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      882 2024-04-29 11:26:05.000000 lpcML-0.0.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 11:26:17.954879 lpcML-0.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-29 11:26:05.000000 lpcML-0.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:26:17.954879 lpcML-0.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 11:26:17.954879 lpcML-0.0.2/src/lpcML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1628 2024-04-29 11:26:17.000000 lpcML-0.0.2/src/lpcML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      190 2024-04-29 11:26:17.000000 lpcML-0.0.2/src/lpcML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 11:26:17.000000 lpcML-0.0.2/src/lpcML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-29 11:26:17.000000 lpcML-0.0.2/src/lpcML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 11:26:17.000000 lpcML-0.0.2/src/lpcML.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:31:56.611522 lpcML-0.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)    35165 2024-04-30 09:31:44.000000 lpcML-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1646 2024-04-30 09:31:56.611522 lpcML-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      900 2024-04-30 09:31:44.000000 lpcML-0.0.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 09:31:56.611522 lpcML-0.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-30 09:31:44.000000 lpcML-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:31:56.611522 lpcML-0.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:31:56.611522 lpcML-0.0.3/src/lpcML/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-04-30 09:31:44.000000 lpcML-0.0.3/src/lpcML/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6736 2024-04-30 09:31:44.000000 lpcML-0.0.3/src/lpcML/data_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4012 2024-04-30 09:31:44.000000 lpcML-0.0.3/src/lpcML/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4200 2024-04-30 09:31:44.000000 lpcML-0.0.3/src/lpcML/model_fitting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:31:56.611522 lpcML-0.0.3/src/lpcML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1646 2024-04-30 09:31:56.000000 lpcML-0.0.3/src/lpcML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      287 2024-04-30 09:31:56.000000 lpcML-0.0.3/src/lpcML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 09:31:56.000000 lpcML-0.0.3/src/lpcML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-30 09:31:56.000000 lpcML-0.0.3/src/lpcML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-30 09:31:56.000000 lpcML-0.0.3/src/lpcML.egg-info/top_level.txt
```

### Comparing `lpcML-0.0.2/LICENSE` & `lpcML-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lpcML-0.0.2/PKG-INFO` & `lpcML-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpcML
-Version: 0.0.2
+Version: 0.0.3
 Summary: LPC ML is a machine learning workflow developed to optimize and analyze the impact of different design parameters on laser power converters (LPCs) solar cells
 Home-page: https://gitlab.citius.usc.es/julian.garcia.fernandez/lpcML
 Author: Julian Garcia Fernandez 
 Author-email: julian.garcia.fernandez2@usc.es
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -15,15 +15,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LPC ML
 
 LPC ML is a tool developed in the CiTIUS, USC by the MODEV group for training a multi-layer perceptron (MLP) neural network to optimize and analyze the impact of different design parameters on laser power converters (LPCs) solar cells.
 
-**Fig.1:** TODO: LPC SCHEME
+![img](images/lpc.PNG)
+
+**Fig.1:** LPC SCHEME
 <!-- Data used to feed the neural networks is shared in the following Zenodo Repository [https://doi.org/10.5281/zenodo.11032095](https://doi.org/10.5281/zenodo.11032095). -->
 
 ## Installation
 First you need to have installed **pip3** on your system. For Ubuntu, open up a terminal and type:
 
     sudo apt update
     sudo apt install python3-pip
```

### Comparing `lpcML-0.0.2/README.md` & `lpcML-0.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # LPC ML
 
 LPC ML is a tool developed in the CiTIUS, USC by the MODEV group for training a multi-layer perceptron (MLP) neural network to optimize and analyze the impact of different design parameters on laser power converters (LPCs) solar cells.
 
-**Fig.1:** TODO: LPC SCHEME
+![img](images/lpc.PNG)
+
+**Fig.1:** LPC SCHEME
 <!-- Data used to feed the neural networks is shared in the following Zenodo Repository [https://doi.org/10.5281/zenodo.11032095](https://doi.org/10.5281/zenodo.11032095). -->
 
 ## Installation
 First you need to have installed **pip3** on your system. For Ubuntu, open up a terminal and type:
 
     sudo apt update
     sudo apt install python3-pip
```

### Comparing `lpcML-0.0.2/setup.py` & `lpcML-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description=''
     with open(Path(Path(__file__).parent,'README.md'), 'r') as fh:
         long_description=fh.read()
     return long_description
 
 setuptools.setup(
     name='lpcML',
-    version='0.0.2',
+    version='0.0.3',
     description='LPC ML is a machine learning workflow developed to optimize and analyze the impact of different design parameters on laser power converters (LPCs) solar cells',
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
     author='Julian Garcia Fernandez ',
     author_email='julian.garcia.fernandez2@usc.es',
     url='https://gitlab.citius.usc.es/julian.garcia.fernandez/lpcML',
     setup_requires=['setuptools'],
```

### Comparing `lpcML-0.0.2/src/lpcML.egg-info/PKG-INFO` & `lpcML-0.0.3/src/lpcML.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpcML
-Version: 0.0.2
+Version: 0.0.3
 Summary: LPC ML is a machine learning workflow developed to optimize and analyze the impact of different design parameters on laser power converters (LPCs) solar cells
 Home-page: https://gitlab.citius.usc.es/julian.garcia.fernandez/lpcML
 Author: Julian Garcia Fernandez 
 Author-email: julian.garcia.fernandez2@usc.es
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -15,15 +15,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LPC ML
 
 LPC ML is a tool developed in the CiTIUS, USC by the MODEV group for training a multi-layer perceptron (MLP) neural network to optimize and analyze the impact of different design parameters on laser power converters (LPCs) solar cells.
 
-**Fig.1:** TODO: LPC SCHEME
+![img](images/lpc.PNG)
+
+**Fig.1:** LPC SCHEME
 <!-- Data used to feed the neural networks is shared in the following Zenodo Repository [https://doi.org/10.5281/zenodo.11032095](https://doi.org/10.5281/zenodo.11032095). -->
 
 ## Installation
 First you need to have installed **pip3** on your system. For Ubuntu, open up a terminal and type:
 
     sudo apt update
     sudo apt install python3-pip
```

