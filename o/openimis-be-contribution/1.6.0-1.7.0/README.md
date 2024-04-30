# Comparing `tmp/openimis-be-contribution-1.6.0.tar.gz` & `tmp/openimis_be_contribution-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-contribution-1.6.0.tar", last modified: Sat Dec 16 00:57:06 2023, max compression
+gzip compressed data, was "openimis_be_contribution-1.7.0.tar", last modified: Tue Apr 30 09:05:36 2024, max compression
```

## Comparing `openimis-be-contribution-1.6.0.tar` & `openimis_be_contribution-1.7.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:06.460407 openimis-be-contribution-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      849 2023-12-16 00:57:06.460407 openimis-be-contribution-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:06.456407 openimis-be-contribution-1.6.0/contribution/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     7278 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:06.456407 openimis-be-contribution-1.6.0/contribution/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/migrations/0002_add_premium_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/migrations/0003_alter_premium_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/migrations/0004_auto_20230718_1155.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/migrations/0005_alter_created_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/migrations/0006_add_source_field_to_contribution.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/migrations/0007_add_missing_fields_not_mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:06.456407 openimis-be-contribution-1.6.0/contribution/reports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   170318 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/reports/contributions_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)   201501 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/reports/payment_category_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)   191164 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/reports/premium_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9750 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/services.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7947 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/tests_gql.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-16 00:56:48.000000 openimis-be-contribution-1.6.0/contribution/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:06.460407 openimis-be-contribution-1.6.0/openimis_be_contribution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2023-12-16 00:57:06.000000 openimis-be-contribution-1.6.0/openimis_be_contribution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2023-12-16 00:57:06.000000 openimis-be-contribution-1.6.0/openimis_be_contribution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:57:06.000000 openimis-be-contribution-1.6.0/openimis_be_contribution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-16 00:57:06.000000 openimis-be-contribution-1.6.0/openimis_be_contribution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-16 00:57:06.000000 openimis-be-contribution-1.6.0/openimis_be_contribution.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:57:06.460407 openimis-be-contribution-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2023-12-16 00:57:05.000000 openimis-be-contribution-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:36.062520 openimis_be_contribution-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-30 09:05:36.062520 openimis_be_contribution-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:36.058520 openimis_be_contribution-1.7.0/contribution/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:36.058520 openimis_be_contribution-1.7.0/contribution/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/migrations/0002_add_premium_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/migrations/0003_alter_premium_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/migrations/0004_auto_20230718_1155.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/migrations/0005_alter_created_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/migrations/0006_add_source_field_to_contribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/migrations/0007_add_missing_fields_not_mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:36.058520 openimis_be_contribution-1.7.0/contribution/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   170318 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/reports/contributions_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   201501 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/reports/payment_category_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)   191164 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/reports/premium_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/tests_gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 09:05:25.000000 openimis_be_contribution-1.7.0/contribution/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:36.062520 openimis_be_contribution-1.7.0/openimis_be_contribution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-30 09:05:36.000000 openimis_be_contribution-1.7.0/openimis_be_contribution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-30 09:05:36.000000 openimis_be_contribution-1.7.0/openimis_be_contribution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:05:36.000000 openimis_be_contribution-1.7.0/openimis_be_contribution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-30 09:05:36.000000 openimis_be_contribution-1.7.0/openimis_be_contribution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 09:05:36.000000 openimis_be_contribution-1.7.0/openimis_be_contribution.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:05:36.062520 openimis_be_contribution-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-30 09:05:35.000000 openimis_be_contribution-1.7.0/setup.py
```

### Comparing `openimis-be-contribution-1.6.0/LICENSE.md` & `openimis_be_contribution-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/README.md` & `openimis_be_contribution-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/contribution/apps.py` & `openimis_be_contribution-1.7.0/contribution/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/contribution/gql_mutations.py` & `openimis_be_contribution-1.7.0/contribution/gql_mutations.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,14 @@
     premium.pay_type = None
     premium.is_photo_fee = None
     premium.is_offline = None
     premium.reporting_id = None
 
 
 def premium_action(data, user):
-
-
     if "client_mutation_id" in data:
         data.pop('client_mutation_id')
     if "client_mutation_label" in data:
         data.pop('client_mutation_label')
     now = datetime.datetime.now()
     data['audit_user_id'] = user.id_for_audit
     data['validity_from'] = now
