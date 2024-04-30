# Comparing `tmp/openimis-be-payment-1.6.0.tar.gz` & `tmp/openimis_be_payment-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-payment-1.6.0.tar", last modified: Sat Dec 16 00:57:08 2023, max compression
+gzip compressed data, was "openimis_be_payment-1.7.0.tar", last modified: Tue Apr 30 09:05:42 2024, max compression
```

## Comparing `openimis-be-payment-1.6.0.tar` & `openimis_be_payment-1.7.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:08.222020 openimis-be-payment-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      811 2023-12-16 00:57:08.222020 openimis-be-payment-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:08.218020 openimis-be-payment-1.6.0/openimis_be_payment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2023-12-16 00:57:08.000000 openimis-be-payment-1.6.0/openimis_be_payment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-16 00:57:08.000000 openimis-be-payment-1.6.0/openimis_be_payment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:57:08.000000 openimis-be-payment-1.6.0/openimis_be_payment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:57:08.000000 openimis-be-payment-1.6.0/openimis_be_payment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-16 00:57:08.000000 openimis-be-payment-1.6.0/openimis_be_payment.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:08.218020 openimis-be-payment-1.6.0/payment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:08.218020 openimis-be-payment-1.6.0/payment/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/migrations/0002_incorrect_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/migrations/0003_auto_20220401_1149.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/migrations/0004_update_django_scheme_with_missing_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/migrations/0005_set_managed_to_true.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/migrations/0006_missing_fields_OP-1560.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/migrations/0008_payment_serial_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5964 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    17144 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/services.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14097 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:56:56.000000 openimis-be-payment-1.6.0/payment/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:57:08.222020 openimis-be-payment-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2023-12-16 00:57:07.000000 openimis-be-payment-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:42.667404 openimis_be_payment-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-30 09:05:42.667404 openimis_be_payment-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:42.667404 openimis_be_payment-1.7.0/openimis_be_payment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-30 09:05:42.000000 openimis_be_payment-1.7.0/openimis_be_payment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-30 09:05:42.000000 openimis_be_payment-1.7.0/openimis_be_payment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:05:42.000000 openimis_be_payment-1.7.0/openimis_be_payment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:05:42.000000 openimis_be_payment-1.7.0/openimis_be_payment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 09:05:42.000000 openimis_be_payment-1.7.0/openimis_be_payment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:42.663404 openimis_be_payment-1.7.0/payment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:42.667404 openimis_be_payment-1.7.0/payment/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/migrations/0002_incorrect_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/migrations/0003_auto_20220401_1149.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/migrations/0004_update_django_scheme_with_missing_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/migrations/0005_set_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/migrations/0006_missing_fields_OP-1560.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/migrations/0008_payment_serial_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17144 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:42.667404 openimis_be_payment-1.7.0/payment/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/tests/tests_gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/tests/tests_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:05:33.000000 openimis_be_payment-1.7.0/payment/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:05:42.667404 openimis_be_payment-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-30 09:05:42.000000 openimis_be_payment-1.7.0/setup.py
```

### Comparing `openimis-be-payment-1.6.0/LICENSE.md` & `openimis_be_payment-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.6.0/PKG-INFO` & `openimis_be_payment-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-payment
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Payment reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-payment-1.6.0/README.md` & `openimis_be_payment-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.6.0/openimis_be_payment.egg-info/PKG-INFO` & `openimis_be_payment-1.7.0/openimis_be_payment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-payment
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Payment reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-payment-1.6.0/openimis_be_payment.egg-info/SOURCES.txt` & `openimis_be_payment-1.7.0/openimis_be_payment.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 payment/gql_mutations.py
 payment/gql_queries.py
 payment/models.py
 payment/schema.py
 payment/services.py
 payment/signals.py
 payment/test_helpers.py
-payment/tests.py
 payment/urls.py
 payment/views.py
 payment/migrations/0001_initial.py
 payment/migrations/0002_incorrect_name.py
 payment/migrations/0003_auto_20220401_1149.py
 payment/migrations/0004_update_django_scheme_with_missing_fields.py
 payment/migrations/0005_set_managed_to_true.py
 payment/migrations/0006_missing_fields_OP-1560.py
 payment/migrations/0008_payment_serial_fix.py
-payment/migrations/__init__.py
+payment/migrations/__init__.py
+payment/tests/__init__.py
+payment/tests/tests_gql.py
+payment/tests/tests_service.py
```

### Comparing `openimis-be-payment-1.6.0/payment/apps.py` & `openimis_be_payment-1.7.0/payment/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.6.0/payment/gql_mutations.py` & `openimis_be_payment-1.7.0/payment/gql_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.6.0/payment/gql_queries.py` & `openimis_be_payment-1.7.0/payment/gql_queries.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.6.0/payment/migrations/0001_initial.py` & `openimis_be_payment-1.7.0/payment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.6.0/payment/migrations/0002_incorrect_name.py` & `openimis_be_payment-1.7.0/payment/migrations/0002_incorrect_name.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.6.0/payment/migrations/0003_auto_20220401_1149.py` & `openimis_be_payment-1.7.0/payment/migrations/0003_auto_20220401_1149.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.6.0/payment/migrations/0004_update_django_scheme_with_missing_fields.py` & `openimis_be_payment-1.7.0/payment/migrations/0004_update_django_scheme_with_missing_fields.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.6.0/payment/migrations/0006_missing_fields_OP-1560.py` & `openimis_be_payment-1.7.0/payment/migrations/0006_missing_fields_OP-1560.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.6.0/payment/migrations/0008_payment_serial_fix.py` & `openimis_be_payment-1.7.0/payment/migrations/0008_payment_serial_fix.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.6.0/payment/models.py` & `openimis_be_payment-1.7.0/payment/models.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.6.0/payment/schema.py` & `openimis_be_payment-1.7.0/payment/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             raise PermissionDenied(_("unauthorized"))
         filters = []
         # OFS-257: Create dynamic filters for the payment mutation
         additional_filter = kwargs.get('additional_filter', None)
         # go to process additional filter only when this arg of filter was passed into query
         if additional_filter:
             filters_from_signal = _get_additional_filter(
-                sender=self, additional_filter=additional_filter, user=info.context.user
+                sender=Payment, additional_filter=additional_filter, user=info.context.user
             )
             # check if there is filter from signal (perms will be checked in the signals)
             if len(filters_from_signal) == 0:
                 raise PermissionDenied(_("unauthorized"))
             filters.extend(filters_from_signal)
         if not info.context.user.has_perms(PaymentConfig.gql_query_payments_perms):
             raise PermissionDenied(_("unauthorized"))
```

### Comparing `openimis-be-payment-1.6.0/payment/services.py` & `openimis_be_payment-1.7.0/payment/services.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.6.0/payment/test_helpers.py` & `openimis_be_payment-1.7.0/payment/test_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.6.0/payment/tests.py` & `openimis_be_payment-1.7.0/payment/tests/tests_service.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.6.0/setup.py` & `openimis_be_payment-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-payment',
-    version='v1.6.0',
+    version='v1.7.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Payment reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
```

