# Comparing `tmp/openimis-be-policy-1.6.0.tar.gz` & `tmp/openimis_be_policy-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-policy-1.6.0.tar", last modified: Sat Dec 16 00:56:45 2023, max compression
+gzip compressed data, was "openimis_be_policy-1.7.0.tar", last modified: Tue Apr 30 09:05:25 2024, max compression
```

## Comparing `openimis-be-policy-1.6.0.tar` & `openimis_be_policy-1.7.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:45.445408 openimis-be-policy-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      879 2023-12-16 00:56:45.445408 openimis-be-policy-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:45.445408 openimis-be-policy-1.6.0/openimis_be_policy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      879 2023-12-16 00:56:45.000000 openimis-be-policy-1.6.0/openimis_be_policy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-16 00:56:45.000000 openimis-be-policy-1.6.0/openimis_be_policy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:56:45.000000 openimis-be-policy-1.6.0/openimis_be_policy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-16 00:56:45.000000 openimis-be-policy-1.6.0/openimis_be_policy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-16 00:56:45.000000 openimis-be-policy-1.6.0/openimis_be_policy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:45.441408 openimis-be-policy-1.6.0/policy/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:45.441408 openimis-be-policy-1.6.0/policy/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/migrations/0002_policy_renewals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/migrations/0003_auto_20201021_0811.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/migrations/0004_add_medical_oficer_reading_rights.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/migrations/0005_add_foreign_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/migrations/0006_set_model_managed_to_true.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/migrations/0007_fix_policy_mutation_name.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:45.445408 openimis-be-policy-1.6.0/policy/reports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   278609 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/reports/policy_renewals.py
--rw-r--r--   0 runner    (1001) docker     (127)   139214 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/reports/primary_operational_indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)    14724 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    47080 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/services.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    24428 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/test_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/test_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/tests_gql.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/validations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8249 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/values.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-16 00:56:33.000000 openimis-be-policy-1.6.0/policy/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:56:45.445408 openimis-be-policy-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2023-12-16 00:56:45.000000 openimis-be-policy-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:25.870013 openimis_be_policy-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-30 09:05:25.870013 openimis_be_policy-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:25.870013 openimis_be_policy-1.7.0/openimis_be_policy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-30 09:05:25.000000 openimis_be_policy-1.7.0/openimis_be_policy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-30 09:05:25.000000 openimis_be_policy-1.7.0/openimis_be_policy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:05:25.000000 openimis_be_policy-1.7.0/openimis_be_policy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-30 09:05:25.000000 openimis_be_policy-1.7.0/openimis_be_policy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 09:05:25.000000 openimis_be_policy-1.7.0/openimis_be_policy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:25.870013 openimis_be_policy-1.7.0/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:25.870013 openimis_be_policy-1.7.0/policy/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/migrations/0002_policy_renewals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/migrations/0003_auto_20201021_0811.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/migrations/0004_add_medical_oficer_reading_rights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/migrations/0005_add_foreign_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/migrations/0006_set_model_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/migrations/0007_fix_policy_mutation_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:25.870013 openimis_be_policy-1.7.0/policy/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   278609 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/reports/policy_renewals.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139214 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/reports/primary_operational_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14818 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49090 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25145 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/test_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12630 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/tests_gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/values.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 09:05:13.000000 openimis_be_policy-1.7.0/policy/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:05:25.870013 openimis_be_policy-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-30 09:05:25.000000 openimis_be_policy-1.7.0/setup.py
```

### Comparing `openimis-be-policy-1.6.0/LICENSE.md` & `openimis_be_policy-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.6.0/PKG-INFO` & `openimis_be_policy-1.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-policy
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Policy reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-policy-1.6.0/README.md` & `openimis_be_policy-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.6.0/openimis_be_policy.egg-info/PKG-INFO` & `openimis_be_policy-1.7.0/openimis_be_policy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-policy
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Policy reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-policy-1.6.0/openimis_be_policy.egg-info/SOURCES.txt` & `openimis_be_policy-1.7.0/openimis_be_policy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.6.0/policy/apps.py` & `openimis_be_policy-1.7.0/policy/apps.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "policy_renewal_interval": 14,  # Notify renewal nb of days before expiry date
     "policy_location_via": "family",  # ... or product
     "default_eligibility_disabled": False,
     "activation_option": 1,
     "ACTIVATION_OPTION_CONTRIBUTION": 1,
     "CTIVATION_OPTION_PAYMENT": 2,
     "ACTIVATION_OPTION_READY": 3,
