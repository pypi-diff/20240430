# Comparing `tmp/STpipe-sc-0.0.3.tar.gz` & `tmp/STpipe-sc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STpipe-sc-0.0.3.tar", last modified: Tue Apr 30 12:15:45 2024, max compression
+gzip compressed data, was "STpipe-sc-0.0.4.tar", last modified: Tue Apr 30 12:26:29 2024, max compression
```

## Comparing `STpipe-sc-0.0.3.tar` & `STpipe-sc-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 12:15:45.495255 STpipe-sc-0.0.3/
--rw-rw-rw-   0        0        0      942 2024-04-30 12:15:45.491203 STpipe-sc-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-30 12:15:45.414989 STpipe-sc-0.0.3/STpipe_sc.egg-info/
--rw-rw-rw-   0        0        0      942 2024-04-30 12:15:44.000000 STpipe-sc-0.0.3/STpipe_sc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2024-04-30 12:15:45.000000 STpipe-sc-0.0.3/STpipe_sc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 12:15:44.000000 STpipe-sc-0.0.3/STpipe_sc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      352 2024-04-30 12:15:44.000000 STpipe-sc-0.0.3/STpipe_sc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-30 12:15:44.000000 STpipe-sc-0.0.3/STpipe_sc.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-30 12:15:45.386979 STpipe-sc-0.0.3/git/
-drwxrwxrwx   0        0        0        0 2024-04-30 12:15:45.387978 STpipe-sc-0.0.3/git/STpipe/
-drwxrwxrwx   0        0        0        0 2024-04-30 12:15:45.450966 STpipe-sc-0.0.3/git/STpipe/stpipe/
--rw-rw-rw-   0        0        0     3771 2024-04-05 16:09:58.000000 STpipe-sc-0.0.3/git/STpipe/stpipe/Findmarkers.py
--rw-rw-rw-   0        0        0    18514 2024-03-31 00:45:27.000000 STpipe-sc-0.0.3/git/STpipe/stpipe/QC.py
--rw-rw-rw-   0        0        0      195 2024-03-24 13:36:13.000000 STpipe-sc-0.0.3/git/STpipe/stpipe/__init__.py
--rw-rw-rw-   0        0        0     1688 2024-04-05 16:09:58.000000 STpipe-sc-0.0.3/git/STpipe/stpipe/cluster.py
--rw-rw-rw-   0        0        0     9970 2024-03-25 17:33:55.000000 STpipe-sc-0.0.3/git/STpipe/stpipe/format.py
--rw-rw-rw-   0        0        0    22097 2024-04-05 16:12:07.000000 STpipe-sc-0.0.3/git/STpipe/stpipe/function.py
--rw-rw-rw-   0        0        0     2527 2024-04-05 16:09:58.000000 STpipe-sc-0.0.3/git/STpipe/stpipe/labeltransfer.py
--rw-rw-rw-   0        0        0    37017 2024-04-05 16:12:05.000000 STpipe-sc-0.0.3/git/STpipe/stpipe/plot.py
--rw-rw-rw-   0        0        0     5580 2024-04-05 16:09:57.000000 STpipe-sc-0.0.3/git/STpipe/stpipe/spatial_metacell.py
--rw-rw-rw-   0        0        0       42 2024-04-30 12:15:45.495255 STpipe-sc-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1098 2024-04-30 12:15:14.000000 STpipe-sc-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 12:15:45.486143 STpipe-sc-0.0.3/stpipe/
--rw-rw-rw-   0        0        0     3771 2024-04-05 16:09:58.000000 STpipe-sc-0.0.3/stpipe/Findmarkers.py
--rw-rw-rw-   0        0        0    18514 2024-03-31 00:45:27.000000 STpipe-sc-0.0.3/stpipe/QC.py
--rw-rw-rw-   0        0        0      195 2024-03-24 13:36:13.000000 STpipe-sc-0.0.3/stpipe/__init__.py
--rw-rw-rw-   0        0        0     1688 2024-04-05 16:09:58.000000 STpipe-sc-0.0.3/stpipe/cluster.py
--rw-rw-rw-   0        0        0     9970 2024-03-25 17:33:55.000000 STpipe-sc-0.0.3/stpipe/format.py
--rw-rw-rw-   0        0        0    22097 2024-04-05 16:12:07.000000 STpipe-sc-0.0.3/stpipe/function.py
--rw-rw-rw-   0        0        0     2527 2024-04-05 16:09:58.000000 STpipe-sc-0.0.3/stpipe/labeltransfer.py
--rw-rw-rw-   0        0        0    37017 2024-04-05 16:12:05.000000 STpipe-sc-0.0.3/stpipe/plot.py
--rw-rw-rw-   0        0        0     5580 2024-04-05 16:09:57.000000 STpipe-sc-0.0.3/stpipe/spatial_metacell.py
+drwxrwxrwx   0        0        0        0 2024-04-30 12:26:29.224020 STpipe-sc-0.0.4/
+-rw-rw-rw-   0        0        0      944 2024-04-30 12:26:29.224020 STpipe-sc-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 12:26:29.174046 STpipe-sc-0.0.4/STpipe_sc.egg-info/
+-rw-rw-rw-   0        0        0      944 2024-04-30 12:26:28.000000 STpipe-sc-0.0.4/STpipe_sc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2024-04-30 12:26:29.000000 STpipe-sc-0.0.4/STpipe_sc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 12:26:28.000000 STpipe-sc-0.0.4/STpipe_sc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      352 2024-04-30 12:26:28.000000 STpipe-sc-0.0.4/STpipe_sc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-30 12:26:28.000000 STpipe-sc-0.0.4/STpipe_sc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 12:26:29.154053 STpipe-sc-0.0.4/git/
+drwxrwxrwx   0        0        0        0 2024-04-30 12:26:29.154053 STpipe-sc-0.0.4/git/STpipe/
+drwxrwxrwx   0        0        0        0 2024-04-30 12:26:29.194036 STpipe-sc-0.0.4/git/STpipe/stpipe/
+-rw-rw-rw-   0        0        0     3771 2024-04-05 16:09:58.000000 STpipe-sc-0.0.4/git/STpipe/stpipe/Findmarkers.py
+-rw-rw-rw-   0        0        0    18514 2024-03-31 00:45:27.000000 STpipe-sc-0.0.4/git/STpipe/stpipe/QC.py
+-rw-rw-rw-   0        0        0      195 2024-03-24 13:36:13.000000 STpipe-sc-0.0.4/git/STpipe/stpipe/__init__.py
+-rw-rw-rw-   0        0        0     1688 2024-04-05 16:09:58.000000 STpipe-sc-0.0.4/git/STpipe/stpipe/cluster.py
+-rw-rw-rw-   0        0        0     9970 2024-03-25 17:33:55.000000 STpipe-sc-0.0.4/git/STpipe/stpipe/format.py
+-rw-rw-rw-   0        0        0    22097 2024-04-05 16:12:07.000000 STpipe-sc-0.0.4/git/STpipe/stpipe/function.py
+-rw-rw-rw-   0        0        0     2527 2024-04-05 16:09:58.000000 STpipe-sc-0.0.4/git/STpipe/stpipe/labeltransfer.py
+-rw-rw-rw-   0        0        0    37017 2024-04-05 16:12:05.000000 STpipe-sc-0.0.4/git/STpipe/stpipe/plot.py
+-rw-rw-rw-   0        0        0     5580 2024-04-05 16:09:57.000000 STpipe-sc-0.0.4/git/STpipe/stpipe/spatial_metacell.py
+-rw-rw-rw-   0        0        0       42 2024-04-30 12:26:29.224020 STpipe-sc-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2024-04-30 12:26:13.000000 STpipe-sc-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 12:26:29.224020 STpipe-sc-0.0.4/stpipe/
+-rw-rw-rw-   0        0        0     3771 2024-04-05 16:09:58.000000 STpipe-sc-0.0.4/stpipe/Findmarkers.py
+-rw-rw-rw-   0        0        0    18514 2024-03-31 00:45:27.000000 STpipe-sc-0.0.4/stpipe/QC.py
+-rw-rw-rw-   0        0        0      195 2024-03-24 13:36:13.000000 STpipe-sc-0.0.4/stpipe/__init__.py
+-rw-rw-rw-   0        0        0     1688 2024-04-05 16:09:58.000000 STpipe-sc-0.0.4/stpipe/cluster.py
+-rw-rw-rw-   0        0        0     9970 2024-03-25 17:33:55.000000 STpipe-sc-0.0.4/stpipe/format.py
+-rw-rw-rw-   0        0        0    22097 2024-04-05 16:12:07.000000 STpipe-sc-0.0.4/stpipe/function.py
+-rw-rw-rw-   0        0        0     2527 2024-04-05 16:09:58.000000 STpipe-sc-0.0.4/stpipe/labeltransfer.py
+-rw-rw-rw-   0        0        0    37017 2024-04-05 16:12:05.000000 STpipe-sc-0.0.4/stpipe/plot.py
+-rw-rw-rw-   0        0        0     5580 2024-04-05 16:09:57.000000 STpipe-sc-0.0.4/stpipe/spatial_metacell.py
```

### Comparing `STpipe-sc-0.0.3/PKG-INFO` & `STpipe-sc-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: STpipe-sc
-Version: 0.0.3
+Version: 0.0.4
 Summary: STpipe is designed to analyze spatial transcriptomic data.
 Home-page: https://github.com/mgy520/STpipe
 Author: Mao Guangyao
 License: MIT License
