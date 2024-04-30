# Comparing `tmp/openimis-be-medical-1.6.0.tar.gz` & `tmp/openimis_be_medical-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-medical-1.6.0.tar", last modified: Sat Dec 16 00:56:19 2023, max compression
+gzip compressed data, was "openimis_be_medical-1.7.0.tar", last modified: Tue Apr 30 09:00:45 2024, max compression
```

## Comparing `openimis-be-medical-1.6.0.tar` & `openimis_be_medical-1.7.0.tar`

### file list

```diff
@@ -1,34 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:19.887917 openimis-be-medical-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      778 2023-12-16 00:56:19.887917 openimis-be-medical-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:19.883917 openimis-be-medical-1.6.0/medical/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/medical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/medical/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/medical/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/medical/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11108 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/medical/gql_mutations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:19.883917 openimis-be-medical-1.6.0/medical/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/medical/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/medical/migrations/0002_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/medical/migrations/0003_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/medical/migrations/0004_add_missing_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/medical/migrations/0005_set_managed_to_true.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/medical/migrations/0006_auto_20230718_1332.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/medical/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11983 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/medical/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8827 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/medical/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/medical/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/medical/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17780 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/medical/tests_api.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/medical/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:56:11.000000 openimis-be-medical-1.6.0/medical/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:19.887917 openimis-be-medical-1.6.0/openimis_be_medical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2023-12-16 00:56:19.000000 openimis-be-medical-1.6.0/openimis_be_medical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-16 00:56:19.000000 openimis-be-medical-1.6.0/openimis_be_medical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:56:19.000000 openimis-be-medical-1.6.0/openimis_be_medical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-16 00:56:19.000000 openimis-be-medical-1.6.0/openimis_be_medical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-16 00:56:19.000000 openimis-be-medical-1.6.0/openimis_be_medical.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:56:19.887917 openimis-be-medical-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2023-12-16 00:56:19.000000 openimis-be-medical-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:45.944982 openimis_be_medical-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-30 09:00:45.944982 openimis_be_medical-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:45.940982 openimis_be_medical-1.7.0/medical/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:45.944982 openimis_be_medical-1.7.0/medical/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/migrations/0002_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/migrations/0003_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/migrations/0004_add_missing_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/migrations/0005_set_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/migrations/0006_auto_20230718_1332.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/migrations/0007_alter_item_maximum_amount_alter_item_quantity_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/migrations/0008_auto_20220804_1112.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/migrations/0009_alter_service_patient_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8395 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19965 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/tests_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:00:37.000000 openimis_be_medical-1.7.0/medical/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:45.944982 openimis_be_medical-1.7.0/openimis_be_medical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-30 09:00:45.000000 openimis_be_medical-1.7.0/openimis_be_medical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-30 09:00:45.000000 openimis_be_medical-1.7.0/openimis_be_medical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:00:45.000000 openimis_be_medical-1.7.0/openimis_be_medical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-30 09:00:45.000000 openimis_be_medical-1.7.0/openimis_be_medical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 09:00:45.000000 openimis_be_medical-1.7.0/openimis_be_medical.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:00:45.944982 openimis_be_medical-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-30 09:00:45.000000 openimis_be_medical-1.7.0/setup.py
```

### Comparing `openimis-be-medical-1.6.0/LICENSE.md` & `openimis_be_medical-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-medical-1.6.0/PKG-INFO` & `openimis_be_medical-1.7.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-medical
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Medical reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-medical-1.6.0/README.md` & `openimis_be_medical-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-medical-1.6.0/medical/apps.py` & `openimis_be_medical-1.7.0/medical/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical-1.6.0/medical/migrations/0001_initial.py` & `openimis_be_medical-1.7.0/medical/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical-1.6.0/medical/migrations/0002_diagnosis.py` & `openimis_be_medical-1.7.0/medical/migrations/0002_diagnosis.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical-1.6.0/medical/migrations/0003_mutations.py` & `openimis_be_medical-1.7.0/medical/migrations/0003_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical-1.6.0/medical/migrations/0004_add_missing_fields.py` & `openimis_be_medical-1.7.0/medical/migrations/0004_add_missing_fields.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical-1.6.0/medical/migrations/0005_set_managed_to_true.py` & `openimis_be_medical-1.7.0/medical/migrations/0005_set_managed_to_true.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical-1.6.0/medical/migrations/0006_auto_20230718_1332.py` & `openimis_be_medical-1.7.0/medical/migrations/0006_auto_20230718_1332.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical-1.6.0/medical/models.py` & `openimis_be_medical-1.7.0/medical/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import string
 import uuid
 
 from core.models import VersionedModel, ObjectMutation
 from django.db import models
