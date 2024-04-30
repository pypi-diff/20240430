# Comparing `tmp/openimis-be-calcrule_social_protection-1.0.0.tar.gz` & `tmp/openimis_be_calcrule_social_protection-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-calcrule_social_protection-1.0.0.tar", last modified: Sat Dec 16 13:39:32 2023, max compression
+gzip compressed data, was "openimis_be_calcrule_social_protection-1.1.0.tar", last modified: Tue Apr 30 08:29:47 2024, max compression
```

## Comparing `openimis-be-calcrule_social_protection-1.0.0.tar` & `openimis_be_calcrule_social_protection-1.1.0.tar`

### file list

```diff
@@ -1,46 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 13:39:32.659994 openimis-be-calcrule_social_protection-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-12-16 13:39:32.659994 openimis-be-calcrule_social_protection-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      224 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 13:39:32.651994 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/calculation_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 13:39:32.651994 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/converters/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 13:39:32.655994 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/converters/beneficiary/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/converters/beneficiary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/converters/beneficiary/beneficiary_to_bill.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/converters/beneficiary/beneficiary_to_bill_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 13:39:32.655994 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/converters/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/converters/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/converters/builder/builder_to_bill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/converters/builder/builder_to_bill_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 13:39:32.655994 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/converters/group_beneficiary/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/converters/group_beneficiary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/converters/group_beneficiary/group_to_bill.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/converters/group_beneficiary/group_to_bill_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 13:39:32.655994 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 13:39:32.655994 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/strategies/benefit_package_base_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/strategies/benefit_package_group_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/strategies/benefit_package_individual_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/strategies/benefit_package_strategy_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/strategies/benefit_package_strategy_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 13:39:23.000000 openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 13:39:32.655994 openimis-be-calcrule_social_protection-1.0.0/openimis_be_calcrule_social_protection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-12-16 13:39:32.000000 openimis-be-calcrule_social_protection-1.0.0/openimis_be_calcrule_social_protection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2023-12-16 13:39:32.000000 openimis-be-calcrule_social_protection-1.0.0/openimis_be_calcrule_social_protection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 13:39:32.000000 openimis-be-calcrule_social_protection-1.0.0/openimis_be_calcrule_social_protection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-12-16 13:39:32.000000 openimis-be-calcrule_social_protection-1.0.0/openimis_be_calcrule_social_protection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-16 13:39:32.000000 openimis-be-calcrule_social_protection-1.0.0/openimis_be_calcrule_social_protection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 13:39:32.659994 openimis-be-calcrule_social_protection-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2023-12-16 13:39:32.000000 openimis-be-calcrule_social_protection-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:47.513834 openimis_be_calcrule_social_protection-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-30 08:29:47.513834 openimis_be_calcrule_social_protection-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:47.509834 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/calculation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:47.509834 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:47.509834 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/beneficiary/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/beneficiary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/beneficiary/beneficiary_to_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/beneficiary/beneficiary_to_bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/beneficiary/beneficiary_to_bill_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:47.509834 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/builder/builder_to_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/builder/builder_to_bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/builder/builder_to_bill_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:47.509834 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/group_beneficiary/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/group_beneficiary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/group_beneficiary/group_to_benefit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/group_beneficiary/group_to_bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/group_beneficiary/group_to_bill_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:47.509834 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:47.513834 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/benefit_package_base_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/benefit_package_group_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/benefit_package_individual_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/benefit_package_strategy_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/benefit_package_strategy_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 08:29:39.000000 openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:29:47.513834 openimis_be_calcrule_social_protection-1.1.0/openimis_be_calcrule_social_protection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-30 08:29:47.000000 openimis_be_calcrule_social_protection-1.1.0/openimis_be_calcrule_social_protection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-30 08:29:47.000000 openimis_be_calcrule_social_protection-1.1.0/openimis_be_calcrule_social_protection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:29:47.000000 openimis_be_calcrule_social_protection-1.1.0/openimis_be_calcrule_social_protection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-30 08:29:47.000000 openimis_be_calcrule_social_protection-1.1.0/openimis_be_calcrule_social_protection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 08:29:47.000000 openimis_be_calcrule_social_protection-1.1.0/openimis_be_calcrule_social_protection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 08:29:47.513834 openimis_be_calcrule_social_protection-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-30 08:29:47.000000 openimis_be_calcrule_social_protection-1.1.0/setup.py
```

### Comparing `openimis-be-calcrule_social_protection-1.0.0/LICENSE.md` & `openimis_be_calcrule_social_protection-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_social_protection-1.0.0/PKG-INFO` & `openimis_be_calcrule_social_protection-1.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calcrule_social_protection
-Version: 1.0.0
+Version: 1.1.0
 Summary: The openIMIS Backend calcrule_social_protection reference module.
 Home-page: https://openimis.org/
 Author: sniedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -16,11 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: django
 Requires-Dist: django-db-signals
 Requires-Dist: djangorestframework
 Requires-Dist: openimis-be-core
