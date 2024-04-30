# Comparing `tmp/symetrics-8.0.0.tar.gz` & `tmp/symetrics-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symetrics-8.0.0.tar", last modified: Tue Apr 30 06:27:29 2024, max compression
+gzip compressed data, was "symetrics-9.0.0.tar", last modified: Tue Apr 30 06:52:16 2024, max compression
```

## Comparing `symetrics-8.0.0.tar` & `symetrics-9.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 06:27:29.407931 symetrics-8.0.0/
--rw-rw-rw-   0        0        0     1151 2024-04-30 06:27:29.406964 symetrics-8.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-30 06:27:29.407931 symetrics-8.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1640 2024-04-30 06:27:22.000000 symetrics-8.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:27:29.380338 symetrics-8.0.0/symetrics/
--rw-rw-rw-   0        0        0      101 2023-12-09 13:09:42.000000 symetrics-8.0.0/symetrics/__init__.py
--rw-rw-rw-   0        0        0      519 2023-12-09 13:09:33.000000 symetrics-8.0.0/symetrics/dbcontext.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:27:29.405825 symetrics-8.0.0/symetrics/src/
--rw-rw-rw-   0        0        0       25 2023-10-25 09:08:07.000000 symetrics-8.0.0/symetrics/src/__init__.py
--rw-rw-rw-   0        0        0      967 2024-01-31 08:23:38.000000 symetrics-8.0.0/symetrics/src/datastruct.py
--rw-rw-rw-   0        0        0    22249 2024-04-30 06:26:19.000000 symetrics-8.0.0/symetrics/symetrics_api.py
-drwxrwxrwx   0        0        0        0 2024-04-30 06:27:29.400491 symetrics-8.0.0/symetrics.egg-info/
--rw-rw-rw-   0        0        0     1151 2024-04-30 06:27:29.000000 symetrics-8.0.0/symetrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2024-04-30 06:27:29.000000 symetrics-8.0.0/symetrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 06:27:29.000000 symetrics-8.0.0/symetrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-30 06:27:29.000000 symetrics-8.0.0/symetrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-30 06:27:29.000000 symetrics-8.0.0/symetrics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 06:52:16.049873 symetrics-9.0.0/
+-rw-rw-rw-   0        0        0     1151 2024-04-30 06:52:16.049873 symetrics-9.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-30 06:52:16.049873 symetrics-9.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1640 2024-04-30 06:52:13.000000 symetrics-9.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:52:16.022906 symetrics-9.0.0/symetrics/
+-rw-rw-rw-   0        0        0      101 2023-12-09 13:09:42.000000 symetrics-9.0.0/symetrics/__init__.py
+-rw-rw-rw-   0        0        0      519 2023-12-09 13:09:33.000000 symetrics-9.0.0/symetrics/dbcontext.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:52:16.049873 symetrics-9.0.0/symetrics/src/
+-rw-rw-rw-   0        0        0       25 2023-10-25 09:08:07.000000 symetrics-9.0.0/symetrics/src/__init__.py
+-rw-rw-rw-   0        0        0     1035 2024-04-30 06:51:43.000000 symetrics-9.0.0/symetrics/src/datastruct.py
+-rw-rw-rw-   0        0        0    22249 2024-04-30 06:26:19.000000 symetrics-9.0.0/symetrics/symetrics_api.py
+drwxrwxrwx   0        0        0        0 2024-04-30 06:52:16.044515 symetrics-9.0.0/symetrics.egg-info/
+-rw-rw-rw-   0        0        0     1151 2024-04-30 06:52:15.000000 symetrics-9.0.0/symetrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2024-04-30 06:52:15.000000 symetrics-9.0.0/symetrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 06:52:15.000000 symetrics-9.0.0/symetrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-30 06:52:15.000000 symetrics-9.0.0/symetrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-30 06:52:15.000000 symetrics-9.0.0/symetrics.egg-info/top_level.txt
```

### Comparing `symetrics-8.0.0/PKG-INFO` & `symetrics-9.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symetrics
-Version: 8.0.0
+Version: 9.0.0
 Summary: Symetrics API
 Home-page: https://lbundalian.github.io/symetrics/
 Author: Linnaeus Bundalian
 Author-email: linnaeusbundalian@gmail.com
 Keywords: python,synonymous variants
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `symetrics-8.0.0/setup.py` & `symetrics-9.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '8.0.0' 
+VERSION = '9.0.0' 
 DESCRIPTION = 'Symetrics API'
 LONG_DESCRIPTION = '''A package to access SYMETRICS database. 
 SYMETRICS database is a consolidation of metrics for synonymous variants which were derived from a number of computational tools each of which contributing to 
 attribute specific metrics such as SYNVEP for general functional constraints, SpliceAI for splicing effect, SILVA for obtaining GERP++ (phylogenetic related constraints)
 CpG/CpG_Exon, dRSCU/RSCU for codon usage and SURF for rna stability. The package also includes a result of the analysis of the influence of each variants exceeding set threshold
 per metrics defined constituting to a score assigned to a gene'''
 REQUIRED_PACKAGES = [
```

### Comparing `symetrics-8.0.0/symetrics/dbcontext.py` & `symetrics-9.0.0/symetrics/dbcontext.py`

 * *Files identical despite different names*

### Comparing `symetrics-8.0.0/symetrics/src/datastruct.py` & `symetrics-9.0.0/symetrics/src/datastruct.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,14 +10,18 @@
     CPGX = auto()
     CPG = auto()
     DRSCU = auto()
     GERP = auto()
     SYNVEP = auto()
     SPLICEAI = auto()
 
+    SPLICE = auto()
+    CPGEXON = auto()
+    CPGLogit = auto()
+
 class GenomeReference(Enum):
 
     '''
     Lists of all possible genome reference for the package
     
     '''
     hg19 = auto()
```

### Comparing `symetrics-8.0.0/symetrics/symetrics_api.py` & `symetrics-9.0.0/symetrics/symetrics_api.py`

 * *Files identical despite different names*

### Comparing `symetrics-8.0.0/symetrics.egg-info/PKG-INFO` & `symetrics-9.0.0/symetrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symetrics
-Version: 8.0.0
+Version: 9.0.0
 Summary: Symetrics API
 Home-page: https://lbundalian.github.io/symetrics/
 Author: Linnaeus Bundalian
 Author-email: linnaeusbundalian@gmail.com
 Keywords: python,synonymous variants
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

