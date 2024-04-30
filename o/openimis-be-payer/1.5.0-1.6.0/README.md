# Comparing `tmp/openimis-be-payer-1.5.0.tar.gz` & `tmp/openimis_be_payer-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-payer-1.5.0.tar", last modified: Sat Dec 16 00:56:59 2023, max compression
+gzip compressed data, was "openimis_be_payer-1.6.0.tar", last modified: Tue Apr 30 09:05:36 2024, max compression
```

## Comparing `openimis-be-payer-1.5.0.tar` & `openimis_be_payer-1.6.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:59.664195 openimis-be-payer-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-12-16 00:56:50.000000 openimis-be-payer-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-16 00:56:50.000000 openimis-be-payer-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      808 2023-12-16 00:56:59.664195 openimis-be-payer-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-12-16 00:56:50.000000 openimis-be-payer-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:59.664195 openimis-be-payer-1.5.0/openimis_be_payer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2023-12-16 00:56:59.000000 openimis-be-payer-1.5.0/openimis_be_payer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2023-12-16 00:56:59.000000 openimis-be-payer-1.5.0/openimis_be_payer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:56:59.000000 openimis-be-payer-1.5.0/openimis_be_payer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-16 00:56:59.000000 openimis-be-payer-1.5.0/openimis_be_payer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-16 00:56:59.000000 openimis-be-payer-1.5.0/openimis_be_payer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:59.664195 openimis-be-payer-1.5.0/payer/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-16 00:56:50.000000 openimis-be-payer-1.5.0/payer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:56:50.000000 openimis-be-payer-1.5.0/payer/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-12-16 00:56:50.000000 openimis-be-payer-1.5.0/payer/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2023-12-16 00:56:50.000000 openimis-be-payer-1.5.0/payer/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2023-12-16 00:56:50.000000 openimis-be-payer-1.5.0/payer/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:59.664195 openimis-be-payer-1.5.0/payer/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2023-12-16 00:56:50.000000 openimis-be-payer-1.5.0/payer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2023-12-16 00:56:50.000000 openimis-be-payer-1.5.0/payer/migrations/0002_add_missing_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2023-12-16 00:56:50.000000 openimis-be-payer-1.5.0/payer/migrations/0003_set_managed_to_true.py
--rw-r--r--   0 runner    (1001) docker     (127)     5493 2023-12-16 00:56:50.000000 openimis-be-payer-1.5.0/payer/migrations/0004_funding_historicalfunding.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:50.000000 openimis-be-payer-1.5.0/payer/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2023-12-16 00:56:50.000000 openimis-be-payer-1.5.0/payer/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2023-12-16 00:56:50.000000 openimis-be-payer-1.5.0/payer/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2023-12-16 00:56:50.000000 openimis-be-payer-1.5.0/payer/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2023-12-16 00:56:50.000000 openimis-be-payer-1.5.0/payer/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-16 00:56:50.000000 openimis-be-payer-1.5.0/payer/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:56:50.000000 openimis-be-payer-1.5.0/payer/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:56:59.664195 openimis-be-payer-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2023-12-16 00:56:59.000000 openimis-be-payer-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:36.300603 openimis_be_payer-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-30 09:05:36.300603 openimis_be_payer-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:36.300603 openimis_be_payer-1.6.0/openimis_be_payer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-30 09:05:36.000000 openimis_be_payer-1.6.0/openimis_be_payer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-30 09:05:36.000000 openimis_be_payer-1.6.0/openimis_be_payer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:05:36.000000 openimis_be_payer-1.6.0/openimis_be_payer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-30 09:05:36.000000 openimis_be_payer-1.6.0/openimis_be_payer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 09:05:36.000000 openimis_be_payer-1.6.0/openimis_be_payer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:36.296603 openimis_be_payer-1.6.0/payer/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/payer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/payer/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/payer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/payer/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/payer/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:36.300603 openimis_be_payer-1.6.0/payer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/payer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/payer/migrations/0002_add_missing_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/payer/migrations/0003_set_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/payer/migrations/0004_funding_historicalfunding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/payer/migrations/0005_alter_funding_date_created_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/payer/migrations/0006_add_search_authority_for_eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/payer/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/payer/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/payer/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/payer/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/payer/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/payer/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:05:28.000000 openimis_be_payer-1.6.0/payer/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:05:36.300603 openimis_be_payer-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-30 09:05:35.000000 openimis_be_payer-1.6.0/setup.py
```

### Comparing `openimis-be-payer-1.5.0/LICENSE.md` & `openimis_be_payer-1.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-payer-1.5.0/PKG-INFO` & `openimis_be_payer-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-payer
-Version: 1.5.0
+Version: 1.6.0
 Summary: The openIMIS Backend Payer reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-payer-1.5.0/README.md` & `openimis_be_payer-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-payer-1.5.0/openimis_be_payer.egg-info/PKG-INFO` & `openimis_be_payer-1.6.0/openimis_be_payer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-payer
-Version: 1.5.0
+Version: 1.6.0
 Summary: The openIMIS Backend Payer reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-payer-1.5.0/openimis_be_payer.egg-info/SOURCES.txt` & `openimis_be_payer-1.6.0/openimis_be_payer.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -18,8 +18,10 @@
 payer/tests.py
 payer/urls.py
 payer/views.py
 payer/migrations/0001_initial.py
 payer/migrations/0002_add_missing_fields.py
 payer/migrations/0003_set_managed_to_true.py
 payer/migrations/0004_funding_historicalfunding.py
+payer/migrations/0005_alter_funding_date_created_and_more.py
+payer/migrations/0006_add_search_authority_for_eo.py
 payer/migrations/__init__.py
```

### Comparing `openimis-be-payer-1.5.0/payer/apps.py` & `openimis_be_payer-1.6.0/payer/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payer-1.5.0/payer/gql_mutations.py` & `openimis_be_payer-1.6.0/payer/gql_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payer-1.5.0/payer/gql_queries.py` & `openimis_be_payer-1.6.0/payer/gql_queries.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payer-1.5.0/payer/migrations/0001_initial.py` & `openimis_be_payer-1.6.0/payer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payer-1.5.0/payer/migrations/0002_add_missing_fields.py` & `openimis_be_payer-1.6.0/payer/migrations/0002_add_missing_fields.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payer-1.5.0/payer/migrations/0004_funding_historicalfunding.py` & `openimis_be_payer-1.6.0/payer/migrations/0004_funding_historicalfunding.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payer-1.5.0/payer/models.py` & `openimis_be_payer-1.6.0/payer/models.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payer-1.5.0/payer/schema.py` & `openimis_be_payer-1.6.0/payer/schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payer-1.5.0/payer/test_helpers.py` & `openimis_be_payer-1.6.0/payer/test_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payer-1.5.0/payer/tests.py` & `openimis_be_payer-1.6.0/payer/tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payer-1.5.0/setup.py` & `openimis_be_payer-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-payer',
-    version='v1.5.0',
+    version='v1.6.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Payer reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
```

