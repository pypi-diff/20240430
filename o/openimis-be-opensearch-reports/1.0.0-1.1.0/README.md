# Comparing `tmp/openimis-be-opensearch_reports-1.0.0.tar.gz` & `tmp/openimis_be_opensearch_reports-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-opensearch_reports-1.0.0.tar", last modified: Sat Dec 16 00:59:01 2023, max compression
+gzip compressed data, was "openimis_be_opensearch_reports-1.1.0.tar", last modified: Tue Apr 30 09:07:47 2024, max compression
```

## Comparing `openimis-be-opensearch_reports-1.0.0.tar` & `openimis_be_opensearch_reports-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:59:01.492546 openimis-be-opensearch_reports-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-16 00:58:49.000000 openimis-be-opensearch_reports-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-12-16 00:58:49.000000 openimis-be-opensearch_reports-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2023-12-16 00:59:01.492546 openimis-be-opensearch_reports-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2023-12-16 00:58:49.000000 openimis-be-opensearch_reports-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:59:01.492546 openimis-be-opensearch_reports-1.0.0/openimis_be_opensearch_reports.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2023-12-16 00:59:01.000000 openimis-be-opensearch_reports-1.0.0/openimis_be_opensearch_reports.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      546 2023-12-16 00:59:01.000000 openimis-be-opensearch_reports-1.0.0/openimis_be_opensearch_reports.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 00:59:01.000000 openimis-be-opensearch_reports-1.0.0/openimis_be_opensearch_reports.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-12-16 00:59:01.000000 openimis-be-opensearch_reports-1.0.0/openimis_be_opensearch_reports.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-16 00:59:01.000000 openimis-be-opensearch_reports-1.0.0/openimis_be_opensearch_reports.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:59:01.492546 openimis-be-opensearch_reports-1.0.0/opensearch_reports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:49.000000 openimis-be-opensearch_reports-1.0.0/opensearch_reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:58:49.000000 openimis-be-opensearch_reports-1.0.0/opensearch_reports/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-12-16 00:58:49.000000 openimis-be-opensearch_reports-1.0.0/opensearch_reports/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 00:59:01.492546 openimis-be-opensearch_reports-1.0.0/opensearch_reports/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 00:58:49.000000 openimis-be-opensearch_reports-1.0.0/opensearch_reports/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-16 00:58:49.000000 openimis-be-opensearch_reports-1.0.0/opensearch_reports/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-16 00:58:49.000000 openimis-be-opensearch_reports-1.0.0/opensearch_reports/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-16 00:58:49.000000 openimis-be-opensearch_reports-1.0.0/opensearch_reports/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 00:58:49.000000 openimis-be-opensearch_reports-1.0.0/opensearch_reports/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 00:59:01.492546 openimis-be-opensearch_reports-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2023-12-16 00:59:01.000000 openimis-be-opensearch_reports-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:47.205124 openimis_be_opensearch_reports-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-04-30 09:07:47.201125 openimis_be_opensearch_reports-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:47.201125 openimis_be_opensearch_reports-1.1.0/openimis_be_opensearch_reports.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-04-30 09:07:47.000000 openimis_be_opensearch_reports-1.1.0/openimis_be_opensearch_reports.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-30 09:07:47.000000 openimis_be_opensearch_reports-1.1.0/openimis_be_opensearch_reports.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:07:47.000000 openimis_be_opensearch_reports-1.1.0/openimis_be_opensearch_reports.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 09:07:47.000000 openimis_be_opensearch_reports-1.1.0/openimis_be_opensearch_reports.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-30 09:07:47.000000 openimis_be_opensearch_reports-1.1.0/openimis_be_opensearch_reports.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:47.201125 openimis_be_opensearch_reports-1.1.0/opensearch_reports/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/opensearch_reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/opensearch_reports/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/opensearch_reports/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/opensearch_reports/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/opensearch_reports/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:47.201125 openimis_be_opensearch_reports-1.1.0/opensearch_reports/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/opensearch_reports/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/opensearch_reports/migrations/0002_default_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/opensearch_reports/migrations/0003_individuals_groups_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/opensearch_reports/migrations/0004_alter_historicalopensearchdashboard_date_created_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/opensearch_reports/migrations/0005_add_opensearch_rights.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/opensearch_reports/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/opensearch_reports/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/opensearch_reports/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/opensearch_reports/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/opensearch_reports/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/opensearch_reports/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/opensearch_reports/validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:07:35.000000 openimis_be_opensearch_reports-1.1.0/opensearch_reports/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:07:47.205124 openimis_be_opensearch_reports-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-30 09:07:46.000000 openimis_be_opensearch_reports-1.1.0/setup.py
```

### Comparing `openimis-be-opensearch_reports-1.0.0/LICENSE` & `openimis_be_opensearch_reports-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openimis-be-opensearch_reports-1.0.0/LICENSE.md` & `openimis_be_opensearch_reports-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-opensearch_reports-1.0.0/PKG-INFO` & `openimis_be_opensearch_reports-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-opensearch_reports
-Version: 1.0.0
+Version: 1.1.0
 Summary: The openIMIS Backend opensearch_reports reference module.
 Home-page: https://openimis.org/
 Author: sniedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-opensearch_reports-1.0.0/README.md` & `openimis_be_opensearch_reports-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-opensearch_reports-1.0.0/openimis_be_opensearch_reports.egg-info/PKG-INFO` & `openimis_be_opensearch_reports-1.1.0/openimis_be_opensearch_reports.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openimis-be-opensearch-reports
-Version: 1.0.0
+Name: openimis-be-opensearch_reports
+Version: 1.1.0
 Summary: The openIMIS Backend opensearch_reports reference module.
 Home-page: https://openimis.org/
 Author: sniedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-opensearch_reports-1.0.0/setup.py` & `openimis_be_opensearch_reports-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-opensearch_reports',
-    version='1.0.0',
+    version='v1.1.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend opensearch_reports reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

