# Comparing `tmp/openimis-be-location-1.6.1rc1.tar.gz` & `tmp/openimis_be_location-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-location-1.6.1rc1.tar", last modified: Mon Feb 26 10:42:37 2024, max compression
+gzip compressed data, was "openimis_be_location-1.7.0.tar", last modified: Tue Apr 30 09:00:41 2024, max compression
```

## Comparing `openimis-be-location-1.6.1rc1.tar` & `openimis_be_location-1.7.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 10:42:37.030855 openimis-be-location-1.6.1rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-02-26 10:42:37.026855 openimis-be-location-1.6.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 10:42:37.022855 openimis-be-location-1.6.1rc1/location/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    12917 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 10:42:37.026855 openimis-be-location-1.6.1rc1/location/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/migrations/0002_location.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/migrations/0003_userdistrict.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/migrations/0004_locationmutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/migrations/0005_healthfacilitycatchment_healthfacilitylegalform_healthfacilitymutation_healthfacilitysublevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/migrations/0006_users_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/migrations/0007_auto_20211103_1046.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/migrations/0008_add_enrollment_officer_gql_query_location_right.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/migrations/0009_add_location_read_right.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/migrations/0010_insert_create_region_location_perms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/migrations/0011_auto_20230317_0924.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/migrations/0012_auto_20230317_0927.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/migrations/0013_auto_20230317_1534.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/migrations/0014_add_missing_fields_to_django_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/migrations/0015_set_managed_to_true.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/migrations/0016_auto_20230816_0934.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/migrations/0017_healthfacility_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/migrations/0018_auto_20230925_2243.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18641 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8025 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/services.py
--rw-r--r--   0 runner    (1001) docker     (127)    18397 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-26 10:42:29.000000 openimis-be-location-1.6.1rc1/location/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 10:42:37.026855 openimis-be-location-1.6.1rc1/openimis_be_location.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-02-26 10:42:36.000000 openimis-be-location-1.6.1rc1/openimis_be_location.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-02-26 10:42:36.000000 openimis-be-location-1.6.1rc1/openimis_be_location.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 10:42:36.000000 openimis-be-location-1.6.1rc1/openimis_be_location.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-26 10:42:36.000000 openimis-be-location-1.6.1rc1/openimis_be_location.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-26 10:42:36.000000 openimis-be-location-1.6.1rc1/openimis_be_location.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 10:42:37.030855 openimis-be-location-1.6.1rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-02-26 10:42:36.000000 openimis-be-location-1.6.1rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:41.457589 openimis_be_location-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-30 09:00:41.457589 openimis_be_location-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:41.453589 openimis_be_location-1.7.0/location/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12917 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:41.457589 openimis_be_location-1.7.0/location/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/migrations/0002_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/migrations/0003_userdistrict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/migrations/0004_locationmutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/migrations/0005_healthfacilitycatchment_healthfacilitylegalform_healthfacilitymutation_healthfacilitysublevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/migrations/0006_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/migrations/0007_auto_20211103_1046.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/migrations/0008_add_enrollment_officer_gql_query_location_right.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/migrations/0009_add_location_read_right.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/migrations/0010_insert_create_region_location_perms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/migrations/0011_auto_20230317_0924.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/migrations/0012_auto_20230317_0927.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/migrations/0013_auto_20230317_1534.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/migrations/0014_add_missing_fields_to_django_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/migrations/0015_set_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/migrations/0016_auto_20230816_0934.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/migrations/0017_healthfacility_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/migrations/0018_auto_20230925_2243.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19009 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8025 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20788 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 09:00:30.000000 openimis_be_location-1.7.0/location/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:41.457589 openimis_be_location-1.7.0/openimis_be_location.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-30 09:00:41.000000 openimis_be_location-1.7.0/openimis_be_location.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-30 09:00:41.000000 openimis_be_location-1.7.0/openimis_be_location.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:00:41.000000 openimis_be_location-1.7.0/openimis_be_location.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 09:00:41.000000 openimis_be_location-1.7.0/openimis_be_location.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 09:00:41.000000 openimis_be_location-1.7.0/openimis_be_location.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:00:41.457589 openimis_be_location-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-30 09:00:41.000000 openimis_be_location-1.7.0/setup.py
```

### Comparing `openimis-be-location-1.6.1rc1/LICENSE.md` & `openimis_be_location-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/PKG-INFO` & `openimis_be_location-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-location
-Version: 1.6.1rc1
+Version: 1.7.0
 Summary: The openIMIS Backend Location reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-location-1.6.1rc1/README.md` & `openimis_be_location-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/apps.py` & `openimis_be_location-1.7.0/location/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/dataloaders.py` & `openimis_be_location-1.7.0/location/dataloaders.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/gql_mutations.py` & `openimis_be_location-1.7.0/location/gql_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/gql_queries.py` & `openimis_be_location-1.7.0/location/gql_queries.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/migrations/0001_initial.py` & `openimis_be_location-1.7.0/location/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/migrations/0002_location.py` & `openimis_be_location-1.7.0/location/migrations/0002_location.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/migrations/0003_userdistrict.py` & `openimis_be_location-1.7.0/location/migrations/0003_userdistrict.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/migrations/0004_locationmutation.py` & `openimis_be_location-1.7.0/location/migrations/0004_locationmutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/migrations/0005_healthfacilitycatchment_healthfacilitylegalform_healthfacilitymutation_healthfacilitysublevel.py` & `openimis_be_location-1.7.0/location/migrations/0005_healthfacilitycatchment_healthfacilitylegalform_healthfacilitymutation_healthfacilitysublevel.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/migrations/0006_users_api.py` & `openimis_be_location-1.7.0/location/migrations/0006_users_api.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/migrations/0007_auto_20211103_1046.py` & `openimis_be_location-1.7.0/location/migrations/0007_auto_20211103_1046.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/migrations/0008_add_enrollment_officer_gql_query_location_right.py` & `openimis_be_location-1.7.0/location/migrations/0008_add_enrollment_officer_gql_query_location_right.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,29 +4,32 @@
 from core.models import RoleRight, Role
 
 
 def forwards_func(apps, schema_editor):
     # Add enrollment officer right to read location data
 
     # Enrollment officer is predefined system role with id 1