+Requires-Dist: openimis-be-invoice
+Requires-Dist: openimis-be-individual
+Requires-Dist: openimis-be-social_protection
+Requires-Dist: openimis-be-payroll
 
 # openIMIS Backend calcrule_social_protection reference module
 # description
 This calculation will calculate amount of payment for beneficiary based on whether they meet criteria specified in custom filters of payment plan.
```

### Comparing `openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/apps.py` & `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/apps.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import importlib
 import inspect
 from django.apps import AppConfig
 from calculation.apps import CALCULATION_RULES
 
 MODULE_NAME = 'calcrule_social_protection'
 DEFAULT_CFG = {
-    'calculate_business_event': 'calcrule_social_protection.calculate'
+    'calculate_business_event': 'calcrule_social_protection.calculate',
+    'code_length': 8
 }
 
 
 def read_all_calculation_rules():
     """function to read all calculation rules from that module"""
     for name, cls in inspect.getmembers(importlib.import_module('calcrule_social_protection.calculation_rule'),
                                         inspect.isclass):
@@ -18,14 +19,15 @@
             cls.ready()
 
 
 class CalcruleSocialProtectionConfig(AppConfig):
     name = MODULE_NAME
 
     calculate_business_event = None
+    code_length = None
 
     def ready(self):
         from core.models import ModuleConfiguration
         cfg = ModuleConfiguration.get_or_default(MODULE_NAME, DEFAULT_CFG)
         read_all_calculation_rules()
         self.__load_config(cfg)
```

### Comparing `openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/calculation_rule.py` & `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/calculation_rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from calcrule_social_protection.strategies import (
     BenefitPackageStrategyStorage
 )
 from calcrule_social_protection.config import CLASS_RULE_PARAM_VALIDATION, DESCRIPTION_CONTRIBUTION_VALUATION, FROM_TO
 from core.abs_calculation_rule import AbsCalculationRule
 from core.signals import *
 from core import datetime
-
+from contribution_plan.models import PaymentPlan
 
 class SocialProtectionCalculationRule(AbsCalculationRule):
     version = 1
     uuid = "32d96b58-898a-460a-b357-5fd4b95cd87c"
     calculation_rule_name = "Calculation rule: social protection"
     description = DESCRIPTION_CONTRIBUTION_VALUATION
     impacted_class_parameter = CLASS_RULE_PARAM_VALIDATION
@@ -17,20 +17,20 @@
     date_valid_to = None
     status = "active"
     from_to = FROM_TO
     type = "social_protection"
     sub_type = "benefit_plan"
     CLASS_NAME_CHECK = ['PaymentPlan']
 
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
@@ -40,24 +40,27 @@
                 cls.signal_get_rule_details.connect(cls.get_rule_details, dispatch_uid="on_get_rule_details_signal")
                 cls.signal_get_param.connect(cls.get_parameters, dispatch_uid="on_get_param_signal")
                 cls.signal_get_linked_class.connect(cls.get_linked_class, dispatch_uid="on_get_linked_class_signal")
                 cls.signal_calculate_event.connect(cls.run_calculation_rules, dispatch_uid="on_calculate_event_signal")
                 cls.signal_convert_from_to.connect(cls.run_convert, dispatch_uid="on_convert_from_to")
 
     @classmethod
-    def run_calculation_rules(cls, sender, payment_plan, user, context, **kwargs):
-        return cls.calculate_if_active_for_object(payment_plan, **kwargs)
+    def run_calculation_rules(cls, sender, instance, user, context, **kwargs):
+        if isinstance(instance, PaymentPlan):
+            return cls.calculate_if_active_for_object(instance, **kwargs)
+        else:
+            return False
 
     @classmethod
     def calculate_if_active_for_object(cls, payment_plan, **kwargs):
         if cls.active_for_object(payment_plan):
             return cls.calculate(payment_plan, **kwargs)
 
     @classmethod
