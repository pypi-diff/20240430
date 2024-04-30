# Comparing `tmp/opencti_excel_uploader-1.0.2.tar.gz` & `tmp/opencti_excel_uploader-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencti_excel_uploader-1.0.2.tar", last modified: Tue Apr 30 11:17:25 2024, max compression
+gzip compressed data, was "opencti_excel_uploader-1.0.3.tar", last modified: Tue Apr 30 12:12:19 2024, max compression
```

## Comparing `opencti_excel_uploader-1.0.2.tar` & `opencti_excel_uploader-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 11:17:25.153211 opencti_excel_uploader-1.0.2/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 11:17:25.153211 opencti_excel_uploader-1.0.2/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      501 2024-04-30 10:50:47.000000 opencti_excel_uploader-1.0.2/README.md
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 11:17:25.149211 opencti_excel_uploader-1.0.2/opencti_excel_uploader/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader/__init__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     2388 2024-04-30 11:16:34.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader/__main__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader/models.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    13835 2024-04-30 10:47:02.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader/xlsx_utils.py
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 11:17:25.153211 opencti_excel_uploader-1.0.2/opencti_excel_uploader.egg-info/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 11:17:25.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader.egg-info/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-30 11:17:25.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-30 11:17:25.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-30 11:17:25.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader.egg-info/entry_points.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-30 11:17:25.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader.egg-info/requires.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-30 11:17:25.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader.egg-info/top_level.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-30 11:17:25.153211 opencti_excel_uploader-1.0.2/setup.cfg
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      896 2024-04-30 11:17:22.000000 opencti_excel_uploader-1.0.2/setup.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 12:12:19.955333 opencti_excel_uploader-1.0.3/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 12:12:19.951333 opencti_excel_uploader-1.0.3/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      501 2024-04-30 10:50:47.000000 opencti_excel_uploader-1.0.3/README.md
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 12:12:19.951333 opencti_excel_uploader-1.0.3/opencti_excel_uploader/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader/__init__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     2892 2024-04-30 12:12:04.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader/__main__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader/models.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    13835 2024-04-30 10:47:02.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader/xlsx_utils.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 12:12:19.951333 opencti_excel_uploader-1.0.3/opencti_excel_uploader.egg-info/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 12:12:19.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-30 12:12:19.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-30 12:12:19.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-30 12:12:19.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader.egg-info/entry_points.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-30 12:12:19.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader.egg-info/requires.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-30 12:12:19.000000 opencti_excel_uploader-1.0.3/opencti_excel_uploader.egg-info/top_level.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-30 12:12:19.955333 opencti_excel_uploader-1.0.3/setup.cfg
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      896 2024-04-30 12:12:16.000000 opencti_excel_uploader-1.0.3/setup.py
```

### Comparing `opencti_excel_uploader-1.0.2/PKG-INFO` & `opencti_excel_uploader-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 1.0.2
+Version: 1.0.3
 Summary: Creates workbench files from excel files for Opencti
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-1.0.2/opencti_excel_uploader/__main__.py` & `opencti_excel_uploader-1.0.3/opencti_excel_uploader/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,21 +3,32 @@
 
 load_dotenv()  # Load the environment variables from .env file
 
 from .xlsx_utils import folder_to_json
 import sys
 
 
+if load_dotenv():  # Load the environment variables from .env file
+    print("Loaded environment variables from .env file.")
+    print(
+        f"OPENCTI_URL: {os.getenv('OPENCTI_URL')}, \n OPENCTI_TOKEN: {os.getenv('OPENCTI_TOKEN')}, \n AUTHOR_FIRSTNAME: {os.getenv('AUTHOR_FIRSTNAME')},\n AUTHOR_LASTNAME: {os.getenv('AUTHOR_LASTNAME')}, \n AUTHOR_EMAIL: {os.getenv('AUTHOR_EMAIL')},\n MARKING_DEFINITION: {os.getenv('MARKING_DEFINITION')}"
+    )
+
+
+else:
+    print("Failed to load .env file.")
+
+
 def main():
     setup_opencti_config()
 
 
 def setup_opencti_config():
     # Load existing environment variables from .env if it exists
-    load_dotenv(".env")
+    load_dotenv(verbose=True)
 
     # Check if environment variables are set
     url = os.getenv("OPENCTI_URL")
     token = os.getenv("OPENCTI_TOKEN")
     author_firstname = os.getenv("AUTHOR_FIRSTNAME")
     author_secondname = os.getenv("AUTHOR_LASTNAME")
     author_email = os.getenv("AUTHOR_EMAIL")
```

### Comparing `opencti_excel_uploader-1.0.2/opencti_excel_uploader/models.py` & `opencti_excel_uploader-1.0.3/opencti_excel_uploader/models.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-1.0.2/opencti_excel_uploader/xlsx_utils.py` & `opencti_excel_uploader-1.0.3/opencti_excel_uploader/xlsx_utils.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-1.0.2/opencti_excel_uploader.egg-info/PKG-INFO` & `opencti_excel_uploader-1.0.3/opencti_excel_uploader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 1.0.2
+Version: 1.0.3
 Summary: Creates workbench files from excel files for Opencti
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-1.0.2/setup.py` & `opencti_excel_uploader-1.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="opencti-excel-uploader",
-    version="1.0.2",
+    version="1.0.3",
     packages=find_packages(),
     description="Creates workbench files from excel files for Opencti",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="asz,jjk,eby",
     author_email="rnd@stratc.org",
     license="MIT",
```