-Requires-Python: ==3.8
+Requires-Python: ==3.8.*
 Requires-Dist: rpy2==3.5.16
 Requires-Dist: anndata2ri==1.3.1
 Requires-Dist: numpy==1.21.6
 Requires-Dist: diffxpy==0.7.4
 Requires-Dist: scipy==1.10.1
 Requires-Dist: pandas==2.0.3
 Requires-Dist: anndata==0.9.2
```

### Comparing `STpipe-sc-0.0.3/STpipe_sc.egg-info/PKG-INFO` & `STpipe-sc-0.0.4/STpipe_sc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: STpipe-sc
-Version: 0.0.3
+Version: 0.0.4
 Summary: STpipe is designed to analyze spatial transcriptomic data.
 Home-page: https://github.com/mgy520/STpipe
 Author: Mao Guangyao
 License: MIT License
-Requires-Python: ==3.8
+Requires-Python: ==3.8.*
 Requires-Dist: rpy2==3.5.16
 Requires-Dist: anndata2ri==1.3.1
 Requires-Dist: numpy==1.21.6
 Requires-Dist: diffxpy==0.7.4
 Requires-Dist: scipy==1.10.1
 Requires-Dist: pandas==2.0.3
 Requires-Dist: anndata==0.9.2
```

### Comparing `STpipe-sc-0.0.3/STpipe_sc.egg-info/SOURCES.txt` & `STpipe-sc-0.0.4/STpipe_sc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.3/git/STpipe/stpipe/Findmarkers.py` & `STpipe-sc-0.0.4/git/STpipe/stpipe/Findmarkers.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.3/git/STpipe/stpipe/QC.py` & `STpipe-sc-0.0.4/git/STpipe/stpipe/QC.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.3/git/STpipe/stpipe/cluster.py` & `STpipe-sc-0.0.4/git/STpipe/stpipe/cluster.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.3/git/STpipe/stpipe/format.py` & `STpipe-sc-0.0.4/git/STpipe/stpipe/format.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.3/git/STpipe/stpipe/function.py` & `STpipe-sc-0.0.4/git/STpipe/stpipe/function.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.3/git/STpipe/stpipe/labeltransfer.py` & `STpipe-sc-0.0.4/git/STpipe/stpipe/labeltransfer.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.3/git/STpipe/stpipe/plot.py` & `STpipe-sc-0.0.4/git/STpipe/stpipe/plot.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.3/git/STpipe/stpipe/spatial_metacell.py` & `STpipe-sc-0.0.4/git/STpipe/stpipe/spatial_metacell.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.3/setup.py` & `STpipe-sc-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='STpipe-sc',
-    version='0.0.3',
+    version='0.0.4',
     description=('STpipe is designed to analyze spatial transcriptomic data.'),
     author='Mao Guangyao',
     license='MIT License',
     url='https://github.com/mgy520/STpipe',
     packages=find_namespace_packages(),