+from django.utils import timezone as django_tz 
 from core import models as core_models
 from django.db.models.signals import pre_save
 from django.dispatch import receiver
 from graphql import ResolveInfo
 from django.conf import settings
 import core
 from medical.apps import MedicalConfig
@@ -58,16 +60,16 @@
     id = models.AutoField(db_column='ItemID', primary_key=True)
     uuid = models.CharField(db_column='ItemUUID', max_length=36, default=uuid.uuid4, unique=True)
     code = models.CharField(db_column='ItemCode', max_length=6)
     name = models.CharField(db_column='ItemName', max_length=100)
     type = models.CharField(db_column='ItemType', max_length=1)
     package = models.CharField(db_column='ItemPackage', max_length=255, blank=True, null=True)
     price = models.DecimalField(db_column='ItemPrice', max_digits=18, decimal_places=2)
-    quantity = models.DecimalField(db_column='Quantity', max_digits=18, decimal_places=2, null=True)
-    maximum_amount = models.DecimalField(db_column='MaximumAmount', max_digits=18, decimal_places=2, null=True)
+    quantity = models.DecimalField(db_column='Quantity', max_digits=18, decimal_places=2,blank = True, null=True)
+    maximum_amount = models.DecimalField(db_column='MaximumAmount', max_digits=18, decimal_places=2,blank=True, null=True)
     care_type = models.CharField(db_column='ItemCareType', max_length=1)
     frequency = models.SmallIntegerField(db_column='ItemFrequency', blank=True, null=True)
     patient_category = models.SmallIntegerField(db_column='ItemPatCat')
     audit_user_id = models.IntegerField(db_column='AuditUserID')
     # row_id = models.BinaryField(db_column='RowID', blank=True, null=True)
 
     def __bool__(self):
@@ -150,30 +152,39 @@
     if instance != old_instance:
         # One or more fields have changed, so save history
         old_instance.save_history()
         from core import datetime
         now = datetime.datetime.now()
         instance.validity_from = now
 
+class PackageTypes(models.TextChoices):
+    P = "P", "P"
+    S = "S", "S"
+    F = "F", "F"
 
 class Service(VersionedModel, ItemOrService):
+
+    DEFAULT_PATIENT_CATEGORY = 15
+
     id = models.AutoField(db_column='ServiceID', primary_key=True)
     uuid = models.CharField(db_column='ServiceUUID',
                             max_length=36, default=uuid.uuid4, unique=True)
     # legacy_id = models.IntegerField(db_column='LegacyID', blank=True, null=True)
     category = models.CharField(db_column='ServCategory', max_length=1, blank=True, null=True)
     code = models.CharField(db_column='ServCode', max_length=6)
     name = models.CharField(db_column='ServName', max_length=100)
     type = models.CharField(db_column='ServType', max_length=1)
+    packagetype = models.CharField(db_column='ServPackageType', choices=PackageTypes.choices, max_length=1, default=PackageTypes.S)
+    manualPrice = models.BooleanField(default=False)
     level = models.CharField(db_column='ServLevel', max_length=1)
     price = models.DecimalField(db_column='ServPrice', max_digits=18, decimal_places=2)
-    maximum_amount = models.DecimalField(db_column='MaximumAmount', max_digits=18, decimal_places=2, null=True)
+    maximum_amount = models.DecimalField(db_column='MaximumAmount', max_digits=18, decimal_places=2, blank=True, null=True)
     care_type = models.CharField(db_column='ServCareType', max_length=1)
     frequency = models.SmallIntegerField(db_column='ServFrequency', blank=True, null=True)
-    patient_category = models.SmallIntegerField(db_column='ServPatCat')
+    patient_category = models.SmallIntegerField(db_column='ServPatCat', default=DEFAULT_PATIENT_CATEGORY)
 
     # validity_from = fields.DateTimeField(db_column='ValidityFrom', blank=True, null=True)
     # validity_to = fields.DateTimeField(db_column='ValidityTo', blank=True, null=True)
     audit_user_id = models.IntegerField(db_column='AuditUserID', blank=True, null=True)
     # row_id = models.BinaryField(db_column='RowID', blank=True, null=True)
 
     def __bool__(self):