+    "contribution_receipt_length": 5
 }
 
 
 class PolicyConfig(AppConfig):
     name = MODULE_NAME
 
     gql_query_policies_perms = []
@@ -40,14 +41,15 @@
     policy_renewal_interval = None
     policy_location_via = None
     default_eligibility_disabled = None
     ACTIVATION_OPTION_CONTRIBUTION = None
     ACTIVATION_OPTION_PAYMENT = None
     ACTIVATION_OPTION_READY = None
     activation_option = None
+    contribution_receipt_length = None
 
     def __load_config(self, cfg):
         for field in cfg:
             if hasattr(PolicyConfig, field):
                 setattr(PolicyConfig, field, cfg[field])
 
     def ready(self):
```

### Comparing `openimis-be-policy-1.6.0/policy/gql_mutations.py` & `openimis_be_policy-1.7.0/policy/gql_mutations.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,17 @@
     enroll_date = graphene.Date(required=True)
     start_date = graphene.Date(required=True)
     expiry_date = graphene.Date(required=True)
     value = graphene.Decimal(max_digits=18, decimal_places=2, required=True)
     product_id = graphene.Int(required=True)
     family_id = graphene.Int(required=True)
     officer_id = graphene.Int(required=True)
+    is_paid = graphene.Boolean(required=False)
+    receipt = graphene.String(required=False)
+    payer_uuid = graphene.String(required=False)
 
 
 class CreateRenewOrUpdatePolicyMutation(OpenIMISMutation):
     @classmethod
     def do_mutate(cls, perms, user, **data):
         if type(user) is AnonymousUser or not user.id:
             raise ValidationError(
```

### Comparing `openimis-be-policy-1.6.0/policy/gql_queries.py` & `openimis_be_policy-1.7.0/policy/gql_queries.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.6.0/policy/migrations/0001_initial.py` & `openimis_be_policy-1.7.0/policy/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.6.0/policy/migrations/0002_policy_renewals.py` & `openimis_be_policy-1.7.0/policy/migrations/0002_policy_renewals.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.6.0/policy/migrations/0003_auto_20201021_0811.py` & `openimis_be_policy-1.7.0/policy/migrations/0003_auto_20201021_0811.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.6.0/policy/migrations/0004_add_medical_oficer_reading_rights.py` & `openimis_be_policy-1.7.0/policy/migrations/0004_add_medical_oficer_reading_rights.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.6.0/policy/migrations/0005_add_foreign_keys.py` & `openimis_be_policy-1.7.0/policy/migrations/0005_add_foreign_keys.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.6.0/policy/models.py` & `openimis_be_policy-1.7.0/policy/models.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.6.0/policy/report.py` & `openimis_be_policy-1.7.0/policy/report.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.6.0/policy/reports/policy_renewals.py` & `openimis_be_policy-1.7.0/policy/reports/policy_renewals.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.6.0/policy/reports/primary_operational_indicators.py` & `openimis_be_policy-1.7.0/policy/reports/primary_operational_indicators.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.6.0/policy/schema.py` & `openimis_be_policy-1.7.0/policy/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     )
     policies_by_family = graphene.relay.ConnectionField(
         PolicyByFamilyOrInsureeConnection,
         family_uuid=graphene.String(required=True),
         active_or_last_expired_only=graphene.Boolean(),
         show_history=graphene.Boolean(),
         order_by=graphene.String(),
+        target_date=graphene.Date(),
     )
     # TODO: refactoring
     # Eligibility is calculated for a Policy... which is bound to a Family (not an Insuree)
     # YET: family member may not be covered by the policy!!
     # This requires to refactor the EligibilityService
     policy_eligibility_by_insuree = graphene.Field(
         EligibilityGQLType,
@@ -214,15 +215,16 @@
         if not info.context.user.has_perms(PolicyConfig.gql_query_policies_by_family_perms):
             raise PermissionDenied(_("unauthorized"))
         req = ByFamilyRequest(
             family_uuid=kwargs.get('family_uuid'),
             active_or_last_expired_only=kwargs.get(
                 'active_or_last_expired_only', False),
             show_history=kwargs.get('show_history', False),
-            order_by=kwargs.get('order_by', None)
+            order_by=kwargs.get('order_by', None),
+            target_date=kwargs.get('target_date', None)
         )
         res = ByFamilyService(user=info.context.user).request(req)
         return [Query._to_policy_by_family_or_insuree_item(x) for x in res.items]
 
     @staticmethod
     def _resolve_policy_eligibility_by_insuree(user, req):
         res = EligibilityService(user=user).request(req)
```

### Comparing `openimis-be-policy-1.6.0/policy/services.py` & `openimis_be_policy-1.7.0/policy/services.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from dataclasses import dataclass
 from datetime import datetime as py_datetime, date as py_date
 
 import core
 from claim.models import ClaimService, Claim, ClaimItem
 from django import dispatch
-from django.core.exceptions import PermissionDenied
+from django.core.exceptions import PermissionDenied, ValidationError
 from django.db import connection
 from django.db.models import Q, Count, Min, Max, Sum, F
 from django.db.models.functions import Coalesce
 from django.template import Template, Context
 from django.utils.translation import gettext as _
 from graphene.utils.str_converters import to_snake_case
 
@@ -39,39 +39,72 @@
 class PolicyService:
     def __init__(self, user):
         self.user = user
 
     @register_service_signal('policy_service.create_or_update')
     def update_or_create(self, data, user):
         policy_uuid = data.get('uuid', None)
+        if 'enroll_date' in data and data['enroll_date'] > py_date.today():
+            raise ValidationError("policy.enroll_date_in_the_future")
         if policy_uuid:
             return self.update_policy(data, user)
         else:
             return self.create_policy(data, user)
 
     @register_service_signal('policy_service.update')
     def update_policy(self, data, user):
+        if "is_paid" in data:
+            data.pop("is_paid")
         data = self._clean_mutation_info(data)
         policy_uuid = data.pop('uuid') if 'uuid' in data else None
         policy = Policy.objects.get(uuid=policy_uuid)
         policy.save_history()
         reset_policy_before_update(policy)
         [setattr(policy, key, data[key]) for key in data]
         policy.save()
         update_insuree_policies(policy, user.id_for_audit)
         return policy
 
     @register_service_signal('policy_service.create')
     def create_policy(self, data, user):
+        is_paid = data.pop("is_paid", False)
+        receipt = data.pop("receipt", None)
+        payer_uuid = data.pop("payer_uuid", None)
         data = self._clean_mutation_info(data)
         policy = Policy.objects.create(**data)
+        if receipt is not None:
+            from contribution.services import check_unique_premium_receipt_code_within_product
+            is_invalid = check_unique_premium_receipt_code_within_product(code=receipt, policy_uuid=policy.uuid)
+            if is_invalid:
+                raise ValidationError("Receipt already exist for a given product.")
+        else:
+            receipt = self.generate_contribution_receipt(policy.product, policy.enroll_date)
         policy.save()
         update_insuree_policies(policy, user.id_for_audit)
+        if is_paid:
+            from contribution.gql_mutations import premium_action
+            premium_data = {"policy_uuid": policy.uuid, "amount": policy.value,
+                            "receipt": receipt, "pay_date": data["enroll_date"], "pay_type": "C"}
+            if payer_uuid is not None:
+                premium_data["payer_uuid"] = payer_uuid
+            premium_action(premium_data, user)
         return policy
 
+    def generate_contribution_receipt(self, product, enroll_date):
+        from contribution.models import Premium
+        code_length = PolicyConfig.contribution_receipt_length
+        if not code_length and type(code_length) is not int:
+            raise ValueError("Invalid config for `generate_contribution_receipt`, expected `code_length` value.")
+        prefix = "RE-" + str(product.code) + "-" + str(enroll_date) + "-"
+        last_contribution = Premium.objects.filter(validity_to__isnull=True, receipt__icontains=prefix)
+        code = 0
+        if last_contribution:
+            code = int(last_contribution.latest('receipt').receipt[-code_length:])
+        return prefix + str(code + 1).zfill(code_length)
+
     def _clean_mutation_info(self, data):
         if "client_mutation_id" in data:
             data.pop('client_mutation_id')
         if "client_mutation_label" in data:
             data.pop('client_mutation_label')
         return data
 
@@ -279,50 +312,46 @@
             .annotate(total_rem_op=Sum('claim_ded_rems__rem_op')) \
             .annotate(total_rem_ip=Sum('claim_ded_rems__rem_ip')) \
             .annotate(total_rem_consult=Sum('claim_ded_rems__rem_consult')) \
             .annotate(total_rem_surgery=Sum('claim_ded_rems__rem_surgery')) \
             .annotate(total_rem_delivery=Sum('claim_ded_rems__rem_delivery')) \
             .annotate(total_rem_hospitalization=Sum('claim_ded_rems__rem_hospitalization')) \
             .annotate(total_rem_antenatal=Sum('claim_ded_rems__rem_antenatal'))
-                
         res.query.group_by = ['id']
+        if hasattr(req, 'chf_id'):
+            res= res.filter(insuree_policies__insuree__chf_id = req.chf_id)
         if not req.show_history:
-            res = res.filter(*core.filter_validity())
+            if req.target_date: 
+                res = res.filter(*core.filter_validity(), expiry_date__gt = req.target_date, effective_date__lte = req.target_date)
+            else:
+                res = res.filter(*core.filter_validity())
         if req.active_or_last_expired_only:
             # sort on status, so that any active policy (status = 2) pops up...
             res = res.annotate(not_null_expiry_date=Coalesce('expiry_date', py_date.max)) \
                 .annotate(not_null_validity_to=Coalesce('validity_to', py_datetime.max)) \
                 .order_by('product__code', 'status', '-not_null_expiry_date', '-not_null_validity_to', '-validity_from')
         return res
 
 
 class ByInsureeService(FilteredPoliciesService):
     def __init__(self, user):
         super(ByInsureeService, self).__init__(user)
 
     def request(self, by_insuree_request):
-        insurees = Insuree.objects.filter(
-            chf_id=by_insuree_request.chf_id,
-            *core.filter_validity() if not by_insuree_request.show_history else []
-        )
         res = self.build_query(by_insuree_request)
-        res = res.prefetch_related('insuree_policies')
-        res = res.filter(insuree_policies__insuree__in=insurees)
-        # .distinct('product__code') >> DISTINCT ON fields not supported by MS-SQL
-        if by_insuree_request.target_date:
-            res = get_queryset_valid_at_date(res, by_insuree_request.target_date)
+        res = res.filter(insuree_policies__insuree__chf_id=by_insuree_request.chf_id)
         if by_insuree_request.active_or_last_expired_only:
             products = {}
-            for r in res:
-                if r.product.code not in products.keys():
-                    products[r.product.code] = r
+            for policy in res:
+                if policy.status == Policy.STATUS_IDLE or policy.status == Policy.STATUS_READY:
+                    products['policy.product.code-%s' % policy.uuid] = policy
+                elif policy.product.code not in products.keys():
+                    products[policy.product.code] = policy
             res = products.values()
-        items = tuple(
-            map(lambda x: FilteredPoliciesService._to_item(x), res)
-        )
+        items = [FilteredPoliciesService._to_item(x) for x in res]
         # possible improvement: sort via the ORM
         # ... but beware of the active_or_last_expired_only filtering!
         order_attr = to_snake_case(by_insuree_request.order_by if by_insuree_request.order_by else "expiry_date")
         desc = False
         if order_attr.startswith('-'):
             order_attr = order_attr[1:]
             desc = True
@@ -332,19 +361,20 @@
             items=items
         )
 
 
 @core.comparable
 class ByFamilyRequest(object):
 
