# Comparing `tmp/lnt_hr_ai-0.0.4.tar.gz` & `tmp/lnt_hr_ai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnt_hr_ai-0.0.4.tar", last modified: Thu Apr 25 04:50:21 2024, max compression
+gzip compressed data, was "lnt_hr_ai-0.0.5.tar", last modified: Tue Apr 30 05:26:32 2024, max compression
```

## Comparing `lnt_hr_ai-0.0.4.tar` & `lnt_hr_ai-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 04:50:21.289841 lnt_hr_ai-0.0.4/
-drwxrwxrwx   0        0        0        0 2024-04-25 04:50:21.284926 lnt_hr_ai-0.0.4/DataAnalysis_Package/
--rw-rw-rw-   0        0        0     7576 2024-04-25 04:49:27.000000 lnt_hr_ai-0.0.4/DataAnalysis_Package/Data_PreProcessing.py
--rw-rw-rw-   0        0        0    46380 2024-04-25 04:49:24.000000 lnt_hr_ai-0.0.4/DataAnalysis_Package/Data_Visualization.py
--rw-rw-rw-   0        0        0    18374 2024-04-25 04:49:42.000000 lnt_hr_ai-0.0.4/DataAnalysis_Package/ML_MODELS.py
--rw-rw-rw-   0        0        0     4573 2024-04-25 04:45:16.000000 lnt_hr_ai-0.0.4/DataAnalysis_Package/Statistical_Analysis.py
--rw-rw-rw-   0        0        0      182 2024-04-23 08:32:50.000000 lnt_hr_ai-0.0.4/DataAnalysis_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 04:50:21.288844 lnt_hr_ai-0.0.4/LnT_HR_AI.egg-info/
--rw-rw-rw-   0        0        0      749 2024-04-25 04:50:21.000000 lnt_hr_ai-0.0.4/LnT_HR_AI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2024-04-25 04:50:21.000000 lnt_hr_ai-0.0.4/LnT_HR_AI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 04:50:21.000000 lnt_hr_ai-0.0.4/LnT_HR_AI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2024-04-25 04:50:21.000000 lnt_hr_ai-0.0.4/LnT_HR_AI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-25 04:50:21.000000 lnt_hr_ai-0.0.4/LnT_HR_AI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      749 2024-04-25 04:50:21.289841 lnt_hr_ai-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-23 09:03:04.000000 lnt_hr_ai-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-25 04:50:21.291347 lnt_hr_ai-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1042 2024-04-25 04:49:33.000000 lnt_hr_ai-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 05:26:32.344548 lnt_hr_ai-0.0.5/
+drwxrwxrwx   0        0        0        0 2024-04-30 05:26:32.339497 lnt_hr_ai-0.0.5/DataAnalysis_Package/
+-rw-rw-rw-   0        0        0     7576 2024-04-25 04:49:27.000000 lnt_hr_ai-0.0.5/DataAnalysis_Package/Data_PreProcessing.py
+-rw-rw-rw-   0        0        0    46380 2024-04-25 04:49:24.000000 lnt_hr_ai-0.0.5/DataAnalysis_Package/Data_Visualization.py
+-rw-rw-rw-   0        0        0    18374 2024-04-25 04:49:42.000000 lnt_hr_ai-0.0.5/DataAnalysis_Package/ML_MODELS.py
+-rw-rw-rw-   0        0        0     4573 2024-04-25 04:45:16.000000 lnt_hr_ai-0.0.5/DataAnalysis_Package/Statistical_Analysis.py
+-rw-rw-rw-   0        0        0      182 2024-04-30 05:26:25.000000 lnt_hr_ai-0.0.5/DataAnalysis_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 05:26:32.343546 lnt_hr_ai-0.0.5/LnT_HR_AI.egg-info/
+-rw-rw-rw-   0        0        0      749 2024-04-30 05:26:32.000000 lnt_hr_ai-0.0.5/LnT_HR_AI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2024-04-30 05:26:32.000000 lnt_hr_ai-0.0.5/LnT_HR_AI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 05:26:32.000000 lnt_hr_ai-0.0.5/LnT_HR_AI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      241 2024-04-30 05:26:32.000000 lnt_hr_ai-0.0.5/LnT_HR_AI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       82 2024-04-30 05:26:32.000000 lnt_hr_ai-0.0.5/LnT_HR_AI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-30 05:26:32.000000 lnt_hr_ai-0.0.5/LnT_HR_AI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      749 2024-04-30 05:26:32.343546 lnt_hr_ai-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-23 09:03:04.000000 lnt_hr_ai-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-30 05:26:32.344548 lnt_hr_ai-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1528 2024-04-30 05:25:53.000000 lnt_hr_ai-0.0.5/setup.py
```

### Comparing `lnt_hr_ai-0.0.4/DataAnalysis_Package/Data_PreProcessing.py` & `lnt_hr_ai-0.0.5/DataAnalysis_Package/Data_PreProcessing.py`

 * *Files identical despite different names*

### Comparing `lnt_hr_ai-0.0.4/DataAnalysis_Package/Data_Visualization.py` & `lnt_hr_ai-0.0.5/DataAnalysis_Package/Data_Visualization.py`

 * *Files identical despite different names*

### Comparing `lnt_hr_ai-0.0.4/DataAnalysis_Package/ML_MODELS.py` & `lnt_hr_ai-0.0.5/DataAnalysis_Package/ML_MODELS.py`

 * *Files identical despite different names*

### Comparing `lnt_hr_ai-0.0.4/DataAnalysis_Package/Statistical_Analysis.py` & `lnt_hr_ai-0.0.5/DataAnalysis_Package/Statistical_Analysis.py`

 * *Files identical despite different names*

### Comparing `lnt_hr_ai-0.0.4/LnT_HR_AI.egg-info/PKG-INFO` & `lnt_hr_ai-0.0.5/LnT_HR_AI.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LnT_HR_AI
-Version: 0.0.4
+Version: 0.0.5
 Summary: Data analysis for Attrition predictions
 Author: Radeesh
 Author-email: <vpsrad2002@gmail.com>
 Keywords: python,Machine Learning,Data Analysis,Data Science,Data processing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lnt_hr_ai-0.0.4/PKG-INFO` & `lnt_hr_ai-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LnT_HR_AI
-Version: 0.0.4
+Version: 0.0.5
 Summary: Data analysis for Attrition predictions
 Author: Radeesh
 Author-email: <vpsrad2002@gmail.com>
 Keywords: python,Machine Learning,Data Analysis,Data Science,Data processing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

