# Comparing `tmp/openimis-be-calcrule-contribution-legacy-1.5.0.tar.gz` & `tmp/openimis_be_calcrule_contribution_legacy-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-calcrule-contribution-legacy-1.5.0.tar", last modified: Sat Dec 16 00:57:58 2023, max compression
+gzip compressed data, was "openimis_be_calcrule_contribution_legacy-1.6.0.tar", last modified: Tue Apr 30 09:06:46 2024, max compression
```

## Comparing `openimis-be-calcrule-contribution-legacy-1.5.0.tar` & `openimis_be_calcrule_contribution_legacy-1.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:58.440544 openimis-be-calcrule-contribution-legacy-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2023-12-16 00:57:58.440544 openimis-be-calcrule-contribution-legacy-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      697 2023-12-16 00:57:50.000000 openimis-be-calcrule-contribution-legacy-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:58.436544 openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-12-16 00:57:50.000000 openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:57:50.000000 openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2023-12-16 00:57:50.000000 openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     8446 2023-12-16 00:57:50.000000 openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/calculation_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2023-12-16 00:57:50.000000 openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:58.436544 openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/converters/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2023-12-16 00:57:50.000000 openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2023-12-16 00:57:50.000000 openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/converters/contract_cpd_to_invoice_line_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2023-12-16 00:57:50.000000 openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/converters/contract_to_invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2023-12-16 00:57:50.000000 openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/converters/policy_to_invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2023-12-16 00:57:50.000000 openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/converters/policy_to_line_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:58.440544 openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:50.000000 openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-16 00:57:50.000000 openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2023-12-16 00:57:50.000000 openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-16 00:57:50.000000 openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-16 00:57:50.000000 openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:57:50.000000 openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:58.440544 openimis-be-calcrule-contribution-legacy-1.5.0/openimis_be_calcrule_contribution_legacy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2023-12-16 00:57:58.000000 openimis-be-calcrule-contribution-legacy-1.5.0/openimis_be_calcrule_contribution_legacy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2023-12-16 00:57:58.000000 openimis-be-calcrule-contribution-legacy-1.5.0/openimis_be_calcrule_contribution_legacy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:57:58.000000 openimis-be-calcrule-contribution-legacy-1.5.0/openimis_be_calcrule_contribution_legacy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-16 00:57:58.000000 openimis-be-calcrule-contribution-legacy-1.5.0/openimis_be_calcrule_contribution_legacy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-16 00:57:58.000000 openimis-be-calcrule-contribution-legacy-1.5.0/openimis_be_calcrule_contribution_legacy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:57:58.440544 openimis-be-calcrule-contribution-legacy-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2023-12-16 00:57:58.000000 openimis-be-calcrule-contribution-legacy-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:46.479104 openimis_be_calcrule_contribution_legacy-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-30 09:06:46.479104 openimis_be_calcrule_contribution_legacy-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-30 09:06:35.000000 openimis_be_calcrule_contribution_legacy-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:46.475104 openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-30 09:06:35.000000 openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:35.000000 openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-30 09:06:35.000000 openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-04-30 09:06:35.000000 openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/calculation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-30 09:06:35.000000 openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:46.479104 openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-30 09:06:35.000000 openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-30 09:06:35.000000 openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/converters/contract_cpd_to_invoice_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-30 09:06:35.000000 openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/converters/contract_to_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-30 09:06:35.000000 openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/converters/policy_to_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-30 09:06:35.000000 openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/converters/policy_to_line_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:46.479104 openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:35.000000 openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 09:06:35.000000 openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-30 09:06:35.000000 openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 09:06:35.000000 openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 09:06:35.000000 openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:35.000000 openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:46.479104 openimis_be_calcrule_contribution_legacy-1.6.0/openimis_be_calcrule_contribution_legacy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-30 09:06:46.000000 openimis_be_calcrule_contribution_legacy-1.6.0/openimis_be_calcrule_contribution_legacy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-30 09:06:46.000000 openimis_be_calcrule_contribution_legacy-1.6.0/openimis_be_calcrule_contribution_legacy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:06:46.000000 openimis_be_calcrule_contribution_legacy-1.6.0/openimis_be_calcrule_contribution_legacy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-30 09:06:46.000000 openimis_be_calcrule_contribution_legacy-1.6.0/openimis_be_calcrule_contribution_legacy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 09:06:46.000000 openimis_be_calcrule_contribution_legacy-1.6.0/openimis_be_calcrule_contribution_legacy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:06:46.479104 openimis_be_calcrule_contribution_legacy-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-30 09:06:46.000000 openimis_be_calcrule_contribution_legacy-1.6.0/setup.py
```

### Comparing `openimis-be-calcrule-contribution-legacy-1.5.0/PKG-INFO` & `openimis_be_calcrule_contribution_legacy-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calcrule-contribution-legacy
-Version: 1.5.0
+Version: 1.6.0
 Summary: The openIMIS Backend calculation rule contribution legacy reference module.
 Home-page: https://openimis.org/
 Author: Seweryn Niedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calcrule-contribution-legacy-1.5.0/README.md` & `openimis_be_calcrule_contribution_legacy-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/apps.py` & `openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/calculation_rule.py` & `openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/calculation_rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,20 +22,20 @@
     date_valid_from = datetime.datetime(2000, 1, 1)
     date_valid_to = None
     status = "active"
     from_to = FROM_TO
     type = "account_receivable"
     sub_type = "contribution"
 
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

### Comparing `openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/converters/contract_cpd_to_invoice_line_item.py` & `openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/converters/contract_cpd_to_invoice_line_item.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/converters/contract_to_invoice.py` & `openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/converters/contract_to_invoice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/converters/policy_to_invoice.py` & `openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/converters/policy_to_invoice.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/converters/policy_to_line_item.py` & `openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/converters/policy_to_line_item.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-contribution-legacy-1.5.0/calcrule_contribution_legacy/signals.py` & `openimis_be_calcrule_contribution_legacy-1.6.0/calcrule_contribution_legacy/signals.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-contribution-legacy-1.5.0/openimis_be_calcrule_contribution_legacy.egg-info/PKG-INFO` & `openimis_be_calcrule_contribution_legacy-1.6.0/openimis_be_calcrule_contribution_legacy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calcrule-contribution-legacy
-Version: 1.5.0
+Version: 1.6.0
 Summary: The openIMIS Backend calculation rule contribution legacy reference module.
 Home-page: https://openimis.org/
 Author: Seweryn Niedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calcrule-contribution-legacy-1.5.0/openimis_be_calcrule_contribution_legacy.egg-info/SOURCES.txt` & `openimis_be_calcrule_contribution_legacy-1.6.0/openimis_be_calcrule_contribution_legacy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-contribution-legacy-1.5.0/setup.py` & `openimis_be_calcrule_contribution_legacy-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-calcrule-contribution-legacy',
-    version='v1.5.0',
+    version='v1.6.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend calculation rule contribution legacy reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