-    eo_role = Role.objects.filter(is_system=1, validity_to__isnull=True).get()
+    eo_roles = Role.objects.filter(is_system=1, validity_to__isnull=True)
     # Required Role ID is gql_query_location_perm (121901)
     right_id = 121901
-    RoleRight(
-        role_id=eo_role.id,
-        right_id=right_id,
-        audit_user_id=None,
-    ).save()
+    for eo_role in eo_roles:
+        RoleRight(
+            role_id=eo_role.id,
+            right_id=right_id,
+            audit_user_id=None,
+        ).save()
 
 
 def reverse_func(apps, schema_editor):
     # Same data as in forward function
-    eo_role = Role.objects.filter(is_system=1, validity_to__isnull=True).get()
     right_id = 121901
-    RoleRight.objects.filter(role_id=eo_role.id, right_id=right_id, validity_to__isnull=True).delete()
+    eo_roles = Role.objects.filter(is_system=1, validity_to__isnull=True)
+
+        
+    RoleRight.objects.filter(role__in=eo_roles, right_id=right_id, validity_to__isnull=True).delete()
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ("location", "0007_auto_20211103_1046"),
     ]
```

### Comparing `openimis-be-location-1.6.1rc1/location/migrations/0009_add_location_read_right.py` & `openimis_be_location-1.7.0/location/migrations/0009_add_location_read_right.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/migrations/0010_insert_create_region_location_perms.py` & `openimis_be_location-1.7.0/location/migrations/0010_insert_create_region_location_perms.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/migrations/0011_auto_20230317_0924.py` & `openimis_be_location-1.7.0/location/migrations/0011_auto_20230317_0924.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/migrations/0013_auto_20230317_1534.py` & `openimis_be_location-1.7.0/location/migrations/0013_auto_20230317_1534.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/migrations/0014_add_missing_fields_to_django_scheme.py` & `openimis_be_location-1.7.0/location/migrations/0014_add_missing_fields_to_django_scheme.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/migrations/0015_set_managed_to_true.py` & `openimis_be_location-1.7.0/location/migrations/0015_set_managed_to_true.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/migrations/0016_auto_20230816_0934.py` & `openimis_be_location-1.7.0/location/migrations/0016_auto_20230816_0934.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/migrations/0018_auto_20230925_2243.py` & `openimis_be_location-1.7.0/location/migrations/0018_auto_20230925_2243.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/models.py` & `openimis_be_location-1.7.0/location/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from functools import reduce
 import django
 from django.core.cache import cache
 import uuid
 
 from core import filter_validity
 from django.conf import settings
