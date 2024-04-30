# Comparing `tmp/openimis-be-calcrule_unconditional_cash_payment-1.5.0.tar.gz` & `tmp/openimis_be_calcrule_unconditional_cash_payment-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-calcrule_unconditional_cash_payment-1.5.0.tar", last modified: Sat Dec 16 01:07:12 2023, max compression
+gzip compressed data, was "openimis_be_calcrule_unconditional_cash_payment-1.6.0.tar", last modified: Tue Apr 30 09:07:24 2024, max compression
```

## Comparing `openimis-be-calcrule_unconditional_cash_payment-1.5.0.tar` & `openimis_be_calcrule_unconditional_cash_payment-1.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:07:12.820506 openimis-be-calcrule_unconditional_cash_payment-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-12-16 01:07:01.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-12-16 01:07:12.820506 openimis-be-calcrule_unconditional_cash_payment-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-16 01:07:01.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:07:12.816506 openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-16 01:07:01.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 01:07:01.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2023-12-16 01:07:01.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2023-12-16 01:07:01.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/calculation_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2023-12-16 01:07:01.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:07:12.816506 openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/converters/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-12-16 01:07:01.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2023-12-16 01:07:01.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/converters/policy_to_bill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-12-16 01:07:01.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/converters/policy_to_bill_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:07:12.816506 openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 01:07:01.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-16 01:07:01.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-16 01:07:01.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-16 01:07:01.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-16 01:07:01.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 01:07:01.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:07:12.820506 openimis-be-calcrule_unconditional_cash_payment-1.5.0/openimis_be_calcrule_unconditional_cash_payment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-12-16 01:07:12.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/openimis_be_calcrule_unconditional_cash_payment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-12-16 01:07:12.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/openimis_be_calcrule_unconditional_cash_payment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 01:07:12.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/openimis_be_calcrule_unconditional_cash_payment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-12-16 01:07:12.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/openimis_be_calcrule_unconditional_cash_payment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-16 01:07:12.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/openimis_be_calcrule_unconditional_cash_payment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 01:07:12.820506 openimis-be-calcrule_unconditional_cash_payment-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2023-12-16 01:07:12.000000 openimis-be-calcrule_unconditional_cash_payment-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:24.109018 openimis_be_calcrule_unconditional_cash_payment-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-30 09:07:12.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-30 09:07:24.109018 openimis_be_calcrule_unconditional_cash_payment-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-30 09:07:12.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:24.105018 openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-30 09:07:12.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:07:12.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-30 09:07:12.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-30 09:07:12.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/calculation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-30 09:07:12.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:24.105018 openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-30 09:07:12.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-30 09:07:12.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/converters/policy_to_bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-30 09:07:12.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/converters/policy_to_bill_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:24.105018 openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:12.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 09:07:12.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-30 09:07:12.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 09:07:12.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 09:07:12.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:07:12.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:24.109018 openimis_be_calcrule_unconditional_cash_payment-1.6.0/openimis_be_calcrule_unconditional_cash_payment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-30 09:07:24.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/openimis_be_calcrule_unconditional_cash_payment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-30 09:07:24.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/openimis_be_calcrule_unconditional_cash_payment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:07:24.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/openimis_be_calcrule_unconditional_cash_payment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 09:07:24.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/openimis_be_calcrule_unconditional_cash_payment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 09:07:24.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/openimis_be_calcrule_unconditional_cash_payment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:07:24.109018 openimis_be_calcrule_unconditional_cash_payment-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-30 09:07:23.000000 openimis_be_calcrule_unconditional_cash_payment-1.6.0/setup.py
```

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.5.0/LICENSE.md` & `openimis_be_calcrule_unconditional_cash_payment-1.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.5.0/PKG-INFO` & `openimis_be_calcrule_unconditional_cash_payment-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calcrule_unconditional_cash_payment
-Version: 1.5.0
+Version: 1.6.0
 Summary: The openIMIS Backend calcrule_unconditional_cash_payment reference module.
 Home-page: https://openimis.org/
 Author: Wojciech Zgliniecki
 Author-email: wzgliniecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/apps.py` & `openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/calculation_rule.py` & `openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/calculation_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,20 +20,20 @@
     date_valid_from = datetime.datetime(2000, 1, 1)
     date_valid_to = None
     status = "active"
     from_to = FROM_TO
     type = "account_payable"
     sub_type = "cash_payment"
 
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

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/config.py` & `openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/config.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/converters/policy_to_bill.py` & `openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/converters/policy_to_bill.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/converters/policy_to_bill_item.py` & `openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/converters/policy_to_bill_item.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.5.0/calcrule_unconditional_cash_payment/signals.py` & `openimis_be_calcrule_unconditional_cash_payment-1.6.0/calcrule_unconditional_cash_payment/signals.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.5.0/openimis_be_calcrule_unconditional_cash_payment.egg-info/PKG-INFO` & `openimis_be_calcrule_unconditional_cash_payment-1.6.0/openimis_be_calcrule_unconditional_cash_payment.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openimis-be-calcrule-unconditional-cash-payment
-Version: 1.5.0
+Name: openimis-be-calcrule_unconditional_cash_payment
+Version: 1.6.0
 Summary: The openIMIS Backend calcrule_unconditional_cash_payment reference module.
 Home-page: https://openimis.org/
 Author: Wojciech Zgliniecki
 Author-email: wzgliniecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.5.0/openimis_be_calcrule_unconditional_cash_payment.egg-info/SOURCES.txt` & `openimis_be_calcrule_unconditional_cash_payment-1.6.0/openimis_be_calcrule_unconditional_cash_payment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.5.0/setup.py` & `openimis_be_calcrule_unconditional_cash_payment-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-calcrule_unconditional_cash_payment',
-    version='v1.5.0',
+    version='v1.6.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend calcrule_unconditional_cash_payment reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