-    python_requires='==3.8',
+    python_requires='==3.8.*',
     install_requires=[
             'rpy2==3.5.16',
             'anndata2ri==1.3.1',
             'numpy==1.21.6',
             'diffxpy==0.7.4',
             'scipy==1.10.1',
             'pandas==2.0.3',
```

### Comparing `STpipe-sc-0.0.3/stpipe/Findmarkers.py` & `STpipe-sc-0.0.4/stpipe/Findmarkers.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.3/stpipe/QC.py` & `STpipe-sc-0.0.4/stpipe/QC.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.3/stpipe/cluster.py` & `STpipe-sc-0.0.4/stpipe/cluster.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.3/stpipe/format.py` & `STpipe-sc-0.0.4/stpipe/format.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.3/stpipe/function.py` & `STpipe-sc-0.0.4/stpipe/function.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.3/stpipe/labeltransfer.py` & `STpipe-sc-0.0.4/stpipe/labeltransfer.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.3/stpipe/plot.py` & `STpipe-sc-0.0.4/stpipe/plot.py`

 * *Files identical despite different names*

### Comparing `STpipe-sc-0.0.3/stpipe/spatial_metacell.py` & `STpipe-sc-0.0.4/stpipe/spatial_metacell.py`

 * *Files identical despite different names*

