# Comparing `tmp/openimis-be-medical_pricelist-1.6.0.tar.gz` & `tmp/openimis_be_medical_pricelist-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-medical_pricelist-1.6.0.tar", last modified: Sat Dec 16 00:56:18 2023, max compression
+gzip compressed data, was "openimis_be_medical_pricelist-1.6.1.tar", last modified: Tue Apr 30 09:00:51 2024, max compression
```

## Comparing `openimis-be-medical_pricelist-1.6.0.tar` & `openimis_be_medical_pricelist-1.6.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:18.563741 openimis-be-medical_pricelist-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-12-16 00:56:09.000000 openimis-be-medical_pricelist-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-16 00:56:09.000000 openimis-be-medical_pricelist-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      829 2023-12-16 00:56:18.563741 openimis-be-medical_pricelist-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2023-12-16 00:56:09.000000 openimis-be-medical_pricelist-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:18.559741 openimis-be-medical_pricelist-1.6.0/medical_pricelist/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-16 00:56:09.000000 openimis-be-medical_pricelist-1.6.0/medical_pricelist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-16 00:56:09.000000 openimis-be-medical_pricelist-1.6.0/medical_pricelist/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2023-12-16 00:56:09.000000 openimis-be-medical_pricelist-1.6.0/medical_pricelist/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    11780 2023-12-16 00:56:09.000000 openimis-be-medical_pricelist-1.6.0/medical_pricelist/gql_mutations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:18.559741 openimis-be-medical_pricelist-1.6.0/medical_pricelist/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2023-12-16 00:56:09.000000 openimis-be-medical_pricelist-1.6.0/medical_pricelist/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2023-12-16 00:56:09.000000 openimis-be-medical_pricelist-1.6.0/medical_pricelist/migrations/0002_itemspricelistmutation_servicespricelistmutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2023-12-16 00:56:09.000000 openimis-be-medical_pricelist-1.6.0/medical_pricelist/migrations/0003_update_django_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-12-16 00:56:09.000000 openimis-be-medical_pricelist-1.6.0/medical_pricelist/migrations/0004_set_managed_to_true.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:09.000000 openimis-be-medical_pricelist-1.6.0/medical_pricelist/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2023-12-16 00:56:09.000000 openimis-be-medical_pricelist-1.6.0/medical_pricelist/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9521 2023-12-16 00:56:09.000000 openimis-be-medical_pricelist-1.6.0/medical_pricelist/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-12-16 00:56:09.000000 openimis-be-medical_pricelist-1.6.0/medical_pricelist/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2023-12-16 00:56:09.000000 openimis-be-medical_pricelist-1.6.0/medical_pricelist/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-16 00:56:09.000000 openimis-be-medical_pricelist-1.6.0/medical_pricelist/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-16 00:56:09.000000 openimis-be-medical_pricelist-1.6.0/medical_pricelist/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-16 00:56:09.000000 openimis-be-medical_pricelist-1.6.0/medical_pricelist/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:56:18.559741 openimis-be-medical_pricelist-1.6.0/openimis_be_medical_pricelist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2023-12-16 00:56:18.000000 openimis-be-medical_pricelist-1.6.0/openimis_be_medical_pricelist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      910 2023-12-16 00:56:18.000000 openimis-be-medical_pricelist-1.6.0/openimis_be_medical_pricelist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:56:18.000000 openimis-be-medical_pricelist-1.6.0/openimis_be_medical_pricelist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-16 00:56:18.000000 openimis-be-medical_pricelist-1.6.0/openimis_be_medical_pricelist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-16 00:56:18.000000 openimis-be-medical_pricelist-1.6.0/openimis_be_medical_pricelist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:56:18.563741 openimis-be-medical_pricelist-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2023-12-16 00:56:18.000000 openimis-be-medical_pricelist-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:51.119534 openimis_be_medical_pricelist-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-30 09:00:42.000000 openimis_be_medical_pricelist-1.6.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 09:00:42.000000 openimis_be_medical_pricelist-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-30 09:00:51.119534 openimis_be_medical_pricelist-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-30 09:00:42.000000 openimis_be_medical_pricelist-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:51.119534 openimis_be_medical_pricelist-1.6.1/medical_pricelist/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 09:00:42.000000 openimis_be_medical_pricelist-1.6.1/medical_pricelist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 09:00:42.000000 openimis_be_medical_pricelist-1.6.1/medical_pricelist/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-30 09:00:42.000000 openimis_be_medical_pricelist-1.6.1/medical_pricelist/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11780 2024-04-30 09:00:42.000000 openimis_be_medical_pricelist-1.6.1/medical_pricelist/gql_mutations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:51.119534 openimis_be_medical_pricelist-1.6.1/medical_pricelist/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-30 09:00:42.000000 openimis_be_medical_pricelist-1.6.1/medical_pricelist/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-30 09:00:42.000000 openimis_be_medical_pricelist-1.6.1/medical_pricelist/migrations/0002_itemspricelistmutation_servicespricelistmutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-30 09:00:42.000000 openimis_be_medical_pricelist-1.6.1/medical_pricelist/migrations/0003_update_django_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-30 09:00:42.000000 openimis_be_medical_pricelist-1.6.1/medical_pricelist/migrations/0004_set_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:42.000000 openimis_be_medical_pricelist-1.6.1/medical_pricelist/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-04-30 09:00:42.000000 openimis_be_medical_pricelist-1.6.1/medical_pricelist/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9521 2024-04-30 09:00:42.000000 openimis_be_medical_pricelist-1.6.1/medical_pricelist/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-30 09:00:42.000000 openimis_be_medical_pricelist-1.6.1/medical_pricelist/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-30 09:00:42.000000 openimis_be_medical_pricelist-1.6.1/medical_pricelist/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 09:00:42.000000 openimis_be_medical_pricelist-1.6.1/medical_pricelist/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 09:00:42.000000 openimis_be_medical_pricelist-1.6.1/medical_pricelist/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 09:00:42.000000 openimis_be_medical_pricelist-1.6.1/medical_pricelist/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:51.119534 openimis_be_medical_pricelist-1.6.1/openimis_be_medical_pricelist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-30 09:00:51.000000 openimis_be_medical_pricelist-1.6.1/openimis_be_medical_pricelist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-30 09:00:51.000000 openimis_be_medical_pricelist-1.6.1/openimis_be_medical_pricelist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:00:51.000000 openimis_be_medical_pricelist-1.6.1/openimis_be_medical_pricelist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 09:00:51.000000 openimis_be_medical_pricelist-1.6.1/openimis_be_medical_pricelist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 09:00:51.000000 openimis_be_medical_pricelist-1.6.1/openimis_be_medical_pricelist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:00:51.119534 openimis_be_medical_pricelist-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-30 09:00:50.000000 openimis_be_medical_pricelist-1.6.1/setup.py
```

### Comparing `openimis-be-medical_pricelist-1.6.0/LICENSE.md` & `openimis_be_medical_pricelist-1.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-medical_pricelist-1.6.0/PKG-INFO` & `openimis_be_medical_pricelist-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-medical_pricelist
-Version: 1.6.0
+Version: 1.6.1
 Summary: The openIMIS Backend Medical Pricelist reference module.
 Home-page: https://openimis.org/
 Author: Eric Darchis
 Author-email: edarchis@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-medical_pricelist-1.6.0/README.md` & `openimis_be_medical_pricelist-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-medical_pricelist-1.6.0/medical_pricelist/apps.py` & `openimis_be_medical_pricelist-1.6.1/medical_pricelist/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical_pricelist-1.6.0/medical_pricelist/gql_mutations.py` & `openimis_be_medical_pricelist-1.6.1/medical_pricelist/gql_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical_pricelist-1.6.0/medical_pricelist/migrations/0001_initial.py` & `openimis_be_medical_pricelist-1.6.1/medical_pricelist/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical_pricelist-1.6.0/medical_pricelist/migrations/0002_itemspricelistmutation_servicespricelistmutation.py` & `openimis_be_medical_pricelist-1.6.1/medical_pricelist/migrations/0002_itemspricelistmutation_servicespricelistmutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical_pricelist-1.6.0/medical_pricelist/migrations/0003_update_django_scheme.py` & `openimis_be_medical_pricelist-1.6.1/medical_pricelist/migrations/0003_update_django_scheme.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical_pricelist-1.6.0/medical_pricelist/migrations/0004_set_managed_to_true.py` & `openimis_be_medical_pricelist-1.6.1/medical_pricelist/migrations/0004_set_managed_to_true.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical_pricelist-1.6.0/medical_pricelist/models.py` & `openimis_be_medical_pricelist-1.6.1/medical_pricelist/models.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical_pricelist-1.6.0/medical_pricelist/schema.py` & `openimis_be_medical_pricelist-1.6.1/medical_pricelist/schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical_pricelist-1.6.0/medical_pricelist/services.py` & `openimis_be_medical_pricelist-1.6.1/medical_pricelist/services.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical_pricelist-1.6.0/medical_pricelist/test_helpers.py` & `openimis_be_medical_pricelist-1.6.1/medical_pricelist/test_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical_pricelist-1.6.0/openimis_be_medical_pricelist.egg-info/PKG-INFO` & `openimis_be_medical_pricelist-1.6.1/openimis_be_medical_pricelist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openimis-be-medical-pricelist
-Version: 1.6.0
+Name: openimis-be-medical_pricelist
+Version: 1.6.1
 Summary: The openIMIS Backend Medical Pricelist reference module.
 Home-page: https://openimis.org/
 Author: Eric Darchis
 Author-email: edarchis@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-medical_pricelist-1.6.0/openimis_be_medical_pricelist.egg-info/SOURCES.txt` & `openimis_be_medical_pricelist-1.6.1/openimis_be_medical_pricelist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-medical_pricelist-1.6.0/setup.py` & `openimis_be_medical_pricelist-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-medical_pricelist',
-    version='v1.6.0',
+    version='v1.6.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Medical Pricelist reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Eric Darchis',
```

