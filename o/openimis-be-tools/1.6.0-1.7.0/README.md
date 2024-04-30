# Comparing `tmp/openimis-be-tools-1.6.0.tar.gz` & `tmp/openimis_be_tools-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-tools-1.6.0.tar", last modified: Sat Dec 16 00:57:32 2023, max compression
+gzip compressed data, was "openimis_be_tools-1.7.0.tar", last modified: Tue Apr 30 09:06:06 2024, max compression
```

## Comparing `openimis-be-tools-1.6.0.tar` & `openimis_be_tools-1.7.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:32.817669 openimis-be-tools-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2023-12-16 00:57:32.817669 openimis-be-tools-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:32.817669 openimis-be-tools-1.6.0/openimis_be_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2023-12-16 00:57:32.000000 openimis-be-tools-1.6.0/openimis_be_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-16 00:57:32.000000 openimis-be-tools-1.6.0/openimis_be_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:57:32.000000 openimis-be-tools-1.6.0/openimis_be_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-16 00:57:32.000000 openimis-be-tools-1.6.0/openimis_be_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-16 00:57:32.000000 openimis-be-tools-1.6.0/openimis_be_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:57:32.817669 openimis-be-tools-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-12-16 00:57:32.000000 openimis-be-tools-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:32.813669 openimis-be-tools-1.6.0/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:32.817669 openimis-be-tools-1.6.0/tools/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/migrations/0002_extract_file_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/migrations/0003_auto_20211220_0920.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/migrations/0004_registers_right_for_scheme_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/migrations/0005_items_services_rights.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/migrations/0006_update_django_scheme_with_missing_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/migrations/0007_set_managed_to_true.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     6984 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    72802 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:32.817669 openimis-be-tools-1.6.0/tools/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (127)    60122 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/tests/test_upload_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    58395 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/tests/test_upload_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22712 2023-12-16 00:57:21.000000 openimis-be-tools-1.6.0/tools/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:06.523431 openimis_be_tools-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-30 09:06:06.523431 openimis_be_tools-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:06.523431 openimis_be_tools-1.7.0/openimis_be_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-30 09:06:06.000000 openimis_be_tools-1.7.0/openimis_be_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-30 09:06:06.000000 openimis_be_tools-1.7.0/openimis_be_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:06:06.000000 openimis_be_tools-1.7.0/openimis_be_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-30 09:06:06.000000 openimis_be_tools-1.7.0/openimis_be_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 09:06:06.000000 openimis_be_tools-1.7.0/openimis_be_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:06:06.523431 openimis_be_tools-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-30 09:06:06.000000 openimis_be_tools-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:06.523431 openimis_be_tools-1.7.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:06.523431 openimis_be_tools-1.7.0/tools/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/migrations/0002_extract_file_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/migrations/0003_auto_20211220_0920.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/migrations/0004_registers_right_for_scheme_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/migrations/0005_items_services_rights.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/migrations/0006_update_django_scheme_with_missing_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/migrations/0007_set_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72951 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:06.523431 openimis_be_tools-1.7.0/tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60122 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/tests/test_upload_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58395 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/tests/test_upload_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22430 2024-04-30 09:05:53.000000 openimis_be_tools-1.7.0/tools/views.py
```

### Comparing `openimis-be-tools-1.6.0/LICENSE.md` & `openimis_be_tools-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.6.0/PKG-INFO` & `openimis_be_tools-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-tools
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Tools reference module.
 Home-page: https://openimis.org/
 Author: Bluesquare
 Author-email: developers@bluesquare.org
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-tools-1.6.0/README.md` & `openimis_be_tools-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.6.0/openimis_be_tools.egg-info/PKG-INFO` & `openimis_be_tools-1.7.0/openimis_be_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-tools
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Tools reference module.
 Home-page: https://openimis.org/
 Author: Bluesquare
 Author-email: developers@bluesquare.org
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-tools-1.6.0/openimis_be_tools.egg-info/SOURCES.txt` & `openimis_be_tools-1.7.0/openimis_be_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.6.0/setup.py` & `openimis_be_tools-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="openimis-be-tools",
-    version='v1.6.0',
+    version='v1.7.0',
     packages=find_packages(),
     include_package_data=True,
     license="GNU AGPL v3",
     description="The openIMIS Backend Tools reference module.",
     # long_description=README,
     url="https://openimis.org/",
     author="Bluesquare",