@@ -274,23 +285,63 @@
         # One or more fields have changed, so save history
         old_instance.save_history()
         from core import datetime
         now = datetime.datetime.now()
         instance.validity_from = now
 
 
-class ItemMutation(core_models.UUIDModel, ObjectMutation):
+class ServiceService(models.Model):
+    """class representing relation between package and services """
+    id = models.AutoField(primary_key=True, db_column='idSCP')
+    service = models.ForeignKey(Service, models.DO_NOTHING,
+                              db_column='ServiceId', related_name='servicesServices')
+    servicelinkedService = models.ForeignKey( Service,
+                                          models.DO_NOTHING, db_column="ServiceLinked")
+    qty_provided = models.IntegerField(db_column="qty",
+                                      blank=True, null=True)
+    scpDate = models.DateTimeField(db_column="created_date", default=django_tz.now,
+                                   blank=True, null=True)
+    price_asked = models.DecimalField(db_column="price",
+                                   max_digits=18, decimal_places=2, blank=True, null=True)
+    status = models.BooleanField(default=True)
+
+    class Meta:
+        managed = True
+        db_table = 'tblServiceContainedPackage'
+
+
+class ServiceItem(models.Model):
+    """class representing relation between package and product """
+    id = models.AutoField(primary_key=True, db_column='idPCP')
+    item = models.ForeignKey(Item, models.DO_NOTHING, db_column='ItemID', related_name="itemsServices")                           
+    servicelinkedItem = models.ForeignKey( Service,
+                                          models.DO_NOTHING, db_column="ServiceID",related_name='servicesLinked')
+    qty_provided = models.IntegerField(db_column="qty",
+                                      blank=True, null=True)
+    pcpDate = models.DateTimeField(db_column="created_date", default=django_tz.now,
+                                   blank=True, null=True)
+    price_asked = models.DecimalField(db_column="price",
+                                   max_digits=18, decimal_places=2, blank=True, null=True)
+    status = models.BooleanField(default=True)
+    
+    class Meta:
+        managed = True
+        db_table = 'tblProductContainedPackage'
+
+
+
+class ItemMutation(core_models.UUIDModel, core_models.ObjectMutation):
     item = models.ForeignKey(Item, models.DO_NOTHING, related_name='mutations')
     mutation = models.ForeignKey(core_models.MutationLog, models.DO_NOTHING, related_name='items')
 
     class Meta:
         managed = True
         db_table = "medical_ItemMutation"
 
 
-class ServiceMutation(core_models.UUIDModel, ObjectMutation):
+class ServiceMutation(core_models.UUIDModel, core_models.ObjectMutation):
     service = models.ForeignKey(Service, models.DO_NOTHING, related_name='mutations')
     mutation = models.ForeignKey(core_models.MutationLog, models.DO_NOTHING, related_name='services')
 
     class Meta:
         managed = True
         db_table = "medical_ServiceMutation"
```

### Comparing `openimis-be-medical-1.6.0/medical/schema.py` & `openimis_be_medical-1.7.0/medical/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from django.core.exceptions import PermissionDenied
 from django.db.models import Q
 from django.utils.translation import gettext as _
 from graphene_django import DjangoObjectType
 from graphene_django.filter import DjangoFilterConnectionField
 from medical.gql_mutations import CreateServiceMutation, UpdateServiceMutation, DeleteServiceMutation, \
     CreateItemMutation, UpdateItemMutation, DeleteItemMutation
+from .gql_queries import *
 
 from .apps import MedicalConfig
 from .models import Diagnosis, Item, Service
 import graphene_django_optimizer as gql_optimizer
 from .services import check_unique_code_item, check_unique_code_service
 
 
@@ -38,29 +39,14 @@
             'name': ['exact', 'icontains', 'istartswith'],
             'package': ['exact', 'icontains', 'istartswith'],
             'type': ['exact'],
         }
         connection_class = ExtendedConnection
 
 
