# Comparing `tmp/opencti_excel_uploader-1.0.3.tar.gz` & `tmp/opencti_excel_uploader-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencti_excel_uploader-1.0.3.tar", last modified: Tue Apr 30 12:12:19 2024, max compression
+gzip compressed data, was "opencti_excel_uploader-1.0.4.tar", last modified: Tue Apr 30 12:27:42 2024, max compression
```

## Comparing `opencti_excel_uploader-1.0.3.tar` & `opencti_excel_uploader-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 12:12:19.955333 opencti_excel_uploader-1.0.3/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 12:12:19.951333 opencti_excel_uploader-1.0.3/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      501 2024-04-30 10:50:47.000000 opencti_excel_uploader-1.0.3/README.md
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 12:12:19.951333 opencti_excel_uploader-1.0.3/opencti_excel_uploader/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader/__init__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     2892 2024-04-30 12:12:04.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader/__main__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader/models.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    13835 2024-04-30 10:47:02.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader/xlsx_utils.py
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 12:12:19.951333 opencti_excel_uploader-1.0.3/opencti_excel_uploader.egg-info/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 12:12:19.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader.egg-info/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-30 12:12:19.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-30 12:12:19.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-30 12:12:19.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader.egg-info/entry_points.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-30 12:12:19.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader.egg-info/requires.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-30 12:12:19.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader.egg-info/top_level.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-30 12:12:19.955333 opencti_excel_uploader-1.0.3/setup.cfg
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      896 2024-04-30 12:12:16.000000 opencti_excel_uploader-1.0.3/setup.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 12:27:42.296622 opencti_excel_uploader-1.0.4/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 12:27:42.296622 opencti_excel_uploader-1.0.4/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      501 2024-04-30 10:50:47.000000 opencti_excel_uploader-1.0.4/README.md
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 12:27:42.296622 opencti_excel_uploader-1.0.4/opencti_excel_uploader/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader/__init__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     2828 2024-04-30 12:27:17.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader/__main__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader/models.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    13835 2024-04-30 10:47:02.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader/xlsx_utils.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 12:27:42.296622 opencti_excel_uploader-1.0.4/opencti_excel_uploader.egg-info/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 12:27:42.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-30 12:27:42.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-30 12:27:42.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-30 12:27:42.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader.egg-info/entry_points.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-30 12:27:42.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader.egg-info/requires.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-30 12:27:42.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader.egg-info/top_level.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-30 12:27:42.296622 opencti_excel_uploader-1.0.4/setup.cfg
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      896 2024-04-30 12:27:39.000000 opencti_excel_uploader-1.0.4/setup.py
```

### Comparing `opencti_excel_uploader-1.0.3/PKG-INFO` & `opencti_excel_uploader-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 1.0.3
+Version: 1.0.4
 Summary: Creates workbench files from excel files for Opencti
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-1.0.3/opencti_excel_uploader/__main__.py` & `opencti_excel_uploader-1.0.4/opencti_excel_uploader/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import os
 from dotenv import load_dotenv
 
-load_dotenv()  # Load the environment variables from .env file
-
 from .xlsx_utils import folder_to_json
 import sys
 
 
-if load_dotenv():  # Load the environment variables from .env file
+if load_dotenv(".env"):  # Load the environment variables from .env file
     print("Loaded environment variables from .env file.")
     print(
         f"OPENCTI_URL: {os.getenv('OPENCTI_URL')}, \n OPENCTI_TOKEN: {os.getenv('OPENCTI_TOKEN')}, \n AUTHOR_FIRSTNAME: {os.getenv('AUTHOR_FIRSTNAME')},\n AUTHOR_LASTNAME: {os.getenv('AUTHOR_LASTNAME')}, \n AUTHOR_EMAIL: {os.getenv('AUTHOR_EMAIL')},\n MARKING_DEFINITION: {os.getenv('MARKING_DEFINITION')}"
     )
 
 
 else:
@@ -47,15 +45,15 @@
         print("Setup for OPENCTI API Access")
         url = input("Enter OPENCTI_URL: ")
         token = input("Enter OPENCTI_TOKEN: ")
         author_firstname = input("Enter AUTHOR FIRSTNAME: ")
         author_secondname = input("Enter AUTHOR_LASTNAME: ")
         author_email = input("Enter AUTHOR_EMAIL: ")
         marking_definition = input("Enter MARKING_DEFINITION: ")
-        # Write the new environment variables to .env file
+        print("Saving configuration to.env file...")
         with open(".env", "w") as f:
             f.write(f"OPENCTI_URL={url}\n")
             f.write(f"OPENCTI_TOKEN={token}\n")
             f.write(f"AUTHOR_FIRSTNAME={author_firstname}\n")
             f.write(f"AUTHOR_LASTNAME={author_secondname}\n")
             f.write(f"AUTHOR_EMAIL={author_email}\n")
             f.write(f"MARKING_DEFINITION={marking_definition}\n")
```

### Comparing `opencti_excel_uploader-1.0.3/opencti_excel_uploader/models.py` & `opencti_excel_uploader-1.0.4/opencti_excel_uploader/models.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-1.0.3/opencti_excel_uploader/xlsx_utils.py` & `opencti_excel_uploader-1.0.4/opencti_excel_uploader/xlsx_utils.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-1.0.3/opencti_excel_uploader.egg-info/PKG-INFO` & `opencti_excel_uploader-1.0.4/opencti_excel_uploader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 1.0.3
+Version: 1.0.4
 Summary: Creates workbench files from excel files for Opencti
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-1.0.3/setup.py` & `opencti_excel_uploader-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="opencti-excel-uploader",
-    version="1.0.3",
+    version="1.0.4",
     packages=find_packages(),
     description="Creates workbench files from excel files for Opencti",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="asz,jjk,eby",
     author_email="rnd@stratc.org",
     license="MIT",
```