```

### Comparing `openimis-be-tools-1.6.0/tools/apps.py` & `openimis_be_tools-1.7.0/tools/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.6.0/tools/migrations/0001_initial.py` & `openimis_be_tools-1.7.0/tools/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.6.0/tools/migrations/0002_extract_file_field.py` & `openimis_be_tools-1.7.0/tools/migrations/0002_extract_file_field.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.6.0/tools/migrations/0003_auto_20211220_0920.py` & `openimis_be_tools-1.7.0/tools/migrations/0003_auto_20211220_0920.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.6.0/tools/migrations/0005_items_services_rights.py` & `openimis_be_tools-1.7.0/tools/migrations/0005_items_services_rights.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.6.0/tools/migrations/0006_update_django_scheme_with_missing_fields.py` & `openimis_be_tools-1.7.0/tools/migrations/0006_update_django_scheme_with_missing_fields.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.6.0/tools/models.py` & `openimis_be_tools-1.7.0/tools/models.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.6.0/tools/resources.py` & `openimis_be_tools-1.7.0/tools/resources.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.6.0/tools/serializers.py` & `openimis_be_tools-1.7.0/tools/serializers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.6.0/tools/services.py` & `openimis_be_tools-1.7.0/tools/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,16 @@
             errors.append(f"Name cannot be longer than 255 characters: '{name}'")
         else:
             result.append(dict(code=code, name=name))
 
     return result, errors
 
 
-VALID_PATIENT_CATEGORY_INPUTS = [0, 1, "0", "1"] # added string literals for CSVs (again, CSVs must have a special way to be handled...)
+# added string literals for CSVs (again, CSVs must have a special way to be handled...)
+VALID_PATIENT_CATEGORY_INPUTS = [0, 1, "0", "1"]
 
 
 def parse_xml_items(xml):
     """Parses medical.Items in an XML file.
 
     This function parses all the mandatory fields of a medical.Item
     and calls `parse_optional_item_fields` for parsing the optional fields.
@@ -979,15 +980,15 @@
     with tempfile.TemporaryDirectory() as tmp_dir_name:
         master_data_file_path = os.path.join(tmp_dir_name, "MasterData.txt")
         with open(master_data_file_path, "w") as file:
             file.write(json.dumps(results))
 
         zip_file = tempfile.NamedTemporaryFile(
             "wb",
-            prefix=f"master_data_{datetime.now().isoformat()}",
+            prefix=f"master_data_{datetime.now().strftime('%Y%m%d%H%M%S%f')}",
             suffix=".zip",
             delete=False,
         )
         # We close it directly since the only thing we want is to have a temporary file that will not be deleted
         zip_file.close()
 
         pyminizip.compress(
@@ -1009,36 +1010,36 @@
     INNER JOIN tblInsuree I ON C.InsureeId = I.InsureeId"
     INNER JOIN tblHF HF ON C.HFID = HF.HFID"
     WHERE F.ValidityTo Is NULL AND O.ValidityTo IS NULL"
     AND O.Code = @OfficerCode"
     AND C.FeedbackStatus = 4"
 
     """
-    
+
     prompts = FeedbackPrompt.objects.filter(*filter_validity())\