```

### Comparing `openimis-be-contribution-1.6.0/contribution/gql_queries.py` & `openimis_be_contribution-1.7.0/contribution/gql_queries.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/contribution/migrations/0001_initial.py` & `openimis_be_contribution-1.7.0/contribution/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/contribution/migrations/0002_add_premium_fields.py` & `openimis_be_contribution-1.7.0/contribution/migrations/0002_add_premium_fields.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/contribution/migrations/0004_auto_20230718_1155.py` & `openimis_be_contribution-1.7.0/contribution/migrations/0004_auto_20230718_1155.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/contribution/migrations/0005_alter_created_date.py` & `openimis_be_contribution-1.7.0/contribution/migrations/0005_alter_created_date.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/contribution/migrations/0006_add_source_field_to_contribution.py` & `openimis_be_contribution-1.7.0/contribution/migrations/0006_add_source_field_to_contribution.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/contribution/migrations/0007_add_missing_fields_not_mssql.py` & `openimis_be_contribution-1.7.0/contribution/migrations/0007_add_missing_fields_not_mssql.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/contribution/models.py` & `openimis_be_contribution-1.7.0/contribution/models.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/contribution/report.py` & `openimis_be_contribution-1.7.0/contribution/report.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/contribution/reports/contributions_distribution.py` & `openimis_be_contribution-1.7.0/contribution/reports/contributions_distribution.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/contribution/reports/payment_category_overview.py` & `openimis_be_contribution-1.7.0/contribution/reports/payment_category_overview.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/contribution/reports/premium_collection.py` & `openimis_be_contribution-1.7.0/contribution/reports/premium_collection.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/contribution/schema.py` & `openimis_be_contribution-1.7.0/contribution/schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/contribution/services.py` & `openimis_be_contribution-1.7.0/contribution/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 from enum import Enum
 from core.models import filter_validity
 from core.datetimes.shared import datetimedelta
 from django.db.models import Sum, Q
+from django.core.exceptions import ValidationError
+from django.utils.translation import gettext as _
 from django.db.transaction import atomic
 from insuree.models import Insuree, Family, InsureePolicy
 from location.apps import LocationConfig
 from location.models import Location
 from policy.models import Policy
 from policy.services import policy_status_premium_paid
 
@@ -261,36 +263,34 @@
         policy = Policy.objects.select_related('product').filter(uuid=policy_uuid, validity_to__isnull=True).first()
     exists = Premium.objects.filter(policy__product=policy.product, receipt=code, validity_to__isnull=True).exists()
     if exists:
         return [{"message": "Premium code %s already exists" % code}]
     return []
 
 
-def update_or_create_premium(premium, user, action = None):
-    
-    existing_premium = Premium.objects.filter(*filter_validity(),Q(Q(uuid=premium.uuid) |Q(id = premium.id)) ).first()
+def update_or_create_premium(premium, user, action=None):
+    existing_premium = Premium.objects.filter(*filter_validity(), Q(Q(uuid=premium.uuid) | Q(id=premium.id))).first()
     if existing_premium:
         return update_premium(existing_premium, premium, user, action)
     else:  
         return create_premium(premium, user, action)
-        
-def  update_premium(existing_premium, premium, user, action = None):     
+
+
+def update_premium(existing_premium, premium, user, action = None):
     if existing_premium.receipt != premium.receipt:
         if check_unique_premium_receipt_code_within_product(code=premium.receipt, policy=premium.policy):
-            raise ValidationError(
-                _("mutation.code_already_taken"))
+            raise ValidationError(_("mutation.code_already_taken"))
     existing_premium.save_history()
     premium.id = existing_premium.id
     premium.save()
     # Handle the policy updating
     premium_updated(premium, action)
     return premium
 
 
-def  create_premium(premium, user, action = None):     
+def create_premium(premium, user, action = None):
     if check_unique_premium_receipt_code_within_product(code=premium.receipt, policy=premium.policy):
-        raise ValidationError(
-            _("mutation.code_already_taken"))
+        raise ValidationError(_("mutation.code_already_taken"))
     premium.save()
     # Handle the policy updating
     premium_updated(premium, action)
     return premium
```

### Comparing `openimis-be-contribution-1.6.0/contribution/test_helpers.py` & `openimis_be_contribution-1.7.0/contribution/test_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/contribution/tests.py` & `openimis_be_contribution-1.7.0/contribution/tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/contribution/tests_gql.py` & `openimis_be_contribution-1.7.0/contribution/tests_gql.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         cls.ca_user = create_test_interactive_user(username="testLocationNoRight", roles=[9])
         cls.ca_token = get_token(cls.ca_user, DummyContext(user=cls.ca_user))
         cls.admin_dist_user = create_test_interactive_user(username="testLocationDist")
         assign_user_districts(cls.admin_dist_user, ["R1D1", "R2D1", "R2D2", "R2D1", cls.test_village.parent.parent.code])
         cls.admin_dist_token = get_token(cls.admin_dist_user, DummyContext(user=cls.admin_dist_user))
         cls.payer = Payer.objects.filter(*filter_validity()).first()
         cls.product = Product.objects.filter(*filter_validity()).first()
-        cls.policy = create_test_policy(cls.product, cls.test_insuree, custom_props={'value':1000}, link=True, valid=True, check=False)
+        cls.policy = create_test_policy(cls.product, cls.test_insuree, custom_props={'value':1000}, link=True, valid=True)
 
 
         
     def test_add_funding(self):
       
         response = self.query(
       f'''
```

### Comparing `openimis-be-contribution-1.6.0/contribution/utils.py` & `openimis_be_contribution-1.7.0/contribution/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/openimis_be_contribution.egg-info/SOURCES.txt` & `openimis_be_contribution-1.7.0/openimis_be_contribution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.6.0/setup.py` & `openimis_be_contribution-1.7.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-contribution',
-    version='v1.6.0',
+    version='v1.7.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Policy reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
```

