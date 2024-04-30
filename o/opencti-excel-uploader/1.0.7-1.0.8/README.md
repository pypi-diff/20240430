# Comparing `tmp/opencti_excel_uploader-1.0.7.tar.gz` & `tmp/opencti_excel_uploader-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencti_excel_uploader-1.0.7.tar", last modified: Tue Apr 30 13:34:08 2024, max compression
+gzip compressed data, was "opencti_excel_uploader-1.0.8.tar", last modified: Tue Apr 30 13:40:35 2024, max compression
```

## Comparing `opencti_excel_uploader-1.0.7.tar` & `opencti_excel_uploader-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 13:34:08.380507 opencti_excel_uploader-1.0.7/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 13:34:08.376507 opencti_excel_uploader-1.0.7/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      501 2024-04-30 10:50:47.000000 opencti_excel_uploader-1.0.7/README.md
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 13:34:08.364507 opencti_excel_uploader-1.0.7/opencti_excel_uploader/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.7/opencti_excel_uploader/__init__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     3232 2024-04-30 13:33:41.000000 opencti_excel_uploader-1.0.7/opencti_excel_uploader/__main__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.7/opencti_excel_uploader/models.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    13846 2024-04-30 13:33:33.000000 opencti_excel_uploader-1.0.7/opencti_excel_uploader/xlsx_utils.py
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 13:34:08.372507 opencti_excel_uploader-1.0.7/opencti_excel_uploader.egg-info/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 13:34:08.000000 opencti_excel_uploader-1.0.7/opencti_excel_uploader.egg-info/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-30 13:34:08.000000 opencti_excel_uploader-1.0.7/opencti_excel_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-30 13:34:08.000000 opencti_excel_uploader-1.0.7/opencti_excel_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-30 13:34:08.000000 opencti_excel_uploader-1.0.7/opencti_excel_uploader.egg-info/entry_points.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-30 13:34:08.000000 opencti_excel_uploader-1.0.7/opencti_excel_uploader.egg-info/requires.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-30 13:34:08.000000 opencti_excel_uploader-1.0.7/opencti_excel_uploader.egg-info/top_level.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-30 13:34:08.380507 opencti_excel_uploader-1.0.7/setup.cfg
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      896 2024-04-30 13:34:05.000000 opencti_excel_uploader-1.0.7/setup.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 13:40:35.219325 opencti_excel_uploader-1.0.8/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 13:40:35.219325 opencti_excel_uploader-1.0.8/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      501 2024-04-30 10:50:47.000000 opencti_excel_uploader-1.0.8/README.md
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 13:40:35.215325 opencti_excel_uploader-1.0.8/opencti_excel_uploader/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.8/opencti_excel_uploader/__init__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     2960 2024-04-30 13:40:20.000000 opencti_excel_uploader-1.0.8/opencti_excel_uploader/__main__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.8/opencti_excel_uploader/models.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    14402 2024-04-30 13:40:10.000000 opencti_excel_uploader-1.0.8/opencti_excel_uploader/xlsx_utils.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 13:40:35.219325 opencti_excel_uploader-1.0.8/opencti_excel_uploader.egg-info/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 13:40:35.000000 opencti_excel_uploader-1.0.8/opencti_excel_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-30 13:40:35.000000 opencti_excel_uploader-1.0.8/opencti_excel_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-30 13:40:35.000000 opencti_excel_uploader-1.0.8/opencti_excel_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-30 13:40:35.000000 opencti_excel_uploader-1.0.8/opencti_excel_uploader.egg-info/entry_points.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-30 13:40:35.000000 opencti_excel_uploader-1.0.8/opencti_excel_uploader.egg-info/requires.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-30 13:40:35.000000 opencti_excel_uploader-1.0.8/opencti_excel_uploader.egg-info/top_level.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-30 13:40:35.219325 opencti_excel_uploader-1.0.8/setup.cfg
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      896 2024-04-30 13:40:31.000000 opencti_excel_uploader-1.0.8/setup.py
```

### Comparing `opencti_excel_uploader-1.0.7/PKG-INFO` & `opencti_excel_uploader-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 1.0.7
+Version: 1.0.8
 Summary: Creates workbench files from excel files for Opencti
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-1.0.7/opencti_excel_uploader/__main__.py` & `opencti_excel_uploader-1.0.8/opencti_excel_uploader/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -55,34 +55,33 @@
             f.write(f"AUTHOR_LASTNAME={author_secondname}\n")
             f.write(f"AUTHOR_EMAIL={author_email}\n")
             f.write(f"MARKING_DEFINITION={marking_definition}\n")
 
         process_folder()
 
 
-def process_folder():
+def process_folder(
+    author_firstname, author_secondname, author_email, marking_definition
+):
     try:
 
         print("Starting to convert.", flush=True)
         folder_path = sys.argv[1] if len(sys.argv) > 1 else "."
         if folder_path:
             print(f"Folder path: {folder_path}", flush=True)
         else:
             print("No folder path provided. Using current directory.", flush=True)
             folder_path = "."
