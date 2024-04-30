# Comparing `tmp/EcoStock-0.5.tar.gz` & `tmp/EcoStock-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EcoStock-0.5.tar", last modified: Tue Apr 30 18:15:25 2024, max compression
+gzip compressed data, was "EcoStock-0.5.1.tar", last modified: Tue Apr 30 19:09:42 2024, max compression
```

## Comparing `EcoStock-0.5.tar` & `EcoStock-0.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 18:15:25.885397 EcoStock-0.5/
-drwxrwxrwx   0        0        0        0 2024-04-30 18:15:25.880181 EcoStock-0.5/EcoStock/
--rw-rw-rw-   0        0        0     1322 2024-04-30 18:14:54.000000 EcoStock-0.5/EcoStock/__init__.py
--rw-rw-rw-   0        0        0    38261 2024-04-30 18:09:11.000000 EcoStock-0.5/EcoStock/adalo.py
--rw-rw-rw-   0        0        0    10398 2024-04-30 18:09:58.000000 EcoStock-0.5/EcoStock/api.py
--rw-rw-rw-   0        0        0    19977 2024-04-30 16:55:46.000000 EcoStock-0.5/EcoStock/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-30 18:15:25.884461 EcoStock-0.5/EcoStock.egg-info/
--rw-rw-rw-   0        0        0     1733 2024-04-30 18:15:25.000000 EcoStock-0.5/EcoStock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-04-30 18:15:25.000000 EcoStock-0.5/EcoStock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 18:15:25.000000 EcoStock-0.5/EcoStock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2024-04-30 18:15:25.000000 EcoStock-0.5/EcoStock.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-30 18:15:25.000000 EcoStock-0.5/EcoStock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2024-04-29 07:13:36.000000 EcoStock-0.5/LICENSE.md
--rw-rw-rw-   0        0        0     1733 2024-04-30 18:15:25.885397 EcoStock-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1121 2024-04-29 08:30:40.000000 EcoStock-0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-30 18:15:25.886395 EcoStock-0.5/setup.cfg
--rw-rw-rw-   0        0        0     1073 2024-04-30 18:14:36.000000 EcoStock-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 19:09:42.840807 EcoStock-0.5.1/
+drwxrwxrwx   0        0        0        0 2024-04-30 19:09:42.830755 EcoStock-0.5.1/EcoStock/
+-rw-rw-rw-   0        0        0     1110 2024-04-30 19:08:17.000000 EcoStock-0.5.1/EcoStock/__init__.py
+-rw-rw-rw-   0        0        0    18025 2024-04-30 19:03:32.000000 EcoStock-0.5.1/EcoStock/adalo.py
+-rw-rw-rw-   0        0        0     5957 2024-04-30 19:06:14.000000 EcoStock-0.5.1/EcoStock/api.py
+-rw-rw-rw-   0        0        0    19977 2024-04-30 19:06:20.000000 EcoStock-0.5.1/EcoStock/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-30 19:09:42.839807 EcoStock-0.5.1/EcoStock.egg-info/
+-rw-rw-rw-   0        0        0     1735 2024-04-30 19:09:42.000000 EcoStock-0.5.1/EcoStock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-04-30 19:09:42.000000 EcoStock-0.5.1/EcoStock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 19:09:42.000000 EcoStock-0.5.1/EcoStock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-04-30 19:09:42.000000 EcoStock-0.5.1/EcoStock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-30 19:09:42.000000 EcoStock-0.5.1/EcoStock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2024-04-29 07:13:36.000000 EcoStock-0.5.1/LICENSE.md
+-rw-rw-rw-   0        0        0     1735 2024-04-30 19:09:42.840807 EcoStock-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1121 2024-04-29 08:30:40.000000 EcoStock-0.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-30 19:09:42.840807 EcoStock-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1056 2024-04-30 19:06:58.000000 EcoStock-0.5.1/setup.py
```

### Comparing `EcoStock-0.5/EcoStock/functions.py` & `EcoStock-0.5.1/EcoStock/functions.py`

 * *Files identical despite different names*

### Comparing `EcoStock-0.5/EcoStock.egg-info/PKG-INFO` & `EcoStock-0.5.1/EcoStock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 0.5
+Version: 0.5.1
 Summary: A Python package for investigating the correlation between economic and financial data.
 Home-page: https://github.com/Tonij10/fastapi-project
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo and Francesco Caldo
 Author-email: antoniopaparo@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EcoStock-0.5/LICENSE.md` & `EcoStock-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `EcoStock-0.5/PKG-INFO` & `EcoStock-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 0.5
+Version: 0.5.1
 Summary: A Python package for investigating the correlation between economic and financial data.
 Home-page: https://github.com/Tonij10/fastapi-project
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo and Francesco Caldo
 Author-email: antoniopaparo@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EcoStock-0.5/README.md` & `EcoStock-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `EcoStock-0.5/setup.py` & `EcoStock-0.5.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='EcoStock',
-    version='0.5',
+    version='0.5.1',
     author="Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo and Francesco Caldo",
     author_email="antoniopaparo@outlook.com",
     description='A Python package for investigating the correlation between economic and financial data.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tonij10/fastapi-project",
     packages=find_packages(),
@@ -21,16 +21,14 @@
         'numpy',
         'matplotlib',
         'yfinance',
         'plotly',
         'requests',
         'seaborn',
         'statsmodels',
-        'uuid',
-
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
```

