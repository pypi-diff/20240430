# Comparing `tmp/opencti_excel_uploader-1.0.4.tar.gz` & `tmp/opencti_excel_uploader-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencti_excel_uploader-1.0.4.tar", last modified: Tue Apr 30 12:27:42 2024, max compression
+gzip compressed data, was "opencti_excel_uploader-1.0.5.tar", last modified: Tue Apr 30 13:18:20 2024, max compression
```

## Comparing `opencti_excel_uploader-1.0.4.tar` & `opencti_excel_uploader-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 12:27:42.296622 opencti_excel_uploader-1.0.4/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 12:27:42.296622 opencti_excel_uploader-1.0.4/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      501 2024-04-30 10:50:47.000000 opencti_excel_uploader-1.0.4/README.md
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 12:27:42.296622 opencti_excel_uploader-1.0.4/opencti_excel_uploader/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader/__init__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     2828 2024-04-30 12:27:17.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader/__main__.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader/models.py
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    13835 2024-04-30 10:47:02.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader/xlsx_utils.py
-drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 12:27:42.296622 opencti_excel_uploader-1.0.4/opencti_excel_uploader.egg-info/
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 12:27:42.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader.egg-info/PKG-INFO
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-30 12:27:42.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-30 12:27:42.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-30 12:27:42.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader.egg-info/entry_points.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-30 12:27:42.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader.egg-info/requires.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-30 12:27:42.000000 opencti_excel_uploader-1.0.4/opencti_excel_uploader.egg-info/top_level.txt
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-30 12:27:42.296622 opencti_excel_uploader-1.0.4/setup.cfg
--rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      896 2024-04-30 12:27:39.000000 opencti_excel_uploader-1.0.4/setup.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 13:18:20.467459 opencti_excel_uploader-1.0.5/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 13:18:20.463459 opencti_excel_uploader-1.0.5/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      501 2024-04-30 10:50:47.000000 opencti_excel_uploader-1.0.5/README.md
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 13:18:20.463459 opencti_excel_uploader-1.0.5/opencti_excel_uploader/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       27 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader/__init__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     2826 2024-04-30 13:18:00.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader/__main__.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    19553 2024-04-29 12:04:56.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader/models.py
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)    13927 2024-04-30 13:17:51.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader/xlsx_utils.py
+drwxr-xr-x   0 strat-ext-e-03 (1986003676) domain users (1986000513)        0 2024-04-30 13:18:20.463459 opencti_excel_uploader-1.0.5/opencti_excel_uploader.egg-info/
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)     1067 2024-04-30 13:18:20.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      436 2024-04-30 13:18:20.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)        1 2024-04-30 13:18:20.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       80 2024-04-30 13:18:20.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader.egg-info/entry_points.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      114 2024-04-30 13:18:20.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader.egg-info/requires.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       23 2024-04-30 13:18:20.000000 opencti_excel_uploader-1.0.5/opencti_excel_uploader.egg-info/top_level.txt
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)       38 2024-04-30 13:18:20.467459 opencti_excel_uploader-1.0.5/setup.cfg
+-rw-r--r--   0 strat-ext-e-03 (1986003676) domain users (1986000513)      896 2024-04-30 13:18:17.000000 opencti_excel_uploader-1.0.5/setup.py
```

### Comparing `opencti_excel_uploader-1.0.4/PKG-INFO` & `opencti_excel_uploader-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 1.0.4
+Version: 1.0.5
 Summary: Creates workbench files from excel files for Opencti
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-1.0.4/opencti_excel_uploader/__main__.py` & `opencti_excel_uploader-1.0.5/opencti_excel_uploader/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 
 if load_dotenv(".env"):  # Load the environment variables from .env file
     print("Loaded environment variables from .env file.")
     print(
         f"OPENCTI_URL: {os.getenv('OPENCTI_URL')}, \n OPENCTI_TOKEN: {os.getenv('OPENCTI_TOKEN')}, \n AUTHOR_FIRSTNAME: {os.getenv('AUTHOR_FIRSTNAME')},\n AUTHOR_LASTNAME: {os.getenv('AUTHOR_LASTNAME')}, \n AUTHOR_EMAIL: {os.getenv('AUTHOR_EMAIL')},\n MARKING_DEFINITION: {os.getenv('MARKING_DEFINITION')}"
     )