-    def __init__(self, family_uuid, active_or_last_expired_only=False, show_history=False, order_by=None):
+    def __init__(self, family_uuid, active_or_last_expired_only=False, show_history=False, order_by=None, target_date=None):
         self.family_uuid = family_uuid
         self.active_or_last_expired_only = active_or_last_expired_only
         self.show_history = show_history
         self.order_by = order_by
+        self.target_date = target_date
 
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
 
 @core.comparable
 class ByFamilyResponse(object):
@@ -358,17 +388,16 @@
 
 
 class ByFamilyService(FilteredPoliciesService):
     def __init__(self, user):
         super(ByFamilyService, self).__init__(user)
 
     def request(self, by_family_request):
-        family = Family.objects.get(uuid=by_family_request.family_uuid)
         res = self.build_query(by_family_request)
-        res = res.filter(family_id=family.id)
+        res = res.filter(family__uuid=by_family_request.family_uuid)
         # .distinct('product__code') >> DISTINCT ON fields not supported by MS-SQL
         if by_family_request.active_or_last_expired_only:
             products = {}
             for policy in res:
                 if policy.status == Policy.STATUS_IDLE or policy.status == Policy.STATUS_READY:
                     products['policy.product.code-%s' % policy.uuid] = policy
                 elif policy.product.code not in products.keys():
