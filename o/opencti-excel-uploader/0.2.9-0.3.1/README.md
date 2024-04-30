# Comparing `tmp/opencti_excel_uploader-0.2.9.tar.gz` & `tmp/opencti_excel_uploader-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencti_excel_uploader-0.2.9.tar", last modified: Mon Apr 29 13:21:36 2024, max compression
+gzip compressed data, was "opencti_excel_uploader-0.3.1.tar", last modified: Mon Apr 29 14:05:07 2024, max compression
```

## Comparing `opencti_excel_uploader-0.2.9.tar` & `opencti_excel_uploader-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 strat-ext-e-04 (1986003675) domain users (1986000513)        0 2024-04-29 13:21:36.399147 opencti_excel_uploader-0.2.9/
--rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      997 2024-04-29 13:21:36.399147 opencti_excel_uploader-0.2.9/PKG-INFO
--rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      436 2024-04-29 11:43:55.000000 opencti_excel_uploader-0.2.9/README.md
-drwxr-xr-x   0 strat-ext-e-04 (1986003675) domain users (1986000513)        0 2024-04-29 13:21:36.399147 opencti_excel_uploader-0.2.9/opencti_excel_uploader/
--rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)       27 2024-04-29 11:43:55.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader/__init__.py
--rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)     1842 2024-04-29 11:43:55.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader/__main__.py
--rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)    19553 2024-04-29 12:28:49.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader/models.py
--rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      146 2024-04-29 12:25:14.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader/test.py
--rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)    10350 2024-04-29 13:07:32.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader/xlsx_utils.py
--rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)    48307 2024-04-29 12:28:25.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader/xml_utils.py
-drwxr-xr-x   0 strat-ext-e-04 (1986003675) domain users (1986000513)        0 2024-04-29 13:21:36.399147 opencti_excel_uploader-0.2.9/opencti_excel_uploader.egg-info/
--rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      997 2024-04-29 13:21:36.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader.egg-info/PKG-INFO
--rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      503 2024-04-29 13:21:36.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)        1 2024-04-29 13:21:36.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)       80 2024-04-29 13:21:36.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader.egg-info/entry_points.txt
--rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      114 2024-04-29 13:21:36.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader.egg-info/requires.txt
--rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)       23 2024-04-29 13:21:36.000000 opencti_excel_uploader-0.2.9/opencti_excel_uploader.egg-info/top_level.txt
--rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)       38 2024-04-29 13:21:36.399147 opencti_excel_uploader-0.2.9/setup.cfg
--rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      891 2024-04-29 13:21:11.000000 opencti_excel_uploader-0.2.9/setup.py
+drwxr-xr-x   0 strat-ext-e-04 (1986003675) domain users (1986000513)        0 2024-04-29 14:05:06.999842 opencti_excel_uploader-0.3.1/
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      997 2024-04-29 14:05:06.999842 opencti_excel_uploader-0.3.1/PKG-INFO
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      436 2024-04-29 11:43:55.000000 opencti_excel_uploader-0.3.1/README.md
+drwxr-xr-x   0 strat-ext-e-04 (1986003675) domain users (1986000513)        0 2024-04-29 14:05:06.999842 opencti_excel_uploader-0.3.1/opencti_excel_uploader/
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)       27 2024-04-29 11:43:55.000000 opencti_excel_uploader-0.3.1/opencti_excel_uploader/__init__.py
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)     1842 2024-04-29 11:43:55.000000 opencti_excel_uploader-0.3.1/opencti_excel_uploader/__main__.py
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)    19553 2024-04-29 12:28:49.000000 opencti_excel_uploader-0.3.1/opencti_excel_uploader/models.py
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      146 2024-04-29 12:25:14.000000 opencti_excel_uploader-0.3.1/opencti_excel_uploader/test.py
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)    10941 2024-04-29 14:02:55.000000 opencti_excel_uploader-0.3.1/opencti_excel_uploader/xlsx_utils.py
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)    48307 2024-04-29 12:28:25.000000 opencti_excel_uploader-0.3.1/opencti_excel_uploader/xml_utils.py
+drwxr-xr-x   0 strat-ext-e-04 (1986003675) domain users (1986000513)        0 2024-04-29 14:05:06.999842 opencti_excel_uploader-0.3.1/opencti_excel_uploader.egg-info/
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      997 2024-04-29 14:05:06.000000 opencti_excel_uploader-0.3.1/opencti_excel_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      503 2024-04-29 14:05:06.000000 opencti_excel_uploader-0.3.1/opencti_excel_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)        1 2024-04-29 14:05:06.000000 opencti_excel_uploader-0.3.1/opencti_excel_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)       80 2024-04-29 14:05:06.000000 opencti_excel_uploader-0.3.1/opencti_excel_uploader.egg-info/entry_points.txt
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      114 2024-04-29 14:05:06.000000 opencti_excel_uploader-0.3.1/opencti_excel_uploader.egg-info/requires.txt
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)       23 2024-04-29 14:05:06.000000 opencti_excel_uploader-0.3.1/opencti_excel_uploader.egg-info/top_level.txt
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)       38 2024-04-29 14:05:06.999842 opencti_excel_uploader-0.3.1/setup.cfg
+-rw-r--r--   0 strat-ext-e-04 (1986003675) domain users (1986000513)      891 2024-04-29 14:05:01.000000 opencti_excel_uploader-0.3.1/setup.py
```

### Comparing `opencti_excel_uploader-0.2.9/PKG-INFO` & `opencti_excel_uploader-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 0.2.9
+Version: 0.3.1
 Summary: Uploader for cases and reports from Excel files
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-0.2.9/opencti_excel_uploader/__main__.py` & `opencti_excel_uploader-0.3.1/opencti_excel_uploader/__main__.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-0.2.9/opencti_excel_uploader/models.py` & `opencti_excel_uploader-0.3.1/opencti_excel_uploader/models.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-0.2.9/opencti_excel_uploader/xlsx_utils.py` & `opencti_excel_uploader-0.3.1/opencti_excel_uploader/xlsx_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,23 +21,26 @@
 from .xml_utils import create_bundle
 import openpyxl
 
 now = datetime.datetime.now()
 published = now.isoformat() + "Z"
 
 def parse_date(date):
