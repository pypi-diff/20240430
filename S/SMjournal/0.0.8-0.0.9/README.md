# Comparing `tmp/SMjournal-0.0.8.tar.gz` & `tmp/SMjournal-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMjournal-0.0.8.tar", last modified: Fri Apr 12 15:35:26 2024, max compression
+gzip compressed data, was "SMjournal-0.0.9.tar", last modified: Fri Apr 12 15:40:18 2024, max compression
```

## Comparing `SMjournal-0.0.8.tar` & `SMjournal-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 agus      (1000) agus      (1000)        0 2024-04-12 15:35:26.762371 SMjournal-0.0.8/
--rw-rw-r--   0 agus      (1000) agus      (1000)     1077 2024-04-11 13:57:24.000000 SMjournal-0.0.8/LICENSE
--rw-r--r--   0 agus      (1000) agus      (1000)      679 2024-04-12 15:35:26.762371 SMjournal-0.0.8/PKG-INFO
--rw-rw-r--   0 agus      (1000) agus      (1000)        0 2024-04-11 13:57:24.000000 SMjournal-0.0.8/README.md
-drwxrwxr-x   0 agus      (1000) agus      (1000)        0 2024-04-12 15:35:26.758371 SMjournal-0.0.8/SMjournal/
--rw-rw-r--   0 agus      (1000) agus      (1000)      124 2024-04-11 13:57:24.000000 SMjournal-0.0.8/SMjournal/__init__.py
--rw-rw-r--   0 agus      (1000) agus      (1000)     4970 2024-04-12 15:34:47.000000 SMjournal-0.0.8/SMjournal/collinearity.py
--rw-rw-r--   0 agus      (1000) agus      (1000)     4690 2024-04-11 13:57:24.000000 SMjournal-0.0.8/SMjournal/data.py
--rw-rw-r--   0 agus      (1000) agus      (1000)     1512 2024-04-11 13:57:24.000000 SMjournal-0.0.8/SMjournal/low_level.py
--rw-rw-r--   0 agus      (1000) agus      (1000)     4434 2024-04-11 13:57:24.000000 SMjournal-0.0.8/SMjournal/meta_reg.py
--rw-rw-r--   0 agus      (1000) agus      (1000)     2928 2024-04-11 13:57:24.000000 SMjournal-0.0.8/SMjournal/potentiality.py
-drwxrwxr-x   0 agus      (1000) agus      (1000)        0 2024-04-12 15:35:26.758371 SMjournal-0.0.8/SMjournal.egg-info/
--rw-r--r--   0 agus      (1000) agus      (1000)      679 2024-04-12 15:35:26.000000 SMjournal-0.0.8/SMjournal.egg-info/PKG-INFO
--rw-rw-r--   0 agus      (1000) agus      (1000)      343 2024-04-12 15:35:26.000000 SMjournal-0.0.8/SMjournal.egg-info/SOURCES.txt
--rw-rw-r--   0 agus      (1000) agus      (1000)        1 2024-04-12 15:35:26.000000 SMjournal-0.0.8/SMjournal.egg-info/dependency_links.txt
--rw-rw-r--   0 agus      (1000) agus      (1000)       88 2024-04-12 15:35:26.000000 SMjournal-0.0.8/SMjournal.egg-info/requires.txt
--rw-rw-r--   0 agus      (1000) agus      (1000)       10 2024-04-12 15:35:26.000000 SMjournal-0.0.8/SMjournal.egg-info/top_level.txt
--rw-rw-r--   0 agus      (1000) agus      (1000)      106 2024-04-11 13:57:24.000000 SMjournal-0.0.8/pyproject.toml
--rw-rw-r--   0 agus      (1000) agus      (1000)      633 2024-04-12 15:35:26.762371 SMjournal-0.0.8/setup.cfg
+drwxrwxr-x   0 agus      (1000) agus      (1000)        0 2024-04-12 15:40:18.976669 SMjournal-0.0.9/
+-rw-rw-r--   0 agus      (1000) agus      (1000)     1077 2024-04-11 13:57:24.000000 SMjournal-0.0.9/LICENSE
+-rw-r--r--   0 agus      (1000) agus      (1000)      679 2024-04-12 15:40:18.976669 SMjournal-0.0.9/PKG-INFO
+-rw-rw-r--   0 agus      (1000) agus      (1000)        0 2024-04-11 13:57:24.000000 SMjournal-0.0.9/README.md
+drwxrwxr-x   0 agus      (1000) agus      (1000)        0 2024-04-12 15:40:18.976669 SMjournal-0.0.9/SMjournal/
+-rw-rw-r--   0 agus      (1000) agus      (1000)      124 2024-04-11 13:57:24.000000 SMjournal-0.0.9/SMjournal/__init__.py
+-rw-rw-r--   0 agus      (1000) agus      (1000)     4995 2024-04-12 15:39:38.000000 SMjournal-0.0.9/SMjournal/collinearity.py
+-rw-rw-r--   0 agus      (1000) agus      (1000)     4690 2024-04-11 13:57:24.000000 SMjournal-0.0.9/SMjournal/data.py
+-rw-rw-r--   0 agus      (1000) agus      (1000)     1512 2024-04-11 13:57:24.000000 SMjournal-0.0.9/SMjournal/low_level.py
+-rw-rw-r--   0 agus      (1000) agus      (1000)     4434 2024-04-11 13:57:24.000000 SMjournal-0.0.9/SMjournal/meta_reg.py
+-rw-rw-r--   0 agus      (1000) agus      (1000)     2928 2024-04-11 13:57:24.000000 SMjournal-0.0.9/SMjournal/potentiality.py
+drwxrwxr-x   0 agus      (1000) agus      (1000)        0 2024-04-12 15:40:18.976669 SMjournal-0.0.9/SMjournal.egg-info/
+-rw-r--r--   0 agus      (1000) agus      (1000)      679 2024-04-12 15:40:18.000000 SMjournal-0.0.9/SMjournal.egg-info/PKG-INFO
+-rw-rw-r--   0 agus      (1000) agus      (1000)      343 2024-04-12 15:40:18.000000 SMjournal-0.0.9/SMjournal.egg-info/SOURCES.txt
+-rw-rw-r--   0 agus      (1000) agus      (1000)        1 2024-04-12 15:40:18.000000 SMjournal-0.0.9/SMjournal.egg-info/dependency_links.txt
+-rw-rw-r--   0 agus      (1000) agus      (1000)       88 2024-04-12 15:40:18.000000 SMjournal-0.0.9/SMjournal.egg-info/requires.txt
+-rw-rw-r--   0 agus      (1000) agus      (1000)       10 2024-04-12 15:40:18.000000 SMjournal-0.0.9/SMjournal.egg-info/top_level.txt
+-rw-rw-r--   0 agus      (1000) agus      (1000)      106 2024-04-11 13:57:24.000000 SMjournal-0.0.9/pyproject.toml
+-rw-rw-r--   0 agus      (1000) agus      (1000)      633 2024-04-12 15:40:18.980669 SMjournal-0.0.9/setup.cfg
```

### Comparing `SMjournal-0.0.8/LICENSE` & `SMjournal-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.8/PKG-INFO` & `SMjournal-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMjournal
-Version: 0.0.8
+Version: 0.0.9
 Summary: Investigation Journal
 Home-page: https://github.com/AgustinBustos/SMjournal
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SMjournal-0.0.8/SMjournal/collinearity.py` & `SMjournal-0.0.9/SMjournal/collinearity.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,16 +114,18 @@
 
   plt.figure(figsize=(10,7))
 
   # Generate a mask to onlyshow the bottom triangle
   mask = np.triu(np.ones_like(finalCorr, dtype=bool))
 
   # generate heatmap