@@ -464,16 +493,16 @@
                f"with item/svc ok {self.is_item_ok}/{self.is_service_ok} " \
                f" left: {self.item_left}/{self.service_left}"
 
     def __repr__(self):
         return self.__str__()
 
 
-signal_eligibility_service_before = dispatch.Signal(providing_args=["user", "request", "response"])
-signal_eligibility_service_after = dispatch.Signal(providing_args=["user", "request", "response"])
+signal_eligibility_service_before = dispatch.Signal(["user", "request", "response"])
+signal_eligibility_service_after = dispatch.Signal(["user", "request", "response"])
 
 
 class EligibilityService(object):
     def __init__(self, user):
         self.user = user
         self.service = NativeEligibilityService(user)
 
@@ -616,15 +645,15 @@
             min_date_all=Min("min_date"),
         )
         from core import datetime
         min_date_item = datetime.date.from_ad_date(min_date_qs["min_date_lte"]
                                                    if min_date_qs["min_date_lte"]
                                                    else min_date_qs["min_date_all"])
 
-        if queryset_item_or_service.filter(min_date__lte=now).filter(left__isnull=True).first():
+        if queryset_item_or_service.filter(min_date__lte=now).filter(left__isnull=True).order_by('-validity_from').first():
             items_or_services_left = None
         else:
             items_or_services_left = queryset_item_or_service\
                 .filter(Q(min_date__isnull=True) | Q(min_date__lte=now))\
                 .aggregate(Max("left"))["left__max"]
 
         return item_or_service_obj, min_date_item, items_or_services_left