-    def active_for_object(cls, payment_plan):
+    def active_for_object(cls, payment_plan, **kwargs):
         return cls.check_calculation(payment_plan)
 
     @classmethod
     def get_linked_class(cls, sender, class_name, **kwargs):
         return ["Calculation"]
 
     @classmethod
@@ -84,12 +87,12 @@
 
     @classmethod
     def convert(cls, payment_plan, **kwargs):
         BenefitPackageStrategyStorage.choose_strategy(payment_plan).convert(payment_plan, **kwargs)
 
     @classmethod
     def get_payment_cycle_parameters(cls, **kwargs):
-        audit_user_id = kwargs.get('audit_user_id', None)
+        user_id = kwargs.get('user_id', None)
         start_date = kwargs.get('start_date', None)
         end_date = kwargs.get('end_date', None)
         payment_cycle = kwargs.get('payment_cycle', None)
-        return audit_user_id, start_date, end_date, payment_cycle
+        return user_id, start_date, end_date, payment_cycle
```

### Comparing `openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/config.py` & `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,16 +2,16 @@
     {
         "class": "PaymentPlan",
         "parameters": [
             {
                 "type": "number",
                 "name": "fixed_batch",
                 "label": {
-                    "en": "Fixed batch",
-                    "fr": "Fixed batch"
+                    "en": "Fixed amount",
+                    "fr": "Lot fixe"
                 },
                 "rights": {
                     "read": "157101",
                     "write": "157102",
                     "update": "157103",
                     "replace": "157206"
                 },
@@ -20,15 +20,15 @@
                 "default": "0"
             },
             {
                 "type": "number",
                 "name": "limit_per_single_transaction",
                 "label": {
                     "en": "Limit Per Single Transaction",
-                    "fr": "Limit Per Single Transaction"
+                    "fr": "Limite par transaction unique"
                 },
                 "rights": {
                     "read": "157101",
                     "write": "157102",
                     "update": "157103",
                     "replace": "157206"
                 },
```

### Comparing `openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/converters/builder/builder_to_bill.py` & `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/builder/builder_to_bill.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,66 @@
 from django.contrib.contenttypes.models import ContentType
 from invoice.apps import InvoiceConfig
 from invoice.models import Bill
+from calcrule_social_protection.utils import CodeGenerator
+from calcrule_social_protection.apps import CalcruleSocialProtectionConfig
 
 
 class BuilderToBillConverter:
     TYPE = None
 
     @classmethod
     def to_bill_obj(cls, payment_plan, entity, amount, end_date, payment_cycle):
         bill = {}
         cls._build_subject(bill, entity)
-        cls._build_thirdparty(bill, payment_cycle)
-        cls._build_code(bill, payment_plan, entity, end_date)
+        cls._build_thirdparty(bill, payment_plan)
+        cls._build_code(bill)
         cls._build_price(bill, amount)
-        cls._build_terms(bill, payment_plan)
-        cls._build_date_dates(bill, payment_plan)
+        cls._build_terms(bill, payment_plan, entity, end_date)
+        cls._build_date_dates(bill, payment_plan, payment_cycle)
         cls._build_currency(bill)
         cls._build_status(bill)
         return bill
 
     @classmethod
     def _build_subject(cls, bill, entity):
         bill["subject_id"] = f"{entity.id}"
         bill['subject_type_id'] = f"{ContentType.objects.get_for_model(entity).id}"
 
     @classmethod
-    def _build_thirdparty(cls, bill, payment_cycle):
-        bill["thirdparty_id"] = f"{payment_cycle.id}"
-        bill['thirdparty_type_id'] = f"{ContentType.objects.get_for_model(payment_cycle).id}"
+    def _build_thirdparty(cls, bill, payment_plan):
+        bill["thirdparty_id"] = f"{payment_plan.id}"
+        bill['thirdparty_type_id'] = f"{ContentType.objects.get_for_model(payment_plan).id}"
 
     @classmethod
-    def _build_code(cls, bill, payment_plan, entity, end_date):
-        pass
+    def _build_code(cls, bill):
+        code = CodeGenerator.generate_unique_code(
+            'invoice',
+            'Bill',
+            'code',
+            CalcruleSocialProtectionConfig.code_length
+        )
+        bill["code"] = code
 
     @classmethod
     def _build_price(cls, bill, amount):
         bill["amount_net"] = amount
 
     @classmethod
-    def _build_date_dates(cls, bill, payment_plan):
-        from core import datetime, datetimedelta
-        bill["date_due"] = f"{datetime.date.today() + datetimedelta(days=30)}"
-        bill["date_bill"] = f"{datetime.date.today()}"
+    def _build_date_dates(cls, bill, payment_plan, payment_cycle):
+        bill["date_due"] = f"{payment_cycle.end_date}"
+        bill["date_bill"] = f"{payment_cycle.start_date}"
         bill["date_valid_from"] = f"{ payment_plan.benefit_plan.date_valid_from}"
         bill["date_valid_to"] = f"{payment_plan.benefit_plan.date_valid_to}"
 
     @classmethod
     def _build_currency(cls, bill):
         bill["currency_tp_code"] = InvoiceConfig.default_currency_code
         bill["currency_code"] = InvoiceConfig.default_currency_code
 
     @classmethod
     def _build_status(cls, bill):
         bill["status"] = Bill.Status.VALIDATED.value
 
     @classmethod
-    def _build_terms(cls, bill, payment_plan):
-        bill["terms"] = f'{payment_plan.benefit_plan.name}'
+    def _build_terms(cls, bill, payment_plan, entity, end_date):
+        pass
```

### Comparing `openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/converters/builder/builder_to_bill_item.py` & `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/converters/builder/builder_to_bill_item.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/signals.py` & `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/signals.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,45 +4,52 @@
 from calcrule_social_protection.apps import CalcruleSocialProtectionConfig
 from core.models import User
 from core.service_signals import ServiceSignalBindType
 from core.signals import bind_service_signal
 
 from openIMIS.openimisapps import openimis_apps
 
+from calcrule_social_protection.strategies import BaseBenefitPackageStrategy
 from invoice.models import Bill
-from invoice.services import BillService
 from tasks_management.models import Task
 
 logger = logging.getLogger(__name__)
 imis_modules = openimis_apps()
 
 
 def bind_service_signals():
 
     def on_task_complete_calculate(**kwargs):
-        def create_bill(results, bill_status):
-            results['bill_data']['status'] = bill_status
+        def create_bill(results, convert_benefit, payroll_id, bill_status):
             user = User.objects.get(id=result['data']['user']['id'])
             results['user'] = user
-            BillService(user).bill_create(convert_results=results)
+            BaseBenefitPackageStrategy.create_and_save_business_entities(
+                results,
+                convert_benefit,
+                payroll_id,
+                user,
+                bill_status
+            )
 
         try:
             result = kwargs.get('result', None)
             task = result['data']['task']
             if result \
                     and result['success'] \
                     and task['business_event'] == CalcruleSocialProtectionConfig.calculate_business_event:
                 convert_results = task['data']
                 convert_results = convert_results.replace("'", '"')
                 convert_results = json.loads(convert_results)
                 task_status = task['status']
+                convert_benefit = convert_results.pop("benefit", None)
+                payroll_id = convert_results.pop("payroll_id", None)
                 if task_status == Task.Status.COMPLETED:
-                    create_bill(convert_results, Bill.Status.VALIDATED)
+                    create_bill(convert_results, convert_benefit, payroll_id, Bill.Status.VALIDATED)
                 if task_status == Task.Status.FAILED:
-                    create_bill(convert_results, Bill.Status.CANCELLED)
+                    create_bill(convert_results, convert_benefit, payroll_id, Bill.Status.CANCELLED)
                 else:
                     pass
         except Exception as e:
             logger.error("Error while executing on_task_complete_calculate", exc_info=e)
 
     bind_service_signal(
         'task_service.complete_task',
```

### Comparing `openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/strategies/__init__.py` & `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/strategies/benefit_package_base_strategy.py` & `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/benefit_package_base_strategy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,66 @@
+import logging
+
 from django.db import transaction
 
 from calcrule_social_protection.apps import CalcruleSocialProtectionConfig
 from core.models import User
 from core.utils import convert_to_python_value
 from core.signals import register_service_signal
 from invoice.models import Bill
 from invoice.services import BillService
 from social_protection.models import BeneficiaryStatus
+from payroll.services import BenefitConsumptionService, PayrollService
 from tasks_management.apps import TasksManagementConfig
 from tasks_management.models import Task
 from tasks_management.services import TaskService
 
 from calcrule_social_protection.strategies.benefit_package_strategy_interface import BenefitPackageStrategyInterface
 
 
+logger = logging.getLogger(__name__)
+
+
 class BaseBenefitPackageStrategy(BenefitPackageStrategyInterface):
     is_exceed_limit = False
 
     @classmethod
     def check_calculation(cls, calculation, payment_plan):
         return calculation.uuid == str(payment_plan.calculation)
 
     @classmethod
     def calculate(cls, calculation, payment_plan, **kwargs):
         # 1. Get the list of beneficiares assigned to benefit plan from payment plan
-        # each beneficiary group from benefit plan assigned to this payment plan is a single bill
-        beneficiares = cls.BENEFICIARY_OBJECT.objects.filter(
-            benefit_plan=payment_plan.benefit_plan, status=BeneficiaryStatus.ACTIVE
-        )
+        # each beneficiary group from benefit plan assigned to this payment plan is a single benefit
+        payroll = kwargs.get('payroll', None)
+        beneficiaries = kwargs.get('beneficiaries_queryset', None)
+        if not beneficiaries:
+            beneficiaries = cls.BENEFICIARY_OBJECT.objects.filter(
+                benefit_plan=payment_plan.benefit_plan, status=BeneficiaryStatus.ACTIVE
+            )
         # 2. Get the parameters from payment plan with fixed and advanced criteria
         payment_plan_parameters = payment_plan.json_ext
-        audit_user_id, start_date, end_date, payment_cycle = \
+        user_id, start_date, end_date, payment_cycle = \
             calculation.get_payment_cycle_parameters(**kwargs)
-        user = User.objects.filter(i_user__id=audit_user_id).first()
-        payment = payment_plan_parameters['calculation_rule']['fixed_batch']
-        limit = payment_plan_parameters['calculation_rule']['limit_per_single_transaction']
+        user = User.objects.filter(id=user_id).first()
+        payment = float(payment_plan_parameters['calculation_rule']['fixed_batch'])
+        limit = float(payment_plan_parameters['calculation_rule']['limit_per_single_transaction'])
         advanced_filters_criteria = payment_plan_parameters['advanced_criteria'] if 'advanced_criteria' in payment_plan_parameters else []
-        for beneficiary in beneficiares:
+        for beneficiary in beneficiaries:
             calculated_payment = cls._calculate_payment(
                 beneficiary, advanced_filters_criteria, payment, limit
             )
 
             additional_params = {
                 f"{cls.BENEFICIARY_TYPE}": beneficiary,
                 "amount": calculated_payment,
                 "user": user,
                 "end_date": end_date,
-                "payment_cycle": payment_cycle
+                "payment_cycle": payment_cycle,
+                "payroll": payroll,
             }
             calculation.run_convert(
                 payment_plan,
                 **additional_params
             )
         return "Calculation and transformation into bills completed successfully."
 
@@ -75,27 +85,62 @@
                     ).exists()
         return False
 
     @classmethod
     def convert(cls, payment_plan, **kwargs):
         entity = kwargs.get('entity', None)
         amount = kwargs.get('amount', None)
+        payroll = kwargs.get('payroll', None)
         end_date = kwargs.get('end_date', None)
-        payment_cycle = kwargs.get('payment_cycle', None)
         converter = kwargs.get('converter')
         converter_item = kwargs.get('converter_item')
+        converter_benefit = kwargs.get('converter_benefit')
+        payment_cycle = kwargs.get('payment_cycle')
         convert_results = cls._convert_entity_to_bill(
             converter, converter_item, payment_plan, entity, amount, end_date, payment_cycle
         )
         convert_results['user'] = kwargs.get('user', None)
+        convert_results_benefit = cls._convert_entity_to_benefit(
+            converter_benefit, payment_plan, entity, amount, payment_cycle
+        )
+        user = convert_results['user']
         if not cls.is_exceed_limit:
-            result_bill_creation = BillService.bill_create(convert_results=convert_results)
-            return result_bill_creation
+            cls.create_and_save_business_entities(
+                convert_results,
+                convert_results_benefit,
+                payroll.id,
+                user
+            )
         else:
-            cls.create_task_after_exceeding_limit(convert_results=convert_results)
+            cls.create_task_after_exceeding_limit(
+                convert_results=convert_results,
+                convert_results_benefit=convert_results_benefit,
+                payroll=payroll
+            )
+
+    @classmethod
+    def create_and_save_business_entities(
+            cls, convert_results, convert_results_benefit, payroll_id, user, bill_status=None
+    ):
+        if bill_status is not None:
+            convert_results['bill_data']['status'] = bill_status
+        result_bill_creation = BillService.bill_create(convert_results=convert_results)
+        if result_bill_creation["success"]:
+            bill_id = result_bill_creation['data']['id']
+            benefit_service = BenefitConsumptionService(user)
+            benefit_result = benefit_service.create(convert_results_benefit['benefit_data'])
+            if benefit_result["success"]:
+                # create benefit attachemnts - attach bill to benefit
+                bill_queryset = Bill.objects.filter(id__in=[bill_id])
+                benefit_id = benefit_result['data']['id']
+                benefit_service.create_or_update_benefit_attachment(bill_queryset, benefit_id)
+                if payroll_id:
+                    payroll_service = PayrollService(user=user)
+                    payroll_service.attach_benefit_to_payroll(payroll_id, benefit_id)
+        return result_bill_creation
 
     @classmethod
     def _convert_entity_to_bill(
         cls, converter, converter_item, payment_plan, entity, amount, end_date, payment_cycle
     ):
         bill = converter.to_bill_obj(
             payment_plan, entity, amount, end_date, payment_cycle
@@ -106,21 +151,33 @@
         return {
             'bill_data': bill,
             'bill_data_line': bill_line_items,
             'type_conversion': 'beneficiary - bill'
         }
 
     @classmethod
+    def _convert_entity_to_benefit(
+            cls, converter_benefit, payment_plan, entity, amount, payment_cycle
+    ):
+        benefit = converter_benefit.to_benefit_obj(entity, amount, payment_plan, payment_cycle)
+        return {
+            'benefit_data': benefit,
+            'type_conversion': 'beneficiary - benefit'
+        }
+
+    @classmethod
     @transaction.atomic
     @register_service_signal('calcrule_social_protection.create_task')
-    def create_task_after_exceeding_limit(cls, convert_results):
+    def create_task_after_exceeding_limit(cls, convert_results, convert_results_benefit, payroll):
         business_status = {"code": convert_results['bill_data']['code']}
         user = convert_results.pop('user')
+        convert_results['benefit'] = convert_results_benefit
+        convert_results['payroll_id'] = f"{payroll.id}"
         TaskService(user).create({
             'source': 'calcrule_social_protection',
-            'entity': None,
+            'entity': payroll,
             'status': Task.Status.RECEIVED,
             'executor_action_event': TasksManagementConfig.default_executor_event,
             'business_event': CalcruleSocialProtectionConfig.calculate_business_event,
             'business_status': business_status,
             'data': f"{convert_results}"
         })
```

### Comparing `openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/strategies/benefit_package_individual_strategy.py` & `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/benefit_package_group_strategy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-from invoice.services import BillService
-from social_protection.models import Beneficiary
+from social_protection.models import GroupBeneficiary
+
 from calcrule_social_protection.converters import (
-    BeneficiaryToBillConverter,
-    BeneficiaryToBillItemConverter
+    GroupToBillConverter,
+    GroupToBillItemConverter,
+    GroupToBenefitConverter
 )
 from calcrule_social_protection.strategies.benefit_package_base_strategy import BaseBenefitPackageStrategy
 
 
-class IndividualBenefitPackageStrategy(BaseBenefitPackageStrategy):
-    TYPE = "INDIVIDUAL"
-    BENEFICIARY_OBJECT = Beneficiary
-    BENEFICIARY_TYPE = "beneficiary"
+class GroupBenefitPackageStrategy(BaseBenefitPackageStrategy):
+    TYPE = "GROUP"
+    BENEFICIARY_OBJECT = GroupBeneficiary
+    BENEFICIARY_TYPE = "group"
 
     @classmethod
     def convert(cls, payment_plan, **kwargs):
-        beneficiary = kwargs.get('beneficiary', None)
+        group = kwargs.get('group', None)
         additional_parameters = {
-            "entity": beneficiary,
-            "converter": BeneficiaryToBillConverter,
-            "converter_item": BeneficiaryToBillItemConverter,
+            "entity": group,
+            "converter": GroupToBillConverter,
+            "converter_item": GroupToBillItemConverter,
+            "converter_benefit": GroupToBenefitConverter,
             **kwargs
         }
         return super().convert(payment_plan, **additional_parameters)
```

### Comparing `openimis-be-calcrule_social_protection-1.0.0/calcrule_social_protection/strategies/benefit_package_strategy_storage.py` & `openimis_be_calcrule_social_protection-1.1.0/calcrule_social_protection/strategies/benefit_package_strategy_storage.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_social_protection-1.0.0/openimis_be_calcrule_social_protection.egg-info/PKG-INFO` & `openimis_be_calcrule_social_protection-1.1.0/openimis_be_calcrule_social_protection.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openimis-be-calcrule-social-protection
-Version: 1.0.0
+Name: openimis-be-calcrule_social_protection
+Version: 1.1.0
 Summary: The openIMIS Backend calcrule_social_protection reference module.
 Home-page: https://openimis.org/
 Author: sniedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -16,11 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: django
 Requires-Dist: django-db-signals
 Requires-Dist: djangorestframework
 Requires-Dist: openimis-be-core
+Requires-Dist: openimis-be-invoice
+Requires-Dist: openimis-be-individual
+Requires-Dist: openimis-be-social_protection
+Requires-Dist: openimis-be-payroll
 
 # openIMIS Backend calcrule_social_protection reference module
 # description
 This calculation will calculate amount of payment for beneficiary based on whether they meet criteria specified in custom filters of payment plan.
```

### Comparing `openimis-be-calcrule_social_protection-1.0.0/openimis_be_calcrule_social_protection.egg-info/SOURCES.txt` & `openimis_be_calcrule_social_protection-1.1.0/openimis_be_calcrule_social_protection.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,27 @@
 calcrule_social_protection/apps.py
 calcrule_social_protection/calculation_rule.py
 calcrule_social_protection/config.py
 calcrule_social_protection/models.py
 calcrule_social_protection/signals.py
 calcrule_social_protection/tests.py
 calcrule_social_protection/urls.py
+calcrule_social_protection/utils.py
 calcrule_social_protection/views.py
 calcrule_social_protection/converters/__init__.py
 calcrule_social_protection/converters/beneficiary/__init__.py
+calcrule_social_protection/converters/beneficiary/beneficiary_to_benefit.py
 calcrule_social_protection/converters/beneficiary/beneficiary_to_bill.py
 calcrule_social_protection/converters/beneficiary/beneficiary_to_bill_item.py
 calcrule_social_protection/converters/builder/__init__.py
+calcrule_social_protection/converters/builder/builder_to_benefit.py
 calcrule_social_protection/converters/builder/builder_to_bill.py
 calcrule_social_protection/converters/builder/builder_to_bill_item.py
 calcrule_social_protection/converters/group_beneficiary/__init__.py
+calcrule_social_protection/converters/group_beneficiary/group_to_benefit.py
 calcrule_social_protection/converters/group_beneficiary/group_to_bill.py
 calcrule_social_protection/converters/group_beneficiary/group_to_bill_item.py
 calcrule_social_protection/migrations/__init__.py
 calcrule_social_protection/strategies/__init__.py
 calcrule_social_protection/strategies/benefit_package_base_strategy.py
 calcrule_social_protection/strategies/benefit_package_group_strategy.py
 calcrule_social_protection/strategies/benefit_package_individual_strategy.py
```

### Comparing `openimis-be-calcrule_social_protection-1.0.0/setup.py` & `openimis_be_calcrule_social_protection-1.1.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,29 +5,33 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-calcrule_social_protection',
-    version='v1.0.0',
+    version='1.1.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend calcrule_social_protection reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
     author='sniedzielski',
     author_email='sniedzielski@soldevelo.com',
     install_requires=[
         'django',
         'django-db-signals',
         'djangorestframework',
-        'openimis-be-core'
+        'openimis-be-core',
+        'openimis-be-invoice',
+        'openimis-be-individual',
+        'openimis-be-social_protection',
+        'openimis-be-payroll'
     ],
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 3.0',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3',
```