-        folder_to_json(folder_path)
+        folder_to_json(
+            folder_path,
+            author_firstname,
+            author_secondname,
+            author_email,
+            marking_definition,
+        )
     except Exception as e:
         print(f"Error: {e}", flush=True)
 
 
 if __name__ == "__main__":
     print("Starting...", flush=True)
     setup_opencti_config()
-    print("Configuration saved. Please ensure to keep your .env file secure!")
-    author_firstname = os.getenv("AUTHOR_FIRSTNAME")
-    print(f"author_firstname: {author_firstname}")
-    author_secondname = os.getenv("AUTHOR_LASTNAME")
-    print(f"author_secondname: {author_secondname}")
-    author_email = os.getenv("AUTHOR_EMAIL")
-    print(f"author_email: {author_email}")
-    marking_definition = os.getenv("MARKING_DEFINITION")
-    print(f"marking_definition: {marking_definition}")
```

### Comparing `opencti_excel_uploader-1.0.7/opencti_excel_uploader/models.py` & `opencti_excel_uploader-1.0.8/opencti_excel_uploader/models.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-1.0.7/opencti_excel_uploader/xlsx_utils.py` & `opencti_excel_uploader-1.0.8/opencti_excel_uploader/xlsx_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,15 @@
 import uuid
 import datetime
 import os
 import json
 import random
 import openpyxl
 from dotenv import load_dotenv
-from .__main__ import (
-    author_firstname,
-    author_secondname,
-    marking_definition,
-    author_email,
-)
+
 
 load_dotenv()
 
 
 now = datetime.datetime.now()
 published = now.isoformat() + "Z"
 
@@ -51,15 +46,17 @@
 
             if not found_duplicate:
                 unique_dicts.append(d)
 
     return unique_dicts
 
 
-def create_bundle(i):
+def create_bundle(
+    i, author_firstname, author_secondname, author_email, marking_definition
+):
     bundle = {
         "type": "bundle",
         "id": "bundle--"
         + str(uuid.uuid5(uuid.NAMESPACE_DNS, "bundle" + str(random.random()))),
         "bundle_name": "unnamed",
         "objects": [
             {
@@ -366,15 +363,17 @@
             name=row["Name"],
             description=row["Description"],
         )
         vulnerabilities.append(vulnerability)
     return vulnerabilities
 
 
-def process_report(df):
+def process_report(
+    df, author_firstname, author_secondname, author_email, marking_definition
+):
     # Initialize related objects and external references
     related_objects = []
     external_ref_list = []
     data = df["Incident"]
     instructions = True
     print("Processing Report...", flush=True)
     # Check length of data
@@ -420,31 +419,45 @@
         objectMarking=marking_definition,
         extRef=[data["External Reference"]].extend(external_ref_list),
         author=author_firstname,
         relatedEntities=related_objects,
     )
 
 
-def excel_to_json(file):
+def excel_to_json(
+    file, author_firstname, author_secondname, author_email, marking_definition
+):
     df = load_excel(file)
-    report = process_report(df)
-    bundle = create_bundle(report)
+    report = process_report(
+        df, author_firstname, author_secondname, author_email, marking_definition
+    )
+    bundle = create_bundle(
+        report, author_firstname, author_secondname, author_email, marking_definition
+    )
     for item in bundle["objects"]:
         print(item)
     desktop_path = os.path.join(os.path.expanduser("~"), "Desktop")
     with open(os.path.join(desktop_path, f"{report.name}.json"), "w") as f:
         print(f"Writing {report.name}.json to the desktop.", flush=True)
         json.dump(bundle, f)
 
 
-def folder_to_json(folder):
+def folder_to_json(
+    folder, author_firstname, author_secondname, author_email, marking_definition
+):
     print(f"Converting all Excel files in {folder} to JSON", flush=True)
     for root, _, files in os.walk(folder):
         print(f"Searching {root} for Excel files.", flush=True)
         # If the folder has no xlsx files, skip
         if not any(file.endswith(".xlsx") for file in files):
             print(f"No Excel files found in {root}. Moving to next folder.", flush=True)
             continue
         for file in files:
             if file.endswith(".xlsx"):
                 print(f"Converting {os.path.join(root, file)} to JSON", flush=True)
-                excel_to_json(os.path.join(root, file))
+                excel_to_json(
+                    os.path.join(root, file),
+                    author_firstname,
+                    author_secondname,
+                    author_email,
+                    marking_definition,
+                )
```

### Comparing `opencti_excel_uploader-1.0.7/opencti_excel_uploader.egg-info/PKG-INFO` & `opencti_excel_uploader-1.0.8/opencti_excel_uploader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 1.0.7
+Version: 1.0.8
 Summary: Creates workbench files from excel files for Opencti
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-1.0.7/setup.py` & `opencti_excel_uploader-1.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="opencti-excel-uploader",
-    version="1.0.7",
+    version="1.0.8",
     packages=find_packages(),
     description="Creates workbench files from excel files for Opencti",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="asz,jjk,eby",
     author_email="rnd@stratc.org",
     license="MIT",
```

