# Comparing `tmp/openimis-be-product-1.6.0.tar.gz` & `tmp/openimis_be_product-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-product-1.6.0.tar", last modified: Sat Dec 16 00:56:32 2023, max compression
+gzip compressed data, was "openimis_be_product-1.6.1.tar", last modified: Tue Apr 30 09:00:55 2024, max compression
```

## Comparing `openimis-be-product-1.6.0.tar` & `openimis_be_product-1.6.1.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:32.241264 openimis-be-product-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      806 2023-12-16 00:56:32.241264 openimis-be-product-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:32.241264 openimis-be-product-1.6.0/openimis_be_product.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2023-12-16 00:56:32.000000 openimis-be-product-1.6.0/openimis_be_product.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-12-16 00:56:32.000000 openimis-be-product-1.6.0/openimis_be_product.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:56:32.000000 openimis-be-product-1.6.0/openimis_be_product.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-16 00:56:32.000000 openimis-be-product-1.6.0/openimis_be_product.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-16 00:56:32.000000 openimis-be-product-1.6.0/openimis_be_product.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:32.237264 openimis-be-product-1.6.0/product/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    17884 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/gql_mutations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:32.241264 openimis-be-product-1.6.0/product/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    18332 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/migrations/0002_productmutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/migrations/0003_add_enrollment_officer_gql_query_products_perms.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/migrations/0004_alter_product_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/migrations/0005_add_ceiling_type_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/migrations/0006_insert_ceiling_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/migrations/0007_auto_20230510_1347.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/migrations/0008_auto_20230510_1347.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21166 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:32.241264 openimis-be-product-1.6.0/product/reports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   160411 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/reports/product_derived_operational_indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)   187881 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/reports/product_sales.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10102 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-16 00:56:22.000000 openimis-be-product-1.6.0/product/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:56:32.241264 openimis-be-product-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-12-16 00:56:31.000000 openimis-be-product-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:55.090599 openimis_be_product-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-30 09:00:55.090599 openimis_be_product-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:55.086599 openimis_be_product-1.6.1/openimis_be_product.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-30 09:00:55.000000 openimis_be_product-1.6.1/openimis_be_product.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-30 09:00:55.000000 openimis_be_product-1.6.1/openimis_be_product.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:00:55.000000 openimis_be_product-1.6.1/openimis_be_product.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 09:00:55.000000 openimis_be_product-1.6.1/openimis_be_product.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 09:00:55.000000 openimis_be_product-1.6.1/openimis_be_product.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:55.086599 openimis_be_product-1.6.1/product/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17884 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/gql_mutations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:55.086599 openimis_be_product-1.6.1/product/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    18371 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/migrations/0002_productmutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/migrations/0003_add_enrollment_officer_gql_query_products_perms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/migrations/0004_alter_product_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/migrations/0005_add_ceiling_type_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/migrations/0006_insert_ceiling_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/migrations/0007_auto_20230510_1347.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/migrations/0008_auto_20230510_1347.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21166 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:55.086599 openimis_be_product-1.6.1/product/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   160407 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/reports/product_derived_operational_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)   187881 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/reports/product_sales.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:55.086599 openimis_be_product-1.6.1/product/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/tests/tests_gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/tests/tests_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 09:00:47.000000 openimis_be_product-1.6.1/product/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:00:55.090599 openimis_be_product-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-30 09:00:54.000000 openimis_be_product-1.6.1/setup.py
```

### Comparing `openimis-be-product-1.6.0/LICENSE.md` & `openimis_be_product-1.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.6.0/PKG-INFO` & `openimis_be_product-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-product
-Version: 1.6.0
+Version: 1.6.1
 Summary: The openIMIS Backend Product reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-product-1.6.0/README.md` & `openimis_be_product-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.6.0/openimis_be_product.egg-info/PKG-INFO` & `openimis_be_product-1.6.1/openimis_be_product.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-product
-Version: 1.6.0
+Version: 1.6.1
 Summary: The openIMIS Backend Product reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-product-1.6.0/openimis_be_product.egg-info/SOURCES.txt` & `openimis_be_product-1.6.1/openimis_be_product.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 product/enums.py
 product/gql_mutations.py
 product/models.py
 product/report.py
 product/schema.py
 product/services.py
 product/test_helpers.py
-product/tests.py
 product/urls.py
 product/views.py
 product/migrations/0001_initial.py
 product/migrations/0002_productmutation.py
 product/migrations/0003_add_enrollment_officer_gql_query_products_perms.py
 product/migrations/0004_alter_product_options.py
 product/migrations/0005_add_ceiling_type_column.py
 product/migrations/0006_insert_ceiling_type.py
 product/migrations/0007_auto_20230510_1347.py
 product/migrations/0008_auto_20230510_1347.py
 product/migrations/__init__.py
 product/reports/__init__.py
 product/reports/product_derived_operational_indicators.py
