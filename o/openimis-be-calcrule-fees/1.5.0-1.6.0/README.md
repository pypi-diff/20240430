# Comparing `tmp/openimis-be-calcrule_fees-1.5.0.tar.gz` & `tmp/openimis_be_calcrule_fees-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-calcrule_fees-1.5.0.tar", last modified: Sat Dec 16 01:03:41 2023, max compression
+gzip compressed data, was "openimis_be_calcrule_fees-1.6.0.tar", last modified: Tue Apr 30 09:07:19 2024, max compression
```

## Comparing `openimis-be-calcrule_fees-1.5.0.tar` & `openimis_be_calcrule_fees-1.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:03:41.854700 openimis-be-calcrule_fees-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2023-12-16 01:03:41.854700 openimis-be-calcrule_fees-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-16 01:03:33.000000 openimis-be-calcrule_fees-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:03:41.850700 openimis-be-calcrule_fees-1.5.0/calcrule_fees/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-16 01:03:33.000000 openimis-be-calcrule_fees-1.5.0/calcrule_fees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 01:03:33.000000 openimis-be-calcrule_fees-1.5.0/calcrule_fees/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2023-12-16 01:03:33.000000 openimis-be-calcrule_fees-1.5.0/calcrule_fees/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2023-12-16 01:03:33.000000 openimis-be-calcrule_fees-1.5.0/calcrule_fees/calculation_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2023-12-16 01:03:33.000000 openimis-be-calcrule_fees-1.5.0/calcrule_fees/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:03:41.850700 openimis-be-calcrule_fees-1.5.0/calcrule_fees/converters/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-12-16 01:03:33.000000 openimis-be-calcrule_fees-1.5.0/calcrule_fees/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2023-12-16 01:03:33.000000 openimis-be-calcrule_fees-1.5.0/calcrule_fees/converters/batch_run_to_bill.py
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2023-12-16 01:03:33.000000 openimis-be-calcrule_fees-1.5.0/calcrule_fees/converters/invoice_payment_to_bill_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:03:41.850700 openimis-be-calcrule_fees-1.5.0/calcrule_fees/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 01:03:33.000000 openimis-be-calcrule_fees-1.5.0/calcrule_fees/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-16 01:03:33.000000 openimis-be-calcrule_fees-1.5.0/calcrule_fees/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-16 01:03:33.000000 openimis-be-calcrule_fees-1.5.0/calcrule_fees/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-16 01:03:33.000000 openimis-be-calcrule_fees-1.5.0/calcrule_fees/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 01:03:33.000000 openimis-be-calcrule_fees-1.5.0/calcrule_fees/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:03:41.854700 openimis-be-calcrule_fees-1.5.0/openimis_be_calcrule_fees.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2023-12-16 01:03:41.000000 openimis-be-calcrule_fees-1.5.0/openimis_be_calcrule_fees.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      660 2023-12-16 01:03:41.000000 openimis-be-calcrule_fees-1.5.0/openimis_be_calcrule_fees.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 01:03:41.000000 openimis-be-calcrule_fees-1.5.0/openimis_be_calcrule_fees.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-16 01:03:41.000000 openimis-be-calcrule_fees-1.5.0/openimis_be_calcrule_fees.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-16 01:03:41.000000 openimis-be-calcrule_fees-1.5.0/openimis_be_calcrule_fees.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 01:03:41.854700 openimis-be-calcrule_fees-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2023-12-16 01:03:41.000000 openimis-be-calcrule_fees-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:19.491811 openimis_be_calcrule_fees-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-30 09:07:19.491811 openimis_be_calcrule_fees-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-30 09:07:05.000000 openimis_be_calcrule_fees-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:19.491811 openimis_be_calcrule_fees-1.6.0/calcrule_fees/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-30 09:07:05.000000 openimis_be_calcrule_fees-1.6.0/calcrule_fees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:07:05.000000 openimis_be_calcrule_fees-1.6.0/calcrule_fees/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-30 09:07:05.000000 openimis_be_calcrule_fees-1.6.0/calcrule_fees/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-04-30 09:07:05.000000 openimis_be_calcrule_fees-1.6.0/calcrule_fees/calculation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-30 09:07:05.000000 openimis_be_calcrule_fees-1.6.0/calcrule_fees/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:19.491811 openimis_be_calcrule_fees-1.6.0/calcrule_fees/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-30 09:07:05.000000 openimis_be_calcrule_fees-1.6.0/calcrule_fees/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-30 09:07:05.000000 openimis_be_calcrule_fees-1.6.0/calcrule_fees/converters/batch_run_to_bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-30 09:07:05.000000 openimis_be_calcrule_fees-1.6.0/calcrule_fees/converters/invoice_payment_to_bill_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:19.491811 openimis_be_calcrule_fees-1.6.0/calcrule_fees/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:05.000000 openimis_be_calcrule_fees-1.6.0/calcrule_fees/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 09:07:05.000000 openimis_be_calcrule_fees-1.6.0/calcrule_fees/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 09:07:05.000000 openimis_be_calcrule_fees-1.6.0/calcrule_fees/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 09:07:05.000000 openimis_be_calcrule_fees-1.6.0/calcrule_fees/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:07:05.000000 openimis_be_calcrule_fees-1.6.0/calcrule_fees/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:19.491811 openimis_be_calcrule_fees-1.6.0/openimis_be_calcrule_fees.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-30 09:07:19.000000 openimis_be_calcrule_fees-1.6.0/openimis_be_calcrule_fees.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-30 09:07:19.000000 openimis_be_calcrule_fees-1.6.0/openimis_be_calcrule_fees.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:07:19.000000 openimis_be_calcrule_fees-1.6.0/openimis_be_calcrule_fees.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 09:07:19.000000 openimis_be_calcrule_fees-1.6.0/openimis_be_calcrule_fees.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 09:07:19.000000 openimis_be_calcrule_fees-1.6.0/openimis_be_calcrule_fees.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:07:19.491811 openimis_be_calcrule_fees-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-30 09:07:19.000000 openimis_be_calcrule_fees-1.6.0/setup.py
```

### Comparing `openimis-be-calcrule_fees-1.5.0/PKG-INFO` & `openimis_be_calcrule_fees-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calcrule_fees
-Version: 1.5.0
+Version: 1.6.0
 Summary: The openIMIS Backend calculation rule fees reference module.
 Home-page: https://openimis.org/
 Author: Seweryn Niedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calcrule_fees-1.5.0/calcrule_fees/apps.py` & `openimis_be_calcrule_fees-1.6.0/calcrule_fees/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_fees-1.5.0/calcrule_fees/calculation_rule.py` & `openimis_be_calcrule_fees-1.6.0/calcrule_fees/calculation_rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,20 +28,20 @@
     date_valid_from = datetime.datetime(2000, 1, 1)
     date_valid_to = None
     status = "active"
     from_to = FROM_TO
     type = "account_payable"
     sub_type = "fees"
 
