# Comparing `tmp/openimis-be-calcrule-capitation_payment-1.6.0.tar.gz` & `tmp/openimis_be_calcrule_capitation_payment-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-calcrule-capitation_payment-1.6.0.tar", last modified: Sat Dec 16 00:58:11 2023, max compression
+gzip compressed data, was "openimis_be_calcrule_capitation_payment-1.7.0.tar", last modified: Tue Apr 30 09:06:56 2024, max compression
```

## Comparing `openimis-be-calcrule-capitation_payment-1.6.0.tar` & `openimis_be_calcrule_capitation_payment-1.7.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:11.152798 openimis-be-calcrule-capitation_payment-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2023-12-16 00:58:11.152798 openimis-be-calcrule-capitation_payment-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      695 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:11.148798 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    12400 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/calculation_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    38368 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:11.148798 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/converters/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/converters/batch_run_to_bill.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/converters/capitation_payment_to_bill_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:11.148798 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/migrations/0002_delete_capitationpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/migrations/0003_delete_capitationpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9218 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    21665 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:58:01.000000 openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:11.148798 openimis-be-calcrule-capitation_payment-1.6.0/openimis_be_calcrule_capitation_payment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2023-12-16 00:58:11.000000 openimis-be-calcrule-capitation_payment-1.6.0/openimis_be_calcrule_capitation_payment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2023-12-16 00:58:11.000000 openimis-be-calcrule-capitation_payment-1.6.0/openimis_be_calcrule_capitation_payment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:58:11.000000 openimis-be-calcrule-capitation_payment-1.6.0/openimis_be_calcrule_capitation_payment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-16 00:58:11.000000 openimis-be-calcrule-capitation_payment-1.6.0/openimis_be_calcrule_capitation_payment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-16 00:58:11.000000 openimis-be-calcrule-capitation_payment-1.6.0/openimis_be_calcrule_capitation_payment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:58:11.152798 openimis-be-calcrule-capitation_payment-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2023-12-16 00:58:10.000000 openimis-be-calcrule-capitation_payment-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:56.536654 openimis_be_calcrule_capitation_payment-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-30 09:06:56.536654 openimis_be_calcrule_capitation_payment-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:56.532654 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/calculation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38368 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:56.532654 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/converters/batch_run_to_bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/converters/capitation_payment_to_bill_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:56.536654 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/migrations/0002_delete_capitationpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/migrations/0003_delete_capitationpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21665 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:47.000000 openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:56.536654 openimis_be_calcrule_capitation_payment-1.7.0/openimis_be_calcrule_capitation_payment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-30 09:06:56.000000 openimis_be_calcrule_capitation_payment-1.7.0/openimis_be_calcrule_capitation_payment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-30 09:06:56.000000 openimis_be_calcrule_capitation_payment-1.7.0/openimis_be_calcrule_capitation_payment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:06:56.000000 openimis_be_calcrule_capitation_payment-1.7.0/openimis_be_calcrule_capitation_payment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 09:06:56.000000 openimis_be_calcrule_capitation_payment-1.7.0/openimis_be_calcrule_capitation_payment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 09:06:56.000000 openimis_be_calcrule_capitation_payment-1.7.0/openimis_be_calcrule_capitation_payment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:06:56.536654 openimis_be_calcrule_capitation_payment-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-30 09:06:56.000000 openimis_be_calcrule_capitation_payment-1.7.0/setup.py
```

### Comparing `openimis-be-calcrule-capitation_payment-1.6.0/LICENSE` & `openimis_be_calcrule_capitation_payment-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.6.0/PKG-INFO` & `openimis_be_calcrule_capitation_payment-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calcrule-capitation_payment
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend calculation rule capitation payment reference module.
 Home-page: https://openimis.org/
 Author: Seweryn Niedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calcrule-capitation_payment-1.6.0/README.md` & `openimis_be_calcrule_capitation_payment-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/apps.py` & `openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/calculation_rule.py` & `openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/calculation_rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,20 +46,20 @@
     date_valid_from = datetime.datetime(2000, 1, 1)
     date_valid_to = None
     status = "active"
     from_to = FROM_TO
     type = "account_payable"
     sub_type = "third_party_payment"
 
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

### Comparing `openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/config.py` & `openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/config.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/converters/batch_run_to_bill.py` & `openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/converters/batch_run_to_bill.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/converters/capitation_payment_to_bill_item.py` & `openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/converters/capitation_payment_to_bill_item.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/legacy.py` & `openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/legacy.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/migrations/0001_initial.py` & `openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/tests.py` & `openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 from product.models import ProductItemOrService
 from product.test_helpers import (
     create_test_product,
     create_test_product_service,
     create_test_product_item,
 )
 from location.test_helpers import (
-    create_test_location,
-    create_test_health_facility
+    create_test_health_facility,
+    create_test_village
 )
 
 _TEST_USER_NAME = "test_batch_run"
 _TEST_USER_PWD = "test_batch_run"
 _TEST_DATA_USER = {
     "username": _TEST_USER_NAME,
     "last_name": _TEST_USER_NAME,
@@ -61,20 +61,20 @@
 
     def test_simple_batch(self):
         """
         This test creates a claim, submits it so that it gets dedrem entries,
         then submits a review rejecting part of it, then process the claim.
         It should not be processed (which was ok) but the dedrem should be deleted.
         """
-        # create location
-        test_region = create_test_location('R')
-        test_district = create_test_location('D', custom_props={"parent_id": test_region.id})
-
+        test_village  =create_test_village()
+        test_ward =test_village.parent
+        test_region =test_village.parent.parent.parent
+        test_district = test_village.parent.parent
         # Given
-        insuree = create_test_insuree()
+        insuree = create_test_insuree(custom_props={'current_village':test_village})
         self.assertIsNotNone(insuree)
         service = create_test_service("A", custom_props={"name": "test_simple_batch"})
         item = create_test_item("A", custom_props={"name": "test_simple_batch"})
 
         product = create_test_product(
             "BCUL0001",
             custom_props={
@@ -219,9 +219,7 @@
         PaymentPlan.objects.filter(id=payment_plan.id).delete()
         product.delete()
         if batch_run is not None:
             batch_run.delete()
         test_health_facility.delete()
         test_service_price_list.delete()
         test_item_price_list.delete()
-        test_district.delete()
-        test_region.delete()
```

### Comparing `openimis-be-calcrule-capitation_payment-1.6.0/calcrule_capitation_payment/utils.py` & `openimis_be_calcrule_capitation_payment-1.7.0/calcrule_capitation_payment/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.6.0/openimis_be_calcrule_capitation_payment.egg-info/PKG-INFO` & `openimis_be_calcrule_capitation_payment-1.7.0/openimis_be_calcrule_capitation_payment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openimis-be-calcrule-capitation-payment
-Version: 1.6.0
+Name: openimis-be-calcrule-capitation_payment
+Version: 1.7.0
 Summary: The openIMIS Backend calculation rule capitation payment reference module.
 Home-page: https://openimis.org/
 Author: Seweryn Niedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calcrule-capitation_payment-1.6.0/openimis_be_calcrule_capitation_payment.egg-info/SOURCES.txt` & `openimis_be_calcrule_capitation_payment-1.7.0/openimis_be_calcrule_capitation_payment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.6.0/setup.py` & `openimis_be_calcrule_capitation_payment-1.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-calcrule-capitation_payment',
-    version='v1.6.0',
+    version='v1.7.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend calculation rule capitation payment reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

