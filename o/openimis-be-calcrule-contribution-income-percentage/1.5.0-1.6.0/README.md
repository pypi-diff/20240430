# Comparing `tmp/openimis-be-calcrule_contribution_income_percentage-1.5.0.tar.gz` & `tmp/openimis_be_calcrule_contribution_income_percentage-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-calcrule_contribution_income_percentage-1.5.0.tar", last modified: Sat Dec 16 00:58:17 2023, max compression
+gzip compressed data, was "openimis_be_calcrule_contribution_income_percentage-1.6.0.tar", last modified: Tue Apr 30 09:07:15 2024, max compression
```

## Comparing `openimis-be-calcrule_contribution_income_percentage-1.5.0.tar` & `openimis_be_calcrule_contribution_income_percentage-1.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:17.004990 openimis-be-calcrule_contribution_income_percentage-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2023-12-16 00:58:08.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-16 00:58:17.004990 openimis-be-calcrule_contribution_income_percentage-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-12-16 00:58:08.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:17.000990 openimis-be-calcrule_contribution_income_percentage-1.5.0/calcrule_contribution_income_percentage/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-12-16 00:58:08.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/calcrule_contribution_income_percentage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:58:08.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/calcrule_contribution_income_percentage/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2023-12-16 00:58:08.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/calcrule_contribution_income_percentage/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6824 2023-12-16 00:58:08.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/calcrule_contribution_income_percentage/calculation_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2023-12-16 00:58:08.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/calcrule_contribution_income_percentage/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:17.000990 openimis-be-calcrule_contribution_income_percentage-1.5.0/calcrule_contribution_income_percentage/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:08.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/calcrule_contribution_income_percentage/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:08.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/calcrule_contribution_income_percentage/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:17.004990 openimis-be-calcrule_contribution_income_percentage-1.5.0/calcrule_contribution_income_percentage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-16 00:58:08.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/calcrule_contribution_income_percentage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:08.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/calcrule_contribution_income_percentage/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:08.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/calcrule_contribution_income_percentage/tests/helpers_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-16 00:58:08.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/calcrule_contribution_income_percentage/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:58:08.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/calcrule_contribution_income_percentage/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:17.004990 openimis-be-calcrule_contribution_income_percentage-1.5.0/openimis_be_calcrule_contribution_income_percentage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-16 00:58:16.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/openimis_be_calcrule_contribution_income_percentage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-12-16 00:58:16.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/openimis_be_calcrule_contribution_income_percentage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:58:16.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/openimis_be_calcrule_contribution_income_percentage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-16 00:58:16.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/openimis_be_calcrule_contribution_income_percentage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-16 00:58:16.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/openimis_be_calcrule_contribution_income_percentage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:58:17.004990 openimis-be-calcrule_contribution_income_percentage-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2023-12-16 00:58:16.000000 openimis-be-calcrule_contribution_income_percentage-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:15.191659 openimis_be_calcrule_contribution_income_percentage-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-30 09:06:59.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-30 09:07:15.191659 openimis_be_calcrule_contribution_income_percentage-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-30 09:06:59.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:15.187659 openimis_be_calcrule_contribution_income_percentage-1.6.0/calcrule_contribution_income_percentage/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-30 09:06:59.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/calcrule_contribution_income_percentage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:59.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/calcrule_contribution_income_percentage/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-30 09:06:59.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/calcrule_contribution_income_percentage/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-30 09:06:59.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/calcrule_contribution_income_percentage/calculation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-30 09:06:59.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/calcrule_contribution_income_percentage/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:15.187659 openimis_be_calcrule_contribution_income_percentage-1.6.0/calcrule_contribution_income_percentage/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:59.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/calcrule_contribution_income_percentage/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:59.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/calcrule_contribution_income_percentage/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:15.187659 openimis_be_calcrule_contribution_income_percentage-1.6.0/calcrule_contribution_income_percentage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 09:06:59.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/calcrule_contribution_income_percentage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:59.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/calcrule_contribution_income_percentage/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:59.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/calcrule_contribution_income_percentage/tests/helpers_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-30 09:06:59.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/calcrule_contribution_income_percentage/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:06:59.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/calcrule_contribution_income_percentage/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:15.187659 openimis_be_calcrule_contribution_income_percentage-1.6.0/openimis_be_calcrule_contribution_income_percentage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-30 09:07:15.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/openimis_be_calcrule_contribution_income_percentage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-30 09:07:15.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/openimis_be_calcrule_contribution_income_percentage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:07:15.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/openimis_be_calcrule_contribution_income_percentage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-30 09:07:15.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/openimis_be_calcrule_contribution_income_percentage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-30 09:07:15.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/openimis_be_calcrule_contribution_income_percentage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:07:15.191659 openimis_be_calcrule_contribution_income_percentage-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-30 09:07:14.000000 openimis_be_calcrule_contribution_income_percentage-1.6.0/setup.py
```

### Comparing `openimis-be-calcrule_contribution_income_percentage-1.5.0/LICENSE` & `openimis_be_calcrule_contribution_income_percentage-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_contribution_income_percentage-1.5.0/PKG-INFO` & `openimis_be_calcrule_contribution_income_percentage-1.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calcrule_contribution_income_percentage
-Version: 1.5.0
+Version: 1.6.0
 Summary: The openIMIS Backend calculation rule fs income percentage reference module.
 Home-page: https://openimis.org/
 Author: Seweryn Niedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calcrule_contribution_income_percentage-1.5.0/README.md` & `openimis_be_calcrule_contribution_income_percentage-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_contribution_income_percentage-1.5.0/calcrule_contribution_income_percentage/apps.py` & `openimis_be_calcrule_contribution_income_percentage-1.6.0/calcrule_contribution_income_percentage/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_contribution_income_percentage-1.5.0/calcrule_contribution_income_percentage/calculation_rule.py` & `openimis_be_calcrule_contribution_income_percentage-1.6.0/calcrule_contribution_income_percentage/calculation_rule.py`

 * *Files 4% similar despite different names*

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
         condition_is_valid = (now >= cls.date_valid_from and now <= cls.date_valid_to) \
             if cls.date_valid_to else (now >= cls.date_valid_from and cls.date_valid_to is None)
         if condition_is_valid:
```

### Comparing `openimis-be-calcrule_contribution_income_percentage-1.5.0/calcrule_contribution_income_percentage/config.py` & `openimis_be_calcrule_contribution_income_percentage-1.6.0/calcrule_contribution_income_percentage/config.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_contribution_income_percentage-1.5.0/openimis_be_calcrule_contribution_income_percentage.egg-info/PKG-INFO` & `openimis_be_calcrule_contribution_income_percentage-1.6.0/openimis_be_calcrule_contribution_income_percentage.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openimis-be-calcrule-contribution-income-percentage
-Version: 1.5.0
+Name: openimis-be-calcrule_contribution_income_percentage
+Version: 1.6.0
 Summary: The openIMIS Backend calculation rule fs income percentage reference module.
 Home-page: https://openimis.org/
 Author: Seweryn Niedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calcrule_contribution_income_percentage-1.5.0/openimis_be_calcrule_contribution_income_percentage.egg-info/SOURCES.txt` & `openimis_be_calcrule_contribution_income_percentage-1.6.0/openimis_be_calcrule_contribution_income_percentage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_contribution_income_percentage-1.5.0/setup.py` & `openimis_be_calcrule_contribution_income_percentage-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-calcrule_contribution_income_percentage',
-    version='v1.5.0',
+    version='v1.6.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend calculation rule fs income percentage reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

