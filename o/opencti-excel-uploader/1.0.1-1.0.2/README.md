# Comparing `tmp/opencti_excel_uploader-1.0.1.tar.gz` & `tmp/opencti_excel_uploader-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencti_excel_uploader-1.0.1.tar", last modified: Tue Apr 30 10:51:42 2024, max compression
+gzip compressed data, was "opencti_excel_uploader-1.0.2.tar", last modified: Tue Apr 30 11:17:25 2024, max compression
```

## Comparing `opencti_excel_uploader-1.0.1.tar` & `opencti_excel_uploader-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 10:51:42.945891 opencti_excel_uploader-1.0.1/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 10:51:42.945891 opencti_excel_uploader-1.0.1/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      501 2024-04-30 10:50:47.000000 opencti_excel_uploader-1.0.1/README.md
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 10:51:42.941891 opencti_excel_uploader-1.0.1/opencti_excel_uploader/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.1/opencti_excel_uploader/__init__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     2427 2024-04-30 08:23:26.000000 opencti_excel_uploader-1.0.1/opencti_excel_uploader/__main__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.1/opencti_excel_uploader/models.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    13835 2024-04-30 10:47:02.000000 opencti_excel_uploader-1.0.1/opencti_excel_uploader/xlsx_utils.py
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 10:51:42.941891 opencti_excel_uploader-1.0.1/opencti_excel_uploader.egg-info/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 10:51:42.000000 opencti_excel_uploader-1.0.1/opencti_excel_uploader.egg-info/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-30 10:51:42.000000 opencti_excel_uploader-1.0.1/opencti_excel_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-30 10:51:42.000000 opencti_excel_uploader-1.0.1/opencti_excel_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-30 10:51:42.000000 opencti_excel_uploader-1.0.1/opencti_excel_uploader.egg-info/entry_points.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-30 10:51:42.000000 opencti_excel_uploader-1.0.1/opencti_excel_uploader.egg-info/requires.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-30 10:51:42.000000 opencti_excel_uploader-1.0.1/opencti_excel_uploader.egg-info/top_level.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-30 10:51:42.945891 opencti_excel_uploader-1.0.1/setup.cfg
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      896 2024-04-30 10:49:38.000000 opencti_excel_uploader-1.0.1/setup.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 11:17:25.153211 opencti_excel_uploader-1.0.2/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 11:17:25.153211 opencti_excel_uploader-1.0.2/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      501 2024-04-30 10:50:47.000000 opencti_excel_uploader-1.0.2/README.md
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 11:17:25.149211 opencti_excel_uploader-1.0.2/opencti_excel_uploader/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader/__init__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     2388 2024-04-30 11:16:34.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader/__main__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader/models.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    13835 2024-04-30 10:47:02.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader/xlsx_utils.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 11:17:25.153211 opencti_excel_uploader-1.0.2/opencti_excel_uploader.egg-info/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 11:17:25.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-30 11:17:25.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-30 11:17:25.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-30 11:17:25.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader.egg-info/entry_points.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-30 11:17:25.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader.egg-info/requires.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-30 11:17:25.000000 opencti_excel_uploader-1.0.2/opencti_excel_uploader.egg-info/top_level.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-30 11:17:25.153211 opencti_excel_uploader-1.0.2/setup.cfg
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      896 2024-04-30 11:17:22.000000 opencti_excel_uploader-1.0.2/setup.py
```

### Comparing `opencti_excel_uploader-1.0.1/PKG-INFO` & `opencti_excel_uploader-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 1.0.1
+Version: 1.0.2
 Summary: Creates workbench files from excel files for Opencti
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-1.0.1/opencti_excel_uploader/__main__.py` & `opencti_excel_uploader-1.0.2/opencti_excel_uploader/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,37 +40,34 @@
         author_secondname = input("Enter AUTHOR_LASTNAME: ")
         author_email = input("Enter AUTHOR_EMAIL: ")
         marking_definition = input("Enter MARKING_DEFINITION: ")
         # Write the new environment variables to .env file
         with open(".env", "w") as f:
             f.write(f"OPENCTI_URL={url}\n")
             f.write(f"OPENCTI_TOKEN={token}\n")
+            f.write(f"AUTHOR_FIRSTNAME={author_firstname}\n")
+            f.write(f"AUTHOR_LASTNAME={author_secondname}\n")
+            f.write(f"AUTHOR_EMAIL={author_email}\n")
+            f.write(f"MARKING_DEFINITION={marking_definition}\n")
 
         print("Configuration saved. Please ensure to keep your .env file secure!")
-
-        # Set environment variables for current session
-        os.environ["OPENCTI_URL"] = url
-        os.environ["OPENCTI_TOKEN"] = token
-
         process_folder()
 
 
 def process_folder():
     try:
 
         print("Starting to convert.", flush=True)
-        # Assuming 'folder_to_json' needs these credentials, pass them as needed
         folder_path = sys.argv[1] if len(sys.argv) > 1 else "."
         if folder_path:
             print(f"Folder path: {folder_path}", flush=True)
         else:
             print("No folder path provided. Using current directory.", flush=True)
             folder_path = "."
         folder_to_json(folder_path)
-        # Modify this line as per actual function signature
     except Exception as e:
         print(f"Error: {e}", flush=True)
 
 
 if __name__ == "__main__":
     print("Starting...", flush=True)
     setup_opencti_config()
```

### Comparing `opencti_excel_uploader-1.0.1/opencti_excel_uploader/models.py` & `opencti_excel_uploader-1.0.2/opencti_excel_uploader/models.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-1.0.1/opencti_excel_uploader/xlsx_utils.py` & `opencti_excel_uploader-1.0.2/opencti_excel_uploader/xlsx_utils.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-1.0.1/opencti_excel_uploader.egg-info/PKG-INFO` & `opencti_excel_uploader-1.0.2/opencti_excel_uploader.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 1.0.1
+Version: 1.0.2
 Summary: Creates workbench files from excel files for Opencti
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-1.0.1/setup.py` & `opencti_excel_uploader-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="opencti-excel-uploader",
-    version="1.0.1",
+    version="1.0.2",
     packages=find_packages(),
     description="Creates workbench files from excel files for Opencti",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="asz,jjk,eby",
     author_email="rnd@stratc.org",
     license="MIT",
```