-        .filter(officer_id = officer.id, claim__feedback_status = Claim.FEEDBACK_SELECTED )\
+        .filter(officer_id=officer.id, claim__feedback_status=Claim.FEEDBACK_SELECTED)\
         .select_related('claim',
-        'claim__insuree',
-        'claim__health_facility')
+                        'claim__insuree',
+                        'claim__health_facility')
     results = []
     format_date = '%d-%m-%Y'
     for p in prompts:
         results.append({
-            "ClaimID" : p.claim_id,
+            "ClaimID": p.claim_id,
             "OfficerID": officer.id,
             "OfficerCode": officer.code,
             "CHFID": p.claim.insuree.chf_id,
             "LastName": p.claim.insuree.last_name,
             "OtherNames": p.claim.insuree.other_names,
             "HFCode": p.claim.health_facility.code,
             "HFName": p.claim.health_facility.name,
             "ClaimCode": p.claim.code,
             "DateFrom": p.claim.date_from.strftime(format_date),
-            "DateTo":  p.claim.date_to.strftime(format_date),
-            "Phone":  officer.phone,
+            "DateTo": p.claim.date_to.strftime(format_date),
+            "Phone": officer.phone,
             "FeedbackPromptDate": p.feedback_prompt_date.strftime(format_date)
         })
 
     with tempfile.TemporaryDirectory() as tmp_dir_name:
         file_name = f"feedbaks_{officer.code}.txt"
         file_path = os.path.join(tmp_dir_name, file_name)
         with open(file_path, "w") as file:
@@ -1244,19 +1245,20 @@
 
     return extract
 
 
 def upload_claim(user, xml):
     logger.info(f"Uploading claim with user {user.id}")
 
-    if settings.ROW_SECURITY :
+    if settings.ROW_SECURITY:
         logger.info("Check that user can upload claims in claims' health facilities")
         hf_code = xml.find("Claim").find("Details").find("HFCode").text