@@ -703,14 +732,15 @@
                                                      filter=get_total_filter(Service.CATEGORY_ANTENATAL),
                                                      distinct=True), 0)) \
             .annotate(total_antenatal_left=F("policy__product__max_no_antenatal") - F("total_antenatal")) \
             .annotate(total_visits=Coalesce(Count("insuree__claim",
                                                   filter=get_total_filter(Service.CATEGORY_VISIT),
                                                   distinct=True), 0)) \
             .annotate(total_visits_left=F("policy__product__max_no_visits") - F("total_visits")) \
+            .order_by('-expiry_date')\
             .first()
 
         if result is None:
             eligibility.total_admissions_left = 0
             eligibility.total_consultations_left = 0
             eligibility.total_surgeries_left = 0
             eligibility.total_deliveries_left = 0
```

### Comparing `openimis-be-policy-1.6.0/policy/tasks.py` & `openimis_be_policy-1.7.0/policy/tasks.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.6.0/policy/test_helpers.py` & `openimis_be_policy-1.7.0/policy/test_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from contribution.models import Premium
 from insuree.models import InsureePolicy, Family, Gender, Insuree
+from insuree.test_helpers import create_test_insuree
 from policy.models import Policy
 from policy.values import policy_values
 from product.models import Product
+from core.utils import filter_validity
 import datetime
 
+
 def create_test_policy(product, insuree, link=True, valid=True, custom_props=None, check=False):
     """
     Compatibility method that only return the Policy
     """
     return create_test_policy2(product, insuree, link, valid, custom_props, check)[0]
 
 def dts(s):
