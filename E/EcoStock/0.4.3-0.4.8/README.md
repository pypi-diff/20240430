# Comparing `tmp/EcoStock-0.4.3.tar.gz` & `tmp/EcoStock-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EcoStock-0.4.3.tar", last modified: Sun Apr 28 15:10:28 2024, max compression
+gzip compressed data, was "EcoStock-0.4.8.tar", last modified: Tue Apr 30 16:07:44 2024, max compression
```

## Comparing `EcoStock-0.4.3.tar` & `EcoStock-0.4.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 15:10:28.859292 EcoStock-0.4.3/
-drwxrwxrwx   0        0        0        0 2024-04-28 15:10:28.849450 EcoStock-0.4.3/EcoStock/
--rw-rw-rw-   0        0        0     1021 2024-04-28 15:09:41.000000 EcoStock-0.4.3/EcoStock/__init__.py
--rw-rw-rw-   0        0        0    12984 2024-04-28 15:02:13.000000 EcoStock-0.4.3/EcoStock/adalo.py
--rw-rw-rw-   0        0        0     5310 2024-04-28 15:01:55.000000 EcoStock-0.4.3/EcoStock/api.py
--rw-rw-rw-   0        0        0    12990 2024-04-28 15:02:03.000000 EcoStock-0.4.3/EcoStock/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:10:28.857293 EcoStock-0.4.3/EcoStock.egg-info/
--rw-rw-rw-   0        0        0     1739 2024-04-28 15:10:28.000000 EcoStock-0.4.3/EcoStock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-04-28 15:10:28.000000 EcoStock-0.4.3/EcoStock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 15:10:28.000000 EcoStock-0.4.3/EcoStock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2024-04-28 15:10:28.000000 EcoStock-0.4.3/EcoStock.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-28 15:10:28.000000 EcoStock-0.4.3/EcoStock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2024-04-28 11:55:32.000000 EcoStock-0.4.3/LICENSE.md
--rw-rw-rw-   0        0        0     1739 2024-04-28 15:10:28.858296 EcoStock-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     1125 2024-04-28 11:55:28.000000 EcoStock-0.4.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-28 15:10:28.859292 EcoStock-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1032 2024-04-28 15:09:43.000000 EcoStock-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:07:44.126445 EcoStock-0.4.8/
+drwxrwxrwx   0        0        0        0 2024-04-30 16:07:44.118558 EcoStock-0.4.8/EcoStock/
+-rw-rw-rw-   0        0        0     1324 2024-04-30 16:07:02.000000 EcoStock-0.4.8/EcoStock/__init__.py
+-rw-rw-rw-   0        0        0    37245 2024-04-30 15:46:50.000000 EcoStock-0.4.8/EcoStock/adalo.py
+-rw-rw-rw-   0        0        0    10701 2024-04-30 15:37:58.000000 EcoStock-0.4.8/EcoStock/api.py
+-rw-rw-rw-   0        0        0    19977 2024-04-30 15:43:00.000000 EcoStock-0.4.8/EcoStock/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-30 16:07:44.124989 EcoStock-0.4.8/EcoStock.egg-info/
+-rw-rw-rw-   0        0        0     1735 2024-04-30 16:07:44.000000 EcoStock-0.4.8/EcoStock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-04-30 16:07:44.000000 EcoStock-0.4.8/EcoStock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 16:07:44.000000 EcoStock-0.4.8/EcoStock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2024-04-30 16:07:44.000000 EcoStock-0.4.8/EcoStock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-30 16:07:44.000000 EcoStock-0.4.8/EcoStock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2024-04-29 07:13:36.000000 EcoStock-0.4.8/LICENSE.md
+-rw-rw-rw-   0        0        0     1735 2024-04-30 16:07:44.125404 EcoStock-0.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1121 2024-04-29 08:30:40.000000 EcoStock-0.4.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-30 16:07:44.126445 EcoStock-0.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2024-04-30 16:06:41.000000 EcoStock-0.4.8/setup.py
```

### Comparing `EcoStock-0.4.3/EcoStock.egg-info/PKG-INFO` & `EcoStock-0.4.8/EcoStock.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 0.4.3
+Version: 0.4.8
 Summary: A Python package for investigating the correlation between economic and financial data.
 Home-page: https://github.com/Tonij10/fastapi-project
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo and Francesco Caldo
 Author-email: antoniopaparo@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# Package Name
+# EcoStock
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 This Python package contains functions for investigating the correlation between economic and financial data.
 
 ## Installation
```

### Comparing `EcoStock-0.4.3/LICENSE.md` & `EcoStock-0.4.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `EcoStock-0.4.3/PKG-INFO` & `EcoStock-0.4.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 0.4.3
+Version: 0.4.8
 Summary: A Python package for investigating the correlation between economic and financial data.
 Home-page: https://github.com/Tonij10/fastapi-project
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo and Francesco Caldo
 Author-email: antoniopaparo@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# Package Name
+# EcoStock
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 This Python package contains functions for investigating the correlation between economic and financial data.
 
 ## Installation
```

### Comparing `EcoStock-0.4.3/README.md` & `EcoStock-0.4.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Package Name
+# EcoStock
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 This Python package contains functions for investigating the correlation between economic and financial data.
 
 ## Installation
```

### Comparing `EcoStock-0.4.3/setup.py` & `EcoStock-0.4.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='EcoStock',
-    version='0.4.3',
+    version='0.4.8',
     author="Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo and Francesco Caldo",
     author_email="antoniopaparo@outlook.com",
     description='A Python package for investigating the correlation between economic and financial data.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tonij10/fastapi-project",
     packages=find_packages(),
@@ -20,14 +20,17 @@
         'pandas',
         'numpy',
         'matplotlib',
         'yfinance',
         'plotly',
         'requests',
         'seaborn',
+        'statsmodels',
+        'uuid',
+
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
```