-  corrplot=sns.heatmap(finalCorr, annot=True, mask=mask, vmin=-1, vmax=1,cmap="rocket_r").set(title='Correlation Coefficient Of Predictors').get_figure()
+  corrplot=sns.heatmap(finalCorr, annot=True, mask=mask, vmin=-1, vmax=1,cmap="rocket_r")
+  corrplot=corrplot.get_figure()
   # corrplot.title('Correlation Coefficient Of Predictors')
+  # .set(title='Correlation Coefficient Of Predictors')
   corrplot.show()
 
 
   
   data=df[to_test]
 
   #block distance
```

### Comparing `SMjournal-0.0.8/SMjournal/data.py` & `SMjournal-0.0.9/SMjournal/data.py`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.8/SMjournal/low_level.py` & `SMjournal-0.0.9/SMjournal/low_level.py`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.8/SMjournal/meta_reg.py` & `SMjournal-0.0.9/SMjournal/meta_reg.py`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.8/SMjournal/potentiality.py` & `SMjournal-0.0.9/SMjournal/potentiality.py`

 * *Files identical despite different names*

### Comparing `SMjournal-0.0.8/SMjournal.egg-info/PKG-INFO` & `SMjournal-0.0.9/SMjournal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMjournal
-Version: 0.0.8
+Version: 0.0.9
 Summary: Investigation Journal
 Home-page: https://github.com/AgustinBustos/SMjournal
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SMjournal-0.0.8/setup.cfg` & `SMjournal-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = SMjournal
-version = 0.0.8
+version = 0.0.9
 author = Agustin Bustos Barton
 author_email = agustinbustosbarton@gmail.com
 description = Investigation Journal
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/AgustinBustos/SMjournal
 classifiers =
```