-    signal_get_rule_name = Signal(providing_args=[])
-    signal_get_rule_details = Signal(providing_args=[])
-    signal_get_param = Signal(providing_args=[])
-    signal_get_linked_class = Signal(providing_args=[])
-    signal_calculate_event = Signal(providing_args=[])
-    signal_convert_from_to = Signal(providing_args=[])
+    signal_get_rule_name = Signal([])
+    signal_get_rule_details = Signal([])
+    signal_get_param = Signal([])
+    signal_get_linked_class = Signal([])
+    signal_calculate_event = Signal([])
+    signal_convert_from_to = Signal([])
 
     @classmethod
     def ready(cls):
         now = datetime.datetime.now()
         condition_is_valid = (now >= cls.date_valid_from and now <= cls.date_valid_to) \
             if cls.date_valid_to else (now >= cls.date_valid_from and cls.date_valid_to is None)
         if condition_is_valid:
```

### Comparing `openimis-be-calcrule_fees-1.5.0/calcrule_fees/config.py` & `openimis_be_calcrule_fees-1.6.0/calcrule_fees/config.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_fees-1.5.0/calcrule_fees/converters/batch_run_to_bill.py` & `openimis_be_calcrule_fees-1.6.0/calcrule_fees/converters/batch_run_to_bill.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_fees-1.5.0/calcrule_fees/converters/invoice_payment_to_bill_item.py` & `openimis_be_calcrule_fees-1.6.0/calcrule_fees/converters/invoice_payment_to_bill_item.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_fees-1.5.0/openimis_be_calcrule_fees.egg-info/PKG-INFO` & `openimis_be_calcrule_fees-1.6.0/openimis_be_calcrule_fees.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openimis-be-calcrule-fees
-Version: 1.5.0
+Name: openimis-be-calcrule_fees
+Version: 1.6.0
 Summary: The openIMIS Backend calculation rule fees reference module.
 Home-page: https://openimis.org/
 Author: Seweryn Niedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calcrule_fees-1.5.0/openimis_be_calcrule_fees.egg-info/SOURCES.txt` & `openimis_be_calcrule_fees-1.6.0/openimis_be_calcrule_fees.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_fees-1.5.0/setup.py` & `openimis_be_calcrule_fees-1.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-calcrule_fees',
-    version='v1.5.0',
+    version='v1.6.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend calculation rule fees reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

