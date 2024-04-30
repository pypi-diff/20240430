# Comparing `tmp/lnt_hr_ai-0.0.5.tar.gz` & `tmp/lnt_hr_ai-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnt_hr_ai-0.0.5.tar", last modified: Tue Apr 30 05:26:32 2024, max compression
+gzip compressed data, was "lnt_hr_ai-0.0.6.tar", last modified: Tue Apr 30 05:35:35 2024, max compression
```

## Comparing `lnt_hr_ai-0.0.5.tar` & `lnt_hr_ai-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 05:26:32.344548 lnt_hr_ai-0.0.5/
-drwxrwxrwx   0        0        0        0 2024-04-30 05:26:32.339497 lnt_hr_ai-0.0.5/DataAnalysis_Package/
--rw-rw-rw-   0        0        0     7576 2024-04-25 04:49:27.000000 lnt_hr_ai-0.0.5/DataAnalysis_Package/Data_PreProcessing.py
--rw-rw-rw-   0        0        0    46380 2024-04-25 04:49:24.000000 lnt_hr_ai-0.0.5/DataAnalysis_Package/Data_Visualization.py
--rw-rw-rw-   0        0        0    18374 2024-04-25 04:49:42.000000 lnt_hr_ai-0.0.5/DataAnalysis_Package/ML_MODELS.py
--rw-rw-rw-   0        0        0     4573 2024-04-25 04:45:16.000000 lnt_hr_ai-0.0.5/DataAnalysis_Package/Statistical_Analysis.py
--rw-rw-rw-   0        0        0      182 2024-04-30 05:26:25.000000 lnt_hr_ai-0.0.5/DataAnalysis_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 05:26:32.343546 lnt_hr_ai-0.0.5/LnT_HR_AI.egg-info/
--rw-rw-rw-   0        0        0      749 2024-04-30 05:26:32.000000 lnt_hr_ai-0.0.5/LnT_HR_AI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2024-04-30 05:26:32.000000 lnt_hr_ai-0.0.5/LnT_HR_AI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 05:26:32.000000 lnt_hr_ai-0.0.5/LnT_HR_AI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      241 2024-04-30 05:26:32.000000 lnt_hr_ai-0.0.5/LnT_HR_AI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       82 2024-04-30 05:26:32.000000 lnt_hr_ai-0.0.5/LnT_HR_AI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-30 05:26:32.000000 lnt_hr_ai-0.0.5/LnT_HR_AI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      749 2024-04-30 05:26:32.343546 lnt_hr_ai-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-23 09:03:04.000000 lnt_hr_ai-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-30 05:26:32.344548 lnt_hr_ai-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1528 2024-04-30 05:25:53.000000 lnt_hr_ai-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 05:35:35.604650 lnt_hr_ai-0.0.6/
+drwxrwxrwx   0        0        0        0 2024-04-30 05:35:35.596620 lnt_hr_ai-0.0.6/DataAnalysis_Package/
+-rw-rw-rw-   0        0        0     7576 2024-04-25 04:49:27.000000 lnt_hr_ai-0.0.6/DataAnalysis_Package/Data_PreProcessing.py
+-rw-rw-rw-   0        0        0    46380 2024-04-25 04:49:24.000000 lnt_hr_ai-0.0.6/DataAnalysis_Package/Data_Visualization.py
+-rw-rw-rw-   0        0        0    18374 2024-04-25 04:49:42.000000 lnt_hr_ai-0.0.6/DataAnalysis_Package/ML_MODELS.py
+-rw-rw-rw-   0        0        0     4573 2024-04-25 04:45:16.000000 lnt_hr_ai-0.0.6/DataAnalysis_Package/Statistical_Analysis.py
+-rw-rw-rw-   0        0        0      182 2024-04-30 05:26:25.000000 lnt_hr_ai-0.0.6/DataAnalysis_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 05:35:35.602648 lnt_hr_ai-0.0.6/LnT_HR_AI.egg-info/
+-rw-rw-rw-   0        0        0      749 2024-04-30 05:35:35.000000 lnt_hr_ai-0.0.6/LnT_HR_AI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2024-04-30 05:35:35.000000 lnt_hr_ai-0.0.6/LnT_HR_AI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 05:35:35.000000 lnt_hr_ai-0.0.6/LnT_HR_AI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      241 2024-04-30 05:35:35.000000 lnt_hr_ai-0.0.6/LnT_HR_AI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       82 2024-04-30 05:35:35.000000 lnt_hr_ai-0.0.6/LnT_HR_AI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-30 05:35:35.000000 lnt_hr_ai-0.0.6/LnT_HR_AI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      749 2024-04-30 05:35:35.602648 lnt_hr_ai-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-23 09:03:04.000000 lnt_hr_ai-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-30 05:35:35.604650 lnt_hr_ai-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1528 2024-04-30 05:35:10.000000 lnt_hr_ai-0.0.6/setup.py
```

### Comparing `lnt_hr_ai-0.0.5/DataAnalysis_Package/Data_PreProcessing.py` & `lnt_hr_ai-0.0.6/DataAnalysis_Package/Data_PreProcessing.py`

 * *Files identical despite different names*

### Comparing `lnt_hr_ai-0.0.5/DataAnalysis_Package/Data_Visualization.py` & `lnt_hr_ai-0.0.6/DataAnalysis_Package/Data_Visualization.py`

 * *Files identical despite different names*

### Comparing `lnt_hr_ai-0.0.5/DataAnalysis_Package/ML_MODELS.py` & `lnt_hr_ai-0.0.6/DataAnalysis_Package/ML_MODELS.py`

 * *Files identical despite different names*

### Comparing `lnt_hr_ai-0.0.5/DataAnalysis_Package/Statistical_Analysis.py` & `lnt_hr_ai-0.0.6/DataAnalysis_Package/Statistical_Analysis.py`

 * *Files identical despite different names*

### Comparing `lnt_hr_ai-0.0.5/LnT_HR_AI.egg-info/PKG-INFO` & `lnt_hr_ai-0.0.6/LnT_HR_AI.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LnT_HR_AI
-Version: 0.0.5
+Version: 0.0.6
 Summary: Data analysis for Attrition predictions
 Author: Radeesh
 Author-email: <vpsrad2002@gmail.com>
 Keywords: python,Machine Learning,Data Analysis,Data Science,Data processing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lnt_hr_ai-0.0.5/PKG-INFO` & `lnt_hr_ai-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LnT_HR_AI
-Version: 0.0.5
+Version: 0.0.6
 Summary: Data analysis for Attrition predictions
 Author: Radeesh
 Author-email: <vpsrad2002@gmail.com>
 Keywords: python,Machine Learning,Data Analysis,Data Science,Data processing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lnt_hr_ai-0.0.5/setup.py` & `lnt_hr_ai-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Data analysis for Attrition predictions'
 # Setting up
 setup(
     name="LnT_HR_AI",
     version=VERSION,
     author="Radeesh",
     author_email="<vpsrad2002@gmail.com>",
```