-        hfs = LocationManager().build_user_location_filter_query(user._u, queryset = HealthFacility.filter_queryset().filter(code=hf_code), loc_types = ['D'])
-        if len(hfs)<1:
+        hfs = LocationManager().build_user_location_filter_query(
+            user._u, queryset=HealthFacility.filter_queryset().filter(code=hf_code), loc_types=['D'])
+        if len(hfs) < 1:
             raise InvalidXMLError(
                 f"User cannot upload claims for health facility {hf_code}"
             )
 
     with connection.cursor() as cursor:
         cursor.execute(
             """
@@ -1643,44 +1645,52 @@
     # TODO : refactor this function and the code used in validating XML uploads
     categories = [row["adult_cat"], row["minor_cat"], row["male_cat"], row["female_cat"]]
     if len(row["code"]) < 1 or len(row["code"]) > 6:
         raise ValidationError(f"Item '{row['code']}': code is invalid. Must be between 1 and 6 characters")
     elif len(row["name"]) < 1 or len(row["name"]) > 100:
         raise ValidationError(f"Item '{row['code']}': name is invalid. Must be between 1 and 100 characters")
     elif row["type"] not in Item.TYPE_VALUES:
-        raise ValidationError(f"Item '{row['code']}': type is invalid. Must be one of the following: {Item.TYPE_VALUES}")
+        raise ValidationError(
+            f"Item '{row['code']}': type is invalid. Must be one of the following: {Item.TYPE_VALUES}")
     elif row["care_type"] not in ItemOrService.CARE_TYPE_VALUES:
-        raise ValidationError(f"Item '{row['code']}': care type is invalid. Must be one of the following: {ItemOrService.CARE_TYPE_VALUES}")
+        raise ValidationError(
+            f"Item '{row['code']}': care type is invalid. Must be one of the following: {ItemOrService.CARE_TYPE_VALUES}")
     elif any([cat not in VALID_PATIENT_CATEGORY_INPUTS for cat in categories]):
-        raise ValidationError(f"Item '{row['code']}': patient categories are invalid. Must be one of the following: [0, 1]")
+        raise ValidationError(
+            f"Item '{row['code']}': patient categories are invalid. Must be one of the following: [0, 1]")
     elif "package" in row and (row["package"] is not None) and len(row["package"]) > 255:
         raise ValidationError(f"Item '{row['code']}': package is invalid. Must be maximum 255 characters")
     return
 
 
 def validate_imported_service_row(row):
     # TODO : refactor this function and the code used in validating XML uploads
     categories = [row["adult_cat"], row["minor_cat"], row["male_cat"], row["female_cat"]]
     if len(row["code"]) < 1 or len(row["code"]) > 6:
         raise ValidationError(f"Service '{row['code']}': code is invalid. Must be between 1 and 6 characters")
     elif len(row["name"]) < 1 or len(row["name"]) > 100:
         raise ValidationError(f"Service '{row['code']}': name is invalid. Must be between 1 and 100 characters")
     elif row["type"] not in Service.TYPE_VALUES:
-        raise ValidationError(f"Service '{row['code']}': type is invalid. Must be one of the following: {Service.TYPE_VALUES}")
+        raise ValidationError(
+            f"Service '{row['code']}': type is invalid. Must be one of the following: {Service.TYPE_VALUES}")
     elif row["level"] not in Service.LEVEL_VALUES:
-        raise ValidationError(f"Service '{row['code']}': level is invalid. Must be one of the following: {Service.LEVEL_VALUES}")
+        raise ValidationError(
+            f"Service '{row['code']}': level is invalid. Must be one of the following: {Service.LEVEL_VALUES}")
     elif row["care_type"] not in ItemOrService.CARE_TYPE_VALUES:
-        raise ValidationError(f"Service '{row['code']}': care type is invalid. Must be one of the following: {ItemOrService.CARE_TYPE_VALUES}")
+        raise ValidationError(
+            f"Service '{row['code']}': care type is invalid. Must be one of the following: {ItemOrService.CARE_TYPE_VALUES}")
     elif any([cat not in VALID_PATIENT_CATEGORY_INPUTS for cat in categories]):
-        raise ValidationError(f"Service '{row['code']}': patient categories are invalid. Must be one of the following: [0, 1]")
+        raise ValidationError(
+            f"Service '{row['code']}': patient categories are invalid. Must be one of the following: [0, 1]")
     elif "category" in row and \
             row["category"] is not None and \
             len(row["category"]) and \
             row["category"] not in Service.CATEGORY_VALUES:
-        raise ValidationError(f"Service '{row['code']}': category is invalid. Must be one of the following: {Service.CATEGORY_VALUES}")
+        raise ValidationError(
+            f"Service '{row['code']}': category is invalid. Must be one of the following: {Service.CATEGORY_VALUES}")
     return
 
 
 def return_upload_result_json(success=True, xml_result: UploadResult = None, other_types_result: Result = None,
                               other_types_errors=None):
     """Returns a JSON structure containing the result of a data upload.
```

### Comparing `openimis-be-tools-1.6.0/tools/tests/test_services.py` & `openimis_be_tools-1.7.0/tools/tests/test_services.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 
 from tools.services import upload_claim, InvalidXMLError, get_xml_element, get_xml_element_int,\
     InvalidXmlInt, create_officer_feedbacks_export, create_officer_renewals_export
 from xml.etree import ElementTree
 from datetime import date, datetime, time, timedelta
 
 from core.models import Officer
+from core.test_helpers import create_test_officer
+
 from core.utils import filter_validity
+from core.services import create_or_update_officer_villages
 from location.models import Location
 from policy.services import insert_renewals
 from claim.models import Claim
+from claim.services import create_feedback_prompt
 from claim.test_helpers import (
     create_test_claim,
     create_test_claimservice,
     create_test_claimitem,
     delete_claim_with_itemsvc_dedrem_and_history,
 )
-from claim.gql_mutations import create_feedback_prompt
 
 class UploadClaimsTestCase(TestCase):
     def test_upload_claims_unknown_hf(self):
         with patch('tools.services.settings.ROW_SECURITY', new_callable=PropertyMock) as row_security_mock:
             row_security_mock.return_value = True
             mock_user = mock.Mock(is_anonymous=False)
             mock_user.has_perm = mock.MagicMock(return_value=True)
@@ -81,15 +84,16 @@
     test_user = None
     claim = None
     @classmethod
     def setUpTestData(cls):
         
         cls.claim = create_test_claim(custom_props={'status': Claim.STATUS_CHECKED, 'feedback_status': Claim.FEEDBACK_SELECTED})
         
-        cls.test_officer = Officer.objects.filter(officer_villages__location = cls.claim.insuree.family.location).first()
+        cls.test_officer = create_test_officer(villages = [cls.claim.insuree.family.location])
+        
         insert_renewals(
             date_from= date.today() + timedelta(days=-3650), 
             date_to=date.today()+ timedelta(days=7300), 
             officer_id=cls.test_officer.id, 
             reminding_interval=365, 
             location_id=cls.claim.insuree.family.location.id, 
             location_levels=4)
@@ -97,15 +101,15 @@
     def test_generating_feedback(self):
         class DummyUser:
             id_for_audit = -1
         mock_user = mock.Mock(is_anonymous=False)
         mock_user.has_perm = mock.MagicMock(return_value=True)
         mock_user.is_imis_admin = mock.MagicMock(return_value=False)
         
-        create_feedback_prompt(self.claim.uuid, user=DummyUser())
+        create_feedback_prompt(self.claim, user=DummyUser())
         zip = create_officer_feedbacks_export(mock_user, self.test_officer)
         self.assertNotEqual(zip, None)
         
     def test_generating_renewal(self):
         mock_user = mock.Mock(is_anonymous=False)
         mock_user.has_perm = mock.MagicMock(return_value=True)
         mock_user.is_imis_admin = mock.MagicMock(return_value=False)
```

### Comparing `openimis-be-tools-1.6.0/tools/tests/test_upload_items.py` & `openimis_be_tools-1.7.0/tools/tests/test_upload_items.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.6.0/tools/tests/test_upload_services.py` & `openimis_be_tools-1.7.0/tools/tests/test_upload_services.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.6.0/tools/urls.py` & `openimis_be_tools-1.7.0/tools/urls.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.6.0/tools/utils.py` & `openimis_be_tools-1.7.0/tools/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tools-1.6.0/tools/views.py` & `openimis_be_tools-1.7.0/tools/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import os
 import tempfile
 import xml.etree.ElementTree as ET
 
 from core.models import Officer
+from core.security import checkUserWithRights
 from core.utils import filter_validity
 from django.core.exceptions import PermissionDenied
 from django.db.models.query_utils import Q
 from django.http import HttpResponse
 from django.http.response import FileResponse, JsonResponse
 from django.shortcuts import get_object_or_404
 from django.utils.translation import gettext as _
@@ -15,32 +16,24 @@
 from import_export.resources import ModelResource
 from tablib import Dataset
 
 from location.models import HealthFacility, Location
 from medical.models import Diagnosis, Item, Service
 from location.apps import DEFAULT_CFG as LOCATION_DEFAULT_CFG
 from rest_framework.decorators import api_view, permission_classes, renderer_classes
-from rest_framework.permissions import IsAuthenticated
+
 from rest_framework.response import Response
 from . import serializers, services, utils
 from .apps import ToolsConfig
 from .resources import ItemResource, ServiceResource
 from .services import return_upload_result_json
 
 logger = logging.getLogger(__name__)
 
 
-def checkUserWithRights(rights):
-    class UserWithRights(IsAuthenticated):
-        def has_permission(self, request, view):
-            return super().has_permission(request, view) and request.user.has_perms(
-                rights
-            )
-
-    return UserWithRights
 
 
 @api_view(["GET"])
 @permission_classes(
     [
         checkUserWithRights(
             ToolsConfig.registers_locations_perms,
```