@@ -128,41 +131,11 @@
 
     return policy
 
 
 def create_test_insuree_for_policy(with_family=True, is_head=False, custom_props=None, family_custom_props=None):
     # To establish the mandatory reference between "Insuree" and "Family" objects, we can insert the "Family" object
     # with a temporary ID and later update it to associate with the respective "Insuree" object.
-    if with_family:
-        family = Family.objects.create(
-            validity_from="2019-01-01",
-            head_insuree_id=1,  # dummy
-            audit_user_id=-1,
-            **(family_custom_props if family_custom_props else {})
-        )
-    else:
-        family = None
+    insuree=  create_test_insuree(with_family=with_family, is_head=is_head, custom_props=custom_props, family_custom_props=family_custom_props)
 
-    insuree = Insuree.objects.create(
-        **{
-            "last_name": "Test Last",
-            "other_names": "First Second",
-            "chf_id": "chf_dflt",
-            "family": family,
-            "gender": Gender.objects.get(code='M'),
-            "dob": dts("1970-01-01"),
-            "head": is_head,
-            "card_issued": True,
-            "validity_from": dts("2019-01-01"),
-            "audit_user_id": -1,
-            **(custom_props if custom_props else {})
-        }
-    )
-    insuree.save()
-    if with_family:
-        family.head_insuree_id = insuree.id
-        if family_custom_props:
-            for k, v in family_custom_props.items():
-                setattr(family, k, v)
-        family.save()
 
-    return insuree, family
+    return insuree, insuree.family
```

### Comparing `openimis-be-policy-1.6.0/policy/test_services.py` & `openimis_be_policy-1.7.0/policy/test_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from unittest import mock, skip
 
 from claim.test_helpers import create_test_claim, create_test_claimservice, create_test_claimitem
 from claim.validations import validate_claim, validate_assign_prod_to_claimitems_and_services, process_dedrem
 from core.models import InteractiveUser, User
-from core.test_helpers import create_test_officer 
+from core.test_helpers import create_test_officer
 from django.conf import settings
 from django.test import TestCase
 from insuree.test_helpers import create_test_photo
 from medical.test_helpers import create_test_item, create_test_service
 from medical_pricelist.test_helpers import add_service_to_hf_pricelist, add_item_to_hf_pricelist
 from insuree.test_helpers import create_test_insuree
 from policy.test_helpers import create_test_policy2, create_test_insuree_for_policy
 from product.test_helpers import create_test_product, create_test_product_service, create_test_product_item
-
+from location.test_helpers import create_test_health_facility
 from .services import *
-
+from medical_pricelist.test_helpers import (
+    create_test_item_pricelist,
+    create_test_service_pricelist
+)
 
 class EligibilityServiceTestCase(TestCase):
     def setUp(self) -> None:
         super(EligibilityServiceTestCase, self).setUp()
         self.user = mock.Mock(is_anonymous=False)
         self.user.has_perms = mock.MagicMock(return_value=True)
 
@@ -29,14 +32,15 @@
             mock_user.has_perms = mock.MagicMock(return_value=False)
             req = EligibilityRequest(chf_id="a")
             service = EligibilityService(mock_user)
             with self.assertRaises(PermissionDenied) as cm:
                 service.request(req)
             mock_user.has_perms.assert_called_with(PolicyConfig.gql_query_eligibilities_perms)
 