-
-
 else:
     print("Failed to load .env file.")
 
 
 def main():
     setup_opencti_config()
```

### Comparing `opencti_excel_uploader-1.0.4/opencti_excel_uploader/models.py` & `opencti_excel_uploader-1.0.5/opencti_excel_uploader/models.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-1.0.4/opencti_excel_uploader/xlsx_utils.py` & `opencti_excel_uploader-1.0.5/opencti_excel_uploader/xlsx_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,20 @@
 import random
 import openpyxl
 from dotenv import load_dotenv
 
 
 load_dotenv()
 
+author_firstname = os.getenv("AUTHOR_FIRSTNAME")
+author_secondname = os.getenv("AUTHOR_LASTNAME")
+author_email = os.getenv("AUTHOR_EMAIL")
+marking_definition = os.getenv("MARKING_DEFINITION")
+
+
 now = datetime.datetime.now()
 published = now.isoformat() + "Z"
 
 
 def drop_duplicates(list_of_dicts):
     """Drops duplicates from a list of dictionaries"""
     unique_dicts = []
@@ -57,18 +63,18 @@
         "bundle_name": "unnamed",
         "objects": [
             {
                 "id": "marking-definition--826578e1-40ad-459f-bc73-ede076f81f37",
                 "entity_type": "Marking-Definition",
                 "standard_id": "marking-definition--826578e1-40ad-459f-bc73-ede076f81f37",
                 "definition_type": "TLP",
-                "definition": os.getenv("marking_definition"),
+                "definition": marking_definition,
                 "x_opencti_color": "#d84315",
                 "x_opencti_order": 3,
-                "name": os.getenv("marking_definition"),
+                "name": marking_definition,
                 "type": "marking-definition",
             }
         ],
     }
     print(f"Creating bundle for basic incident #{i}", flush=True)
     objects = []
     # Create object list
@@ -83,18 +89,18 @@
     # Add the author if the incident is a report
     if isinstance(i, Report) and i.author:
         author_dict = i.find_author()
     else:
         author_dict = {
             "id": "identity--24f595b1-bb5b-5c05-a7d8-337a224de086",
             "identity_class": "individual",
-            "name": os.getenv("AUTHOR_FIRSTNAME"),
-            "contact_information": os.getenv("AUTHOR_EMAIL"),
-            "x_opencti_firstname": os.getenv("AUTHOR_FIRSTNAME"),
-            "x_opencti_lastname": os.getenv("AUTHOR_LASTNAME"),
+            "name": author_firstname,
+            "contact_information": author_email,
+            "x_opencti_firstname": author_firstname,
+            "x_opencti_lastname": author_secondname,
             "x_opencti_id": "f995efca-7522-438a-b68b-44b9b698a285",
             "x_opencti_type": "Individual",
             "type": "identity",
         }
     if author_dict:
         object_list.append(author_dict)
         object_ids.append(author_dict["id"])
@@ -407,17 +413,17 @@
     return Report(
         name=data["Name"].replace("/", "-"),
         description=data["Description"].replace("/", "-"),
         objectLabel=[],
         first_seen=now,
         confidence=90,
         objective=[],
-        objectMarking=os.getenv("marking_definition"),
+        objectMarking=marking_definition,
         extRef=[data["External Reference"]].extend(external_ref_list),
-        author=os.getenv("AUTHOR_FIRSTNAME"),
+        author=author_firstname,
         relatedEntities=related_objects,
     )
 
 
 def excel_to_json(file):
     df = load_excel(file)
     report = process_report(df)
```

### Comparing `opencti_excel_uploader-1.0.4/opencti_excel_uploader.egg-info/PKG-INFO` & `opencti_excel_uploader-1.0.5/opencti_excel_uploader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 1.0.4
+Version: 1.0.5
 Summary: Creates workbench files from excel files for Opencti
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-1.0.4/setup.py` & `opencti_excel_uploader-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="opencti-excel-uploader",
-    version="1.0.4",
+    version="1.0.5",
     packages=find_packages(),
     description="Creates workbench files from excel files for Opencti",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="asz,jjk,eby",
     author_email="rnd@stratc.org",
     license="MIT",
```