+    if isinstance(date, datetime.datetime):
+        print(f"Date {date} is already a datetime object.")
+        return date
+    
     formats = ["%Y-%m-%d", "%Y-%m-%d %H:%M:%S", "%Y-%m-%d %H:%M:%S.%f", "%Y-%d-%m", "%Y-%d-%m %H:%M:%S", "%Y-%d-%m %H:%M:%S.%f"]
     
     for fmt in formats:
         try:
-            date=datetime.datetime.strptime(date, fmt)
-            print(date, type(date))
-            return date
-        except ValueError:
-            pass
+            return datetime.datetime.strptime(date, fmt)
+        except ValueError as e:
+            print(f"ValueError: {e} does not match format {fmt}. Trying next format.")
+            continue
     
     return now
     
 def stix_id(entity_type):
     random_str = str(random.randint(1000, 9999))
     return f"{entity_type}--{str(uuid.uuid5(uuid.NAMESPACE_DNS, random_str))}"
 
@@ -81,21 +84,24 @@
         observables_data = observables_data.drop(0)
 
     # Create a list of observables
     observables = []
     for _, row in observables_data.iterrows():
         if row["URL"] == "":
             break
+        observable_date = parse_date(row["Datetime"])
+        print(f"Processing observable {row['URL']} with date {observable_date}.", flush=True)
         observable = Observable(
             url=row["URL"],
-            date=parse_date(row["Datetime"]),
+            date=observable_date,
             archivedUrl=row["Archived link"],
             language=row["Language"],
         )
         observables.append(observable)
+        print("Observable processed.", flush=True)
     return observables
 
 
 def process_identity(identity_data, instructions):
     opencti_client = get_opencti_client()
     # Drop first row with instructions
     if instructions:
@@ -155,21 +161,25 @@
     # Drop first row with instructions
     if instructions:
         event_data = event_data.drop(0)
 
     # Create a list of events
     events = []
     for _, row in event_data.iterrows():
+        start_date = parse_date(row["Start date"])
+        end_date = parse_date(row["End date"])
+        print(f"Processing event. Start date: {start_date}, End date: {end_date}", flush=True)
         event = Event(
             name=row["Name"],
             description=row["Description"],
-            start_date=parse_date(row["Start date"]),
-            end_date=parse_date(row["End date"]),
+            start_date=start_date,
+            end_date=end_date,
         )
         events.append(event)
+        print("Event processed.", flush=True)
     return events
 
 
 def process_attack_pattern(attack_pattern_df):
     # Find TTPs used in Incident
     attack_pattern_df["Used in Incident"] = attack_pattern_df[
         "Used in Incident"
@@ -296,16 +306,16 @@
             related_objects.extend(
                 process_campaign(df[key], external_ref_list, instructions)
             )
         if key == "Vulnerabilities":
             related_objects.extend(process_vulnerabilities(df[key], instructions))
 
     return Report(
-        name=data["Name"],
-        description=data["Description"],
+        name=data["Name"].replace("/", "-"),
+        description=data["Description"].replace("/", "-"),
         objectLabel=[],
         first_seen=now,
         confidence=90,
         objective=[],
         objectMarking="TLP:AMBER+STRICT",
         extRef=[data["External Reference"]].extend(external_ref_list),
         author="EEAS",
```

### Comparing `opencti_excel_uploader-0.2.9/opencti_excel_uploader/xml_utils.py` & `opencti_excel_uploader-0.3.1/opencti_excel_uploader/xml_utils.py`

 * *Files identical despite different names*

### Comparing `opencti_excel_uploader-0.2.9/opencti_excel_uploader.egg-info/PKG-INFO` & `opencti_excel_uploader-0.3.1/opencti_excel_uploader.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencti-excel-uploader
-Version: 0.2.9
+Version: 0.3.1
 Summary: Uploader for cases and reports from Excel files
 Author: asz,jjk,eby
 Author-email: rnd@stratc.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opencti_excel_uploader-0.2.9/setup.py` & `opencti_excel_uploader-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="opencti-excel-uploader",
-    version="0.2.9",
+    version="0.3.1",
     packages=find_packages(),
     description="Uploader for cases and reports from Excel files",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="asz,jjk,eby",
     author_email="rnd@stratc.org",
     license="MIT",
```

