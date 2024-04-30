# Comparing `tmp/openimis-be-payment_cycle-1.0.0.tar.gz` & `tmp/openimis_be_payment_cycle-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-payment_cycle-1.0.0.tar", last modified: Sat Dec 16 01:05:38 2023, max compression
+gzip compressed data, was "openimis_be_payment_cycle-1.1.0.tar", last modified: Tue Apr 30 09:07:50 2024, max compression
```

## Comparing `openimis-be-payment_cycle-1.0.0.tar` & `openimis_be_payment_cycle-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:05:38.190097 openimis-be-payment_cycle-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-12-16 01:05:29.000000 openimis-be-payment_cycle-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2023-12-16 01:05:38.190097 openimis-be-payment_cycle-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2023-12-16 01:05:29.000000 openimis-be-payment_cycle-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:05:38.186097 openimis-be-payment_cycle-1.0.0/openimis_be_payment_cycle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2023-12-16 01:05:38.000000 openimis-be-payment_cycle-1.0.0/openimis_be_payment_cycle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      807 2023-12-16 01:05:38.000000 openimis-be-payment_cycle-1.0.0/openimis_be_payment_cycle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 01:05:38.000000 openimis-be-payment_cycle-1.0.0/openimis_be_payment_cycle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-16 01:05:38.000000 openimis-be-payment_cycle-1.0.0/openimis_be_payment_cycle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-16 01:05:38.000000 openimis-be-payment_cycle-1.0.0/openimis_be_payment_cycle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:05:38.186097 openimis-be-payment_cycle-1.0.0/payment_cycle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 01:05:29.000000 openimis-be-payment_cycle-1.0.0/payment_cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 01:05:29.000000 openimis-be-payment_cycle-1.0.0/payment_cycle/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2023-12-16 01:05:29.000000 openimis-be-payment_cycle-1.0.0/payment_cycle/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-16 01:05:29.000000 openimis-be-payment_cycle-1.0.0/payment_cycle/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2023-12-16 01:05:29.000000 openimis-be-payment_cycle-1.0.0/payment_cycle/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:05:38.186097 openimis-be-payment_cycle-1.0.0/payment_cycle/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2023-12-16 01:05:29.000000 openimis-be-payment_cycle-1.0.0/payment_cycle/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-12-16 01:05:29.000000 openimis-be-payment_cycle-1.0.0/payment_cycle/migrations/0002_add_pc_rights_to_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 01:05:29.000000 openimis-be-payment_cycle-1.0.0/payment_cycle/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2023-12-16 01:05:29.000000 openimis-be-payment_cycle-1.0.0/payment_cycle/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2023-12-16 01:05:29.000000 openimis-be-payment_cycle-1.0.0/payment_cycle/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7401 2023-12-16 01:05:29.000000 openimis-be-payment_cycle-1.0.0/payment_cycle/services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:05:38.186097 openimis-be-payment_cycle-1.0.0/payment_cycle/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-12-16 01:05:29.000000 openimis-be-payment_cycle-1.0.0/payment_cycle/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2023-12-16 01:05:29.000000 openimis-be-payment_cycle-1.0.0/payment_cycle/tests/benefitPlanPaymentCycleServiceTests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2023-12-16 01:05:29.000000 openimis-be-payment_cycle-1.0.0/payment_cycle/tests/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-12-16 01:05:29.000000 openimis-be-payment_cycle-1.0.0/payment_cycle/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-16 01:05:29.000000 openimis-be-payment_cycle-1.0.0/payment_cycle/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 01:05:29.000000 openimis-be-payment_cycle-1.0.0/payment_cycle/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 01:05:38.190097 openimis-be-payment_cycle-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2023-12-16 01:05:37.000000 openimis-be-payment_cycle-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:50.960748 openimis_be_payment_cycle-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-30 09:07:50.960748 openimis_be_payment_cycle-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:50.960748 openimis_be_payment_cycle-1.1.0/openimis_be_payment_cycle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-30 09:07:50.000000 openimis_be_payment_cycle-1.1.0/openimis_be_payment_cycle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-30 09:07:50.000000 openimis_be_payment_cycle-1.1.0/openimis_be_payment_cycle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:07:50.000000 openimis_be_payment_cycle-1.1.0/openimis_be_payment_cycle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-30 09:07:50.000000 openimis_be_payment_cycle-1.1.0/openimis_be_payment_cycle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 09:07:50.000000 openimis_be_payment_cycle-1.1.0/openimis_be_payment_cycle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:50.960748 openimis_be_payment_cycle-1.1.0/payment_cycle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:50.960748 openimis_be_payment_cycle-1.1.0/payment_cycle/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/migrations/0002_add_pc_rights_to_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/migrations/0003_alter_historicalpaymentcycle_date_created_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/migrations/0004_add_start_and_end_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/migrations/0005_remove_run_month.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/migrations/0006_auto_20240315_0943.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/migrations/0007_paymentcyclemutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:50.960748 openimis_be_payment_cycle-1.1.0/payment_cycle/signals/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/signals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:50.960748 openimis_be_payment_cycle-1.1.0/payment_cycle/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/tests/paymentCycleServiceTests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:07:42.000000 openimis_be_payment_cycle-1.1.0/payment_cycle/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:07:50.960748 openimis_be_payment_cycle-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-30 09:07:50.000000 openimis_be_payment_cycle-1.1.0/setup.py
```

### Comparing `openimis-be-payment_cycle-1.0.0/LICENSE.md` & `openimis_be_payment_cycle-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-payment_cycle-1.0.0/PKG-INFO` & `openimis_be_payment_cycle-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-payment_cycle
-Version: 1.0.0
+Version: 1.1.0
 Summary: The openIMIS Backend payment_cycle reference module.
 Home-page: https://openimis.org/
 Author: Kamil Malinowski
 Author-email: kmalinowski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-payment_cycle-1.0.0/README.md` & `openimis_be_payment_cycle-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-payment_cycle-1.0.0/openimis_be_payment_cycle.egg-info/PKG-INFO` & `openimis_be_payment_cycle-1.1.0/openimis_be_payment_cycle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openimis-be-payment-cycle
