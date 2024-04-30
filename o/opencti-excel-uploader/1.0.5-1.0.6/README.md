# Comparing `tmp/opencti_excel_uploader-1.0.5.tar.gz` & `tmp/opencti_excel_uploader-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencti_excel_uploader-1.0.5.tar", last modified: Tue Apr 30 13:18:20 2024, max compression
+gzip compressed data, was "opencti_excel_uploader-1.0.6.tar", last modified: Tue Apr 30 13:24:58 2024, max compression
```

## Comparing `opencti_excel_uploader-1.0.5.tar` & `opencti_excel_uploader-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 13:18:20.467459 opencti_excel_uploader-1.0.5/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 13:18:20.463459 opencti_excel_uploader-1.0.5/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      501 2024-04-30 10:50:47.000000 opencti_excel_uploader-1.0.5/README.md
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 13:18:20.463459 opencti_excel_uploader-1.0.5/opencti_excel_uploader/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader/__init__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     2826 2024-04-30 13:18:00.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader/__main__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader/models.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    13927 2024-04-30 13:17:51.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader/xlsx_utils.py
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 13:18:20.463459 opencti_excel_uploader-1.0.5/opencti_excel_uploader.egg-info/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 13:18:20.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader.egg-info/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-30 13:18:20.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-30 13:18:20.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-30 13:18:20.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader.egg-info/entry_points.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-30 13:18:20.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader.egg-info/requires.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-30 13:18:20.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader.egg-info/top_level.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-30 13:18:20.467459 opencti_excel_uploader-1.0.5/setup.cfg
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      896 2024-04-30 13:18:17.000000 opencti_excel_uploader-1.0.5/setup.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 13:24:58.542184 opencti_excel_uploader-1.0.6/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 13:24:58.542184 opencti_excel_uploader-1.0.6/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      501 2024-04-30 10:50:47.000000 opencti_excel_uploader-1.0.6/README.md
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 13:24:58.538184 opencti_excel_uploader-1.0.6/opencti_excel_uploader/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.6/opencti_excel_uploader/__init__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     2826 2024-04-30 13:18:00.000000 opencti_excel_uploader-1.0.6/opencti_excel_uploader/__main__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.6/opencti_excel_uploader/models.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    14112 2024-04-30 13:24:45.000000 opencti_excel_uploader-1.0.6/opencti_excel_uploader/xlsx_utils.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 13:24:58.542184 opencti_excel_uploader-1.0.6/opencti_excel_uploader.egg-info/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 13:24:58.000000 opencti_excel_uploader-1.0.6/opencti_excel_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-30 13:24:58.000000 opencti_excel_uploader-1.0.6/opencti_excel_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-30 13:24:58.000000 opencti_excel_uploader-1.0.6/opencti_excel_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-30 13:24:58.000000 opencti_excel_uploader-1.0.6/opencti_excel_uploader.egg-info/entry_points.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-30 13:24:58.000000 opencti_excel_uploader-1.0.6/opencti_excel_uploader.egg-info/requires.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-30 13:24:58.000000 opencti_excel_uploader-1.0.6/opencti_excel_uploader.egg-info/top_level.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-30 13:24:58.542184 opencti_excel_uploader-1.0.6/setup.cfg
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      896 2024-04-30 13:24:55.000000 opencti_excel_uploader-1.0.6/setup.py
```

### Comparing `opencti_excel_uploader-1.0.5/PKG-INFO` & `opencti_excel_uploader-1.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 1.0.5
+Version: 1.0.6
 Summary: Creates workbench files from excel files for Opencti
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-1.0.5/opencti_excel_uploader/__main__.py` & `opencti_excel_uploader-1.0.6/opencti_excel_uploader/__main__.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-1.0.5/opencti_excel_uploader/models.py` & `opencti_excel_uploader-1.0.6/opencti_excel_uploader/models.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-1.0.5/opencti_excel_uploader/xlsx_utils.py` & `opencti_excel_uploader-1.0.6/opencti_excel_uploader/xlsx_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,21 @@
 import openpyxl
 from dotenv import load_dotenv
 
 
 load_dotenv()
 
 author_firstname = os.getenv("AUTHOR_FIRSTNAME")
+print(f"author_firstname: {author_firstname}")
 author_secondname = os.getenv("AUTHOR_LASTNAME")
+print(f"author_secondname: {author_secondname}")
 author_email = os.getenv("AUTHOR_EMAIL")
+print(f"author_email: {author_email}")
 marking_definition = os.getenv("MARKING_DEFINITION")
-
+print(f"marking_definition: {marking_definition}")
 
 now = datetime.datetime.now()
 published = now.isoformat() + "Z"
 
 
 def drop_duplicates(list_of_dicts):
     """Drops duplicates from a list of dictionaries"""
```

### Comparing `opencti_excel_uploader-1.0.5/opencti_excel_uploader.egg-info/PKG-INFO` & `opencti_excel_uploader-1.0.6/opencti_excel_uploader.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 1.0.5
+Version: 1.0.6
 Summary: Creates workbench files from excel files for Opencti
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-1.0.5/setup.py` & `opencti_excel_uploader-1.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="opencti-excel-uploader",
-    version="1.0.5",
+    version="1.0.6",
     packages=find_packages(),
     description="Creates workbench files from excel files for Opencti",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="asz,jjk,eby",
     author_email="rnd@stratc.org",
     license="MIT",
```