+    @skip("this test hangs on psql, the mock destroys normal queries happening inside EligibilityRequest")
     def test_eligibility_request_all_good(self):
         with mock.patch("django.db.backends.utils.CursorWrapper") as mock_cursor:
             return_values = [
                 list(range(1, 13)),
                 [
                     core.datetime.date(2020, 1, 9),
                     core.datetime.date(2020, 1, 10),
@@ -325,15 +329,20 @@
         item.delete()
         policy.insuree_policies.all().delete()
         policy.delete()
         product.delete()
         insuree.delete()
 
     def test_eligibility_signal(self):
+        
         insuree, family = create_test_insuree_for_policy()
+        #spl = create_test_service_pricelist(location_id=family.location.parent.id)
+        #ipl = create_test_item_pricelist(location_id=family.location.parent.id)
+        #hf =create_test_health_facility(code= 'tst-18', location_id=family.location.parent.id,  custom_props={'id':18, 'items_pricelist': ipl, 'services_pricelist': spl })
+
         product = create_test_product("ELI1")
         (policy, insuree_policy) = create_test_policy2(product, insuree)
         item = create_test_item("A")
         item_pl_detail = add_item_to_hf_pricelist(item)
         product_item = create_test_product_item(product, item, custom_props={"limit_no_adult": 12})
         claim = create_test_claim(custom_props={"insuree_id": insuree.id})
         claim_item = create_test_claimitem(claim, "A", custom_props={"item_id": item.id})
@@ -470,20 +479,19 @@
         family.delete()
 
     def test_renewals_sms(self):
         # Given
         from core import datetime, datetimedelta
 
         insuree, family = create_test_insuree_for_policy(
-            custom_props={"chf_id": "TESTCHFSMS", "phone": "+33644444719"},
-            family_custom_props={"location_id": 62},
-        )
+            custom_props={"chf_id": "TESTCHFSMS", 'last_name':'Test Last',"phone": "+33644444719"}        )
         product = create_test_product("VISIT")
         officer = create_test_officer(
-            custom_props={"phone": "+32444444444", "phone_communication": True}
+            custom_props={"phone": "+32444444444", "phone_communication": True},
+            villages = [family.location]
         )
 
         (policy_expiring, _) = create_test_policy2(
             product=product,
             insuree=insuree,
             custom_props={"expiry_date": "2019-01-01", "officer": officer},
         )
@@ -513,17 +521,17 @@
         self.assertEquals(
             insuree_sms[0].sms_message, "FAMSMS;TESTCHFSMS;Test Last;Test product VISIT"
         )
 
         officer_sms = [sms for sms in sms_queue if sms.phone == "+32444444444"]
         self.assertEquals(len(officer_sms), 1)
         self.assertIn("TESTCHFSMS", officer_sms[0].sms_message)
-        self.assertIn("Agilo", officer_sms[0].sms_message)
-        self.assertIn("Remorlogy", officer_sms[0].sms_message)
-        self.assertIn("Jambero", officer_sms[0].sms_message)
+        self.assertIn(family.location.name, officer_sms[0].sms_message)
+        self.assertIn(family.location.parent.name, officer_sms[0].sms_message)
+        self.assertIn(family.location.parent.parent.name, officer_sms[0].sms_message)
         self.assertIn("Test product VISIT", officer_sms[0].sms_message)
 
         # tearDown
         officer.policy_renewals.all().delete()
         policy_expiring.insuree_policies.all().delete()
         policy_expiring.delete()
         policy_not_expired_yet.insuree_policies.all().delete()
@@ -536,15 +544,15 @@
     def test_insert_renewal_details(self):
         # Given
         from core import datetime, datetimedelta
 
         insuree_newpic, family_newpic = create_test_insuree_for_policy(
             custom_props={"photo_date": datetime.datetime.now() - datetimedelta(days=30)})
         insuree_oldpic, family_oldpic = create_test_insuree_for_policy(
-            custom_props={"photo_date": "2010-01-01", "chf_id": "CHFMARK"})  # 5 years by default
+            custom_props={"photo_date": "2010-01-01", "chf_id": "CHFMARK", 'last_name':'Test Last'})  # 5 years by default
         product = create_test_product("VISIT")
         officer = create_test_officer(custom_props={"phone": "+32444444444", "phone_communication": True})
         photo_newpic = create_test_photo(insuree_newpic.id, officer.id)
         photo_oldpic = create_test_photo(insuree_oldpic.id, officer.id)
 
         (policy_new_pic, inspolicy_new_pic) = create_test_policy2(
             product=product,
```

### Comparing `openimis-be-policy-1.6.0/policy/test_values.py` & `openimis_be_policy-1.7.0/policy/test_values.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.6.0/policy/tests.py` & `openimis_be_policy-1.7.0/policy/tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.6.0/policy/utils.py` & `openimis_be_policy-1.7.0/policy/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.6.0/policy/validations.py` & `openimis_be_policy-1.7.0/policy/validations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.6.0/policy/values.py` & `openimis_be_policy-1.7.0/policy/values.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.6.0/setup.py` & `openimis_be_policy-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-policy',
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