-Version: 1.0.0
+Name: openimis-be-payment_cycle
+Version: 1.1.0
 Summary: The openIMIS Backend payment_cycle reference module.
 Home-page: https://openimis.org/
 Author: Kamil Malinowski
 Author-email: kmalinowski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-payment_cycle-1.0.0/payment_cycle/apps.py` & `openimis_be_payment_cycle-1.1.0/payment_cycle/apps.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 MODULE_NAME = 'payment_cycle'
 
 DEFAULT_CONFIG = {
     'gql_query_payment_cycle_perms': ['200001'],
     'gql_create_payment_cycle_perms': ['200002'],
     'gql_update_payment_cycle_perms': ['200003'],
     'gql_delete_payment_cycle_perms': ['200004'],
-    'gql_mutation_process_payment_cycle_perms': ['200005']
+    'gql_check_payment_cycle': True,
 }
 
 
 class PaymentCycleConfig(AppConfig):
     default_auto_field = 'django.db.models.BigAutoField'
     name = MODULE_NAME
 
     gql_query_payment_cycle_perms = None
     gql_create_payment_cycle_perms = None
     gql_update_payment_cycle_perms = None
     gql_delete_payment_cycle_perms = None
-    gql_mutation_process_payment_cycle_perms = None
+    gql_check_payment_cycle = None
 
     def ready(self):
         from core.models import ModuleConfiguration
 
         cfg = ModuleConfiguration.get_or_default(self.name, DEFAULT_CONFIG)
         self.__load_config(cfg)
```

### Comparing `openimis-be-payment_cycle-1.0.0/payment_cycle/migrations/0001_initial.py` & `openimis_be_payment_cycle-1.1.0/payment_cycle/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment_cycle-1.0.0/payment_cycle/migrations/0002_add_pc_rights_to_admin.py` & `openimis_be_payment_cycle-1.1.0/payment_cycle/migrations/0002_add_pc_rights_to_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment_cycle-1.0.0/payment_cycle/tests/helpers.py` & `openimis_be_payment_cycle-1.1.0/payment_cycle/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment_cycle-1.0.0/setup.py` & `openimis_be_payment_cycle-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-payment_cycle',
-    version='1.0.0',
+    version='v1.1.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend payment_cycle reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