-product/reports/product_sales.py
+product/reports/product_sales.py
+product/tests/__init__.py
+product/tests/tests_gql.py
+product/tests/tests_services.py
```

### Comparing `openimis-be-product-1.6.0/product/apps.py` & `openimis_be_product-1.6.1/product/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.6.0/product/enums.py` & `openimis_be_product-1.6.1/product/enums.py`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.6.0/product/gql_mutations.py` & `openimis_be_product-1.6.1/product/gql_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.6.0/product/migrations/0001_initial.py` & `openimis_be_product-1.6.1/product/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
+         ('location', '0001_initial'),
     ]
 
     operations = [
         migrations.CreateModel(
             name='Product',
             fields=[
                 ('validity_from', core.fields.DateTimeField(db_column='ValidityFrom', default=datetime.datetime.now)),
```

### Comparing `openimis-be-product-1.6.0/product/migrations/0002_productmutation.py` & `openimis_be_product-1.6.1/product/migrations/0002_productmutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.6.0/product/migrations/0003_add_enrollment_officer_gql_query_products_perms.py` & `openimis_be_product-1.6.1/product/migrations/0003_add_enrollment_officer_gql_query_products_perms.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,31 +2,34 @@
 
 from django.db import migrations
 from core.models import RoleRight, Role
 
 
 def forwards_func(apps, schema_editor):
     # Add enrollment officer right to read location data
-
     # Enrollment officer is predefined system role with id 1
-    eo_role = Role.objects.filter(is_system=1, validity_to__isnull=True).get()
+    eo_roles = Role.objects.filter(is_system=1, validity_to__isnull=True)
     # Required Role ID is gql_query_products_perm (121001)
     right_id = 121001
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
+        
+        
+
 
 
 def reverse_func(apps, schema_editor):
     # Same data as in forward function
-    eo_role = Role.objects.filter(is_system=1, validity_to__isnull=True).get()
+    eo_roles = Role.objects.filter(is_system=1, validity_to__isnull=True)
     right_id = 121001
-    RoleRight.objects.filter(role_id=eo_role.id, right_id=right_id, validity_to__isnull=True).delete()
+    RoleRight.objects.filter(role__in=eo_roles, right_id=right_id, validity_to__isnull=True).delete()
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ("product", "0002_productmutation"),
     ]
```

### Comparing `openimis-be-product-1.6.0/product/migrations/0005_add_ceiling_type_column.py` & `openimis_be_product-1.6.1/product/migrations/0005_add_ceiling_type_column.py`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.6.0/product/migrations/0006_insert_ceiling_type.py` & `openimis_be_product-1.6.1/product/migrations/0006_insert_ceiling_type.py`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.6.0/product/migrations/0007_auto_20230510_1347.py` & `openimis_be_product-1.6.1/product/migrations/0007_auto_20230510_1347.py`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.6.0/product/models.py` & `openimis_be_product-1.6.1/product/models.py`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.6.0/product/report.py` & `openimis_be_product-1.6.1/product/report.py`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.6.0/product/reports/product_derived_operational_indicators.py` & `openimis_be_product-1.6.1/product/reports/product_derived_operational_indicators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1620,15 +1620,15 @@
                             "borderWidth": 1,
                             "growWeight": 0
                         },
                         {
                             "elementType": "table_text",
                             "id": 628,
                             "width": 130,
-                            "content": "Insurees Per Claim Ratio\n",
+                            "content": "Insurees Per Claim Ratio",
                             "eval": false,
                             "colspan": "",
                             "styleId": "349",
                             "bold": true,
                             "italic": false,
                             "underline": false,
                             "strikethrough": false,
@@ -1680,15 +1680,15 @@
                     "pageBreak": false,
                     "repeatGroupHeader": false,
                     "columnData": [
                         {
                             "elementType": "table_text",
                             "id": 258,
                             "width": 42,
-                            "content": "${product_code} + '-'+ ${product_name} + ' - National' if ${location_type} == 'N' else (${product_code} + ' - '+ ${product_name} + ' in ' + ${location_code} + ' - ' + ${location_name})\n",
+                            "content": "${product_code} + '-'+ ${product_name} + ' - National' if ${location_type} == 'N' else (${product_code} + ' - '+ ${product_name} + ' in ' + ${location_code} + ' - ' + ${location_name})",
                             "eval": true,
                             "colspan": "9",
                             "styleId": "286",
                             "bold": true,
                             "italic": false,
                             "underline": false,
                             "strikethrough": false,
```

### Comparing `openimis-be-product-1.6.0/product/reports/product_sales.py` & `openimis_be_product-1.6.1/product/reports/product_sales.py`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.6.0/product/schema.py` & `openimis_be_product-1.6.1/product/schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.6.0/product/services.py` & `openimis_be_product-1.6.1/product/services.py`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.6.0/product/test_helpers.py` & `openimis_be_product-1.6.1/product/test_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.6.0/product/tests.py` & `openimis_be_product-1.6.1/product/tests/tests_services.py`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.6.0/setup.py` & `openimis_be_product-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-product',
-    version='v1.6.0',
+    version='v1.6.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Product reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
```

