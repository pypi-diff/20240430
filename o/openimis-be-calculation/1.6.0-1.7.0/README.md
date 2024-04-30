# Comparing `tmp/openimis-be-calculation-1.6.0.tar.gz` & `tmp/openimis_be_calculation-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-calculation-1.6.0.tar", last modified: Sat Dec 16 00:57:36 2023, max compression
+gzip compressed data, was "openimis_be_calculation-1.7.0.tar", last modified: Tue Apr 30 09:06:12 2024, max compression
```

## Comparing `openimis-be-calculation-1.6.0.tar` & `openimis_be_calculation-1.7.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:36.467223 openimis-be-calculation-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2023-12-16 00:57:36.467223 openimis-be-calculation-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:36.463223 openimis-be-calculation-1.6.0/calculation/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/calculation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/calculation/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/calculation/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/calculation/calculation_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/calculation/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:36.463223 openimis-be-calculation-1.6.0/calculation/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     9423 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/calculation/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/calculation/migrations/0002_auto_20210118_1426.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/calculation/migrations/0003_add_calculation_roles_for_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/calculation/migrations/0004_auto_20230126_0903.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/calculation/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/calculation/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10505 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/calculation/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/calculation/services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:36.463223 openimis-be-calculation-1.6.0/calculation/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/calculation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/calculation/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/calculation/tests/helpers_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/calculation/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:57:28.000000 openimis-be-calculation-1.6.0/calculation/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:57:36.467223 openimis-be-calculation-1.6.0/openimis_be_calculation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2023-12-16 00:57:36.000000 openimis-be-calculation-1.6.0/openimis_be_calculation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-12-16 00:57:36.000000 openimis-be-calculation-1.6.0/openimis_be_calculation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:57:36.000000 openimis-be-calculation-1.6.0/openimis_be_calculation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-16 00:57:36.000000 openimis-be-calculation-1.6.0/openimis_be_calculation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-16 00:57:36.000000 openimis-be-calculation-1.6.0/openimis_be_calculation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:57:36.467223 openimis-be-calculation-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-12-16 00:57:36.000000 openimis-be-calculation-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:12.099028 openimis_be_calculation-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-30 09:06:12.099028 openimis_be_calculation-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:12.095028 openimis_be_calculation-1.7.0/calculation/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/calculation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:12.095028 openimis_be_calculation-1.7.0/calculation/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/migrations/0002_auto_20210118_1426.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/migrations/0003_add_calculation_roles_for_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/migrations/0004_auto_20230126_0903.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:12.099028 openimis_be_calculation-1.7.0/calculation/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/tests/helpers_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:03.000000 openimis_be_calculation-1.7.0/calculation/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:12.099028 openimis_be_calculation-1.7.0/openimis_be_calculation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-30 09:06:12.000000 openimis_be_calculation-1.7.0/openimis_be_calculation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-30 09:06:12.000000 openimis_be_calculation-1.7.0/openimis_be_calculation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:06:12.000000 openimis_be_calculation-1.7.0/openimis_be_calculation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-30 09:06:12.000000 openimis_be_calculation-1.7.0/openimis_be_calculation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 09:06:12.000000 openimis_be_calculation-1.7.0/openimis_be_calculation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:06:12.099028 openimis_be_calculation-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-30 09:06:11.000000 openimis_be_calculation-1.7.0/setup.py
```

### Comparing `openimis-be-calculation-1.6.0/LICENSE.md` & `openimis_be_calculation-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-calculation-1.6.0/PKG-INFO` & `openimis_be_calculation-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calculation
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Calculation reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calculation-1.6.0/README.md` & `openimis_be_calculation-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-calculation-1.6.0/calculation/apps.py` & `openimis_be_calculation-1.7.0/calculation/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calculation-1.6.0/calculation/calculation_rule.py` & `openimis_be_calculation-1.7.0/calculation/calculation_rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,20 +19,20 @@
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
         condition_is_valid = (cls.date_valid_from <= now <= cls.date_valid_to) \
             if cls.date_valid_to else (now >= cls.date_valid_from and cls.date_valid_to is None)
         if condition_is_valid:
```

### Comparing `openimis-be-calculation-1.6.0/calculation/config.py` & `openimis_be_calculation-1.7.0/calculation/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                         }
                     },
                 ],
                 "default": "5"
             },
             {
                 "type": "checkbox",
-                "name": "includeFamilly",
+                "name": "includeFamily",
                 "label": {
                     "en": "include family members",
                     "fr": "Inclure les membres de la familles"
                 },
                 "rights": {
                     "read": "151201",
                     "write": "151202",
```

### Comparing `openimis-be-calculation-1.6.0/calculation/migrations/0001_initial.py` & `openimis_be_calculation-1.7.0/calculation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calculation-1.6.0/calculation/migrations/0002_auto_20210118_1426.py` & `openimis_be_calculation-1.7.0/calculation/migrations/0002_auto_20210118_1426.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calculation-1.6.0/calculation/migrations/0004_auto_20230126_0903.py` & `openimis_be_calculation-1.7.0/calculation/migrations/0004_auto_20230126_0903.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calculation-1.6.0/calculation/schema.py` & `openimis_be_calculation-1.7.0/calculation/schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calculation-1.6.0/calculation/services.py` & `openimis_be_calculation-1.7.0/calculation/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,17 @@
             return calculation_rule
 
 def run_calculation_rules(instance, context, user, **kwargs):
     for calculation_rule in CALCULATION_RULES:
         result_signal = calculation_rule.signal_calculate_event.send(
             sender=instance.__class__.__name__, instance=instance, user=user, context=context, **kwargs
         )
-        if result_signal[0][1]:
+        if  result_signal and len(result_signal) and result_signal[0][1]:
             return result_signal
+
     # if no listened calculation rules - return None
     return None
 
 
 def get_parameters(class_name, instance):
     """ className is the class name of the object where the calculation param need to be added
         instance is where the link with a calculation need to be found,
```

### Comparing `openimis-be-calculation-1.6.0/openimis_be_calculation.egg-info/PKG-INFO` & `openimis_be_calculation-1.7.0/openimis_be_calculation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calculation
-Version: 1.6.0
+Version: 1.7.0
 Summary: The openIMIS Backend Calculation reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calculation-1.6.0/openimis_be_calculation.egg-info/SOURCES.txt` & `openimis_be_calculation-1.7.0/openimis_be_calculation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-calculation-1.6.0/setup.py` & `openimis_be_calculation-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-calculation',
-    version='v1.6.0',
+    version='v1.7.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Calculation reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