-class ServiceGQLType(DjangoObjectType):
-    class Meta:
-        model = Service
-        interfaces = (graphene.relay.Node,)
-        filter_fields = {
-            'uuid': ['exact'],
-            'code': ['exact', 'icontains', 'istartswith'],
-            'name': ['exact', 'icontains', 'istartswith'],
-            'type': ['exact'],
-            'care_type': ['exact'],
-            'category': ['exact'],
-        }
-        connection_class = ExtendedConnection
-
-
 class Query(graphene.ObjectType):
     diagnoses = DjangoFilterConnectionField(DiagnosisGQLType)
     diagnoses_str = DjangoFilterConnectionField(
         DiagnosisGQLType,
         str=graphene.String()
     )
     medical_items = OrderedDjangoFilterConnectionField(
```

### Comparing `openimis-be-medical-1.6.0/medical/services.py` & `openimis_be_medical-1.7.0/medical/services.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical-1.6.0/medical/test_helpers.py` & `openimis_be_medical-1.7.0/medical/test_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 def get_item_of_type(item_type, valid=True):
     return Item.objects.filter(type=item_type).filter(validity_to__isnull=valid).first()
 
 
 def create_test_service(category, valid=True, custom_props={}):
     return Service.objects.create(
         **{
+            "maximum_amount":5000,
             "code": "TST-" + category,
             "category": category,
             "name": "Test service " + category,
             "type": Service.TYPE_CURATIVE,
             "level": 1,
             "price": 100,
             "patient_category": 15,
@@ -27,14 +28,16 @@
         }
     )
 
 
 def create_test_item(item_type, valid=True, custom_props=None):
     return Item.objects.create(
         **{
+            "quantity":1,
+            "maximum_amount":225000,
             "code": "XXX",
             "type": item_type,
             "name": "Test item",
             "price": 100,
             "patient_category": 15,
             "care_type": 1,
             "validity_from": "2019-06-01",
```

### Comparing `openimis-be-medical-1.6.0/medical/tests_api.py` & `openimis_be_medical-1.7.0/medical/tests_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from dataclasses import dataclass
 
 from core.models import User
 from core.test_helpers import create_test_interactive_user
 from django.conf import settings
 from graphene_django.utils.testing import GraphQLTestCase
 from graphql_jwt.shortcuts import get_token
-from medical.models import Item
+from medical.models import Item, ServiceItem, ServiceService
 from medical.test_helpers import create_test_item, create_test_service
+from medical.utils import item_create_hook, service_create_hook
 from rest_framework import status
 
 # from openIMIS import schema
 
 
 @dataclass
 class DummyContext:
@@ -190,15 +191,15 @@
         query = 'query { medicalServices(showHistory: true, code:"M1") { edges { node { id name } } } }'
         response = self.query(query, headers={"HTTP_AUTHORIZATION": f"{self.AUTH_HEADER} {self.noright_token}"})
         response_admin = self.query(query, headers={"HTTP_AUTHORIZATION": f"{self.AUTH_HEADER} {self.admin_token}"})
 
         content = json.loads(response.content)
         content_admin = json.loads(response_admin.content)
         self.assertEqual(len(content["data"]["medicalServices"]["edges"]), 1)
-        self.assertEqual(len(content_admin["data"]["medicalServices"]["edges"]), 2)
+        self.assertEqual(len(content_admin["data"]["medicalServices"]["edges"]), 1)
 
     def test_no_right_items_query(self):
         """
         Query with a valid token but not the right to perform this full operation.
         Unlike some other modules, medical services and items are available to everyone but limited,
         i.e. no showHistory so we're accessing a modified service and make sure that history is not available.
         """
@@ -279,15 +280,17 @@
         response = self.query(
             '''
             mutation {
               createItem(input: {
                 clientMutationId: "testapi2"
                 code: "TSTAPI"
                 name: "Auto test of create API"
-                type: "D"
+                type: "D",
+                maximumAmount: "225000.0",
+                quantity: "2.0"
                 careType: "B"
                 patientCategory: 11
                 price: "321"
                 package: "box of 1"
               }) {
                 internalId
                 clientMutationId
@@ -324,15 +327,16 @@
               updateItem(input: {
                 clientMutationId: "testapi4"
                 uuid: "%s"
                 code: "SVCAX4"
                 name: "New name"
                 type: "D"
                 careType: "O"
-                patientCategory: 5
+                patientCategory: 5,
+                quantity: "1.0"
                 price: "555"
                 package: "box of 12"
               }) {
                 internalId
                 clientMutationId
               }
             }
@@ -365,14 +369,16 @@
                 code: "SVCAX4"
                 name: "New name"
                 type: "A"
                 level: "H"
                 careType: "O"
                 patientCategory: 5
                 price: "555"
+                manualPrice: "0"
+                packagetype: "S"
               }) {
                 internalId
                 clientMutationId
               }
             }
             ''' % self.test_service_update.uuid,
             headers={"HTTP_AUTHORIZATION": f"{self.AUTH_HEADER} {self.admin_token}"},
@@ -440,7 +446,58 @@
 
         self.assertResponseNoErrors(response)
         self.assertEqual(content["data"]["deleteItem"]["clientMutationId"], "testapi5")
 
         self.test_item_delete.refresh_from_db()
 
         self.assertIsNotNone(self.test_item_delete.validity_to)
+
+    def test_process_child_relation(self):
+        self.query(
+            '''
+            mutation {
+              updateService(input: {
+                clientMutationId: "testapi4"
+                uuid: "%s"
+                code: "SVCAX4"
+                name: "New name"
+                type: "A"
+                level: "H"
+                careType: "O"
+                patientCategory: 5
+                price: "555"
+                manualPrice: "0"
+                packagetype: "S"
+                services:  [
+                    {
+                        serviceId: %s,
+                        priceAsked: "600.00",
+                        qtyProvided: "1.00",
+                        status: 1
+                    }
+                ]
+                items:  [
+                    {
+                        itemId: %s,
+                        priceAsked: "1200.00",
+                        qtyProvided: "800.00",
+                        status: 1
+                    }
+                ]
+              }) {
+                internalId
+                clientMutationId
+              }
+            }
+            ''' % (self.test_service_update.uuid, self.test_service.id, self.test_item.id),
+            headers={"HTTP_AUTHORIZATION": f"{self.AUTH_HEADER} {self.admin_token}"},
+        )
+        self.test_service_update.refresh_from_db()
+        serv_item = ServiceItem.objects.filter(servicelinkedItem=self.test_service_update.id).first()
+        self.assertEquals(serv_item.price_asked, 1200)
+        self.assertEquals(serv_item.qty_provided, 800)
+        self.assertEquals(serv_item.item.id, self.test_item.id)
+
+        service_serv = ServiceService.objects.filter(servicelinkedService=self.test_service_update.id).first()
+        self.assertEquals(service_serv.price_asked, 600)
+        self.assertEquals(service_serv.qty_provided, 1)
+        self.assertEquals(service_serv.service.id, self.test_service.id)
```

### Comparing `openimis-be-medical-1.6.0/openimis_be_medical.egg-info/PKG-INFO` & `openimis_be_medical-1.7.0/openimis_be_medical.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-medical
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Medical reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-medical-1.6.0/openimis_be_medical.egg-info/SOURCES.txt` & `openimis_be_medical-1.7.0/openimis_be_medical.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,31 @@
 README.md
 setup.py
 medical/__init__.py
 medical/admin.py
 medical/apps.py
 medical/exceptions.py
 medical/gql_mutations.py
+medical/gql_queries.py
 medical/models.py
 medical/schema.py
 medical/services.py
 medical/test_helpers.py
 medical/tests_api.py
 medical/urls.py
+medical/utils.py
 medical/views.py
 medical/migrations/0001_initial.py
 medical/migrations/0002_diagnosis.py
 medical/migrations/0003_mutations.py
 medical/migrations/0004_add_missing_fields.py
 medical/migrations/0005_set_managed_to_true.py
 medical/migrations/0006_auto_20230718_1332.py
+medical/migrations/0007_alter_item_maximum_amount_alter_item_quantity_and_more.py
+medical/migrations/0008_auto_20220804_1112.py
+medical/migrations/0009_alter_service_patient_category.py
 medical/migrations/__init__.py
 openimis_be_medical.egg-info/PKG-INFO
 openimis_be_medical.egg-info/SOURCES.txt
 openimis_be_medical.egg-info/dependency_links.txt
 openimis_be_medical.egg-info/requires.txt
 openimis_be_medical.egg-info/top_level.txt
```

### Comparing `openimis-be-medical-1.6.0/setup.py` & `openimis_be_medical-1.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-medical',
-    version='v1.6.0',
+    version='v1.7.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Medical reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
```