-from django.db import models
+from django.db import models, connection
+
 from django.db.models.expressions import RawSQL
 from core import models as core_models
 from graphql import ResolveInfo
 from .apps import LocationConfig
 import logging
 from django.db.models import Q
 
@@ -41,15 +42,15 @@
             )
             SELECT * FROM CTE_PARENTS;
         """,
             (location_id,),
         )
         return self.get_location_from_ids((parents), loc_type) if loc_type else parents
 
-    def allowed(self, user_id, loc_types=['R', 'D', 'W', 'V'], strict=True, qs = False):
+    def allowed(self, user_id, loc_types=['R', 'D', 'W', 'V'], strict=True, qs=False):
         query = f"""
             WITH {"" if settings.MSSQL else "RECURSIVE"} USER_LOC AS (SELECT l."LocationId", l."ParentLocationId" FROM "tblUsersDistricts" ud JOIN "tblLocations" l ON ud."LocationId" = l."LocationId"  WHERE ud."ValidityTo"  is Null AND "UserID" = %s ),
              CTE_PARENTS AS (
             SELECT
                 parent."LocationId",
                 parent."LocationType",
                 parent."ParentLocationId"
@@ -67,21 +68,28 @@
             FROM
                 "tblLocations"  child
                 INNER JOIN CTE_PARENTS leaf
                     ON child."ParentLocationId" = leaf."LocationId"
             )
             SELECT DISTINCT "LocationId" FROM CTE_PARENTS WHERE "LocationType" in ('{"','".join(loc_types)}')
         """
-        
-        if qs:
-            #location_allowed = Location.objects.filter( id__in =[obj.id for obj in Location.objects.raw( query,(user_id,))])
-            location_allowed = Location.objects.filter( id__in =RawSQL( query,(user_id,)))
-        
+
+        if qs is not None:
+            # location_allowed = Location.objects.filter( id__in =[obj.id for obj in Location.objects.raw( query,(user_id,))])
+            if settings.MSSQL: # MSSQL don't support WITH in subqueries
+
+                with connection.cursor() as cursor:
+                    cursor.execute(query, (user_id,))
+                    ids = cursor.fetchall()
+                    location_allowed = Location.objects.filter(id__in=[x for x, in ids])
+            else:
+                location_allowed = Location.objects.filter(id__in=RawSQL(query, (user_id,)))
+
         else:
-            location_allowed = Location.objects.raw( query,(user_id,))
+            location_allowed = Location.objects.raw(query, (user_id,))
 
         return location_allowed
 
     def children(self, location_id, loc_type=None):
         children = Location.objects.raw(
             f"""
                 WITH {"" if settings.MSSQL else "RECURSIVE"} CTE_CHILDREN AS (
@@ -112,27 +120,27 @@
         return self.get_location_from_ids((children), loc_type) if loc_type else children
 
 
     def build_user_location_filter_query(self, user: core_models.InteractiveUser, prefix='location', queryset=None, loc_types=['R', 'D', 'W', 'V']):
         q_allowed_location = None
         if not isinstance(user, core_models.InteractiveUser):
             logger.warning(f"Access without filter for user {user.id} ")
-            if queryset:
+            if queryset is not None:
                 return queryset
             else:
                 return Q()
         elif not user.is_imis_admin:
             q_allowed_location = Q((f"{prefix}__in", self.allowed(user.id, loc_types))) | Q((f"{prefix}__isnull", True))
 
-            if queryset:
+            if queryset is not None:
                 return queryset.filter(q_allowed_location)
             else:
                 return q_allowed_location
         else:
-            if queryset:
+            if queryset is not None:
                 return queryset
             else:
                 return Q()
 
 
 
     def get_location_from_ids(self, qsr, loc_type):
@@ -193,15 +201,15 @@
                 from claim.models import ClaimAdmin
                 return ClaimAdmin.objects \
                     .filter(code=user.username, has_login=True, validity_to__isnull=True) \
                     .get().officer_allowed_locations
             elif user.is_imis_admin:
                 return Location.objects
             else:
-                return cls.objects.allowed(user.i_user_id, qs = True)
+                return cls.objects.allowed(user.i_user_id, qs=True)
         return queryset
 
     @staticmethod
     def build_user_location_filter_query(cls, user: core_models.InteractiveUser, queryset=None):
         return cls.objects.build_user_location_filter_query(user, queryset=queryset)
 
     class Meta:
@@ -356,43 +364,43 @@
         :param user: InteractiveUser to filter on
         :return: UserDistrict *objects*
         """
 
         if user.is_superuser is True or (hasattr(user, "is_imis_admin") and user.is_imis_admin):
             all_districts = Location.objects.filter(type='D', *filter_validity())
             districts = []
-            idx = 0 
-            for d in  all_districts:
+            idx = 0
+            for d in all_districts:
                 districts.append(
                     UserDistrict(
                         id=idx,
                         user=user,
                         location=d
                     )
                 )
-            
+
             return districts
 
         elif not isinstance(user, core_models.InteractiveUser):
             if isinstance(user, core_models.TechnicalUser):
                 logger.warning(f"get_user_districts called with a technical user `{user.username}`. "
                                "We'll return an empty list, but it should be handled before reaching here.")
             return UserDistrict.objects.none()
         else:
             return (
-            UserDistrict.objects
+                UserDistrict.objects
                 .filter(location__type='D')
                 .filter(*filter_validity())
                 .filter(*filter_validity(prefix='location__'))
                 .filter(user=user)
                 .prefetch_related("location")
                 .prefetch_related("location__parent")
                 .order_by("location__parent__code")
                 .order_by("location__code")
-        )
+            )
 
     @classmethod
     def get_user_locations(cls, user):
         """
         Retrieve the list of Locations in the UserDistricts of a certain user.
         :param user: InteractiveUser to filter on
         :return: Location objects to filter on.
```

### Comparing `openimis-be-location-1.6.1rc1/location/schema.py` & `openimis_be_location-1.7.0/location/schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/services.py` & `openimis_be_location-1.7.0/location/services.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/location/test_graphql.py` & `openimis_be_location-1.7.0/location/test_graphql.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,20 +37,20 @@
     @classmethod
     def setUpTestData(cls):
         if cls.test_region is None:
             cls.test_village  =create_test_village()
             cls.test_ward =cls.test_village.parent
             cls.test_region =cls.test_village.parent.parent.parent
             cls.test_district = cls.test_village.parent.parent
-        cls.admin_user = create_test_interactive_user(username="testLocationAdmin")
+        cls.admin_user = create_test_interactive_user(username="testLocationAdmin", roles=[7])
         cls.admin_token = get_token(cls.admin_user, DummyContext(user=cls.admin_user))
         cls.noright_user = create_test_interactive_user(username="testLocationNoRight", roles=[1])
         cls.noright_token = get_token(cls.noright_user, DummyContext(user=cls.noright_user))
         cls.admin_dist_user = create_test_interactive_user(username="testLocationDist")
-        assign_user_districts(cls.admin_dist_user, ["R1D1", "R2D1", "R2D2"])
+        assign_user_districts(cls.noright_user, ["R1D1", "R2D1", "R2D2"])
         cls.admin_dist_token = get_token(cls.admin_dist_user, DummyContext(user=cls.admin_dist_user))
         cls.test_location_delete = create_test_location('V', custom_props={"code": "TODEL", "name": "To delete",
                                                                            "parent_id": cls.test_ward.id})
 
     def _getLocationFromAPI(self, code):
         response = self.query(
             '''
@@ -252,15 +252,34 @@
         )
 
         self.assertEquals(response.status_code, status.HTTP_200_OK)
         content = json.loads(response.content)
 
         self.assertResponseNoErrors(response)
         self.assertEqual(content["data"]["deleteLocation"]["clientMutationId"], "testlocation5")
-
+        ## check the mutation answer
+        response = self.query('''
+        {
+        mutationLogs(clientMutationId: "testlocation5")
+        {
+            
+        pageInfo { hasNextPage, hasPreviousPage, startCursor, endCursor}
+        edges
+        {
+        node
+        {
+            id,status,error,clientMutationId,clientMutationLabel,clientMutationDetails,requestDateTime,jsonExt
+        }
+        }
+        }
+        }
+            ''',
+            headers={"HTTP_AUTHORIZATION": f"Bearer {self.admin_token}"})
+        self.assertResponseNoErrors(response)
+        
         self.test_location_delete.refresh_from_db()
 
         self.assertIsNotNone(self.test_location_delete.validity_to)
 
         # TODO test the newParentUUID
 
 
@@ -278,15 +297,15 @@
         super().setUpClass()
         
         cls.admin_user = create_test_interactive_user(username="testHFAdmin")
         cls.admin_token = get_token(cls.admin_user, DummyContext(user=cls.admin_user))
         cls.noright_user = create_test_interactive_user(username="testHFNoRight", roles=[1])
         cls.noright_token = get_token(cls.noright_user, DummyContext(user=cls.noright_user))
         cls.admin_dist_user = create_test_interactive_user(username="testHFDist")
-        assign_user_districts(cls.admin_dist_user, ["R1D1", "R2D1", "R2D2"])
+        assign_user_districts(cls.noright_user, ["R1D1", "R2D1", "R2D2"])
         cls.admin_dist_token = get_token(cls.admin_dist_user, DummyContext(user=cls.admin_dist_user))
 
         if cls.test_region is None:
             cls.test_village = create_test_village()
             cls.test_ward = cls.test_village.parent
             cls.test_district = cls.test_ward.parent
             cls.test_region = cls.test_district.parent
@@ -420,15 +439,15 @@
 
         client_mutation_id = uuid.uuid4()
         client_mutation_label = "Update health facility MDF"
 
         query = f"""
             mutation {{            
                 updateHealthFacility(
-                input: {{clientMutationId: "{client_mutation_id}", clientMutationLabel: "{client_mutation_label}", uuid: "{self.test_hf.uuid}", code: "{self.test_hf.code}", name: "{self.test_hf.name}", locationId: {self.test_hf.location.id}, level: "{self.test_hf.level}", legalFormId: "{self.test_hf.legal_form}", careType: "{self.test_hf.care_type}", accCode: "{self.test_hf.acc_code}", address: "{self.test_hf.address}", phone: "0123456789", status: "AC"}}
+                input: {{clientMutationId: "{client_mutation_id}", clientMutationLabel: "{client_mutation_label}", uuid: "{self.test_hf.uuid}", code: "{self.test_hf.code}", name: "{self.test_hf.name}", locationId: {self.test_hf.location.id}, level: "{self.test_hf.level}", legalFormId: "{self.test_hf.legal_form.code}", careType: "{self.test_hf.care_type}", accCode: "{self.test_hf.acc_code}", address: "{self.test_hf.address}", phone: "0123456789", status: "AC"}}
             ) {{
                 clientMutationId
                 internalId
                 }}
             }}
 
             """
@@ -456,7 +475,72 @@
             }
             ''',
             headers={"HTTP_AUTHORIZATION": f"Bearer {self.admin_token}"},
         )
         self.assertEquals(response.status_code, status.HTTP_200_OK)
         content = json.loads(response.content)
         self.assertResponseNoErrors(response)
+        
+    def test_user_districts_admin(self):
+        
+        response = self.query(
+            '''
+            query
+                {
+                userDistricts
+                {
+                    id,uuid,code,name,parent{id, uuid, code, name}
+                }
+                }
+            ''',
+            headers={"HTTP_AUTHORIZATION": f"Bearer {self.admin_token}"},
+        )
+        self.assertEquals(response.status_code, status.HTTP_200_OK)
+        content = json.loads(response.content)
+        self.assertResponseNoErrors(response)
+
+    def test_user_districts_not_admin(self):
+        
+        response = self.query(
+            '''
+            query
+                {
+                userDistricts
+                {
+                    id,uuid,code,name,parent{id, uuid, code, name}
+                }
+                }
+            ''',
+            headers={"HTTP_AUTHORIZATION": f"Bearer {self.noright_token}"},
+        )
+        self.assertEquals(response.status_code, status.HTTP_200_OK)
+        content = json.loads(response.content)
+        self.assertResponseNoErrors(response)
+        
+    def test_location_not_admin(self):
+        
+        response = self.query(
+            '''
+        query
+    {
+      locations(
+    type: "D",
+    orderBy: "code"
+  )
+      {
+        
+    pageInfo { hasNextPage, hasPreviousPage, startCursor, endCursor}
+    edges
+    {
+      node
+      {
+        id,uuid,type,code,name,malePopulation,femalePopulation,otherPopulation,families,clientMutationId
+      }
+    }
+      }
+    }
+            ''',
+            headers={"HTTP_AUTHORIZATION": f"Bearer {self.noright_token}"},
+        )
+        self.assertEquals(response.status_code, status.HTTP_200_OK)
+        content = json.loads(response.content)
+        self.assertResponseNoErrors(response)
```

### Comparing `openimis-be-location-1.6.1rc1/location/test_helpers.py` & `openimis_be_location-1.7.0/location/test_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     test_ward = create_test_location('W', custom_props={"parent": test_district,"name":"Ward" + custom_props["name"]})
     custom_props["parent"]=test_ward
     test_village = create_test_location('V', custom_props=custom_props)
     
     return test_village
 
 def create_test_health_facility(code, location_id, valid=True, custom_props={}):
-    code= "TST-" + code
+    code= ("TST-" + code) if len(code)<5 else code
     if custom_props is not None and 'code' in custom_props:
         code = custom_props.pop('code')
     hf = HealthFacility.objects.filter(code=code, validity_to__isnull= not valid).first()
     if hf is not None:
         return hf
     else:
         return HealthFacility.objects.create(
```

### Comparing `openimis-be-location-1.6.1rc1/location/tests.py` & `openimis_be_location-1.7.0/location/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,14 @@
         village = create_test_village()
         hierachy = LocationManager().children(self.test_village.parent.parent.parent.id)
         self.assertEqual(len(hierachy),4)
         district = LocationManager().children(self.test_village.parent.parent.parent.id, loc_type = 'D')
         self.assertEqual(len(district),1)
         
     def test_allowed_location(self):
-        allowed = LocationManager().allowed(self.test_user.id, loc_types = ['R','D','W'])
+        allowed = LocationManager().allowed(self.test_user.id, loc_types = ['R','D','W'], qs = True)
         self.assertEqual(len(allowed),3)
 
         other = create_test_location('D',  custom_props={'parent':self.test_village.parent.parent.parent, 'code':'NOTALLO'})
-        allowed = LocationManager().allowed(self.test_user.id, loc_types = ['R','D','W'])
+        allowed = LocationManager().allowed(self.test_user.id, loc_types = ['R','D','W'],qs = True)
         self.assertEqual(len(allowed),2)
```

### Comparing `openimis-be-location-1.6.1rc1/openimis_be_location.egg-info/PKG-INFO` & `openimis_be_location-1.7.0/openimis_be_location.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-location
-Version: 1.6.1rc1
+Version: 1.7.0
 Summary: The openIMIS Backend Location reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-location-1.6.1rc1/openimis_be_location.egg-info/SOURCES.txt` & `openimis_be_location-1.7.0/openimis_be_location.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.6.1rc1/setup.py` & `openimis_be_location-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-location',
-    version='v1.6.1-rc.1',
+    version='v1.7.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Location reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
```

