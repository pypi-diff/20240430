# Comparing `tmp/pyopencga-2.9.2.tar.gz` & `tmp/pyopencga-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopencga-2.9.2.tar", last modified: Mon Jul 24 11:54:11 2023, max compression
+gzip compressed data, was "pyopencga-3.0.0.tar", last modified: Thu Mar  7 17:49:12 2024, max compression
```

## Comparing `pyopencga-2.9.2.tar` & `pyopencga-3.0.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:54:11.918333 pyopencga-2.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-24 11:51:52.000000 pyopencga-2.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-24 11:54:11.918333 pyopencga-2.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-24 11:51:52.000000 pyopencga-2.9.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:54:11.914333 pyopencga-2.9.2/pyopencga/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-24 11:51:53.000000 pyopencga-2.9.2/pyopencga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-07-24 11:51:53.000000 pyopencga-2.9.2/pyopencga/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-24 11:51:53.000000 pyopencga-2.9.2/pyopencga/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-07-24 11:51:53.000000 pyopencga-2.9.2/pyopencga/opencga_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-24 11:51:53.000000 pyopencga-2.9.2/pyopencga/opencga_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:54:11.918333 pyopencga-2.9.2/pyopencga/rest_clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 11:51:54.000000 pyopencga-2.9.2/pyopencga/rest_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-07-24 11:51:54.000000 pyopencga-2.9.2/pyopencga/rest_clients/_parent_rest_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-24 11:51:54.000000 pyopencga-2.9.2/pyopencga/rest_clients/admin_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-07-24 11:51:54.000000 pyopencga-2.9.2/pyopencga/rest_clients/alignment_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52128 2023-07-24 11:51:54.000000 pyopencga-2.9.2/pyopencga/rest_clients/clinical_analysis_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52556 2023-07-24 11:51:54.000000 pyopencga-2.9.2/pyopencga/rest_clients/clinical_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-07-24 11:51:54.000000 pyopencga-2.9.2/pyopencga/rest_clients/cohort_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-07-24 11:51:54.000000 pyopencga-2.9.2/pyopencga/rest_clients/disease_panel_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-07-24 11:51:54.000000 pyopencga-2.9.2/pyopencga/rest_clients/family_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26628 2023-07-24 11:51:54.000000 pyopencga-2.9.2/pyopencga/rest_clients/file_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-24 11:51:54.000000 pyopencga-2.9.2/pyopencga/rest_clients/ga4gh_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18007 2023-07-24 11:51:54.000000 pyopencga-2.9.2/pyopencga/rest_clients/individual_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-07-24 11:51:54.000000 pyopencga-2.9.2/pyopencga/rest_clients/job_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-24 11:51:54.000000 pyopencga-2.9.2/pyopencga/rest_clients/meta_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-07-24 11:51:54.000000 pyopencga-2.9.2/pyopencga/rest_clients/project_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-07-24 11:51:54.000000 pyopencga-2.9.2/pyopencga/rest_clients/sample_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-07-24 11:51:55.000000 pyopencga-2.9.2/pyopencga/rest_clients/study_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-07-24 11:51:55.000000 pyopencga-2.9.2/pyopencga/rest_clients/user_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    61336 2023-07-24 11:51:55.000000 pyopencga-2.9.2/pyopencga/rest_clients/variant_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25700 2023-07-24 11:51:55.000000 pyopencga-2.9.2/pyopencga/rest_clients/variant_operation_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-07-24 11:51:53.000000 pyopencga-2.9.2/pyopencga/rest_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-24 11:51:54.000000 pyopencga-2.9.2/pyopencga/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 11:54:11.914333 pyopencga-2.9.2/pyopencga.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-24 11:54:11.000000 pyopencga-2.9.2/pyopencga.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-24 11:54:11.000000 pyopencga-2.9.2/pyopencga.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 11:54:11.000000 pyopencga-2.9.2/pyopencga.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 11:54:11.000000 pyopencga-2.9.2/pyopencga.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 11:54:11.000000 pyopencga-2.9.2/pyopencga.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 11:54:11.918333 pyopencga-2.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-24 11:51:52.000000 pyopencga-2.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:49:12.235914 pyopencga-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-07 17:46:26.000000 pyopencga-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-03-07 17:49:12.235914 pyopencga-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-03-07 17:46:26.000000 pyopencga-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:49:12.231914 pyopencga-3.0.0/pyopencga/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-07 17:46:28.000000 pyopencga-3.0.0/pyopencga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13671 2024-03-07 17:46:28.000000 pyopencga-3.0.0/pyopencga/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-07 17:46:28.000000 pyopencga-3.0.0/pyopencga/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13389 2024-03-07 17:46:28.000000 pyopencga-3.0.0/pyopencga/opencga_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-03-07 17:46:28.000000 pyopencga-3.0.0/pyopencga/opencga_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:49:12.235914 pyopencga-3.0.0/pyopencga/rest_clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 17:46:28.000000 pyopencga-3.0.0/pyopencga/rest_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-03-07 17:46:29.000000 pyopencga-3.0.0/pyopencga/rest_clients/_parent_rest_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-03-07 17:46:29.000000 pyopencga-3.0.0/pyopencga/rest_clients/admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14511 2024-03-07 17:46:29.000000 pyopencga-3.0.0/pyopencga/rest_clients/alignment_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59985 2024-03-07 17:46:29.000000 pyopencga-3.0.0/pyopencga/rest_clients/clinical_analysis_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52556 2024-03-07 17:46:29.000000 pyopencga-3.0.0/pyopencga/rest_clients/clinical_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14689 2024-03-07 17:46:29.000000 pyopencga-3.0.0/pyopencga/rest_clients/cohort_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14182 2024-03-07 17:46:30.000000 pyopencga-3.0.0/pyopencga/rest_clients/disease_panel_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-03-07 17:46:30.000000 pyopencga-3.0.0/pyopencga/rest_clients/family_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27172 2024-03-07 17:46:30.000000 pyopencga-3.0.0/pyopencga/rest_clients/file_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-03-07 17:46:30.000000 pyopencga-3.0.0/pyopencga/rest_clients/ga4gh_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19110 2024-03-07 17:46:30.000000 pyopencga-3.0.0/pyopencga/rest_clients/individual_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-03-07 17:46:30.000000 pyopencga-3.0.0/pyopencga/rest_clients/job_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-03-07 17:46:31.000000 pyopencga-3.0.0/pyopencga/rest_clients/meta_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-03-07 17:46:31.000000 pyopencga-3.0.0/pyopencga/rest_clients/organization_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-03-07 17:46:31.000000 pyopencga-3.0.0/pyopencga/rest_clients/project_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19207 2024-03-07 17:46:31.000000 pyopencga-3.0.0/pyopencga/rest_clients/sample_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15763 2024-03-07 17:46:31.000000 pyopencga-3.0.0/pyopencga/rest_clients/study_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-03-07 17:46:31.000000 pyopencga-3.0.0/pyopencga/rest_clients/user_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61600 2024-03-07 17:46:31.000000 pyopencga-3.0.0/pyopencga/rest_clients/variant_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25932 2024-03-07 17:46:31.000000 pyopencga-3.0.0/pyopencga/rest_clients/variant_operation_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-03-07 17:46:28.000000 pyopencga-3.0.0/pyopencga/rest_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-03-07 17:46:29.000000 pyopencga-3.0.0/pyopencga/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 17:49:12.235914 pyopencga-3.0.0/pyopencga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-03-07 17:49:12.000000 pyopencga-3.0.0/pyopencga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-07 17:49:12.000000 pyopencga-3.0.0/pyopencga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 17:49:12.000000 pyopencga-3.0.0/pyopencga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-07 17:49:12.000000 pyopencga-3.0.0/pyopencga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-07 17:49:12.000000 pyopencga-3.0.0/pyopencga.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 17:49:12.235914 pyopencga-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-03-07 17:46:26.000000 pyopencga-3.0.0/setup.py
```

### Comparing `pyopencga-2.9.2/LICENSE` & `pyopencga-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopencga-2.9.2/PKG-INFO` & `pyopencga-3.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencga
-Version: 2.9.2
+Version: 3.0.0
 Summary: A REST client for OpenCGA REST web services
 Home-page: https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
 Author: David Gomez-Peregrina, Pablo Marin-Garcia, Daniel Perez-Gil
 Author-email: david.gomez@mgviz.org, pmarin@kanteron.com, dp529@cam.ac.uk
 License: Apache Software License
 Project-URL: Documentation, http://docs.opencb.org/display/opencga/Python
 Project-URL: Source, https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
@@ -17,14 +17,19 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: requests>=2.7
+Requires-Dist: pip>=7.1.2
+Requires-Dist: pathlib>=1.0.1
+Requires-Dist: pyyaml>=3.12
+Requires-Dist: pandas>=1.1.5
 
 .. contents::
 
 PyOpenCGA
 ==========
 
 This Python client package makes use of the comprehensive RESTful web services API implemented for the `OpenCGA`_ platform.
```

### Comparing `pyopencga-2.9.2/README.rst` & `pyopencga-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyopencga-2.9.2/pyopencga/commons.py` & `pyopencga-3.0.0/pyopencga/commons.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.9.2/pyopencga/opencga_client.py` & `pyopencga-3.0.0/pyopencga/opencga_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.9.2/pyopencga/opencga_config.py` & `pyopencga-3.0.0/pyopencga/opencga_config.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.9.2/pyopencga/rest_clients/_parent_rest_clients.py` & `pyopencga-3.0.0/pyopencga/rest_clients/_parent_rest_clients.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.9.2/pyopencga/rest_clients/admin_client.py` & `pyopencga-3.0.0/pyopencga/rest_clients/admin_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-04-18
+    Autogenerated on: 2024-03-06
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Admin(_ParentRestClient):
     """
     This class contains methods for the 'Admin' webservices
-    Client version: 2.8.0-SNAPSHOT
+    Client version: 3.0.0-SNAPSHOT
     PATH: /{apiVersion}/admin
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Admin, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def group_by_audit(self, fields, entity, **options):
         """
         Group by operation.
         PATH: /{apiVersion}/admin/audit/groupBy
 
         :param str entity: Entity to be grouped by. Allowed values: ['AUDIT
-            USER PROJECT STUDY FILE SAMPLE JOB INDIVIDUAL COHORT DISEASE_PANEL
-            FAMILY CLINICAL_ANALYSIS INTERPRETATION VARIANT ALIGNMENT CLINICAL
-            EXPRESSION RGA FUNCTIONAL'] (REQUIRED)
+            ORGANIZATION USER PROJECT STUDY FILE SAMPLE JOB INDIVIDUAL COHORT
+            DISEASE_PANEL FAMILY CLINICAL_ANALYSIS INTERPRETATION VARIANT
+            ALIGNMENT CLINICAL EXPRESSION RGA FUNCTIONAL'] (REQUIRED)
         :param str fields: Comma separated list of fields by which to group
             by. (REQUIRED)
         :param bool count: Count the number of elements matching the group.
         :param int limit: Maximum number of documents (groups) to be returned.
         :param str action: Action performed.
         :param str before: Object before update.
         :param str after: Object after update.
@@ -41,26 +41,14 @@
             yyyyMMddHHmmss-yyyyMMddHHmmss.
         """
 
         options['fields'] = fields
         options['entity'] = entity
         return self._get(category='admin', resource='groupBy', subcategory='audit', **options)
 
-    def index_stats_catalog(self, **options):
-        """
-        Sync Catalog into the Solr.
-        PATH: /{apiVersion}/admin/catalog/indexStats
-
-        :param str collection: Collection to be indexed (file, sample,
-            individual, family, cohort and/or job). If not provided, all of
-            them will be indexed.
-        """
-
-        return self._post(category='admin', resource='indexStats', subcategory='catalog', **options)
-
     def install_catalog(self, data=None, **options):
         """
         Install OpenCGA database.
         PATH: /{apiVersion}/admin/catalog/install
 
         :param dict data: JSON containing the mandatory parameters. (REQUIRED)
         """
@@ -69,14 +57,15 @@
 
     def jwt_catalog(self, data=None, **options):
         """
         Change JWT secret key.
         PATH: /{apiVersion}/admin/catalog/jwt
 
         :param dict data: JSON containing the parameters. (REQUIRED)
+        :param str organization: Organization id.
         """
 
         return self._post(category='admin', resource='jwt', subcategory='catalog', data=data, **options)
 
     def create_users(self, data=None, **options):
         """
         Create a new user.
@@ -89,42 +78,74 @@
 
     def import_users(self, data=None, **options):
         """
         Import users or a group of users from LDAP or AAD.
         PATH: /{apiVersion}/admin/users/import
 
         :param dict data: JSON containing the parameters. (REQUIRED)
+        :param str organization: Organization id.
         """
 
         return self._post(category='admin', resource='import', subcategory='users', data=data, **options)
 
+    def permissions_users(self, **options):
+        """
+        User permissions.
+        PATH: /{apiVersion}/admin/users/permissions
+
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
+        :param str entry_ids: Comma separated list of entry ids.
+        :param str permissions: Comma separated list of permissions to be
+            retrieved.
+        :param str category: Category corresponding to the id's provided.
+        """
+
+        return self._get(category='admin', resource='permissions', subcategory='users', **options)
+
     def search_users(self, **options):
         """
         User search method.
         PATH: /{apiVersion}/admin/users/search
 
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param int limit: Number of results to be returned.
         :param int skip: Number of results to skip.
         :param bool count: Get the total number of results matching the query.
             Deactivated by default.
+        :param str organization: Organization id.
         :param str user: User ID.
         :param str account: Account type [GUEST, FULL, ADMINISTRATOR].
         :param str authentication_id: Authentication origin ID.
         """
 
         return self._get(category='admin', resource='search', subcategory='users', **options)
 
     def sync_users(self, data=None, **options):
         """
         Synchronise a group of users from an authentication origin with a
             group in a study from catalog.
         PATH: /{apiVersion}/admin/users/sync
 
         :param dict data: JSON containing the parameters. (REQUIRED)
+        :param str organization: Organization id.
         """
 
         return self._post(category='admin', resource='sync', subcategory='users', data=data, **options)
 
+    def users_update_groups(self, user, data=None, **options):
+        """
+        Add or remove users from existing groups.
+        PATH: /{apiVersion}/admin/users/{user}/groups/update
+
+        :param dict data: JSON containing the parameters. (REQUIRED)
+        :param str user: User ID. (REQUIRED)
+        :param str organization: Organization id.
+        :param str action: Action to be performed: ADD or REMOVE user to/from
+            groups. Allowed values: ['ADD REMOVE']
+        """
+
+        return self._post(category='admin/users', resource='update', query_id=user, subcategory='groups', data=data, **options)
+
```

### Comparing `pyopencga-2.9.2/pyopencga/rest_clients/alignment_client.py` & `pyopencga-3.0.0/pyopencga/rest_clients/alignment_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-04-18
+    Autogenerated on: 2024-03-06
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Alignment(_ParentRestClient):
     """
     This class contains methods for the 'Analysis - Alignment' webservices
-    Client version: 2.8.0-SNAPSHOT
+    Client version: 3.0.0-SNAPSHOT
     PATH: /{apiVersion}/analysis/alignment
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Alignment, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def run_bwa(self, data=None, **options):
@@ -77,16 +77,16 @@
 
     def query_coverage(self, file, **options):
         """
         Query the coverage of an alignment file for regions or genes.
         PATH: /{apiVersion}/analysis/alignment/coverage/query
 
         :param str file: File ID. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str region: Comma separated list of regions 'chr:start-end,
             e.g.: 2,3:63500-65000.
         :param str gene: Comma separated list of genes, e.g.: BCRA2,TP53.
         :param int offset: Offset to extend the region, gene or exon at up and
             downstream.
         :param bool only_exons: Only exons are taking into account when genes
             are specified.
@@ -107,16 +107,16 @@
         """
         Compute coverage ratio from file #1 vs file #2, (e.g. somatic vs
             germline).
         PATH: /{apiVersion}/analysis/alignment/coverage/ratio
 
         :param str file2: Input file #2 (e.g. germline file). (REQUIRED)
         :param str file1: Input file #1 (e.g. somatic file). (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool skip_log2: Do not apply Log2 to normalise the coverage
             ratio.
         :param str region: Comma separated list of regions 'chr:start-end,
             e.g.: 2,3:63500-65000.
         :param str gene: Comma separated list of genes, e.g.: BCRA2,TP53.
         :param int offset: Offset to extend the region, gene or exon at up and
             downstream.
@@ -136,16 +136,16 @@
         """
         Compute coverage stats per transcript for a list of genes.
         PATH: /{apiVersion}/analysis/alignment/coverage/stats
 
         :param str gene: Comma separated list of genes, e.g.: BCRA2,TP53.
             (REQUIRED)
         :param str file: File ID. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param int threshold: Only regions whose coverage depth is under this
             threshold will be reported.
         """
 
         options['file'] = file
         options['gene'] = gene
         return self._get(category='analysis', resource='stats', subcategory='alignment/coverage', **options)
@@ -253,16 +253,16 @@
         PATH: /{apiVersion}/analysis/alignment/query
 
         :param str file: File ID. (REQUIRED)
         :param int limit: Number of results to be returned.
         :param int skip: Number of results to skip.
         :param bool count: Get the total number of results matching the query.
             Deactivated by default.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str region: Comma separated list of regions 'chr:start-end,
             e.g.: 2,3:63500-65000.
         :param str gene: Comma separated list of genes, e.g.: BCRA2,TP53.
         :param int offset: Offset to extend the region, gene or exon at up and
             downstream.
         :param bool only_exons: Only exons are taking into account when genes
             are specified.
```

### Comparing `pyopencga-2.9.2/pyopencga/rest_clients/clinical_analysis_client.py` & `pyopencga-3.0.0/pyopencga/rest_clients/clinical_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-04-18
+    Autogenerated on: 2022-08-02 08:25:32
+>>>>>>> develop
+>>>>>>> release-2.4.x
+>>>>>>> release-2.4.x
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
-class ClinicalAnalysis(_ParentRestClient):
+class Clinical(_ParentRestClient):
     """
     This class contains methods for the 'Analysis - Clinical' webservices
-    Client version: 2.8.0-SNAPSHOT
+    Client version: 2.3.3-SNAPSHOT [fb5e7ed17448243b10ddd619bdf973e4b20b0a74]
+>>>>>>> develop
+>>>>>>> release-2.4.x
+>>>>>>> release-2.4.x
     PATH: /{apiVersion}/analysis/clinical
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
-        super(ClinicalAnalysis, self).__init__(configuration, token, login_handler, *args, **kwargs)
+        super(Clinical, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
         """
         Update the set of permissions granted for the member.
         PATH: /{apiVersion}/analysis/clinical/acl/{members}/update
 
         :param dict data: JSON containing the parameters to add ACLs.
             (REQUIRED)
         :param str action: Action to be performed [ADD, SET, REMOVE or RESET].
-            Allowed values: ['SET ADD REMOVE RESET'] (REQUIRED)
+            (REQUIRED)
         :param str members: Comma separated list of user or group IDs.
             (REQUIRED)
         :param str study: Study [[user@]project:]study where study and project
             can be either the ID or UUID.
         :param bool propagate: Propagate permissions to related families,
             individuals, samples and files.
         """
@@ -77,16 +83,16 @@
         return self._post(category='analysis', resource='create', subcategory='clinical', data=data, **options)
 
     def distinct(self, field, **options):
         """
         Clinical Analysis distinct method.
         PATH: /{apiVersion}/analysis/clinical/distinct
 
-        :param str field: Comma separated list of fields for which to obtain
-            the distinct values. (REQUIRED)
+        :param str field: Field for which to obtain the distinct values.
+            (REQUIRED)
         :param str study: Study [[user@]project:]study where study and project
             can be either the ID or UUID.
         :param str id: Comma separated list of Clinical Analysis IDs up to a
             maximum of 100.
         :param str uuid: Comma separated list of Clinical Analysis UUIDs up to
             a maximum of 100.
         :param str type: Clinical Analysis type.
@@ -124,16 +130,16 @@
         return self._get(category='analysis', resource='distinct', subcategory='clinical', **options)
 
     def distinct_interpretation(self, field, **options):
         """
         Interpretation distinct method.
         PATH: /{apiVersion}/analysis/clinical/interpretation/distinct
 
-        :param str field: Comma separated list of fields for which to obtain
-            the distinct values. (REQUIRED)
+        :param str field: Field for which to obtain the distinct values.
+            (REQUIRED)
         :param str study: Study [[user@]project:]study where study and project
             can be either the ID or UUID.
         :param str id: Comma separated list of Interpretation IDs up to a
             maximum of 100.
         :param str uuid: Comma separated list of Interpretation UUIDs up to a
             maximum of 100.
         :param str clinical_analysis_id: Clinical Analysis id.
@@ -638,14 +644,26 @@
         :param str status: Filter by status.
         :param str internal_status: Filter by internal status.
         :param bool deleted: Boolean to retrieve deleted entries.
         """
 
         return self._get(category='analysis', resource='search', subcategory='clinical', **options)
 
+    def actionable_variant(self, **options):
+        """
+        Fetch actionable clinical variants.
+        PATH: /{apiVersion}/analysis/clinical/variant/actionable
+
+        :param str study: Study [[user@]project:]study where study and project
+            can be either the ID or UUID.
+        :param str sample: Sample ID.
+        """
+
+        return self._get(category='analysis', resource='actionable', subcategory='clinical/variant', **options)
+
     def query_variant(self, **options):
         """
         Fetch clinical variants.
         PATH: /{apiVersion}/analysis/clinical/variant/query
 
         :param str include: Fields included in the response, whole JSON path
             must be provided.
@@ -657,16 +675,14 @@
             Deactivated by default.
         :param bool approximate_count: Get an approximate count, instead of an
             exact total count. Reduces execution time.
         :param int approximate_count_sampling_size: Sampling size to get the
             approximate count. Larger values increase accuracy but also
             increase execution time.
         :param str saved_filter: Use a saved filter at User level.
-        :param str include_interpretation: Interpretation ID to include the
-            fields related to this interpretation.
         :param str id: List of IDs, these can be rs IDs (dbSNP) or variants in
             the format chrom:start:ref:alt, e.g. rs116600158,19:7177679:C:T.
         :param str region: List of regions, these can be just a single
             chromosome name or regions in the format chr:start-end, e.g.:
             2,3:100000-200000.
         :param str type: List of types, accepted values are SNV, MNV, INDEL,
             SV, COPY_NUMBER, COPY_NUMBER_LOSS, COPY_NUMBER_GAIN, INSERTION,
@@ -699,17 +715,16 @@
             allele will match, regardless of its position e.g. 1/2 will match
             with genotypes 1/2, 1/3, 1/4, .... Genotype aliases accepted:
             HOM_REF, HOM_ALT, HET, HET_REF, HET_ALT, HET_MISS and MISS  e.g.
             HG0097:HOM_REF;HG0098:HET_REF,HOM_ALT . 3) Sample with segregation
             mode: {sample}:{segregation}. Only one sample accepted.Accepted
             segregation modes: [ autosomalDominant, autosomalRecessive,
             XLinkedDominant, XLinkedRecessive, YLinked, mitochondrial, deNovo,
-            deNovoStrict, mendelianError, compoundHeterozygous ]. Value is case
-            insensitive. e.g. HG0097:DeNovo Sample must have parents defined
-            and indexed. .
+            mendelianError, compoundHeterozygous ]. Value is case insensitive.
+            e.g. HG0097:DeNovo Sample must have parents defined and indexed. .
         :param str sample_data: Filter by any SampleData field from samples.
             [{sample}:]{key}{op}{value}[,;]* . If no sample is specified, will
             use all samples from 'sample' or 'genotype' filter. e.g. DP>200 or
             HG0097:DP>200,HG0098:DP<10 . Many FORMAT fields can be combined.
             e.g. HG0097:DP>200;GT=1/1,0/1,HG0098:DP<10.
         :param str sample_annotation: Selects some samples using metadata
             information from Catalog. e.g.
@@ -735,15 +750,15 @@
         :param str family: Filter variants where any of the samples from the
             given family contains the variant (HET or HOM_ALT).
         :param str family_disorder: Specify the disorder to use for the family
             segregation.
         :param str family_segregation: Filter by segregation mode from a given
             family. Accepted values: [ autosomalDominant, autosomalRecessive,
             XLinkedDominant, XLinkedRecessive, YLinked, mitochondrial, deNovo,
-            deNovoStrict, mendelianError, compoundHeterozygous ].
+            mendelianError, compoundHeterozygous ].
         :param str family_members: Sub set of the members of a given family.
         :param str family_proband: Specify the proband child to use for the
             family segregation.
         :param str gene: List of genes, most gene IDs are accepted (HGNC,
             Ensembl gene, ...). This is an alias to 'xref' parameter.
         :param str ct: List of SO consequence types, e.g.
             missense_variant,stop_lost or SO:0001583,SO:0001578. Accepts
@@ -853,21 +868,22 @@
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param str study: Study [[user@]project:]study where study and project
             can be either the ID or UUID.
         :param str comments_action: Action to be performed if the array of
-            comments is being updated. Allowed values: ['ADD REMOVE REPLACE']
+            comments is being updated. Allowed values: ['ADD', 'REMOVE',
+            'REPLACE']
         :param str flags_action: Action to be performed if the array of flags
-            is being updated. Allowed values: ['ADD SET REMOVE']
+            is being updated. Allowed values: ['ADD', 'SET', 'REMOVE']
         :param str files_action: Action to be performed if the array of files
-            is being updated. Allowed values: ['ADD SET REMOVE']
+            is being updated. Allowed values: ['ADD', 'SET', 'REMOVE']
         :param str panels_action: Action to be performed if the array of
-            panels is being updated. Allowed values: ['ADD SET REMOVE']
+            panels is being updated. Allowed values: ['ADD', 'SET', 'REMOVE']
         :param bool include_result: Flag indicating to include the created or
             updated document result in the response.
         """
 
         return self._post(category='analysis', resource='update', subcategory='clinical', second_query_id=clinical_analyses, data=data, **options)
 
     def info(self, clinical_analysis, **options):
@@ -897,16 +913,16 @@
             (REQUIRED)
         :param str clinical_analysis: Clinical analysis ID. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param str study: [[user@]project:]study id.
-        :param str set_as: Set interpretation as. Allowed values: ['PRIMARY
-            SECONDARY']
+        :param str set_as: Set interpretation as. Allowed values: ['PRIMARY',
+            'SECONDARY']
         :param bool include_result: Flag indicating to include the created or
             updated document result in the response.
         """
 
         return self._post(category='analysis/clinical', resource='create', query_id=clinical_analysis, subcategory='interpretation', data=data, **options)
 
     def clear_interpretation(self, clinical_analysis, interpretations, **options):
@@ -962,28 +978,28 @@
         :param str clinical_analysis: Clinical analysis ID. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param str study: [[user@]project:]study ID.
         :param str primary_findings_action: Action to be performed if the
-            array of primary findings is being updated. Allowed values: ['ADD
-            SET REMOVE REPLACE']
+            array of primary findings is being updated. Allowed values: ['ADD',
+            'SET', 'REMOVE', 'REPLACE']
         :param str methods_action: Action to be performed if the array of
-            methods is being updated. Allowed values: ['ADD SET REMOVE']
+            methods is being updated. Allowed values: ['ADD', 'SET', 'REMOVE']
         :param str secondary_findings_action: Action to be performed if the
-            array of secondary findings is being updated. Allowed values: ['ADD
-            SET REMOVE REPLACE']
+            array of secondary findings is being updated. Allowed values:
+            ['ADD', 'SET', 'REMOVE', 'REPLACE']
         :param str comments_action: Action to be performed if the array of
             comments is being updated. To REMOVE or REPLACE, the date will need
-            to be provided to identify the comment. Allowed values: ['ADD
-            REMOVE REPLACE']
+            to be provided to identify the comment. Allowed values: ['ADD',
+            'REMOVE', 'REPLACE']
         :param str panels_action: Action to be performed if the array of
-            panels is being updated. Allowed values: ['ADD SET REMOVE']
-        :param str set_as: Set interpretation as. Allowed values: ['PRIMARY
-            SECONDARY']
+            panels is being updated. Allowed values: ['ADD', 'SET', 'REMOVE']
+        :param str set_as: Set interpretation as. Allowed values: ['PRIMARY',
+            'SECONDARY']
         :param bool include_result: Flag indicating to include the created or
             updated document result in the response.
         """
 
         return self._post(category='analysis/clinical', resource='update', query_id=clinical_analysis, subcategory='interpretation', second_query_id=interpretation, data=data, **options)
```

### Comparing `pyopencga-2.9.2/pyopencga/rest_clients/clinical_client.py` & `pyopencga-3.0.0/pyopencga/rest_clients/clinical_analysis_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,80 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2022-08-02 08:25:32
->>>>>>> develop
->>>>>>> release-2.4.x
->>>>>>> release-2.4.x
+    Autogenerated on: 2024-03-06
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
-class Clinical(_ParentRestClient):
+class ClinicalAnalysis(_ParentRestClient):
     """
     This class contains methods for the 'Analysis - Clinical' webservices
-    Client version: 2.3.3-SNAPSHOT [fb5e7ed17448243b10ddd619bdf973e4b20b0a74]
->>>>>>> develop
->>>>>>> release-2.4.x
->>>>>>> release-2.4.x
+    Client version: 3.0.0-SNAPSHOT
     PATH: /{apiVersion}/analysis/clinical
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
-        super(Clinical, self).__init__(configuration, token, login_handler, *args, **kwargs)
+        super(ClinicalAnalysis, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
         """
         Update the set of permissions granted for the member.
         PATH: /{apiVersion}/analysis/clinical/acl/{members}/update
 
         :param dict data: JSON containing the parameters to add ACLs.
             (REQUIRED)
         :param str action: Action to be performed [ADD, SET, REMOVE or RESET].
-            (REQUIRED)
+            Allowed values: ['SET ADD REMOVE RESET'] (REQUIRED)
         :param str members: Comma separated list of user or group IDs.
             (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool propagate: Propagate permissions to related families,
             individuals, samples and files.
         """
 
         options['action'] = action
         return self._post(category='analysis', resource='update', subcategory='clinical/acl', second_query_id=members, data=data, **options)
 
+    def load_annotation_sets(self, variable_set_id, path, data=None, **options):
+        """
+        Load annotation sets from a TSV file.
+        PATH: /{apiVersion}/analysis/clinical/annotationSets/load
+
+        :param str path: Path where the TSV file is located in OpenCGA or
+            where it should be located. (REQUIRED)
+        :param str variable_set_id: Variable set ID or name. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
+        :param bool parents: Flag indicating whether to create parent
+            directories if they don't exist (only when TSV file was not
+            previously associated).
+        :param str annotation_set_id: Annotation set id. If not provided,
+            variableSetId will be used.
+        :param dict data: JSON containing the 'content' of the TSV file if
+            this has not yet been registered into OpenCGA.
+        """
+
+        options['variableSetId'] = variable_set_id
+        options['path'] = path
+        return self._post(category='analysis', resource='load', subcategory='clinical/annotationSets', data=data, **options)
+
     def update_clinical_configuration(self, data=None, **options):
         """
         Update Clinical Analysis configuration.
         PATH: /{apiVersion}/analysis/clinical/clinical/configuration/update
 
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param dict data: Configuration params to update.
         """
 
         return self._post(category='analysis', resource='update', subcategory='clinical/clinical/configuration', data=data, **options)
 
     def create(self, data=None, **options):
         """
@@ -66,16 +83,16 @@
 
         :param dict data: JSON containing clinical analysis information.
             (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool skip_create_default_interpretation: Flag to skip creating
             and initialise an empty default primary interpretation (Id will be
             '{clinicalAnalysisId}.1'). This flag is only considered if no
             Interpretation object is passed.
         :param bool include_result: Flag indicating to include the created or
             updated document result in the response.
         """
@@ -83,24 +100,29 @@
         return self._post(category='analysis', resource='create', subcategory='clinical', data=data, **options)
 
     def distinct(self, field, **options):
         """
         Clinical Analysis distinct method.
         PATH: /{apiVersion}/analysis/clinical/distinct
 
-        :param str field: Field for which to obtain the distinct values.
-            (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str field: Comma separated list of fields for which to obtain
+            the distinct values. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str id: Comma separated list of Clinical Analysis IDs up to a
-            maximum of 100.
+            maximum of 100. Also admits basic regular expressions using the
+            operator '~', i.e. '~{perl-regex}' e.g. '~value' for case
+            sensitive, '~/value/i' for case insensitive search.
         :param str uuid: Comma separated list of Clinical Analysis UUIDs up to
             a maximum of 100.
         :param str type: Clinical Analysis type.
-        :param str disorder: Clinical Analysis disorder.
+        :param str disorder: Clinical Analysis disorder. Also admits basic
+            regular expressions using the operator '~', i.e. '~{perl-regex}'
+            e.g. '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
         :param str files: Clinical Analysis files.
         :param str sample: Sample associated to the proband or any member of a
             family.
         :param str individual: Proband or any member of a family.
         :param str proband: Clinical Analysis proband.
         :param str proband_samples: Clinical Analysis proband samples.
         :param str family: Clinical Analysis family.
@@ -119,36 +141,44 @@
         :param str due_date: Clinical Analysis due date. Format:
             yyyyMMddHHmmss. Examples: >2018, 2017-2018, <201805.
         :param str quality_control_summary: Clinical Analysis quality control
             summary.
         :param str release: Release when it was created.
         :param str status: Filter by status.
         :param str internal_status: Filter by internal status.
+        :param str annotation: Annotation filters. Example:
+            age>30;gender=FEMALE. For more information, please visit
+            http://docs.opencb.org/display/opencga/AnnotationSets+1.4.0.
         :param bool deleted: Boolean to retrieve deleted entries.
         """
 
         options['field'] = field
         return self._get(category='analysis', resource='distinct', subcategory='clinical', **options)
 
     def distinct_interpretation(self, field, **options):
         """
         Interpretation distinct method.
         PATH: /{apiVersion}/analysis/clinical/interpretation/distinct
 
-        :param str field: Field for which to obtain the distinct values.
-            (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str field: Comma separated list of fields for which to obtain
+            the distinct values. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str id: Comma separated list of Interpretation IDs up to a
-            maximum of 100.
+            maximum of 100. Also admits basic regular expressions using the
+            operator '~', i.e. '~{perl-regex}' e.g. '~value' for case
+            sensitive, '~/value/i' for case insensitive search.
         :param str uuid: Comma separated list of Interpretation UUIDs up to a
             maximum of 100.
         :param str clinical_analysis_id: Clinical Analysis id.
         :param str analyst_id: Analyst ID.
-        :param str method_name: Interpretation method name.
+        :param str method_name: Interpretation method name. Also admits basic
+            regular expressions using the operator '~', i.e. '~{perl-regex}'
+            e.g. '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
         :param str panels: Interpretation panels.
         :param str primary_findings: Interpretation primary findings.
         :param str secondary_findings: Interpretation secondary findings.
         :param str creation_date: Interpretation Creation date. Format:
             yyyyMMddHHmmss. Examples: >2018, 2017-2018, <201805.
         :param str modification_date: Interpretation Modification date.
             Format: yyyyMMddHHmmss. Examples: >2018, 2017-2018, <201805.
@@ -168,23 +198,28 @@
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param int limit: Number of results to be returned.
         :param int skip: Number of results to skip.
         :param bool sort: Sort the results.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str id: Comma separated list of Interpretation IDs up to a
-            maximum of 100.
+            maximum of 100. Also admits basic regular expressions using the
+            operator '~', i.e. '~{perl-regex}' e.g. '~value' for case
+            sensitive, '~/value/i' for case insensitive search.
         :param str uuid: Comma separated list of Interpretation UUIDs up to a
             maximum of 100.
         :param str clinical_analysis_id: Clinical Analysis id.
         :param str analyst_id: Analyst ID.
-        :param str method_name: Interpretation method name.
+        :param str method_name: Interpretation method name. Also admits basic
+            regular expressions using the operator '~', i.e. '~{perl-regex}'
+            e.g. '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
         :param str panels: Interpretation panels.
         :param str primary_findings: Interpretation primary findings.
         :param str secondary_findings: Interpretation secondary findings.
         :param str creation_date: Interpretation Creation date. Format:
             yyyyMMddHHmmss. Examples: >2018, 2017-2018, <201805.
         :param str modification_date: Interpretation Modification date.
             Format: yyyyMMddHHmmss. Examples: >2018, 2017-2018, <201805.
@@ -202,16 +237,16 @@
 
         :param str interpretations: Comma separated list of clinical
             interpretation IDs  up to a maximum of 100. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str version: Comma separated list of interpretation versions.
             'all' to get all the interpretation versions. Not supported if
             multiple interpretation ids are provided.
         :param bool deleted: Boolean to retrieve deleted entries.
         """
 
         return self._get(category='analysis', resource='info', subcategory='clinical/interpretation', second_query_id=interpretations, **options)
@@ -219,16 +254,16 @@
     def run_interpreter_cancer_tiering(self, data=None, **options):
         """
         Run cancer tiering interpretation analysis.
         PATH: /{apiVersion}/analysis/clinical/interpreter/cancerTiering/run
 
         :param dict data: Cancer tiering interpretation analysis params.
             (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -237,16 +272,16 @@
 
     def run_interpreter_exomiser(self, data=None, **options):
         """
         Run exomiser interpretation analysis.
         PATH: /{apiVersion}/analysis/clinical/interpreter/exomiser/run
 
         :param dict data: Exomizer interpretation analysis params. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -255,16 +290,16 @@
 
     def run_interpreter_team(self, data=None, **options):
         """
         Run TEAM interpretation analysis.
         PATH: /{apiVersion}/analysis/clinical/interpreter/team/run
 
         :param dict data: TEAM interpretation analysis params. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -273,16 +308,16 @@
 
     def run_interpreter_tiering(self, data=None, **options):
         """
         Run tiering interpretation analysis.
         PATH: /{apiVersion}/analysis/clinical/interpreter/tiering/run
 
         :param dict data: Tiering interpretation analysis params. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -291,26 +326,45 @@
 
     def run_interpreter_zetta(self, data=None, **options):
         """
         Run Zetta interpretation analysis.
         PATH: /{apiVersion}/analysis/clinical/interpreter/zetta/run
 
         :param dict data: Zetta interpretation analysis params. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
 
         return self._post(category='analysis', resource='run', subcategory='clinical/interpreter/zetta', data=data, **options)
 
+    def load(self, data=None, **options):
+        """
+        Load clinical analyses from a file.
+        PATH: /{apiVersion}/analysis/clinical/load
+
+        :param dict data: Parameters to load clinical analysis in OpenCGA
+            catalog from a file. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
+        :param str job_id: Job ID. It must be a unique string within the
+            study. An ID will be autogenerated automatically if not provided.
+        :param str job_description: Job description.
+        :param str job_depends_on: Comma separated list of existing job IDs
+            the job will depend on.
+        :param str job_tags: Job tags.
+        """
+
+        return self._post(category='analysis', resource='load', subcategory='clinical', data=data, **options)
+
     def aggregation_stats_rga(self, field, **options):
         """
         RGA aggregation stats.
         PATH: /{apiVersion}/analysis/clinical/rga/aggregationStats
 
         :param str field: List of fields separated by semicolons, e.g.:
             clinicalSignificances;type. For nested fields use >>, e.g.:
@@ -333,16 +387,16 @@
         :param str db_snps: Filter by DB_SNP id.
         :param str knockout_type: Filter by knockout type.
         :param str filter: Filter by filter (PASS, NOT_PASS).
         :param str type: Filter by variant type.
         :param str clinical_significance: Filter by clinical significance.
         :param str population_frequency: Filter by population frequency.
         :param str consequence_type: Filter by consequence type.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         options['field'] = field
         return self._get(category='analysis', resource='aggregationStats', subcategory='clinical/rga', **options)
 
     def query_rga_gene(self, **options):
         """
@@ -378,16 +432,16 @@
         :param str db_snps: Filter by DB_SNP id.
         :param str knockout_type: Filter by knockout type.
         :param str filter: Filter by filter (PASS, NOT_PASS).
         :param str type: Filter by variant type.
         :param str clinical_significance: Filter by clinical significance.
         :param str population_frequency: Filter by population frequency.
         :param str consequence_type: Filter by consequence type.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         return self._get(category='analysis', resource='query', subcategory='clinical/rga/gene', **options)
 
     def summary_rga_gene(self, **options):
         """
         RGA gene summary stats.
@@ -413,28 +467,28 @@
         :param str db_snps: Filter by DB_SNP id.
         :param str knockout_type: Filter by knockout type.
         :param str filter: Filter by filter (PASS, NOT_PASS).
         :param str type: Filter by variant type.
         :param str clinical_significance: Filter by clinical significance.
         :param str population_frequency: Filter by population frequency.
         :param str consequence_type: Filter by consequence type.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         return self._get(category='analysis', resource='summary', subcategory='clinical/rga/gene', **options)
 
     def run_rga_index(self, data=None, **options):
         """
         Generate Recessive Gene Analysis secondary index.
         PATH: /{apiVersion}/analysis/clinical/rga/index/run
 
         :param dict data: Recessive Gene Analysis index params. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         :param bool auxiliar_index: Index auxiliar collection to improve
@@ -472,16 +526,16 @@
         :param str db_snps: Filter by DB_SNP id.
         :param str knockout_type: Filter by knockout type.
         :param str filter: Filter by filter (PASS, NOT_PASS).
         :param str type: Filter by variant type.
         :param str clinical_significance: Filter by clinical significance.
         :param str population_frequency: Filter by population frequency.
         :param str consequence_type: Filter by consequence type.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         return self._get(category='analysis', resource='query', subcategory='clinical/rga/individual', **options)
 
     def summary_rga_individual(self, **options):
         """
         RGA individual summary stats.
@@ -507,16 +561,16 @@
         :param str db_snps: Filter by DB_SNP id.
         :param str knockout_type: Filter by knockout type.
         :param str filter: Filter by filter (PASS, NOT_PASS).
         :param str type: Filter by variant type.
         :param str clinical_significance: Filter by clinical significance.
         :param str population_frequency: Filter by population frequency.
         :param str consequence_type: Filter by consequence type.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         return self._get(category='analysis', resource='summary', subcategory='clinical/rga/individual', **options)
 
     def query_rga_variant(self, **options):
         """
         Query variant RGA.
@@ -551,16 +605,16 @@
         :param str db_snps: Filter by DB_SNP id.
         :param str knockout_type: Filter by knockout type.
         :param str filter: Filter by filter (PASS, NOT_PASS).
         :param str type: Filter by variant type.
         :param str clinical_significance: Filter by clinical significance.
         :param str population_frequency: Filter by population frequency.
         :param str consequence_type: Filter by consequence type.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         return self._get(category='analysis', resource='query', subcategory='clinical/rga/variant', **options)
 
     def summary_rga_variant(self, **options):
         """
         RGA variant summary stats.
@@ -586,16 +640,16 @@
         :param str db_snps: Filter by DB_SNP id.
         :param str knockout_type: Filter by knockout type.
         :param str filter: Filter by filter (PASS, NOT_PASS).
         :param str type: Filter by variant type.
         :param str clinical_significance: Filter by clinical significance.
         :param str population_frequency: Filter by population frequency.
         :param str consequence_type: Filter by consequence type.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         return self._get(category='analysis', resource='summary', subcategory='clinical/rga/variant', **options)
 
     def search(self, **options):
         """
         Clinical analysis search.
@@ -605,22 +659,28 @@
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param int limit: Number of results to be returned.
         :param int skip: Number of results to skip.
         :param bool count: Get the total number of results matching the query.
             Deactivated by default.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param bool flatten_annotations: Flatten the annotations?.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str id: Comma separated list of Clinical Analysis IDs up to a
-            maximum of 100.
+            maximum of 100. Also admits basic regular expressions using the
+            operator '~', i.e. '~{perl-regex}' e.g. '~value' for case
+            sensitive, '~/value/i' for case insensitive search.
         :param str uuid: Comma separated list of Clinical Analysis UUIDs up to
             a maximum of 100.
         :param str type: Clinical Analysis type.
-        :param str disorder: Clinical Analysis disorder.
+        :param str disorder: Clinical Analysis disorder. Also admits basic
+            regular expressions using the operator '~', i.e. '~{perl-regex}'
+            e.g. '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
         :param str files: Clinical Analysis files.
         :param str sample: Sample associated to the proband or any member of a
             family.
         :param str individual: Proband or any member of a family.
         :param str proband: Clinical Analysis proband.
         :param str proband_samples: Clinical Analysis proband samples.
         :param str family: Clinical Analysis family.
@@ -639,31 +699,22 @@
         :param str due_date: Clinical Analysis due date. Format:
             yyyyMMddHHmmss. Examples: >2018, 2017-2018, <201805.
         :param str quality_control_summary: Clinical Analysis quality control
             summary.
         :param str release: Release when it was created.
         :param str status: Filter by status.
         :param str internal_status: Filter by internal status.
+        :param str annotation: Annotation filters. Example:
+            age>30;gender=FEMALE. For more information, please visit
+            http://docs.opencb.org/display/opencga/AnnotationSets+1.4.0.
         :param bool deleted: Boolean to retrieve deleted entries.
         """
 
         return self._get(category='analysis', resource='search', subcategory='clinical', **options)
 
-    def actionable_variant(self, **options):
-        """
-        Fetch actionable clinical variants.
-        PATH: /{apiVersion}/analysis/clinical/variant/actionable
-
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
-        :param str sample: Sample ID.
-        """
-
-        return self._get(category='analysis', resource='actionable', subcategory='clinical/variant', **options)
-
     def query_variant(self, **options):
         """
         Fetch clinical variants.
         PATH: /{apiVersion}/analysis/clinical/variant/query
 
         :param str include: Fields included in the response, whole JSON path
             must be provided.
@@ -675,26 +726,28 @@
             Deactivated by default.
         :param bool approximate_count: Get an approximate count, instead of an
             exact total count. Reduces execution time.
         :param int approximate_count_sampling_size: Sampling size to get the
             approximate count. Larger values increase accuracy but also
             increase execution time.
         :param str saved_filter: Use a saved filter at User level.
+        :param str include_interpretation: Interpretation ID to include the
+            fields related to this interpretation.
         :param str id: List of IDs, these can be rs IDs (dbSNP) or variants in
             the format chrom:start:ref:alt, e.g. rs116600158,19:7177679:C:T.
         :param str region: List of regions, these can be just a single
             chromosome name or regions in the format chr:start-end, e.g.:
             2,3:100000-200000.
         :param str type: List of types, accepted values are SNV, MNV, INDEL,
             SV, COPY_NUMBER, COPY_NUMBER_LOSS, COPY_NUMBER_GAIN, INSERTION,
             DELETION, DUPLICATION, TANDEM_DUPLICATION, BREAKEND, e.g.
             SNV,INDEL.
         :param str study: Filter variants from the given studies, these can be
             either the numeric ID or the alias with the format
-            user@project:study.
+            organization@project:study.
         :param str file: Filter variants from the files specified. This will
             set includeFile parameter when not provided.
         :param str filter: Specify the FILTER for any of the files. If 'file'
             filter is provided, will match the file and the filter. e.g.:
             PASS,LowGQX.
         :param str qual: Specify the QUAL for any of the files. If 'file'
             filter is provided, will match the file and the qual. e.g.: >123.4.
@@ -715,16 +768,17 @@
             allele will match, regardless of its position e.g. 1/2 will match
             with genotypes 1/2, 1/3, 1/4, .... Genotype aliases accepted:
             HOM_REF, HOM_ALT, HET, HET_REF, HET_ALT, HET_MISS and MISS  e.g.
             HG0097:HOM_REF;HG0098:HET_REF,HOM_ALT . 3) Sample with segregation
             mode: {sample}:{segregation}. Only one sample accepted.Accepted
             segregation modes: [ autosomalDominant, autosomalRecessive,
             XLinkedDominant, XLinkedRecessive, YLinked, mitochondrial, deNovo,
-            mendelianError, compoundHeterozygous ]. Value is case insensitive.
-            e.g. HG0097:DeNovo Sample must have parents defined and indexed. .
+            deNovoStrict, mendelianError, compoundHeterozygous ]. Value is case
+            insensitive. e.g. HG0097:DeNovo Sample must have parents defined
+            and indexed. .
         :param str sample_data: Filter by any SampleData field from samples.
             [{sample}:]{key}{op}{value}[,;]* . If no sample is specified, will
             use all samples from 'sample' or 'genotype' filter. e.g. DP>200 or
             HG0097:DP>200,HG0098:DP<10 . Many FORMAT fields can be combined.
             e.g. HG0097:DP>200;GT=1/1,0/1,HG0098:DP<10.
         :param str sample_annotation: Selects some samples using metadata
             information from Catalog. e.g.
@@ -750,15 +804,15 @@
         :param str family: Filter variants where any of the samples from the
             given family contains the variant (HET or HOM_ALT).
         :param str family_disorder: Specify the disorder to use for the family
             segregation.
         :param str family_segregation: Filter by segregation mode from a given
             family. Accepted values: [ autosomalDominant, autosomalRecessive,
             XLinkedDominant, XLinkedRecessive, YLinked, mitochondrial, deNovo,
-            mendelianError, compoundHeterozygous ].
+            deNovoStrict, mendelianError, compoundHeterozygous ].
         :param str family_members: Sub set of the members of a given family.
         :param str family_proband: Specify the proband child to use for the
             family segregation.
         :param str gene: List of genes, most gene IDs are accepted (HGNC,
             Ensembl gene, ...). This is an alias to 'xref' parameter.
         :param str ct: List of SO consequence types, e.g.
             missense_variant,stop_lost or SO:0001583,SO:0001578. Accepts
@@ -827,16 +881,16 @@
         """
         Returns the acl of the clinical analyses. If member is provided, it
             will only return the acl for the member.
         PATH: /{apiVersion}/analysis/clinical/{clinicalAnalyses}/acl
 
         :param str clinical_analyses: Comma separated list of clinical
             analysis IDs or names up to a maximum of 100. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str member: User or group ID.
         :param bool silent: Boolean to retrieve all possible entries that are
             queried for, false to raise an exception whenever one of the
             entries looked for cannot be shown for whichever reason.
         """
 
         return self._get(category='analysis', resource='acl', subcategory='clinical', second_query_id=clinical_analyses, **options)
@@ -844,16 +898,16 @@
     def delete(self, clinical_analyses, **options):
         """
         Delete clinical analyses.
         PATH: /{apiVersion}/analysis/clinical/{clinicalAnalyses}/delete
 
         :param str clinical_analyses: Comma separated list of clinical
             analysis IDs or names up to a maximum of 100. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool force: Force deletion if the ClinicalAnalysis contains
             interpretations or is locked.
         """
 
         return self._delete(category='analysis', resource='delete', subcategory='clinical', second_query_id=clinical_analyses, **options)
 
     def update(self, clinical_analyses, data=None, **options):
@@ -865,44 +919,75 @@
             (REQUIRED)
         :param str clinical_analyses: Comma separated list of clinical
             analysis IDs. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str comments_action: Action to be performed if the array of
-            comments is being updated. Allowed values: ['ADD', 'REMOVE',
-            'REPLACE']
+            comments is being updated. Allowed values: ['ADD REMOVE REPLACE']
         :param str flags_action: Action to be performed if the array of flags
-            is being updated. Allowed values: ['ADD', 'SET', 'REMOVE']
+            is being updated. Allowed values: ['ADD SET REMOVE']
+        :param str analysts_action: Action to be performed if the array of
+            analysts is being updated. Allowed values: ['ADD SET REMOVE']
         :param str files_action: Action to be performed if the array of files
-            is being updated. Allowed values: ['ADD', 'SET', 'REMOVE']
+            is being updated. Allowed values: ['ADD SET REMOVE']
         :param str panels_action: Action to be performed if the array of
-            panels is being updated. Allowed values: ['ADD', 'SET', 'REMOVE']
+            panels is being updated. Allowed values: ['ADD SET REMOVE']
+        :param str annotation_sets_action: Action to be performed if the array
+            of annotationSets is being updated. Allowed values: ['ADD SET
+            REMOVE']
         :param bool include_result: Flag indicating to include the created or
             updated document result in the response.
         """
 
         return self._post(category='analysis', resource='update', subcategory='clinical', second_query_id=clinical_analyses, data=data, **options)
 
+    def update_annotation_sets_annotations(self, clinical_analysis, annotation_set, data=None, **options):
+        """
+        Update annotations from an annotationSet.
+        PATH: /{apiVersion}/analysis/clinical/{clinicalAnalysis}/annotationSets/{annotationSet}/annotations/update
+
+        :param str annotation_set: AnnotationSet ID to be updated. (REQUIRED)
+        :param str clinical_analysis: Clinical analysis ID. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
+        :param str action: Action to be performed: ADD to add new annotations;
+            REPLACE to replace the value of an already existing annotation; SET
+            to set the new list of annotations removing any possible old
+            annotations; REMOVE to remove some annotations; RESET to set some
+            annotations to the default value configured in the corresponding
+            variables of the VariableSet if any. Allowed values: ['ADD SET
+            REMOVE RESET REPLACE']
+        :param dict data: Json containing the map of annotations when the
+            action is ADD, SET or REPLACE, a json with only the key 'remove'
+            containing the comma separated variables to be removed as a value
+            when the action is REMOVE or a json with only the key 'reset'
+            containing the comma separated variables that will be set to the
+            default value when the action is RESET.
+        """
+
+        return self._post(category='analysis/clinical', resource='annotations/update', query_id=clinical_analysis, subcategory='annotationSets', second_query_id=annotation_set, data=data, **options)
+
     def info(self, clinical_analysis, **options):
         """
         Clinical analysis info.
         PATH: /{apiVersion}/analysis/clinical/{clinicalAnalysis}/info
 
         :param str clinical_analysis: Comma separated list of clinical
             analysis IDs or names up to a maximum of 100. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param bool flatten_annotations: Flatten the annotations?.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool deleted: Boolean to retrieve deleted entries.
         """
 
         return self._get(category='analysis', resource='info', subcategory='clinical', second_query_id=clinical_analysis, **options)
 
     def create_interpretation(self, clinical_analysis, data=None, **options):
         """
@@ -912,60 +997,60 @@
         :param dict data: JSON containing clinical interpretation information.
             (REQUIRED)
         :param str clinical_analysis: Clinical analysis ID. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: [[user@]project:]study id.
-        :param str set_as: Set interpretation as. Allowed values: ['PRIMARY',
-            'SECONDARY']
+        :param str study: [[organization@]project:]study id.
+        :param str set_as: Set interpretation as. Allowed values: ['PRIMARY
+            SECONDARY']
         :param bool include_result: Flag indicating to include the created or
             updated document result in the response.
         """
 
         return self._post(category='analysis/clinical', resource='create', query_id=clinical_analysis, subcategory='interpretation', data=data, **options)
 
     def clear_interpretation(self, clinical_analysis, interpretations, **options):
         """
         Clear the fields of the main interpretation of the Clinical Analysis.
         PATH: /{apiVersion}/analysis/clinical/{clinicalAnalysis}/interpretation/{interpretations}/clear
 
         :param str clinical_analysis: Clinical analysis ID. (REQUIRED)
         :param str interpretations: Interpretation IDs of the Clinical
             Analysis. (REQUIRED)
-        :param str study: [[user@]project:]study ID.
+        :param str study: [[organization@]project:]study ID.
         """
 
         return self._post(category='analysis/clinical', resource='clear', query_id=clinical_analysis, subcategory='interpretation', second_query_id=interpretations, **options)
 
     def delete_interpretation(self, clinical_analysis, interpretations, **options):
         """
         Delete interpretation.
         PATH: /{apiVersion}/analysis/clinical/{clinicalAnalysis}/interpretation/{interpretations}/delete
 
         :param str interpretations: Interpretation IDs of the Clinical
             Analysis. (REQUIRED)
         :param str clinical_analysis: Clinical analysis ID. (REQUIRED)
-        :param str study: [[user@]project:]study ID.
+        :param str study: [[organization@]project:]study ID.
         :param str set_as_primary: Interpretation id to set as primary from
             the list of secondaries in case of deleting the actual primary one.
         """
 
         return self._delete(category='analysis/clinical', resource='delete', query_id=clinical_analysis, subcategory='interpretation', second_query_id=interpretations, **options)
 
     def revert_interpretation(self, clinical_analysis, interpretation, version, **options):
         """
         Revert to a previous interpretation version.
         PATH: /{apiVersion}/analysis/clinical/{clinicalAnalysis}/interpretation/{interpretation}/revert
 
         :param int version: Version to revert to. (REQUIRED)
         :param str interpretation: Interpretation ID. (REQUIRED)
         :param str clinical_analysis: Clinical analysis ID. (REQUIRED)
-        :param str study: [[user@]project:]study ID.
+        :param str study: [[organization@]project:]study ID.
         """
 
         options['version'] = version
         return self._post(category='analysis/clinical', resource='revert', query_id=clinical_analysis, subcategory='interpretation', second_query_id=interpretation, **options)
 
     def update_interpretation(self, clinical_analysis, interpretation, data=None, **options):
         """
@@ -976,30 +1061,57 @@
             (REQUIRED)
         :param str interpretation: Interpretation ID. (REQUIRED)
         :param str clinical_analysis: Clinical analysis ID. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: [[user@]project:]study ID.
+        :param str study: [[organization@]project:]study ID.
         :param str primary_findings_action: Action to be performed if the
-            array of primary findings is being updated. Allowed values: ['ADD',
-            'SET', 'REMOVE', 'REPLACE']
+            array of primary findings is being updated. Allowed values: ['ADD
+            SET REMOVE REPLACE']
         :param str methods_action: Action to be performed if the array of
-            methods is being updated. Allowed values: ['ADD', 'SET', 'REMOVE']
+            methods is being updated. Allowed values: ['ADD SET REMOVE']
         :param str secondary_findings_action: Action to be performed if the
-            array of secondary findings is being updated. Allowed values:
-            ['ADD', 'SET', 'REMOVE', 'REPLACE']
+            array of secondary findings is being updated. Allowed values: ['ADD
+            SET REMOVE REPLACE']
         :param str comments_action: Action to be performed if the array of
             comments is being updated. To REMOVE or REPLACE, the date will need
-            to be provided to identify the comment. Allowed values: ['ADD',
-            'REMOVE', 'REPLACE']
+            to be provided to identify the comment. Allowed values: ['ADD
+            REMOVE REPLACE']
         :param str panels_action: Action to be performed if the array of
-            panels is being updated. Allowed values: ['ADD', 'SET', 'REMOVE']
-        :param str set_as: Set interpretation as. Allowed values: ['PRIMARY',
-            'SECONDARY']
+            panels is being updated. Allowed values: ['ADD SET REMOVE']
+        :param str set_as: Set interpretation as. Allowed values: ['PRIMARY
+            SECONDARY']
         :param bool include_result: Flag indicating to include the created or
             updated document result in the response.
         """
 
         return self._post(category='analysis/clinical', resource='update', query_id=clinical_analysis, subcategory='interpretation', second_query_id=interpretation, data=data, **options)
 
+    def update_report(self, clinical_analysis, data=None, **options):
+        """
+        Update clinical analysis report.
+        PATH: /{apiVersion}/analysis/clinical/{clinicalAnalysis}/report/update
+
+        :param dict data: JSON containing clinical report information.
+            (REQUIRED)
+        :param str clinical_analysis: Clinical analysis ID. (REQUIRED)
+        :param str include: Fields included in the response, whole JSON path
+            must be provided.
+        :param str exclude: Fields excluded in the response, whole JSON path
+            must be provided.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
+        :param str comments_action: Action to be performed if the array of
+            comments is being updated. Allowed values: ['ADD REMOVE REPLACE']
+        :param str supporting_evidences_action: Action to be performed if the
+            array of supporting evidences is being updated. Allowed values:
+            ['ADD SET REMOVE']
+        :param str files_action: Action to be performed if the array of files
+            is being updated. Allowed values: ['ADD SET REMOVE']
+        :param bool include_result: Flag indicating to include the created or
+            updated document result in the response.
+        """
+
+        return self._post(category='analysis/clinical', resource='update', query_id=clinical_analysis, subcategory='report', data=data, **options)
+
```

### Comparing `pyopencga-2.9.2/pyopencga/rest_clients/cohort_client.py` & `pyopencga-3.0.0/pyopencga/rest_clients/cohort_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-04-18
+    Autogenerated on: 2024-03-06
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Cohort(_ParentRestClient):
     """
     This class contains methods for the 'Cohorts' webservices
-    Client version: 2.8.0-SNAPSHOT
+    Client version: 3.0.0-SNAPSHOT
     PATH: /{apiVersion}/cohorts
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Cohort, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
@@ -28,58 +28,31 @@
 
         :param dict data: JSON containing the parameters to add ACLs.
             (REQUIRED)
         :param str action: Action to be performed [ADD, SET, REMOVE or RESET].
             Allowed values: ['SET ADD REMOVE RESET'] (REQUIRED)
         :param str members: Comma separated list of user or group ids.
             (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         options['action'] = action
         return self._post(category='cohorts', resource='update', subcategory='acl', second_query_id=members, data=data, **options)
 
-    def aggregation_stats(self, **options):
-        """
-        Fetch catalog cohort stats.
-        PATH: /{apiVersion}/cohorts/aggregationStats
-
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
-        :param str type: Type.
-        :param str creation_year: Creation year.
-        :param str creation_month: Creation month (JANUARY, FEBRUARY...).
-        :param str creation_day: Creation day.
-        :param str creation_day_of_week: Creation day of week (MONDAY,
-            TUESDAY...).
-        :param str num_samples: Number of samples.
-        :param str status: Status.
-        :param str release: Release.
-        :param str annotation: Annotation filters. Example:
-            age>30;gender=FEMALE. For more information, please visit
-            http://docs.opencb.org/display/opencga/AnnotationSets+1.4.0.
-        :param bool default: Calculate default stats.
-        :param str field: List of fields separated by semicolons, e.g.:
-            studies;type. For nested fields use >>, e.g.:
-            studies>>biotype;type;numSamples[0..10]:1.
-        """
-
-        return self._get(category='cohorts', resource='aggregationStats', **options)
-
     def load_annotation_sets(self, variable_set_id, path, data=None, **options):
         """
         Load annotation sets from a TSV file.
         PATH: /{apiVersion}/cohorts/annotationSets/load
 
         :param str path: Path where the TSV file is located in OpenCGA or
             where it should be located. (REQUIRED)
         :param str variable_set_id: Variable set ID or name. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool parents: Flag indicating whether to create parent
             directories if they don't exist (only when TSV file was not
             previously associated).
         :param str annotation_set_id: Annotation set id. If not provided,
             variableSetId will be used.
         :param dict data: JSON containing the 'content' of the TSV file if
             this has not yet been registered into OpenCGA.
@@ -95,16 +68,16 @@
         PATH: /{apiVersion}/cohorts/create
 
         :param dict data: JSON containing cohort information. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str variable_set: Deprecated: Use /generate web service and
             filter by annotation.
         :param str variable: Deprecated: Use /generate web service and filter
             by annotation.
         :param bool include_result: Flag indicating to include the created or
             updated document result in the response.
         """
@@ -114,20 +87,24 @@
     def distinct(self, field, **options):
         """
         Cohort distinct method.
         PATH: /{apiVersion}/cohorts/distinct
 
         :param str field: Comma separated list of fields for which to obtain
             the distinct values. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str id: Comma separated list of cohort IDs up to a maximum of
-            100.
+            100. Also admits basic regular expressions using the operator '~',
+            i.e. '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i'
+            for case insensitive search.
         :param str name: Comma separated list of cohort names up to a maximum
-            of 100.
+            of 100. Also admits basic regular expressions using the operator
+            '~', i.e. '~{perl-regex}' e.g. '~value' for case sensitive,
+            '~/value/i' for case insensitive search.
         :param str uuid: Comma separated list of cohort IDs up to a maximum of
             100.
         :param str type: Cohort type.
         :param str creation_date: creationDate.
         :param str modification_date: modificationDate.
         :param bool deleted: deleted.
         :param str status: status.
@@ -148,28 +125,31 @@
         PATH: /{apiVersion}/cohorts/generate
 
         :param dict data: JSON containing cohort information. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str id: Comma separated list sample IDs or UUIDs up to a
             maximum of 100.
         :param bool somatic: Somatic sample.
         :param str individual_id: Individual ID or UUID.
         :param str file_ids: Comma separated list of file IDs, paths or UUIDs.
         :param str creation_date: Creation date. Format: yyyyMMddHHmmss.
             Examples: >2018, 2017-2018, <201805.
         :param str modification_date: Modification date. Format:
             yyyyMMddHHmmss. Examples: >2018, 2017-2018, <201805.
         :param str internal_status: Filter by internal status.
         :param str status: Filter by status.
         :param str phenotypes: Comma separated list of phenotype ids or names.
+            Also admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
         :param str annotation: Annotation filters. Example:
             age>30;gender=FEMALE. For more information, please visit
             http://docs.opencb.org/display/opencga/AnnotationSets+1.4.0.
         :param str acl: Filter entries for which a user has the provided
             permissions. Format: acl={user}:{permissions}. Example:
             acl=john:WRITE,WRITE_ANNOTATIONS will return all entries for which
             user john has both WRITE and WRITE_ANNOTATIONS permissions. Only
@@ -193,20 +173,24 @@
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param int limit: Number of results to be returned.
         :param int skip: Number of results to skip.
         :param bool count: Get the total number of results matching the query.
             Deactivated by default.
         :param bool flatten_annotations: Flatten the annotations?.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str id: Comma separated list of cohort IDs up to a maximum of
-            100.
+            100. Also admits basic regular expressions using the operator '~',
+            i.e. '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i'
+            for case insensitive search.
         :param str name: Comma separated list of cohort names up to a maximum
-            of 100.
+            of 100. Also admits basic regular expressions using the operator
+            '~', i.e. '~{perl-regex}' e.g. '~value' for case sensitive,
+            '~/value/i' for case insensitive search.
         :param str uuid: Comma separated list of cohort IDs up to a maximum of
             100.
         :param str type: Cohort type.
         :param str creation_date: creationDate.
         :param str modification_date: modificationDate.
         :param bool deleted: deleted.
         :param str status: status.
@@ -224,32 +208,32 @@
         """
         Return the acl of the cohort. If member is provided, it will only
             return the acl for the member.
         PATH: /{apiVersion}/cohorts/{cohorts}/acl
 
         :param str cohorts: Comma separated list of cohort IDs or UUIDs up to
             a maximum of 100. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str member: User or group id.
         :param bool silent: Boolean to retrieve all possible entries that are
             queried for, false to raise an exception whenever one of the
             entries looked for cannot be shown for whichever reason.
         """
 
         return self._get(category='cohorts', resource='acl', query_id=cohorts, **options)
 
     def delete(self, cohorts, **options):
         """
         Delete cohorts.
         PATH: /{apiVersion}/cohorts/{cohorts}/delete
 
         :param str cohorts: Comma separated list of cohort ids. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         return self._delete(category='cohorts', resource='delete', query_id=cohorts, **options)
 
     def info(self, cohorts, **options):
         """
         Get cohort information.
@@ -258,16 +242,16 @@
         :param str cohorts: Comma separated list of cohort IDs or UUIDs up to
             a maximum of 100. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param bool flatten_annotations: Flatten the annotations?.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool deleted: Boolean to retrieve deleted cohorts.
         """
 
         return self._get(category='cohorts', resource='info', query_id=cohorts, **options)
 
     def update(self, cohorts, data=None, **options):
         """
@@ -275,16 +259,16 @@
         PATH: /{apiVersion}/cohorts/{cohorts}/update
 
         :param str cohorts: Comma separated list of cohort ids. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str samples_action: Action to be performed if the array of
             samples is being updated. Allowed values: ['ADD SET REMOVE']
         :param str annotation_sets_action: Action to be performed if the array
             of annotationSets is being updated. Allowed values: ['ADD SET
             REMOVE']
         :param bool include_result: Flag indicating to include the created or
             updated document result in the response.
@@ -296,16 +280,16 @@
     def update_annotation_sets_annotations(self, cohort, annotation_set, data=None, **options):
         """
         Update annotations from an annotationSet.
         PATH: /{apiVersion}/cohorts/{cohort}/annotationSets/{annotationSet}/annotations/update
 
         :param str annotation_set: AnnotationSet ID to be updated. (REQUIRED)
         :param str cohort: Cohort ID. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str action: Action to be performed: ADD to add new annotations;
             REPLACE to replace the value of an already existing annotation; SET
             to set the new list of annotations removing any possible old
             annotations; REMOVE to remove some annotations; RESET to set some
             annotations to the default value configured in the corresponding
             variables of the VariableSet if any. Allowed values: ['ADD SET
             REMOVE RESET REPLACE']
```

### Comparing `pyopencga-2.9.2/pyopencga/rest_clients/disease_panel_client.py` & `pyopencga-3.0.0/pyopencga/rest_clients/job_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,236 +1,284 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-04-18
+    Autogenerated on: 2024-03-06
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
-class DiseasePanel(_ParentRestClient):
+class Job(_ParentRestClient):
     """
-    This class contains methods for the 'Disease Panels' webservices
-    Client version: 2.8.0-SNAPSHOT
-    PATH: /{apiVersion}/panels
+    This class contains methods for the 'Jobs' webservices
+    Client version: 3.0.0-SNAPSHOT
+    PATH: /{apiVersion}/jobs
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
-        super(DiseasePanel, self).__init__(configuration, token, login_handler, *args, **kwargs)
+        super(Job, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
         """
         Update the set of permissions granted for the member.
-        PATH: /{apiVersion}/panels/acl/{members}/update
+        PATH: /{apiVersion}/jobs/acl/{members}/update
 
-        :param dict data: JSON containing the parameters to update the
-            permissions. (REQUIRED)
+        :param dict data: JSON containing the parameters to add ACLs.
+            (REQUIRED)
         :param str action: Action to be performed [ADD, SET, REMOVE or RESET].
             Allowed values: ['SET ADD REMOVE RESET'] (REQUIRED)
         :param str members: Comma separated list of user or group ids.
             (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
         """
 
         options['action'] = action
-        return self._post(category='panels', resource='update', subcategory='acl', second_query_id=members, data=data, **options)
+        return self._post(category='jobs', resource='update', subcategory='acl', second_query_id=members, data=data, **options)
 
     def create(self, data=None, **options):
         """
-        Create a panel.
-        PATH: /{apiVersion}/panels/create
+        Register an executed job with POST method.
+        PATH: /{apiVersion}/jobs/create
 
-        :param str include: Fields included in the response, whole JSON path
-            must be provided.
-        :param str exclude: Fields excluded in the response, whole JSON path
-            must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
-        :param bool include_result: Flag indicating to include the created or
-            updated document result in the response.
-        :param dict data: Panel parameters.
+        :param dict data: job. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
-        return self._post(category='panels', resource='create', data=data, **options)
+        return self._post(category='jobs', resource='create', data=data, **options)
 
     def distinct(self, field, **options):
         """
-        Panel distinct method.
-        PATH: /{apiVersion}/panels/distinct
+        Job distinct method.
+        PATH: /{apiVersion}/jobs/distinct
 
         :param str field: Comma separated list of fields for which to obtain
             the distinct values. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
-        :param str id: Comma separated list of panel IDs  up to a maximum of
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
+        :param bool other_studies: Flag indicating the entries being queried
+            can belong to any related study, not just the primary one.
+        :param str id: Comma separated list of job IDs up to a maximum of 100.
+            Also admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
+        :param str uuid: Comma separated list of job UUIDs up to a maximum of
             100.
-        :param str uuid: Comma separated list of panel UUIDs  up to a maximum
-            of 100.
-        :param str name: Comma separated list of panel names  up to a maximum
-            of 100.
-        :param str internal_status: Filter by internal status.
-        :param str disorders: Comma separated list of disorder ids or names.
-        :param str variants: Comma separated list of variant ids.
-        :param str genes: Comma separated list of gene ids.
-        :param str source: Comma separated list of source ids or names.
-        :param str regions: Comma separated list of regions.
-        :param str categories: Comma separated list of category names.
-        :param str tags: Panel tags.
-        :param bool deleted: Boolean to retrieve deleted entries.
+        :param str tool_id: Tool ID executed by the job. Also admits basic
+            regular expressions using the operator '~', i.e. '~{perl-regex}'
+            e.g. '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
+        :param str tool_type: Tool type executed by the job [OPERATION,
+            ANALYSIS].
+        :param str user_id: User that created the job.
+        :param str priority: Priority of the job.
         :param str status: Filter by status.
+        :param str internal_status: Filter by internal status.
         :param str creation_date: Creation date. Format: yyyyMMddHHmmss.
             Examples: >2018, 2017-2018, <201805.
         :param str modification_date: Modification date. Format:
             yyyyMMddHHmmss. Examples: >2018, 2017-2018, <201805.
+        :param bool visited: Visited status of job.
+        :param str tags: Job tags.
+        :param str input: Comma separated list of file IDs used as input.
+        :param str output: Comma separated list of file IDs used as output.
         :param str acl: Filter entries for which a user has the provided
             permissions. Format: acl={user}:{permissions}. Example:
             acl=john:WRITE,WRITE_ANNOTATIONS will return all entries for which
             user john has both WRITE and WRITE_ANNOTATIONS permissions. Only
             study owners or administrators can query by this field. .
         :param str release: Release when it was created.
-        :param int snapshot: Snapshot value (Latest version of the entry in
-            the specified release).
+        :param bool deleted: Boolean to retrieve deleted entries.
         """
 
         options['field'] = field
-        return self._get(category='panels', resource='distinct', **options)
+        return self._get(category='jobs', resource='distinct', **options)
 
-    def import_panels(self, data=None, **options):
+    def retry(self, data=None, **options):
         """
-        Import panels.
-        PATH: /{apiVersion}/panels/import
+        Relaunch a failed job.
+        PATH: /{apiVersion}/jobs/retry
 
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param dict data: job. (REQUIRED)
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
+        :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
-        :param str job_description: Job description.
         :param str job_tags: Job tags.
-        :param dict data: Panel parameters.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
-        return self._post(category='panels', resource='import', data=data, **options)
+        return self._post(category='jobs', resource='retry', data=data, **options)
 
     def search(self, **options):
         """
-        Panel search.
-        PATH: /{apiVersion}/panels/search
+        Job search method.
+        PATH: /{apiVersion}/jobs/search
 
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param int limit: Number of results to be returned.
         :param int skip: Number of results to skip.
         :param bool count: Get the total number of results matching the query.
             Deactivated by default.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
-        :param str id: Comma separated list of panel IDs  up to a maximum of
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
+        :param bool other_studies: Flag indicating the entries being queried
+            can belong to any related study, not just the primary one.
+        :param str id: Comma separated list of job IDs up to a maximum of 100.
+            Also admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
+        :param str uuid: Comma separated list of job UUIDs up to a maximum of
             100.
-        :param str uuid: Comma separated list of panel UUIDs  up to a maximum
-            of 100.
-        :param str name: Comma separated list of panel names  up to a maximum
-            of 100.
-        :param str internal_status: Filter by internal status.
-        :param str disorders: Comma separated list of disorder ids or names.
-        :param str variants: Comma separated list of variant ids.
-        :param str genes: Comma separated list of gene ids.
-        :param str source: Comma separated list of source ids or names.
-        :param str regions: Comma separated list of regions.
-        :param str categories: Comma separated list of category names.
-        :param str tags: Panel tags.
-        :param bool deleted: Boolean to retrieve deleted entries.
+        :param str tool_id: Tool ID executed by the job. Also admits basic
+            regular expressions using the operator '~', i.e. '~{perl-regex}'
+            e.g. '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
+        :param str tool_type: Tool type executed by the job [OPERATION,
+            ANALYSIS].
+        :param str user_id: User that created the job.
+        :param str priority: Priority of the job.
         :param str status: Filter by status.
+        :param str internal_status: Filter by internal status.
         :param str creation_date: Creation date. Format: yyyyMMddHHmmss.
             Examples: >2018, 2017-2018, <201805.
         :param str modification_date: Modification date. Format:
             yyyyMMddHHmmss. Examples: >2018, 2017-2018, <201805.
+        :param bool visited: Visited status of job.
+        :param str tags: Job tags.
+        :param str input: Comma separated list of file IDs used as input.
+        :param str output: Comma separated list of file IDs used as output.
         :param str acl: Filter entries for which a user has the provided
             permissions. Format: acl={user}:{permissions}. Example:
             acl=john:WRITE,WRITE_ANNOTATIONS will return all entries for which
             user john has both WRITE and WRITE_ANNOTATIONS permissions. Only
             study owners or administrators can query by this field. .
         :param str release: Release when it was created.
-        :param int snapshot: Snapshot value (Latest version of the entry in
-            the specified release).
+        :param bool deleted: Boolean to retrieve deleted entries.
         """
 
-        return self._get(category='panels', resource='search', **options)
+        return self._get(category='jobs', resource='search', **options)
 
-    def acl(self, panels, **options):
+    def top(self, **options):
         """
-        Returns the acl of the panels. If member is provided, it will only
-            return the acl for the member.
-        PATH: /{apiVersion}/panels/{panels}/acl
+        Provide a summary of the running jobs.
+        PATH: /{apiVersion}/jobs/top
 
-        :param str panels: Comma separated list of panel IDs up to a maximum
-            of 100. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param int limit: Maximum number of jobs to be returned.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
+        :param str internal_status: Filter by internal status.
+        :param str priority: Priority of the job.
+        :param str user_id: User that created the job.
+        :param str tool_id: Tool ID executed by the job. Also admits basic
+            regular expressions using the operator '~', i.e. '~{perl-regex}'
+            e.g. '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
+        """
+
+        return self._get(category='jobs', resource='top', **options)
+
+    def acl(self, jobs, **options):
+        """
+        Return the acl of the job. If member is provided, it will only return
+            the acl for the member.
+        PATH: /{apiVersion}/jobs/{jobs}/acl
+
+        :param str jobs: Comma separated list of job IDs or UUIDs up to a
+            maximum of 100. (REQUIRED)
         :param str member: User or group id.
         :param bool silent: Boolean to retrieve all possible entries that are
             queried for, false to raise an exception whenever one of the
             entries looked for cannot be shown for whichever reason.
         """
 
-        return self._get(category='panels', resource='acl', query_id=panels, **options)
+        return self._get(category='jobs', resource='acl', query_id=jobs, **options)
 
-    def delete(self, panels, **options):
+    def delete(self, jobs, **options):
         """
-        Delete existing panels.
-        PATH: /{apiVersion}/panels/{panels}/delete
+        Delete existing jobs.
+        PATH: /{apiVersion}/jobs/{jobs}/delete
 
-        :param str panels: Comma separated list of panel ids. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str jobs: Comma separated list of job ids. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
-        return self._delete(category='panels', resource='delete', query_id=panels, **options)
+        return self._delete(category='jobs', resource='delete', query_id=jobs, **options)
 
-    def info(self, panels, **options):
+    def info(self, jobs, **options):
         """
-        Panel info.
-        PATH: /{apiVersion}/panels/{panels}/info
+        Get job information.
+        PATH: /{apiVersion}/jobs/{jobs}/info
 
-        :param str panels: Comma separated list of panel IDs up to a maximum
-            of 100. (REQUIRED)
+        :param str jobs: Comma separated list of job IDs or UUIDs up to a
+            maximum of 100. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
-        :param str version: Comma separated list of panel versions. 'all' to
-            get all the panel versions. Not supported if multiple panel ids are
-            provided.
-        :param bool deleted: Boolean to retrieve deleted panels.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
+        :param bool deleted: Boolean to retrieve deleted jobs.
         """
 
-        return self._get(category='panels', resource='info', query_id=panels, **options)
+        return self._get(category='jobs', resource='info', query_id=jobs, **options)
 
-    def update(self, panels, data=None, **options):
+    def update(self, jobs, data=None, **options):
         """
-        Update panel attributes.
-        PATH: /{apiVersion}/panels/{panels}/update
+        Update some job attributes.
+        PATH: /{apiVersion}/jobs/{jobs}/update
 
-        :param str panels: Comma separated list of panel ids. (REQUIRED)
+        :param str jobs: Comma separated list of job IDs or UUIDs up to a
+            maximum of 100. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool include_result: Flag indicating to include the created or
             updated document result in the response.
-        :param dict data: Panel parameters.
+        :param dict data: body.
+        """
+
+        return self._post(category='jobs', resource='update', query_id=jobs, data=data, **options)
+
+    def head_log(self, job, **options):
+        """
+        Show the first lines of a log file (up to a limit).
+        PATH: /{apiVersion}/jobs/{job}/log/head
+
+        :param str job: Job ID or UUID. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
+        :param int offset: Starting byte from which the file will be read.
+        :param int lines: Maximum number of lines to be returned up to a
+            maximum of 1000.
+        :param str type: Log file to be shown (stdout or stderr).
+        """
+
+        return self._get(category='jobs', resource='head', query_id=job, subcategory='log', **options)
+
+    def tail_log(self, job, **options):
+        """
+        Show the last lines of a log file (up to a limit).
+        PATH: /{apiVersion}/jobs/{job}/log/tail
+
+        :param str job: Job ID or UUID. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
+        :param int lines: Maximum number of lines to be returned up to a
+            maximum of 1000.
+        :param str type: Log file to be shown (stdout or stderr).
         """
 
-        return self._post(category='panels', resource='update', query_id=panels, data=data, **options)
+        return self._get(category='jobs', resource='tail', query_id=job, subcategory='log', **options)
```

### Comparing `pyopencga-2.9.2/pyopencga/rest_clients/family_client.py` & `pyopencga-3.0.0/pyopencga/rest_clients/family_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-04-18
+    Autogenerated on: 2024-03-06
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Family(_ParentRestClient):
     """
     This class contains methods for the 'Families' webservices
-    Client version: 2.8.0-SNAPSHOT
+    Client version: 3.0.0-SNAPSHOT
     PATH: /{apiVersion}/families
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Family, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
@@ -28,63 +28,34 @@
 
         :param dict data: JSON containing the parameters to add ACLs.
             (REQUIRED)
         :param str action: Action to be performed [ADD, SET, REMOVE or RESET].
             Allowed values: ['SET ADD REMOVE RESET'] (REQUIRED)
         :param str members: Comma separated list of user or group ids.
             (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str propagate: Propagate family permissions to related
             individuals and samples. Allowed values: ['NO YES
             YES_AND_VARIANT_VIEW']
         """
 
         options['action'] = action
         return self._post(category='families', resource='update', subcategory='acl', second_query_id=members, data=data, **options)
 
-    def aggregation_stats(self, **options):
-        """
-        Fetch catalog family stats.
-        PATH: /{apiVersion}/families/aggregationStats
-
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
-        :param str creation_year: Creation year.
-        :param str creation_month: Creation month (JANUARY, FEBRUARY...).
-        :param str creation_day: Creation day.
-        :param str creation_day_of_week: Creation day of week (MONDAY,
-            TUESDAY...).
-        :param str status: Status.
-        :param str phenotypes: Phenotypes.
-        :param str release: Release.
-        :param str version: Version.
-        :param str num_members: Number of members.
-        :param str expected_size: Expected size.
-        :param str annotation: Annotation filters. Example:
-            age>30;gender=FEMALE. For more information, please visit
-            http://docs.opencb.org/display/opencga/AnnotationSets+1.4.0.
-        :param bool default: Calculate default stats.
-        :param str field: List of fields separated by semicolons, e.g.:
-            studies;type. For nested fields use >>, e.g.:
-            studies>>biotype;type;numSamples[0..10]:1.
-        """
-
-        return self._get(category='families', resource='aggregationStats', **options)
-
     def load_annotation_sets(self, variable_set_id, path, data=None, **options):
         """
         Load annotation sets from a TSV file.
         PATH: /{apiVersion}/families/annotationSets/load
 
         :param str path: Path where the TSV file is located in OpenCGA or
             where it should be located. (REQUIRED)
         :param str variable_set_id: Variable set ID or name. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool parents: Flag indicating whether to create parent
             directories if they don't exist (only when TSV file was not
             previously associated).
         :param str annotation_set_id: Annotation set id. If not provided,
             variableSetId will be used.
         :param dict data: JSON containing the 'content' of the TSV file if
             this has not yet been registered into OpenCGA.
@@ -100,16 +71,16 @@
         PATH: /{apiVersion}/families/create
 
         :param dict data: JSON containing family information. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str members: Comma separated list of member ids to be
             associated to the created family.
         :param bool include_result: Flag indicating to include the created or
             updated document result in the response.
         """
 
         return self._post(category='families', resource='create', data=data, **options)
@@ -117,27 +88,38 @@
     def distinct(self, field, **options):
         """
         Family distinct method.
         PATH: /{apiVersion}/families/distinct
 
         :param str field: Comma separated list of fields for which to obtain
             the distinct values. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str id: Comma separated list family IDs up to a maximum of 100.
+            Also admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
         :param str name: Comma separated list family names up to a maximum of
-            100.
+            100. Also admits basic regular expressions using the operator '~',
+            i.e. '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i'
+            for case insensitive search.
         :param str uuid: Comma separated list family UUIDs up to a maximum of
             100.
         :param str members: Comma separated list of family members.
         :param int expected_size: Expected size of the family (number of
             members).
         :param str samples: Comma separated list of member's samples.
         :param str phenotypes: Comma separated list of phenotype ids or names.
+            Also admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
         :param str disorders: Comma separated list of disorder ids or names.
+            Also admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
         :param str creation_date: Creation date. Format: yyyyMMddHHmmss.
             Examples: >2018, 2017-2018, <201805.
         :param str modification_date: Modification date. Format:
             yyyyMMddHHmmss. Examples: >2018, 2017-2018, <201805.
         :param bool deleted: Boolean to retrieve deleted entries.
         :param str internal_status: Filter by internal status.
         :param str status: Filter by status.
@@ -167,27 +149,38 @@
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param int limit: Number of results to be returned.
         :param int skip: Number of results to skip.
         :param bool count: Get the total number of results matching the query.
             Deactivated by default.
         :param bool flatten_annotations: Flatten the annotations?.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str id: Comma separated list family IDs up to a maximum of 100.
+            Also admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
         :param str name: Comma separated list family names up to a maximum of
-            100.
+            100. Also admits basic regular expressions using the operator '~',
+            i.e. '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i'
+            for case insensitive search.
         :param str uuid: Comma separated list family UUIDs up to a maximum of
             100.
         :param str members: Comma separated list of family members.
         :param int expected_size: Expected size of the family (number of
             members).
         :param str samples: Comma separated list of member's samples.
         :param str phenotypes: Comma separated list of phenotype ids or names.
+            Also admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
         :param str disorders: Comma separated list of disorder ids or names.
+            Also admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
         :param str creation_date: Creation date. Format: yyyyMMddHHmmss.
             Examples: >2018, 2017-2018, <201805.
         :param str modification_date: Modification date. Format:
             yyyyMMddHHmmss. Examples: >2018, 2017-2018, <201805.
         :param bool deleted: Boolean to retrieve deleted entries.
         :param str internal_status: Filter by internal status.
         :param str status: Filter by status.
@@ -210,32 +203,32 @@
         """
         Returns the acl of the families. If member is provided, it will only
             return the acl for the member.
         PATH: /{apiVersion}/families/{families}/acl
 
         :param str families: Comma separated list of family IDs or names up to
             a maximum of 100. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str member: User or group id.
         :param bool silent: Boolean to retrieve all possible entries that are
             queried for, false to raise an exception whenever one of the
             entries looked for cannot be shown for whichever reason.
         """
 
         return self._get(category='families', resource='acl', query_id=families, **options)
 
     def delete(self, families, **options):
         """
         Delete existing families.
         PATH: /{apiVersion}/families/{families}/delete
 
         :param str families: Comma separated list of family ids. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         return self._delete(category='families', resource='delete', query_id=families, **options)
 
     def info(self, families, **options):
         """
         Get family information.
@@ -244,16 +237,16 @@
         :param str families: Comma separated list of family IDs or names up to
             a maximum of 100. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param bool flatten_annotations: Flatten the annotations?.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str version: Comma separated list of family versions. 'all' to
             get all the family versions. Not supported if multiple family ids
             are provided.
         :param bool deleted: Boolean to retrieve deleted families.
         """
 
         return self._get(category='families', resource='info', query_id=families, **options)
@@ -264,16 +257,16 @@
         PATH: /{apiVersion}/families/{families}/update
 
         :param str families: Comma separated list of family ids. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool update_roles: Update the member roles within the family.
         :param bool update_pedigree_graph: Update the family pedigree graph.
         :param str annotation_sets_action: Action to be performed if the array
             of annotationSets is being updated. Allowed values: ['ADD SET
             REMOVE']
         :param bool include_result: Flag indicating to include the created or
             updated document result in the response.
@@ -285,16 +278,16 @@
     def update_annotation_sets_annotations(self, family, annotation_set, data=None, **options):
         """
         Update annotations from an annotationSet.
         PATH: /{apiVersion}/families/{family}/annotationSets/{annotationSet}/annotations/update
 
         :param str annotation_set: AnnotationSet ID to be updated. (REQUIRED)
         :param str family: Family id. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str action: Action to be performed: ADD to add new annotations;
             REPLACE to replace the value of an already existing annotation; SET
             to set the new list of annotations removing any possible old
             annotations; REMOVE to remove some annotations; RESET to set some
             annotations to the default value configured in the corresponding
             variables of the VariableSet if any. Allowed values: ['ADD SET
             REMOVE RESET REPLACE']
```

### Comparing `pyopencga-2.9.2/pyopencga/rest_clients/file_client.py` & `pyopencga-3.0.0/pyopencga/rest_clients/file_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-04-18
+    Autogenerated on: 2024-03-06
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class File(_ParentRestClient):
     """
     This class contains methods for the 'Files' webservices
-    Client version: 2.8.0-SNAPSHOT
+    Client version: 3.0.0-SNAPSHOT
     PATH: /{apiVersion}/files
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(File, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
@@ -28,66 +28,31 @@
 
         :param dict data: JSON containing the parameters to add ACLs.
             (REQUIRED)
         :param str action: Action to be performed [ADD, SET, REMOVE or RESET].
             Allowed values: ['SET ADD REMOVE RESET'] (REQUIRED)
         :param str members: Comma separated list of user or group ids.
             (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         options['action'] = action
         return self._post(category='files', resource='update', subcategory='acl', second_query_id=members, data=data, **options)
 
-    def aggregation_stats(self, **options):
-        """
-        Fetch catalog file stats.
-        PATH: /{apiVersion}/files/aggregationStats
-
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
-        :param str name: Name.
-        :param str type: Type.
-        :param str format: Format.
-        :param str bioformat: Bioformat.
-        :param str creation_year: Creation year.
-        :param str creation_month: Creation month (JANUARY, FEBRUARY...).
-        :param str creation_day: Creation day.
-        :param str creation_day_of_week: Creation day of week (MONDAY,
-            TUESDAY...).
-        :param str status: Status.
-        :param str release: Release.
-        :param bool external: External.
-        :param str size: Size.
-        :param str software: Software.
-        :param str experiment: Experiment.
-        :param str num_samples: Number of samples.
-        :param str num_related_files: Number of related files.
-        :param str annotation: Annotation filters. Example:
-            age>30;gender=FEMALE. For more information, please visit
-            http://docs.opencb.org/display/opencga/AnnotationSets+1.4.0.
-        :param bool default: Calculate default stats.
-        :param str field: List of fields separated by semicolons, e.g.:
-            studies;type. For nested fields use >>, e.g.:
-            studies>>biotype;type;numSamples[0..10]:1.
-        """
-
-        return self._get(category='files', resource='aggregationStats', **options)
-
     def load_annotation_sets(self, variable_set_id, path, data=None, **options):
         """
         Load annotation sets from a TSV file.
         PATH: /{apiVersion}/files/annotationSets/load
 
         :param str path: Path where the TSV file is located in OpenCGA or
             where it should be located. (REQUIRED)
         :param str variable_set_id: Variable set ID or name. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool parents: Flag indicating whether to create parent
             directories if they don't exist (only when TSV file was not
             previously associated).
         :param str annotation_set_id: Annotation set id. If not provided,
             variableSetId will be used.
         :param dict data: JSON containing the 'content' of the TSV file if
             this has not yet been registered into OpenCGA.
@@ -107,38 +72,49 @@
 
     def create(self, data=None, **options):
         """
         Create file or folder.
         PATH: /{apiVersion}/files/create
 
         :param dict data: File parameters. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool parents: Create the parent directories if they do not
             exist.
         """
 
         return self._post(category='files', resource='create', data=data, **options)
 
     def distinct(self, field, **options):
         """
         File distinct method.
         PATH: /{apiVersion}/files/distinct
 
         :param str field: Comma separated list of fields for which to obtain
             the distinct values. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str id: Comma separated list of file IDs up to a maximum of
-            100.
+            100. Also admits basic regular expressions using the operator '~',
+            i.e. '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i'
+            for case insensitive search.
         :param str uuid: Comma separated list file UUIDs up to a maximum of
             100.
-        :param str name: Comma separated list of file names.
-        :param str path: Comma separated list of paths.
-        :param str uri: Comma separated list of uris.
+        :param str name: Comma separated list of file names. Also admits basic
+            regular expressions using the operator '~', i.e. '~{perl-regex}'
+            e.g. '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
+        :param str path: Comma separated list of paths. Also admits basic
+            regular expressions using the operator '~', i.e. '~{perl-regex}'
+            e.g. '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
+        :param str uri: Comma separated list of uris. Also admits basic
+            regular expressions using the operator '~', i.e. '~{perl-regex}'
+            e.g. '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
         :param str type: File type, either FILE or DIRECTORY.
         :param str bioformat: Comma separated Bioformat values. For existing
             Bioformats see files/bioformats.
         :param str format: Comma separated Format values. For existing Formats
             see files/formats.
         :param bool external: Boolean field indicating whether to filter by
             external or non external files.
@@ -150,15 +126,17 @@
         :param str directory: Directory under which we want to look for files
             or folders.
         :param str creation_date: Creation date. Format: yyyyMMddHHmmss.
             Examples: >2018, 2017-2018, <201805.
         :param str modification_date: Modification date. Format:
             yyyyMMddHHmmss. Examples: >2018, 2017-2018, <201805.
         :param str description: Description.
-        :param str tags: Tags.
+        :param str tags: Tags. Also admits basic regular expressions using the
+            operator '~', i.e. '~{perl-regex}' e.g. '~value' for case
+            sensitive, '~/value/i' for case insensitive search.
         :param str size: File size.
         :param str sample_ids: Comma separated list sample IDs or UUIDs up to
             a maximum of 100.
         :param str job_id: Job ID that created the file(s) or folder(s).
         :param str annotation: Annotation filters. Example:
             age>30;gender=FEMALE. For more information, please visit
             http://docs.opencb.org/display/opencga/AnnotationSets+1.4.0.
@@ -182,16 +160,16 @@
         :param dict data: Fetch parameters. (REQUIRED)
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         return self._post(category='files', resource='fetch', data=data, **options)
 
     def formats(self, **options):
         """
         List of accepted file formats.
@@ -202,30 +180,30 @@
 
     def link(self, data=None, **options):
         """
         Link an external file into catalog.
         PATH: /{apiVersion}/files/link
 
         :param dict data: File parameters. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool parents: Create the parent directories if they do not
             exist.
         """
 
         return self._post(category='files', resource='link', data=data, **options)
 
     def run_link(self, data=None, **options):
         """
         Link an external file into catalog asynchronously.
         PATH: /{apiVersion}/files/link/run
 
         :param dict data: File parameters. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_description: Job description.
         :param str job_tags: Job tags.
         """
@@ -235,16 +213,16 @@
     def run_postlink(self, data=None, **options):
         """
         Associate non-registered samples for files with high volumes of
             samples.
         PATH: /{apiVersion}/files/postlink/run
 
         :param dict data: File parameters. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_description: Job description.
         :param str job_tags: Job tags.
         """
@@ -262,23 +240,34 @@
             must be provided.
         :param int limit: Number of results to be returned.
         :param int skip: Number of results to skip.
         :param bool count: Get the total number of results matching the query.
             Deactivated by default.
         :param bool flatten_annotations: Boolean indicating to flatten the
             annotations.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str id: Comma separated list of file IDs up to a maximum of
-            100.
+            100. Also admits basic regular expressions using the operator '~',
+            i.e. '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i'
+            for case insensitive search.
         :param str uuid: Comma separated list file UUIDs up to a maximum of
             100.
-        :param str name: Comma separated list of file names.
-        :param str path: Comma separated list of paths.
-        :param str uri: Comma separated list of uris.
+        :param str name: Comma separated list of file names. Also admits basic
+            regular expressions using the operator '~', i.e. '~{perl-regex}'
+            e.g. '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
+        :param str path: Comma separated list of paths. Also admits basic
+            regular expressions using the operator '~', i.e. '~{perl-regex}'
+            e.g. '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
+        :param str uri: Comma separated list of uris. Also admits basic
+            regular expressions using the operator '~', i.e. '~{perl-regex}'
+            e.g. '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
         :param str type: File type, either FILE or DIRECTORY.
         :param str bioformat: Comma separated Bioformat values. For existing
             Bioformats see files/bioformats.
         :param str format: Comma separated Format values. For existing Formats
             see files/formats.
         :param bool external: Boolean field indicating whether to filter by
             external or non external files.
@@ -290,15 +279,17 @@
         :param str directory: Directory under which we want to look for files
             or folders.
         :param str creation_date: Creation date. Format: yyyyMMddHHmmss.
             Examples: >2018, 2017-2018, <201805.
         :param str modification_date: Modification date. Format:
             yyyyMMddHHmmss. Examples: >2018, 2017-2018, <201805.
         :param str description: Description.
-        :param str tags: Tags.
+        :param str tags: Tags. Also admits basic regular expressions using the
+            operator '~', i.e. '~{perl-regex}' e.g. '~value' for case
+            sensitive, '~/value/i' for case insensitive search.
         :param str size: File size.
         :param str sample_ids: Comma separated list sample IDs or UUIDs up to
             a maximum of 100.
         :param str job_id: Job ID that created the file(s) or folder(s).
         :param str annotation: Annotation filters. Example:
             age>30;gender=FEMALE. For more information, please visit
             http://docs.opencb.org/display/opencga/AnnotationSets+1.4.0.
@@ -319,28 +310,28 @@
         PATH: /{apiVersion}/files/upload
 
         :param inputstream file: File to upload.
         :param str file_name: File name to overwrite the input fileName.
         :param str file_format: File format. Allowed values: ['VCF BCF GVCF
             TBI BIGWIG SAM BAM BAI CRAM CRAI FASTQ FASTA PED
             TAB_SEPARATED_VALUES COMMA_SEPARATED_VALUES XML PROTOCOL_BUFFER
-            JSON AVRO PARQUET IMAGE PLAIN BINARY NONE UNKNOWN']
+            JSON AVRO PARQUET PDF IMAGE PLAIN BINARY NONE UNKNOWN']
         :param str bioformat: File bioformat. Allowed values:
             ['MICROARRAY_EXPRESSION_ONECHANNEL_AGILENT
             MICROARRAY_EXPRESSION_ONECHANNEL_AFFYMETRIX
             MICROARRAY_EXPRESSION_ONECHANNEL_GENEPIX
             MICROARRAY_EXPRESSION_TWOCHANNELS_AGILENT
             MICROARRAY_EXPRESSION_TWOCHANNELS_GENEPIX DATAMATRIX_EXPRESSION
             IDLIST IDLIST_RANKED ANNOTATION_GENEVSANNOTATION OTHER_NEWICK
             OTHER_BLAST OTHER_INTERACTION OTHER_GENOTYPE OTHER_PLINK OTHER_VCF
             OTHER_PED VCF4 VARIANT ALIGNMENT COVERAGE SEQUENCE PEDIGREE
             REFERENCE_GENOME NONE UNKNOWN']
         :param str checksum: Expected MD5 file checksum.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str relative_file_path: Path within catalog where the file will
             be located (default: root folder).
         :param str description: description.
         :param bool parents: Create the parent directories if they do not
             exist.
         """
 
@@ -351,16 +342,16 @@
         Return the acl defined for the file or folder. If member is provided,
             it will only return the acl for the member.
         PATH: /{apiVersion}/files/{files}/acl
 
         :param str files: Comma separated list of file IDs or names up to a
             maximum of 100. (REQUIRED)
         :param str study: Comma separated list of Studies
-            [[user@]project:]study where study and project can be either the ID
-            or UUID up to a maximum of 100.
+            [[organization@]project:]study where study and project can be
+            either the ID or UUID up to a maximum of 100.
         :param str member: User or group id.
         :param bool silent: Boolean to retrieve all possible entries that are
             queried for, false to raise an exception whenever one of the
             entries looked for cannot be shown for whichever reason.
         """
 
         return self._get(category='files', resource='acl', query_id=files, **options)
@@ -368,16 +359,16 @@
     def delete(self, files, **options):
         """
         Delete existing files and folders.
         PATH: /{apiVersion}/files/{files}/delete
 
         :param str files: Comma separated list of file ids, names or paths.
             (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool skip_trash: Skip trash and delete the files/folders from
             disk directly (CANNOT BE RECOVERED).
         """
 
         return self._delete(category='files', resource='delete', query_id=files, **options)
 
     def info(self, files, **options):
@@ -388,30 +379,30 @@
         :param str files: Comma separated list of file IDs or names up to a
             maximum of 100. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param bool flatten_annotations: Flatten the annotations?.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool deleted: Boolean to retrieve deleted files.
         """
 
         return self._get(category='files', resource='info', query_id=files, **options)
 
     def unlink(self, files, **options):
         """
         Unlink linked files and folders.
         PATH: /{apiVersion}/files/{files}/unlink
 
         :param str files: Comma separated list of file ids, names or paths.
             (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         return self._delete(category='files', resource='unlink', query_id=files, **options)
 
     def update(self, files, data=None, **options):
         """
         Update some file attributes.
@@ -420,16 +411,16 @@
         :param dict data: Parameters to modify. (REQUIRED)
         :param str files: Comma separated list of file ids, names or paths.
             Paths must be separated by : instead of /. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str sample_ids_action: Action to be performed if the array of
             samples is being updated. Allowed values: ['ADD SET REMOVE']
         :param str annotation_sets_action: Action to be performed if the array
             of annotationSets is being updated. Allowed values: ['ADD SET
             REMOVE']
         :param str related_files_action: Action to be performed if the array
             of relatedFiles is being updated. Allowed values: ['ADD SET
@@ -444,16 +435,16 @@
         """
         Update annotations from an annotationSet.
         PATH: /{apiVersion}/files/{file}/annotationSets/{annotationSet}/annotations/update
 
         :param str annotation_set: AnnotationSet ID to be updated. (REQUIRED)
         :param str file: File id, name or path. Paths must be separated by :
             instead of /. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str action: Action to be performed: ADD to add new annotations;
             REPLACE to replace the value of an already existing annotation; SET
             to set the new list of annotations removing any possible old
             annotations; REMOVE to remove some annotations; RESET to set some
             annotations to the default value configured in the corresponding
             variables of the VariableSet if any. Allowed values: ['ADD SET
             REMOVE RESET REPLACE']
@@ -470,85 +461,85 @@
     def download(self, file, **options):
         """
         Download file.
         PATH: /{apiVersion}/files/{file}/download
 
         :param str file: File id, name or path. Paths must be separated by :
             instead of /. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         return self._get(category='files', resource='download', query_id=file, **options)
 
     def grep(self, file, **options):
         """
         Filter lines of the file containing the pattern.
         PATH: /{apiVersion}/files/{file}/grep
 
         :param str file: File uuid, id, or name. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str pattern: String pattern.
         :param bool ignore_case: Flag to perform a case insensitive search.
         :param int max_count: Stop reading a file after 'n' matching lines. 0
             means no limit.
         """
 
         return self._get(category='files', resource='grep', query_id=file, **options)
 
     def head(self, file, **options):
         """
         Show the first lines of a file (up to a limit).
         PATH: /{apiVersion}/files/{file}/head
 
         :param str file: File uuid, id, or name. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param int offset: Starting byte from which the file will be read.
         :param int lines: Maximum number of lines to be returned up to a
             maximum of 1000.
         """
 
         return self._get(category='files', resource='head', query_id=file, **options)
 
     def image(self, file, **options):
         """
         Obtain the base64 content of an image.
         PATH: /{apiVersion}/files/{file}/image
 
         :param str file: File ID. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         return self._get(category='files', resource='image', query_id=file, **options)
 
     def refresh(self, file, **options):
         """
         Refresh metadata from the selected file or folder. Return updated
             files.
         PATH: /{apiVersion}/files/{file}/refresh
 
         :param str file: File id, name or path. Paths must be separated by :
             instead of /. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         return self._get(category='files', resource='refresh', query_id=file, **options)
 
     def tail(self, file, **options):
         """
         Show the last lines of a file (up to a limit).
         PATH: /{apiVersion}/files/{file}/tail
 
         :param str file: File uuid, id, or name. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param int lines: Maximum number of lines to be returned up to a
             maximum of 1000.
         """
 
         return self._get(category='files', resource='tail', query_id=file, **options)
 
     def list(self, folder, **options):
@@ -561,16 +552,16 @@
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param int limit: Number of results to be returned.
         :param int skip: Number of results to skip.
         :param bool count: Get the total number of results matching the query.
             Deactivated by default.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         return self._get(category='files', resource='list', query_id=folder, **options)
 
     def tree(self, folder, **options):
         """
         Obtain a tree view of the files and folders within a folder.
@@ -578,14 +569,14 @@
 
         :param str folder: Folder id or name. Paths must be separated by :
             instead of /. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param int max_depth: Maximum depth to get files from.
         """
 
         return self._get(category='files', resource='tree', query_id=folder, **options)
```

### Comparing `pyopencga-2.9.2/pyopencga/rest_clients/ga4gh_client.py` & `pyopencga-3.0.0/pyopencga/rest_clients/ga4gh_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-04-18
+    Autogenerated on: 2024-03-06
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class GA4GH(_ParentRestClient):
     """
     This class contains methods for the 'GA4GH' webservices
-    Client version: 2.8.0-SNAPSHOT
+    Client version: 3.0.0-SNAPSHOT
     PATH: /{apiVersion}/ga4gh
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(GA4GH, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def search_reads(self, **options):
@@ -30,16 +30,16 @@
         return self._post(category='ga4gh', resource='search', subcategory='reads', **options)
 
     def fetch_reads(self, study, file, **options):
         """
         Fetch alignment files using HTSget protocol.
         PATH: /{apiVersion}/ga4gh/reads/{study}/{file}
 
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID. (REQUIRED)
         :param str file: File id, name or path. (REQUIRED)
         :param str reference_name: Reference sequence name (Example: 'chr1',
             '1' or 'chrX'.
         :param int start: The start position of the range on the reference,
             0-based, inclusive.
         :param int end: The end position of the range on the reference,
             0-based, exclusive.
```

### Comparing `pyopencga-2.9.2/pyopencga/rest_clients/individual_client.py` & `pyopencga-3.0.0/pyopencga/rest_clients/individual_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-04-18
+    Autogenerated on: 2024-03-06
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Individual(_ParentRestClient):
     """
     This class contains methods for the 'Individuals' webservices
-    Client version: 2.8.0-SNAPSHOT
+    Client version: 3.0.0-SNAPSHOT
     PATH: /{apiVersion}/individuals
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Individual, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
@@ -30,69 +30,33 @@
             permissions. If propagate flag is set to true, it will propagate
             the permissions defined to the samples that are associated to the
             matching individuals. (REQUIRED)
         :param str action: Action to be performed [ADD, SET, REMOVE or RESET].
             Allowed values: ['SET ADD REMOVE RESET'] (REQUIRED)
         :param str members: Comma separated list of user or group ids.
             (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool propagate: Propagate individual permissions to related
             samples.
         """
 
         options['action'] = action
         return self._post(category='individuals', resource='update', subcategory='acl', second_query_id=members, data=data, **options)
 
-    def aggregation_stats(self, **options):
-        """
-        Fetch catalog individual stats.
-        PATH: /{apiVersion}/individuals/aggregationStats
-
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
-        :param bool has_father: Has father.
-        :param bool has_mother: Has mother.
-        :param str sex: Sex.
-        :param str karyotypic_sex: Karyotypic sex.
-        :param str ethnicity: Ethnicity.
-        :param str population: Population.
-        :param str creation_year: Creation year.
-        :param str creation_month: Creation month (JANUARY, FEBRUARY...).
-        :param str creation_day: Creation day.
-        :param str creation_day_of_week: Creation day of week (MONDAY,
-            TUESDAY...).
-        :param str status: Status.
-        :param str life_status: Life status.
-        :param str phenotypes: Phenotypes.
-        :param str num_samples: Number of samples.
-        :param bool parental_consanguinity: Parental consanguinity.
-        :param str release: Release.
-        :param str version: Version.
-        :param str annotation: Annotation filters. Example:
-            age>30;gender=FEMALE. For more information, please visit
-            http://docs.opencb.org/display/opencga/AnnotationSets+1.4.0.
-        :param bool default: Calculate default stats.
-        :param str field: List of fields separated by semicolons, e.g.:
-            studies;type. For nested fields use >>, e.g.:
-            studies>>biotype;type;numSamples[0..10]:1.
-        """
-
-        return self._get(category='individuals', resource='aggregationStats', **options)
-
     def load_annotation_sets(self, variable_set_id, path, data=None, **options):
         """
         Load annotation sets from a TSV file.
         PATH: /{apiVersion}/individuals/annotationSets/load
 
         :param str path: Path where the TSV file is located in OpenCGA or
             where it should be located. (REQUIRED)
         :param str variable_set_id: Variable set ID or name. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool parents: Flag indicating whether to create parent
             directories if they don't exist (only when TSV file was not
             previously associated).
         :param str annotation_set_id: Annotation set id. If not provided,
             variableSetId will be used.
         :param dict data: JSON containing the 'content' of the TSV file if
             this has not yet been registered into OpenCGA.
@@ -108,16 +72,16 @@
         PATH: /{apiVersion}/individuals/create
 
         :param dict data: JSON containing individual information. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str samples: Comma separated list of sample ids to be
             associated to the created individual.
         :param bool include_result: Flag indicating to include the created or
             updated document result in the response.
         """
 
         return self._post(category='individuals', resource='create', data=data, **options)
@@ -125,34 +89,53 @@
     def distinct(self, field, **options):
         """
         Individual distinct method.
         PATH: /{apiVersion}/individuals/distinct
 
         :param str field: Comma separated list of fields for which to obtain
             the distinct values. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str id: Comma separated list individual IDs up to a maximum of
-            100.
+            100. Also admits basic regular expressions using the operator '~',
+            i.e. '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i'
+            for case insensitive search.
         :param str uuid: Comma separated list individual UUIDs up to a maximum
             of 100.
         :param str name: Comma separated list individual names up to a maximum
-            of 100.
+            of 100. Also admits basic regular expressions using the operator
+            '~', i.e. '~{perl-regex}' e.g. '~value' for case sensitive,
+            '~/value/i' for case insensitive search.
         :param str family_ids: Comma separated list of family ids the
             individuals may belong to.
         :param str father: Father ID, name or UUID.
         :param str mother: Mother ID, name or UUID.
         :param str samples: Sample ID, name or UUID.
         :param str sex: Individual sex.
-        :param str ethnicity: Individual ethnicity.
+        :param str ethnicity: Individual ethnicity. Also admits basic regular
+            expressions using the operator '~', i.e. '~{perl-regex}' e.g.
+            '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
         :param str date_of_birth: Individual date of birth.
         :param str disorders: Comma separated list of disorder ids or names.
+            Also admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
         :param str phenotypes: Comma separated list of phenotype ids or names.
-        :param str population_name: Population name.
-        :param str population_subpopulation: Subpopulation name.
+            Also admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
+        :param str population_name: Population name. Also admits basic regular
+            expressions using the operator '~', i.e. '~{perl-regex}' e.g.
+            '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
+        :param str population_subpopulation: Subpopulation name. Also admits
+            basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
         :param str karyotypic_sex: Individual karyotypic sex.
         :param str life_status: Individual life status.
         :param str internal_status: Filter by internal status.
         :param str status: Filter by status.
         :param bool deleted: Boolean to retrieve deleted entries.
         :param str creation_date: Creation date. Format: yyyyMMddHHmmss.
             Examples: >2018, 2017-2018, <201805.
@@ -184,34 +167,53 @@
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param int limit: Number of results to be returned.
         :param int skip: Number of results to skip.
         :param bool count: Get the total number of results matching the query.
             Deactivated by default.
         :param bool flatten_annotations: Flatten the annotations?.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str id: Comma separated list individual IDs up to a maximum of
-            100.
+            100. Also admits basic regular expressions using the operator '~',
+            i.e. '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i'
+            for case insensitive search.
         :param str uuid: Comma separated list individual UUIDs up to a maximum
             of 100.
         :param str name: Comma separated list individual names up to a maximum
-            of 100.
+            of 100. Also admits basic regular expressions using the operator
+            '~', i.e. '~{perl-regex}' e.g. '~value' for case sensitive,
+            '~/value/i' for case insensitive search.
         :param str father: Father ID, name or UUID.
         :param str mother: Mother ID, name or UUID.
         :param str samples: Sample ID, name or UUID.
         :param str family_ids: Comma separated list of family ids the
             individuals may belong to.
         :param str sex: Individual sex.
         :param str date_of_birth: Individual date of birth.
-        :param str ethnicity: Individual ethnicity.
+        :param str ethnicity: Individual ethnicity. Also admits basic regular
+            expressions using the operator '~', i.e. '~{perl-regex}' e.g.
+            '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
         :param str disorders: Comma separated list of disorder ids or names.
+            Also admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
         :param str phenotypes: Comma separated list of phenotype ids or names.
-        :param str population_name: Population name.
-        :param str population_subpopulation: Subpopulation name.
+            Also admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
+        :param str population_name: Population name. Also admits basic regular
+            expressions using the operator '~', i.e. '~{perl-regex}' e.g.
+            '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
+        :param str population_subpopulation: Subpopulation name. Also admits
+            basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
         :param str karyotypic_sex: Individual karyotypic sex.
         :param str life_status: Individual life status.
         :param str internal_status: Filter by internal status.
         :param str status: Filter by status.
         :param bool deleted: Boolean to retrieve deleted entries.
         :param str creation_date: Creation date. Format: yyyyMMddHHmmss.
             Examples: >2018, 2017-2018, <201805.
@@ -236,16 +238,16 @@
         """
         Return the acl of the individual. If member is provided, it will only
             return the acl for the member.
         PATH: /{apiVersion}/individuals/{individuals}/acl
 
         :param str individuals: Comma separated list of individual IDs, names
             or UUIDs up to a maximum of 100. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str member: User or group id.
         :param bool silent: Boolean to retrieve all possible entries that are
             queried for, false to raise an exception whenever one of the
             entries looked for cannot be shown for whichever reason.
         """
 
         return self._get(category='individuals', resource='acl', query_id=individuals, **options)
@@ -255,16 +257,16 @@
         Delete existing individuals.
         PATH: /{apiVersion}/individuals/{individuals}/delete
 
         :param str individuals: Comma separated list of individual ids.
             (REQUIRED)
         :param bool force: Force the deletion of individuals that already
             belong to families.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         return self._delete(category='individuals', resource='delete', query_id=individuals, **options)
 
     def info(self, individuals, **options):
         """
         Get individual information.
@@ -273,16 +275,16 @@
         :param str individuals: Comma separated list of individual IDs, names
             or UUIDs up to a maximum of 100. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param bool flatten_annotations: Flatten the annotations?.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str version: Comma separated list of individual versions. 'all'
             to get all the individual versions. Not supported if multiple
             individual ids are provided.
         :param bool deleted: Boolean to retrieve deleted individuals.
         """
 
         return self._get(category='individuals', resource='info', query_id=individuals, **options)
@@ -294,16 +296,16 @@
 
         :param str individuals: Comma separated list of individual ids.
             (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str samples_action: Action to be performed if the array of
             samples is being updated. Allowed values: ['ADD SET REMOVE']
         :param str phenotypes_action: Action to be performed if the array of
             phenotypes is being updated [SET, ADD, REMOVE]. Allowed values:
             ['ADD SET REMOVE']
         :param str disorders_action: Action to be performed if the array of
             disorders is being updated [SET, ADD, REMOVE]. Allowed values:
@@ -321,16 +323,16 @@
     def update_annotation_sets_annotations(self, individual, annotation_set, data=None, **options):
         """
         Update annotations from an annotationSet.
         PATH: /{apiVersion}/individuals/{individual}/annotationSets/{annotationSet}/annotations/update
 
         :param str annotation_set: AnnotationSet ID to be updated. (REQUIRED)
         :param str individual: Individual ID, name or UUID. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str action: Action to be performed: ADD to add new annotations;
             REPLACE to replace the value of an already existing annotation; SET
             to set the new list of annotations removing any possible old
             annotations; REMOVE to remove some annotations; RESET to set some
             annotations to the default value configured in the corresponding
             variables of the VariableSet if any. Allowed values: ['ADD SET
             REMOVE RESET REPLACE']
@@ -351,14 +353,14 @@
 
         :param str individual: Individual ID, name or UUID. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param bool flatten_annotations: Flatten the annotations?.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param int degree: Pedigree degree.
         """
 
         return self._get(category='individuals', resource='relatives', query_id=individual, **options)
```

### Comparing `pyopencga-2.9.2/pyopencga/rest_clients/job_client.py` & `pyopencga-3.0.0/pyopencga/rest_clients/disease_panel_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,300 +1,282 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-04-18
+    Autogenerated on: 2024-03-06
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
-class Job(_ParentRestClient):
+class DiseasePanel(_ParentRestClient):
     """
-    This class contains methods for the 'Jobs' webservices
-    Client version: 2.8.0-SNAPSHOT
-    PATH: /{apiVersion}/jobs
+    This class contains methods for the 'Disease Panels' webservices
+    Client version: 3.0.0-SNAPSHOT
+    PATH: /{apiVersion}/panels
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
-        super(Job, self).__init__(configuration, token, login_handler, *args, **kwargs)
+        super(DiseasePanel, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
         """
         Update the set of permissions granted for the member.
-        PATH: /{apiVersion}/jobs/acl/{members}/update
+        PATH: /{apiVersion}/panels/acl/{members}/update
 
-        :param dict data: JSON containing the parameters to add ACLs.
-            (REQUIRED)
+        :param dict data: JSON containing the parameters to update the
+            permissions. (REQUIRED)
         :param str action: Action to be performed [ADD, SET, REMOVE or RESET].
             Allowed values: ['SET ADD REMOVE RESET'] (REQUIRED)
         :param str members: Comma separated list of user or group ids.
             (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         options['action'] = action
-        return self._post(category='jobs', resource='update', subcategory='acl', second_query_id=members, data=data, **options)
-
-    def aggregation_stats(self, **options):
-        """
-        Fetch catalog job stats.
-        PATH: /{apiVersion}/jobs/aggregationStats
-
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
-        :param str tool_id: Tool id.
-        :param str tool_scope: Tool scope.
-        :param str tool_type: Tool type.
-        :param str tool_resource: Tool resource.
-        :param str user_id: User id.
-        :param str priority: Priority.
-        :param str tags: Tags.
-        :param str executor_id: Executor id.
-        :param str executor_framework: Executor framework.
-        :param str creation_year: Creation year.
-        :param str creation_month: Creation month (JANUARY, FEBRUARY...).
-        :param str creation_day: Creation day.
-        :param str creation_day_of_week: Creation day of week (MONDAY,
-            TUESDAY...).
-        :param str status: Status.
-        :param str release: Release.
-        :param bool default: Calculate default stats.
-        :param str field: List of fields separated by semicolons, e.g.:
-            studies;type. For nested fields use >>, e.g.:
-            studies>>biotype;type;numSamples[0..10]:1.
-        """
-
-        return self._get(category='jobs', resource='aggregationStats', **options)
+        return self._post(category='panels', resource='update', subcategory='acl', second_query_id=members, data=data, **options)
 
     def create(self, data=None, **options):
         """
-        Register an executed job with POST method.
-        PATH: /{apiVersion}/jobs/create
+        Create a panel.
+        PATH: /{apiVersion}/panels/create
 
-        :param dict data: job. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str include: Fields included in the response, whole JSON path
+            must be provided.
+        :param str exclude: Fields excluded in the response, whole JSON path
+            must be provided.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
+        :param bool include_result: Flag indicating to include the created or
+            updated document result in the response.
+        :param dict data: Panel parameters.
         """
 
-        return self._post(category='jobs', resource='create', data=data, **options)
+        return self._post(category='panels', resource='create', data=data, **options)
 
     def distinct(self, field, **options):
         """
-        Job distinct method.
-        PATH: /{apiVersion}/jobs/distinct
+        Panel distinct method.
+        PATH: /{apiVersion}/panels/distinct
 
         :param str field: Comma separated list of fields for which to obtain
             the distinct values. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
-        :param bool other_studies: Flag indicating the entries being queried
-            can belong to any related study, not just the primary one.
-        :param str id: Comma separated list of job IDs up to a maximum of 100.
-        :param str uuid: Comma separated list of job UUIDs up to a maximum of
-            100.
-        :param str tool_id: Tool ID executed by the job.
-        :param str tool_type: Tool type executed by the job [OPERATION,
-            ANALYSIS].
-        :param str user_id: User that created the job.
-        :param str priority: Priority of the job.
-        :param str status: Filter by status.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
+        :param str id: Comma separated list of panel IDs  up to a maximum of
+            100. Also admits basic regular expressions using the operator '~',
+            i.e. '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i'
+            for case insensitive search.
+        :param str uuid: Comma separated list of panel UUIDs  up to a maximum
+            of 100.
+        :param str name: Comma separated list of panel names  up to a maximum
+            of 100. Also admits basic regular expressions using the operator
+            '~', i.e. '~{perl-regex}' e.g. '~value' for case sensitive,
+            '~/value/i' for case insensitive search.
         :param str internal_status: Filter by internal status.
+        :param str disorders: Comma separated list of disorder ids or names.
+            Also admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.. Also admits basic regular expressions
+            using the operator '~', i.e. '~{perl-regex}' e.g. '~value' for case
+            sensitive, '~/value/i' for case insensitive search.
+        :param str variants: Comma separated list of variant ids. Also admits
+            basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
+        :param str genes: Comma separated list of gene ids. Also admits basic
+            regular expressions using the operator '~', i.e. '~{perl-regex}'
+            e.g. '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
+        :param str source: Comma separated list of source ids or names.
+        :param str regions: Comma separated list of regions. Also admits basic
+            regular expressions using the operator '~', i.e. '~{perl-regex}'
+            e.g. '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
+        :param str categories: Comma separated list of category names. Also
+            admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
+        :param str tags: Panel tags. Also admits basic regular expressions
+            using the operator '~', i.e. '~{perl-regex}' e.g. '~value' for case
+            sensitive, '~/value/i' for case insensitive search.
+        :param bool deleted: Boolean to retrieve deleted entries.
+        :param str status: Filter by status.
         :param str creation_date: Creation date. Format: yyyyMMddHHmmss.
             Examples: >2018, 2017-2018, <201805.
         :param str modification_date: Modification date. Format:
             yyyyMMddHHmmss. Examples: >2018, 2017-2018, <201805.
-        :param bool visited: Visited status of job.
-        :param str tags: Job tags.
-        :param str input: Comma separated list of file IDs used as input.
-        :param str output: Comma separated list of file IDs used as output.
         :param str acl: Filter entries for which a user has the provided
             permissions. Format: acl={user}:{permissions}. Example:
             acl=john:WRITE,WRITE_ANNOTATIONS will return all entries for which
             user john has both WRITE and WRITE_ANNOTATIONS permissions. Only
             study owners or administrators can query by this field. .
         :param str release: Release when it was created.
-        :param bool deleted: Boolean to retrieve deleted entries.
+        :param int snapshot: Snapshot value (Latest version of the entry in
+            the specified release).
         """
 
         options['field'] = field
-        return self._get(category='jobs', resource='distinct', **options)
+        return self._get(category='panels', resource='distinct', **options)
 
-    def retry(self, data=None, **options):
+    def import_panels(self, data=None, **options):
         """
-        Relaunch a failed job.
-        PATH: /{apiVersion}/jobs/retry
+        Import panels.
+        PATH: /{apiVersion}/panels/import
 
-        :param dict data: job. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
-        :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
+        :param str job_description: Job description.
         :param str job_tags: Job tags.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param dict data: Panel parameters.
         """
 
-        return self._post(category='jobs', resource='retry', data=data, **options)
+        return self._post(category='panels', resource='import', data=data, **options)
 
     def search(self, **options):
         """
-        Job search method.
-        PATH: /{apiVersion}/jobs/search
+        Panel search.
+        PATH: /{apiVersion}/panels/search
 
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param int limit: Number of results to be returned.
         :param int skip: Number of results to skip.
         :param bool count: Get the total number of results matching the query.
             Deactivated by default.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
-        :param bool other_studies: Flag indicating the entries being queried
-            can belong to any related study, not just the primary one.
-        :param str id: Comma separated list of job IDs up to a maximum of 100.
-        :param str uuid: Comma separated list of job UUIDs up to a maximum of
-            100.
-        :param str tool_id: Tool ID executed by the job.
-        :param str tool_type: Tool type executed by the job [OPERATION,
-            ANALYSIS].
-        :param str user_id: User that created the job.
-        :param str priority: Priority of the job.
-        :param str status: Filter by status.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
+        :param str id: Comma separated list of panel IDs  up to a maximum of
+            100. Also admits basic regular expressions using the operator '~',
+            i.e. '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i'
+            for case insensitive search.
+        :param str uuid: Comma separated list of panel UUIDs  up to a maximum
+            of 100.
+        :param str name: Comma separated list of panel names  up to a maximum
+            of 100. Also admits basic regular expressions using the operator
+            '~', i.e. '~{perl-regex}' e.g. '~value' for case sensitive,
+            '~/value/i' for case insensitive search.
         :param str internal_status: Filter by internal status.
+        :param str disorders: Comma separated list of disorder ids or names.
+            Also admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.. Also admits basic regular expressions
+            using the operator '~', i.e. '~{perl-regex}' e.g. '~value' for case
+            sensitive, '~/value/i' for case insensitive search.
+        :param str variants: Comma separated list of variant ids. Also admits
+            basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
+        :param str genes: Comma separated list of gene ids. Also admits basic
+            regular expressions using the operator '~', i.e. '~{perl-regex}'
+            e.g. '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
+        :param str source: Comma separated list of source ids or names.
+        :param str regions: Comma separated list of regions. Also admits basic
+            regular expressions using the operator '~', i.e. '~{perl-regex}'
+            e.g. '~value' for case sensitive, '~/value/i' for case insensitive
+            search.
+        :param str categories: Comma separated list of category names. Also
+            admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
+        :param str tags: Panel tags. Also admits basic regular expressions
+            using the operator '~', i.e. '~{perl-regex}' e.g. '~value' for case
+            sensitive, '~/value/i' for case insensitive search.
+        :param bool deleted: Boolean to retrieve deleted entries.
+        :param str status: Filter by status.
         :param str creation_date: Creation date. Format: yyyyMMddHHmmss.
             Examples: >2018, 2017-2018, <201805.
         :param str modification_date: Modification date. Format:
             yyyyMMddHHmmss. Examples: >2018, 2017-2018, <201805.
-        :param bool visited: Visited status of job.
-        :param str tags: Job tags.
-        :param str input: Comma separated list of file IDs used as input.
-        :param str output: Comma separated list of file IDs used as output.
         :param str acl: Filter entries for which a user has the provided
             permissions. Format: acl={user}:{permissions}. Example:
             acl=john:WRITE,WRITE_ANNOTATIONS will return all entries for which
             user john has both WRITE and WRITE_ANNOTATIONS permissions. Only
             study owners or administrators can query by this field. .
         :param str release: Release when it was created.
-        :param bool deleted: Boolean to retrieve deleted entries.
-        """
-
-        return self._get(category='jobs', resource='search', **options)
-
-    def top(self, **options):
+        :param int snapshot: Snapshot value (Latest version of the entry in
+            the specified release).
         """
-        Provide a summary of the running jobs.
-        PATH: /{apiVersion}/jobs/top
 
-        :param int limit: Maximum number of jobs to be returned.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
-        :param str internal_status: Filter by internal status.
-        :param str priority: Priority of the job.
-        :param str user_id: User that created the job.
-        :param str tool_id: Tool ID executed by the job.
-        """
+        return self._get(category='panels', resource='search', **options)
 
-        return self._get(category='jobs', resource='top', **options)
-
-    def acl(self, jobs, **options):
+    def acl(self, panels, **options):
         """
-        Return the acl of the job. If member is provided, it will only return
-            the acl for the member.
-        PATH: /{apiVersion}/jobs/{jobs}/acl
+        Returns the acl of the panels. If member is provided, it will only
+            return the acl for the member.
+        PATH: /{apiVersion}/panels/{panels}/acl
 
-        :param str jobs: Comma separated list of job IDs or UUIDs up to a
-            maximum of 100. (REQUIRED)
+        :param str panels: Comma separated list of panel IDs up to a maximum
+            of 100. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str member: User or group id.
         :param bool silent: Boolean to retrieve all possible entries that are
             queried for, false to raise an exception whenever one of the
             entries looked for cannot be shown for whichever reason.
         """
 
-        return self._get(category='jobs', resource='acl', query_id=jobs, **options)
+        return self._get(category='panels', resource='acl', query_id=panels, **options)
 
-    def delete(self, jobs, **options):
+    def delete(self, panels, **options):
         """
-        Delete existing jobs.
-        PATH: /{apiVersion}/jobs/{jobs}/delete
+        Delete existing panels.
+        PATH: /{apiVersion}/panels/{panels}/delete
 
-        :param str jobs: Comma separated list of job ids. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str panels: Comma separated list of panel ids. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
-        return self._delete(category='jobs', resource='delete', query_id=jobs, **options)
+        return self._delete(category='panels', resource='delete', query_id=panels, **options)
 
-    def info(self, jobs, **options):
+    def info(self, panels, **options):
         """
-        Get job information.
-        PATH: /{apiVersion}/jobs/{jobs}/info
+        Panel info.
+        PATH: /{apiVersion}/panels/{panels}/info
 
-        :param str jobs: Comma separated list of job IDs or UUIDs up to a
-            maximum of 100. (REQUIRED)
+        :param str panels: Comma separated list of panel IDs up to a maximum
+            of 100. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
-        :param bool deleted: Boolean to retrieve deleted jobs.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
+        :param str version: Comma separated list of panel versions. 'all' to
+            get all the panel versions. Not supported if multiple panel ids are
+            provided.
+        :param bool deleted: Boolean to retrieve deleted panels.
         """
 
-        return self._get(category='jobs', resource='info', query_id=jobs, **options)
+        return self._get(category='panels', resource='info', query_id=panels, **options)
 
-    def update(self, jobs, data=None, **options):
+    def update(self, panels, data=None, **options):
         """
-        Update some job attributes.
-        PATH: /{apiVersion}/jobs/{jobs}/update
+        Update panel attributes.
+        PATH: /{apiVersion}/panels/{panels}/update
 
-        :param str jobs: Comma separated list of job IDs or UUIDs up to a
-            maximum of 100. (REQUIRED)
+        :param str panels: Comma separated list of panel ids. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool include_result: Flag indicating to include the created or
             updated document result in the response.
-        :param dict data: body.
-        """
-
-        return self._post(category='jobs', resource='update', query_id=jobs, data=data, **options)
-
-    def head_log(self, job, **options):
-        """
-        Show the first lines of a log file (up to a limit).
-        PATH: /{apiVersion}/jobs/{job}/log/head
-
-        :param str job: Job ID or UUID. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
-        :param int offset: Starting byte from which the file will be read.
-        :param int lines: Maximum number of lines to be returned up to a
-            maximum of 1000.
-        :param str type: Log file to be shown (stdout or stderr).
-        """
-
-        return self._get(category='jobs', resource='head', query_id=job, subcategory='log', **options)
-
-    def tail_log(self, job, **options):
-        """
-        Show the last lines of a log file (up to a limit).
-        PATH: /{apiVersion}/jobs/{job}/log/tail
-
-        :param str job: Job ID or UUID. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
-        :param int lines: Maximum number of lines to be returned up to a
-            maximum of 1000.
-        :param str type: Log file to be shown (stdout or stderr).
+        :param dict data: Panel parameters.
         """
 
-        return self._get(category='jobs', resource='tail', query_id=job, subcategory='log', **options)
+        return self._post(category='panels', resource='update', query_id=panels, data=data, **options)
```

### Comparing `pyopencga-2.9.2/pyopencga/rest_clients/meta_client.py` & `pyopencga-3.0.0/pyopencga/rest_clients/meta_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-04-18
+    Autogenerated on: 2024-03-06
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Meta(_ParentRestClient):
     """
     This class contains methods for the 'Meta' webservices
-    Client version: 2.8.0-SNAPSHOT
+    Client version: 3.0.0-SNAPSHOT
     PATH: /{apiVersion}/meta
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Meta, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def about(self, **options):
@@ -47,14 +47,16 @@
 
         return self._get(category='meta', resource='fail', **options)
 
     def model(self, **options):
         """
         Opencga model webservices.
         PATH: /{apiVersion}/meta/model
+
+        :param str model: Model description.
         """
 
         return self._get(category='meta', resource='model', **options)
 
     def ping(self, **options):
         """
         Ping Opencga webservices.
```

### Comparing `pyopencga-2.9.2/pyopencga/rest_clients/sample_client.py` & `pyopencga-3.0.0/pyopencga/rest_clients/sample_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-04-18
+    Autogenerated on: 2024-03-06
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Sample(_ParentRestClient):
     """
     This class contains methods for the 'Samples' webservices
-    Client version: 2.8.0-SNAPSHOT
+    Client version: 3.0.0-SNAPSHOT
     PATH: /{apiVersion}/samples
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Sample, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
@@ -30,61 +30,31 @@
             permissions. If propagate flag is set to true, it will propagate
             the permissions defined to the individuals that are associated to
             the matching samples. (REQUIRED)
         :param str action: Action to be performed [ADD, SET, REMOVE or RESET].
             Allowed values: ['SET ADD REMOVE RESET'] (REQUIRED)
         :param str members: Comma separated list of user or group ids.
             (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         options['action'] = action
         return self._post(category='samples', resource='update', subcategory='acl', second_query_id=members, data=data, **options)
 
-    def aggregation_stats(self, **options):
-        """
-        Fetch catalog sample stats.
-        PATH: /{apiVersion}/samples/aggregationStats
-
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
-        :param str source: Source.
-        :param str creation_year: Creation year.
-        :param str creation_month: Creation month (JANUARY, FEBRUARY...).
-        :param str creation_day: Creation day.
-        :param str creation_day_of_week: Creation day of week (MONDAY,
-            TUESDAY...).
-        :param str status: Status.
-        :param str type: Type.
-        :param str phenotypes: Phenotypes.
-        :param str release: Release.
-        :param str version: Version.
-        :param bool somatic: Somatic.
-        :param str annotation: Annotation filters. Example:
-            age>30;gender=FEMALE. For more information, please visit
-            http://docs.opencb.org/display/opencga/AnnotationSets+1.4.0.
-        :param bool default: Calculate default stats.
-        :param str field: List of fields separated by semicolons, e.g.:
-            studies;type. For nested fields use >>, e.g.:
-            studies>>biotype;type;numSamples[0..10]:1.
-        """
-
-        return self._get(category='samples', resource='aggregationStats', **options)
-
     def load_annotation_sets(self, variable_set_id, path, data=None, **options):
         """
         Load annotation sets from a TSV file.
         PATH: /{apiVersion}/samples/annotationSets/load
 
         :param str path: Path where the TSV file is located in OpenCGA or
             where it should be located. (REQUIRED)
         :param str variable_set_id: Variable set ID or name. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool parents: Flag indicating whether to create parent
             directories if they don't exist (only when TSV file was not
             previously associated).
         :param str annotation_set_id: Annotation set id. If not provided,
             variableSetId will be used.
         :param dict data: JSON containing the 'content' of the TSV file if
             this has not yet been registered into OpenCGA.
@@ -100,32 +70,35 @@
         PATH: /{apiVersion}/samples/create
 
         :param dict data: JSON containing sample information. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool include_result: Flag indicating to include the created or
             updated document result in the response.
         """
 
         return self._post(category='samples', resource='create', data=data, **options)
 
     def distinct(self, field, **options):
         """
         Sample distinct method.
         PATH: /{apiVersion}/samples/distinct
 
         :param str field: Comma separated list of fields for which to obtain
             the distinct values. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str id: Comma separated list sample IDs up to a maximum of 100.
+            Also admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
         :param str uuid: Comma separated list sample UUIDs up to a maximum of
             100.
         :param bool somatic: Somatic sample.
         :param str individual_id: Individual ID or UUID.
         :param str file_ids: Comma separated list of file IDs, paths or UUIDs.
         :param str cohort_ids: Comma separated list of cohort IDs.
         :param str creation_date: Creation date. Format: yyyyMMddHHmmss.
@@ -139,14 +112,17 @@
             method.
         :param str processing_extraction_method: Processing extraction method.
         :param str processing_lab_sample_id: Processing lab sample id.
         :param str collection_from: Collection from.
         :param str collection_type: Collection type.
         :param str collection_method: Collection method.
         :param str phenotypes: Comma separated list of phenotype ids or names.
+            Also admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
         :param str annotation: Annotation filters. Example:
             age>30;gender=FEMALE. For more information, please visit
             http://docs.opencb.org/display/opencga/AnnotationSets+1.4.0.
         :param str acl: Filter entries for which a user has the provided
             permissions. Format: acl={user}:{permissions}. Example:
             acl=john:WRITE,WRITE_ANNOTATIONS will return all entries for which
             user john has both WRITE and WRITE_ANNOTATIONS permissions. Only
@@ -184,16 +160,16 @@
 
     def load(self, file, **options):
         """
         Load samples from a ped file [EXPERIMENTAL].
         PATH: /{apiVersion}/samples/load
 
         :param str file: file. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str variable_set: variableSet.
         """
 
         options['file'] = file
         return self._get(category='samples', resource='load', **options)
 
     def search(self, **options):
@@ -208,17 +184,20 @@
         :param int limit: Number of results to be returned.
         :param int skip: Number of results to skip.
         :param bool count: Get the total number of results matching the query.
             Deactivated by default.
         :param bool include_individual: Include Individual object as an
             attribute.
         :param bool flatten_annotations: Flatten the annotations?.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str id: Comma separated list sample IDs up to a maximum of 100.
+            Also admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
         :param str uuid: Comma separated list sample UUIDs up to a maximum of
             100.
         :param bool somatic: Somatic sample.
         :param str individual_id: Individual ID or UUID.
         :param str file_ids: Comma separated list of file IDs, paths or UUIDs.
         :param str cohort_ids: Comma separated list of cohort IDs.
         :param str creation_date: Creation date. Format: yyyyMMddHHmmss.
@@ -232,14 +211,17 @@
             method.
         :param str processing_extraction_method: Processing extraction method.
         :param str processing_lab_sample_id: Processing lab sample id.
         :param str collection_from: Collection from.
         :param str collection_type: Collection type.
         :param str collection_method: Collection method.
         :param str phenotypes: Comma separated list of phenotype ids or names.
+            Also admits basic regular expressions using the operator '~', i.e.
+            '~{perl-regex}' e.g. '~value' for case sensitive, '~/value/i' for
+            case insensitive search.
         :param str annotation: Annotation filters. Example:
             age>30;gender=FEMALE. For more information, please visit
             http://docs.opencb.org/display/opencga/AnnotationSets+1.4.0.
         :param str acl: Filter entries for which a user has the provided
             permissions. Format: acl={user}:{permissions}. Example:
             acl=john:WRITE,WRITE_ANNOTATIONS will return all entries for which
             user john has both WRITE and WRITE_ANNOTATIONS permissions. Only
@@ -278,16 +260,16 @@
         """
         Returns the acl of the samples. If member is provided, it will only
             return the acl for the member.
         PATH: /{apiVersion}/samples/{samples}/acl
 
         :param str samples: Comma separated list sample IDs or UUIDs up to a
             maximum of 100. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str member: User or group id.
         :param bool silent: Boolean to retrieve all possible entries that are
             queried for, false to raise an exception whenever one of the
             entries looked for cannot be shown for whichever reason.
         """
 
         return self._get(category='samples', resource='acl', query_id=samples, **options)
@@ -302,16 +284,16 @@
         :param bool force: Force the deletion of samples even if they are
             associated to files, individuals or cohorts.
         :param str empty_files_action: Action to be performed over files that
             were associated only to the sample to be deleted. Possible actions
             are NONE, TRASH, DELETE.
         :param bool delete_empty_cohorts: Boolean indicating if the cohorts
             associated only to the sample to be deleted should be also deleted.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         return self._delete(category='samples', resource='delete', query_id=samples, **options)
 
     def info(self, samples, **options):
         """
         Get sample information.
@@ -322,16 +304,16 @@
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param bool include_individual: Include Individual object as an
             attribute.
         :param bool flatten_annotations: Flatten the annotations?.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str version: Comma separated list of sample versions. 'all' to
             get all the sample versions. Not supported if multiple sample ids
             are provided.
         :param bool deleted: Boolean to retrieve deleted entries.
         """
 
         return self._get(category='samples', resource='info', query_id=samples, **options)
@@ -343,16 +325,16 @@
 
         :param str samples: Comma separated list sample IDs or UUIDs up to a
             maximum of 100. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str annotation_sets_action: Action to be performed if the array
             of annotationSets is being updated. Allowed values: ['ADD SET
             REMOVE']
         :param str phenotypes_action: Action to be performed if the array of
             phenotypes is being updated [SET, ADD, REMOVE]. Allowed values:
             ['ADD SET REMOVE']
         :param bool include_result: Flag indicating to include the created or
@@ -365,16 +347,16 @@
     def update_annotation_sets_annotations(self, sample, annotation_set, data=None, **options):
         """
         Update annotations from an annotationSet.
         PATH: /{apiVersion}/samples/{sample}/annotationSets/{annotationSet}/annotations/update
 
         :param str annotation_set: AnnotationSet ID to be updated. (REQUIRED)
         :param str sample: Sample ID. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str action: Action to be performed: ADD to add new annotations;
             REPLACE to replace the value of an already existing annotation; SET
             to set the new list of annotations removing any possible old
             annotations; REMOVE to remove some annotations; RESET to set some
             annotations to the default value configured in the corresponding
             variables of the VariableSet if any. Allowed values: ['ADD SET
             REMOVE RESET REPLACE']
```

### Comparing `pyopencga-2.9.2/pyopencga/rest_clients/study_client.py` & `pyopencga-3.0.0/pyopencga/rest_clients/study_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-04-18
+    Autogenerated on: 2024-03-06
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Study(_ParentRestClient):
     """
     This class contains methods for the 'Studies' webservices
-    Client version: 2.8.0-SNAPSHOT
+    Client version: 3.0.0-SNAPSHOT
     PATH: /{apiVersion}/studies
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Study, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def update_acl(self, members, action, data=None, **options):
@@ -44,29 +44,29 @@
         PATH: /{apiVersion}/studies/create
 
         :param dict data: study. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str project: Project [user@]project where project can be either
-            the ID or the alias.
+        :param str project: Project [organization@]project where project can
+            be either the ID or the alias.
         :param bool include_result: Flag indicating to include the created or
             updated document result in the response.
         """
 
         return self._post(category='studies', resource='create', data=data, **options)
 
     def search(self, project, **options):
         """
         Search studies.
         PATH: /{apiVersion}/studies/search
 
-        :param str project: Project [user@]project where project can be either
-            the ID or the alias. (REQUIRED)
+        :param str project: Project [organization@]project where project can
+            be either the ID or the alias. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param int limit: Number of results to be returned.
         :param int skip: Number of results to skip.
         :param bool count: Get the total number of results matching the query.
@@ -91,62 +91,32 @@
     def acl(self, studies, **options):
         """
         Return the acl of the study. If member is provided, it will only
             return the acl for the member.
         PATH: /{apiVersion}/studies/{studies}/acl
 
         :param str studies: Comma separated list of Studies
-            [[user@]project:]study where study and project can be either the ID
-            or UUID up to a maximum of 100. (REQUIRED)
+            [[organization@]project:]study where study and project can be
+            either the ID or UUID up to a maximum of 100. (REQUIRED)
         :param str member: User or group id.
         :param bool silent: Boolean to retrieve all possible entries that are
             queried for, false to raise an exception whenever one of the
             entries looked for cannot be shown for whichever reason.
         """
 
         return self._get(category='studies', resource='acl', query_id=studies, **options)
 
-    def aggregation_stats(self, studies, **options):
-        """
-        Fetch catalog study stats.
-        PATH: /{apiVersion}/studies/{studies}/aggregationStats
-
-        :param str studies: Comma separated list of studies
-            [[user@]project:]study up to a maximum of 100. (REQUIRED)
-        :param bool default: Calculate default stats.
-        :param str file_fields: List of file fields separated by semicolons,
-            e.g.: studies;type. For nested fields use >>, e.g.:
-            studies>>biotype;type.
-        :param str individual_fields: List of individual fields separated by
-            semicolons, e.g.: studies;type. For nested fields use >>, e.g.:
-            studies>>biotype;type.
-        :param str family_fields: List of family fields separated by
-            semicolons, e.g.: studies;type. For nested fields use >>, e.g.:
-            studies>>biotype;type.
-        :param str sample_fields: List of sample fields separated by
-            semicolons, e.g.: studies;type. For nested fields use >>, e.g.:
-            studies>>biotype;type.
-        :param str cohort_fields: List of cohort fields separated by
-            semicolons, e.g.: studies;type. For nested fields use >>, e.g.:
-            studies>>biotype;type.
-        :param str job_fields: List of job fields separated by semicolons,
-            e.g.: studies;type. For nested fields use >>, e.g.:
-            studies>>biotype;type.
-        """
-
-        return self._get(category='studies', resource='aggregationStats', query_id=studies, **options)
-
     def info(self, studies, **options):
         """
         Fetch study information.
         PATH: /{apiVersion}/studies/{studies}/info
 
         :param str studies: Comma separated list of Studies
-            [[user@]project:]study where study and project can be either the ID
-            or UUID up to a maximum of 100. (REQUIRED)
+            [[organization@]project:]study where study and project can be
+            either the ID or UUID up to a maximum of 100. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         """
 
         return self._get(category='studies', resource='info', query_id=studies, **options)
@@ -164,18 +134,18 @@
         :param int limit: Number of results to be returned.
         :param int skip: Number of results to skip.
         :param bool count: Get the total number of results matching the query.
             Deactivated by default.
         :param str operation_id: Audit operation UUID.
         :param str user_id: User ID.
         :param str action: Action performed by the user.
-        :param str resource: Resource involved. Allowed values: ['AUDIT USER
-            PROJECT STUDY FILE SAMPLE JOB INDIVIDUAL COHORT DISEASE_PANEL
-            FAMILY CLINICAL_ANALYSIS INTERPRETATION VARIANT ALIGNMENT CLINICAL
-            EXPRESSION RGA FUNCTIONAL']
+        :param str resource: Resource involved. Allowed values: ['AUDIT
+            ORGANIZATION USER PROJECT STUDY FILE SAMPLE JOB INDIVIDUAL COHORT
+            DISEASE_PANEL FAMILY CLINICAL_ANALYSIS INTERPRETATION VARIANT
+            ALIGNMENT CLINICAL EXPRESSION RGA FUNCTIONAL']
         :param str resource_id: Resource ID.
         :param str resource_uuid: resource UUID.
         :param str status: Filter by status. Allowed values: ['SUCCESS ERROR']
         :param str date: Date. Format: yyyyMMddHHmmss. Examples: >2018,
             2017-2018, <201805.
         """
 
@@ -183,16 +153,16 @@
 
     def groups(self, study, **options):
         """
         Return the groups present in the study. For owners and administrators
             only.
         PATH: /{apiVersion}/studies/{study}/groups
 
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID. (REQUIRED)
         :param str id: Group id. If provided, it will only fetch information
             for the provided group.
         :param bool silent: Boolean to retrieve all possible entries that are
             queried for, false to raise an exception whenever one of the
             entries looked for cannot be shown for whichever reason.
         """
 
@@ -200,47 +170,47 @@
 
     def update_groups(self, study, data=None, **options):
         """
         Add or remove a group.
         PATH: /{apiVersion}/studies/{study}/groups/update
 
         :param dict data: JSON containing the parameters. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID. (REQUIRED)
         :param str action: Action to be performed: ADD or REMOVE a group.
             Allowed values: ['ADD REMOVE']
         """
 
         return self._post(category='studies', resource='update', query_id=study, subcategory='groups', data=data, **options)
 
     def update_groups_users(self, study, group, data=None, **options):
         """
         Add, set or remove users from an existing group.
         PATH: /{apiVersion}/studies/{study}/groups/{group}/users/update
 
         :param dict data: JSON containing the parameters. (REQUIRED)
         :param str group: Group name. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID. (REQUIRED)
         :param str action: Action to be performed: ADD, SET or REMOVE users
             to/from a group. Allowed values: ['ADD SET REMOVE']
         """
 
         return self._post(category='studies', resource='users/update', query_id=study, subcategory='groups', second_query_id=group, data=data, **options)
 
     def permission_rules(self, study, entity, **options):
         """
         Fetch permission rules.
         PATH: /{apiVersion}/studies/{study}/permissionRules
 
         :param str entity: Entity where the permission rules should be applied
             to. Allowed values: ['SAMPLES FILES COHORTS INDIVIDUALS FAMILIES
             JOBS CLINICAL_ANALYSES DISEASE_PANELS'] (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID. (REQUIRED)
         """
 
         options['entity'] = entity
         return self._get(category='studies', resource='permissionRules', query_id=study, **options)
 
     def update_permission_rules(self, study, entity, data=None, **options):
         """
@@ -248,16 +218,16 @@
         PATH: /{apiVersion}/studies/{study}/permissionRules/update
 
         :param dict data: JSON containing the permission rule to be created or
             removed. (REQUIRED)
         :param str entity: Entity where the permission rules should be applied
             to. Allowed values: ['SAMPLES FILES COHORTS INDIVIDUALS FAMILIES
             JOBS CLINICAL_ANALYSES DISEASE_PANELS'] (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID. (REQUIRED)
         :param str action: Action to be performed: ADD to add a new permission
             rule; REMOVE to remove all permissions assigned by an existing
             permission rule (even if it overlaps any manual permission); REVERT
             to remove all permissions assigned by an existing permission rule
             (keep manual overlaps); NONE to remove an existing permission rule
             without removing any permissions that could have been assigned
             already by the permission rule. Allowed values: ['ADD REMOVE REVERT
@@ -269,16 +239,16 @@
 
     def run_templates(self, study, data=None, **options):
         """
         Execute template.
         PATH: /{apiVersion}/studies/{study}/templates/run
 
         :param dict data: Template loader parameters. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID. (REQUIRED)
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_description: Job description.
         :param str job_tags: Job tags.
         """
@@ -286,41 +256,41 @@
         return self._post(category='studies', resource='run', query_id=study, subcategory='templates', data=data, **options)
 
     def upload_templates(self, study, **options):
         """
         Resource to upload a zipped template.
         PATH: /{apiVersion}/studies/{study}/templates/upload
 
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID. (REQUIRED)
         :param inputstream file: File to upload.
         """
 
         return self._post(category='studies', resource='upload', query_id=study, subcategory='templates', **options)
 
     def delete_templates(self, study, template_id, **options):
         """
         Delete template.
         PATH: /{apiVersion}/studies/{study}/templates/{templateId}/delete
 
         :param str template_id: Template id. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         """
 
         return self._delete(category='studies', resource='delete', query_id=study, subcategory='templates', second_query_id=template_id, **options)
 
     def update(self, study, data=None, **options):
         """
         Update some study attributes.
         PATH: /{apiVersion}/studies/{study}/update
 
         :param dict data: JSON containing the params to be updated. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
         :param bool include_result: Flag indicating to include the created or
             updated document result in the response.
         """
@@ -328,31 +298,31 @@
         return self._post(category='studies', resource='update', query_id=study, data=data, **options)
 
     def variable_sets(self, study, **options):
         """
         Fetch variableSets from a study.
         PATH: /{apiVersion}/studies/{study}/variableSets
 
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID. (REQUIRED)
         :param str id: Id of the variableSet to be retrieved. If no id is
             passed, it will show all the variableSets of the study.
         """
 
         return self._get(category='studies', resource='variableSets', query_id=study, **options)
 
     def update_variable_sets(self, study, data=None, **options):
         """
         Add or remove a variableSet.
         PATH: /{apiVersion}/studies/{study}/variableSets/update
 
         :param dict data: JSON containing the VariableSet to be created or
             removed. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID. (REQUIRED)
         :param str action: Action to be performed: ADD, REMOVE or FORCE_REMOVE
             a variableSet. Allowed values: ['ADD REMOVE FORCE_REMOVE']
         """
 
         return self._post(category='studies', resource='update', query_id=study, subcategory='variableSets', data=data, **options)
 
     def update_variable_sets_variables(self, study, variable_set, data=None, **options):
@@ -360,15 +330,15 @@
         Add or remove variables to a VariableSet.
         PATH: /{apiVersion}/studies/{study}/variableSets/{variableSet}/variables/update
 
         :param dict data: JSON containing the variable to be added or removed.
             For removing, only the variable id will be needed. (REQUIRED)
         :param str variable_set: VariableSet id of the VariableSet to be
             updated. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID. (REQUIRED)
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID. (REQUIRED)
         :param str action: Action to be performed: ADD or REMOVE a variable.
             Allowed values: ['ADD REMOVE']
         """
 
         return self._post(category='studies', resource='variables/update', query_id=study, subcategory='variableSets', second_query_id=variable_set, data=data, **options)
```

### Comparing `pyopencga-2.9.2/pyopencga/rest_clients/user_client.py` & `pyopencga-3.0.0/pyopencga/rest_clients/user_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,51 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-04-18
+    Autogenerated on: 2024-03-06
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class User(_ParentRestClient):
     """
     This class contains methods for the 'Users' webservices
-    Client version: 2.8.0-SNAPSHOT
+    Client version: 3.0.0-SNAPSHOT
     PATH: /{apiVersion}/users
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(User, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
+    def anonymous(self, organization, **options):
+        """
+        Get an anonymous token to gain access to the system.
+        PATH: /{apiVersion}/users/anonymous
+
+        :param str organization: Organization id. (REQUIRED)
+        """
+
+        options['organization'] = organization
+        return self._post(category='users', resource='anonymous', **options)
+
+    def create(self, data=None, **options):
+        """
+        Create a new user.
+        PATH: /{apiVersion}/users/create
+
+        :param dict data: JSON containing the parameters. (REQUIRED)
+        """
+
+        return self._post(category='users', resource='create', data=data, **options)
+
     def login(self, data=None, **options):
         """
         Get identified and gain access to the system.
         PATH: /{apiVersion}/users/login
 
         :param dict data: JSON containing the authentication parameters.
         """
@@ -48,14 +69,15 @@
         PATH: /{apiVersion}/users/{users}/info
 
         :param str users: Comma separated list of user IDs. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
+        :param str organization: Organization id.
         """
 
         return self._get(category='users', resource='info', query_id=users, **options)
 
     def configs(self, user, **options):
         """
         Fetch a user configuration.
@@ -126,30 +148,14 @@
         PATH: /{apiVersion}/users/{user}/password/reset
 
         :param str user: User ID. (REQUIRED)
         """
 
         return self._get(category='users', resource='reset', query_id=user, subcategory='password', **options)
 
-    def projects(self, user, **options):
-        """
-        Retrieve the projects of the user.
-        PATH: /{apiVersion}/users/{user}/projects
-
-        :param str user: User ID. (REQUIRED)
-        :param str include: Fields included in the response, whole JSON path
-            must be provided.
-        :param str exclude: Fields excluded in the response, whole JSON path
-            must be provided.
-        :param int limit: Number of results to be returned.
-        :param int skip: Number of results to skip.
-        """
-
-        return self._get(category='users', resource='projects', query_id=user, **options)
-
     def update(self, user, data=None, **options):
         """
         Update some user attributes.
         PATH: /{apiVersion}/users/{user}/update
 
         :param dict data: JSON containing the params to be updated. (REQUIRED)
         :param str user: User ID. (REQUIRED)
```

### Comparing `pyopencga-2.9.2/pyopencga/rest_clients/variant_client.py` & `pyopencga-3.0.0/pyopencga/rest_clients/variant_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-04-18
+    Autogenerated on: 2024-03-06
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class Variant(_ParentRestClient):
     """
     This class contains methods for the 'Analysis - Variant' webservices
-    Client version: 2.8.0-SNAPSHOT
+    Client version: 3.0.0-SNAPSHOT
     PATH: /{apiVersion}/analysis/variant
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(Variant, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def aggregation_stats(self, **options):
@@ -30,19 +30,19 @@
         :param str region: List of regions, these can be just a single
             chromosome name or regions in the format chr:start-end, e.g.:
             2,3:100000-200000.
         :param str type: List of types, accepted values are SNV, MNV, INDEL,
             SV, COPY_NUMBER, COPY_NUMBER_LOSS, COPY_NUMBER_GAIN, INSERTION,
             DELETION, DUPLICATION, TANDEM_DUPLICATION, BREAKEND, e.g.
             SNV,INDEL.
-        :param str project: Project [user@]project where project can be either
-            the ID or the alias.
+        :param str project: Project [organization@]project where project can
+            be either the ID or the alias.
         :param str study: Filter variants from the given studies, these can be
             either the numeric ID or the alias with the format
-            user@project:study.
+            organization@project:study.
         :param str cohort: Select variants with calculated stats for the
             selected cohorts.
         :param str cohort_stats_ref: Reference Allele Frequency:
             [{study:}]{cohort}[<|>|<=|>=]{number}. e.g. ALL<=0.4.
         :param str cohort_stats_alt: Alternate Allele Frequency:
             [{study:}]{cohort}[<|>|<=|>=]{number}. e.g. ALL<=0.4.
         :param str cohort_stats_maf: Minor Allele Frequency:
@@ -111,16 +111,16 @@
 
     def metadata_annotation(self, **options):
         """
         Read variant annotations metadata from any saved versions.
         PATH: /{apiVersion}/analysis/variant/annotation/metadata
 
         :param str annotation_id: Annotation identifier.
-        :param str project: Project [user@]project where project can be either
-            the ID or the alias.
+        :param str project: Project [organization@]project where project can
+            be either the ID or the alias.
         """
 
         return self._get(category='analysis', resource='metadata', subcategory='variant/annotation', **options)
 
     def query_annotation(self, **options):
         """
         Query variant annotations from any saved versions.
@@ -184,16 +184,16 @@
 
     def run_cohort_stats(self, data=None, **options):
         """
         Compute cohort variant stats for the selected list of samples.
         PATH: /{apiVersion}/analysis/variant/cohort/stats/run
 
         :param dict data: Cohort variant stats params. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -224,18 +224,18 @@
         PATH: /{apiVersion}/analysis/variant/export/run
 
         :param dict data: Variant export params. (REQUIRED)
         :param str include: Fields included in the response, whole JSON path
             must be provided.
         :param str exclude: Fields excluded in the response, whole JSON path
             must be provided.
-        :param str project: Project [user@]project where project can be either
-            the ID or the alias.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str project: Project [organization@]project where project can
+            be either the ID or the alias.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -247,16 +247,16 @@
         Calculate the possible genotypes for the members of a family.
         PATH: /{apiVersion}/analysis/variant/family/genotypes
 
         :param str mode_of_inheritance: Mode of inheritance. Allowed values:
             ['AUTOSOMAL_DOMINANT AUTOSOMAL_RECESSIVE X_LINKED_DOMINANT
             X_LINKED_RECESSIVE Y_LINKED MITOCHONDRIAL DE_NOVO MENDELIAN_ERROR
             COMPOUND_HETEROZYGOUS UNKNOWN'] (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str family: Family id.
         :param str clinical_analysis: Clinical analysis id.
         :param str penetrance: Penetrance. Allowed values: ['COMPLETE
             INCOMPLETE UNKNOWN']
         :param str disorder: Disorder id.
         """
 
@@ -269,16 +269,16 @@
             relatedness scores among the family members.
         PATH: /{apiVersion}/analysis/variant/family/qc/run
 
         :param dict data: Family QC analysis params. Family ID. Relatedness
             method, by default 'PLINK/IBD'. Minor  allele frequence (MAF) is
             used to filter variants before computing relatedness, e.g.:
             1000G:CEU>0.35 or cohort:ALL>0.05. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -292,16 +292,16 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str file: Files to remove.
         :param bool resume: Resume a previously failed indexation.
         """
 
         return self._delete(category='analysis', resource='delete', subcategory='variant/file', **options)
 
     def run_gatk(self, data=None, **options):
@@ -331,16 +331,16 @@
 
         :param dict data: Genome plot analysis params to customize the plot.
             The configuration file includes the title,  the plot density (i.e.,
             the number of points to display), the general query and the list of
             tracks. Currently, the supported track types are: COPY-NUMBER,
             INDEL, REARRANGEMENT and SNV. In addition, each track can contain a
             specific query. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -349,16 +349,16 @@
 
     def run_gwas(self, data=None, **options):
         """
         Run a Genome Wide Association Study between two cohorts.
         PATH: /{apiVersion}/analysis/variant/gwas/run
 
         :param dict data: Gwas analysis params. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -367,16 +367,16 @@
 
     def run_hr_detect(self, data=None, **options):
         """
         Run HRDetect analysis for a given somatic sample.
         PATH: /{apiVersion}/analysis/variant/hrDetect/run
 
         :param dict data: HRDetect analysis parameters. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -385,16 +385,16 @@
 
     def run_index(self, data=None, **options):
         """
          [DEPRECATED] Use operation/variant/index.
         PATH: /{apiVersion}/analysis/variant/index/run
 
         :param dict data: Variant index params. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_description: Job description.
         :param str job_tags: Job tags.
         """
@@ -404,16 +404,16 @@
     def run_individual_qc(self, data=None, **options):
         """
         Run quality control (QC) for a given individual. It includes inferred
             sex and  mendelian errors (UDP).
         PATH: /{apiVersion}/analysis/variant/individual/qc/run
 
         :param dict data: Individual QC analysis params. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -422,16 +422,16 @@
 
     def run_inferred_sex(self, data=None, **options):
         """
         Infer sex from chromosome mean coverages.
         PATH: /{apiVersion}/analysis/variant/inferredSex/run
 
         :param dict data: Inferred sex analysis params. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -483,16 +483,16 @@
 
     def run_mendelian_error(self, data=None, **options):
         """
         Run mendelian error analysis to infer uniparental disomy regions.
         PATH: /{apiVersion}/analysis/variant/mendelianError/run
 
         :param dict data: Mendelian error analysis params. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -500,19 +500,19 @@
         return self._post(category='analysis', resource='run', subcategory='variant/mendelianError', data=data, **options)
 
     def metadata(self, **options):
         """
         .
         PATH: /{apiVersion}/analysis/variant/metadata
 
-        :param str project: Project [user@]project where project can be either
-            the ID or the alias.
+        :param str project: Project [organization@]project where project can
+            be either the ID or the alias.
         :param str study: Filter variants from the given studies, these can be
             either the numeric ID or the alias with the format
-            user@project:study.
+            organization@project:study.
         :param str file: Filter variants from the files specified. This will
             set includeFile parameter when not provided.
         :param str sample: Filter variants by sample genotype. This will
             automatically set 'includeSample' parameter when not provided. This
             filter accepts multiple 3 forms: 1) List of samples: Samples that
             contain the main variant. Accepts AND (;) and OR (,) operators. 
             e.g. HG0097,HG0098 . 2) List of samples with genotypes:
@@ -551,15 +551,15 @@
         """
         Run mutational signature analysis for a given sample. Use context
             index.
         PATH: /{apiVersion}/analysis/variant/mutationalSignature/query
 
         :param str study: Filter variants from the given studies, these can be
             either the numeric ID or the alias with the format
-            user@project:study.
+            organization@project:study.
         :param str sample: Sample name.
         :param str type: Variant type. Valid values: SNV, SV.
         :param str ct: List of SO consequence types, e.g.
             missense_variant,stop_lost or SO:0001583,SO:0001578. Accepts
             aliases 'loss_of_function' and 'protein_altering'.
         :param str biotype: List of biotypes, e.g. protein_coding.
         :param str file_data: Filter by file data (i.e. FILTER, QUAL and INFO
@@ -605,16 +605,16 @@
         Run mutational signature analysis for a given sample.
         PATH: /{apiVersion}/analysis/variant/mutationalSignature/run
 
         :param dict data: Mutational signature analysis parameters to index
             the genome context for that sample, and to compute both catalogue
             counts and signature fitting. In order to skip one of them, , use
             the following keywords: , catalogue, fitting. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -668,19 +668,19 @@
             2,3:100000-200000.
         :param str type: List of types, accepted values are SNV, MNV, INDEL,
             SV, COPY_NUMBER, COPY_NUMBER_LOSS, COPY_NUMBER_GAIN, INSERTION,
             DELETION, DUPLICATION, TANDEM_DUPLICATION, BREAKEND, e.g.
             SNV,INDEL.
         :param str reference: Reference allele.
         :param str alternate: Main alternate allele.
-        :param str project: Project [user@]project where project can be either
-            the ID or the alias.
+        :param str project: Project [organization@]project where project can
+            be either the ID or the alias.
         :param str study: Filter variants from the given studies, these can be
             either the numeric ID or the alias with the format
-            user@project:study.
+            organization@project:study.
         :param str file: Filter variants from the files specified. This will
             set includeFile parameter when not provided.
         :param str filter: Specify the FILTER for any of the files. If 'file'
             filter is provided, will match the file and the filter. e.g.:
             PASS,LowGQX.
         :param str qual: Specify the QUAL for any of the files. If 'file'
             filter is provided, will match the file and the qual. e.g.: >123.4.
@@ -847,16 +847,16 @@
 
     def run_relatedness(self, data=None, **options):
         """
         Compute a score to quantify relatedness between samples.
         PATH: /{apiVersion}/analysis/variant/relatedness/run
 
         :param dict data: Relatedness analysis params. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -891,19 +891,19 @@
         :param str region: List of regions, these can be just a single
             chromosome name or regions in the format chr:start-end, e.g.:
             2,3:100000-200000.
         :param str type: List of types, accepted values are SNV, MNV, INDEL,
             SV, COPY_NUMBER, COPY_NUMBER_LOSS, COPY_NUMBER_GAIN, INSERTION,
             DELETION, DUPLICATION, TANDEM_DUPLICATION, BREAKEND, e.g.
             SNV,INDEL.
-        :param str project: Project [user@]project where project can be either
-            the ID or the alias.
+        :param str project: Project [organization@]project where project can
+            be either the ID or the alias.
         :param str study: Filter variants from the given studies, these can be
             either the numeric ID or the alias with the format
-            user@project:study.
+            organization@project:study.
         :param str file: Filter variants from the files specified. This will
             set includeFile parameter when not provided.
         :param str filter: Specify the FILTER for any of the files. If 'file'
             filter is provided, will match the file and the filter. e.g.:
             PASS,LowGQX.
         :param str sample: Filter variants by sample genotype. This will
             automatically set 'includeSample' parameter when not provided. This
@@ -969,16 +969,16 @@
     def run_sample_eligibility(self, data=None, **options):
         """
         Filter samples by a complex query involving metadata and variants
             data.
         PATH: /{apiVersion}/analysis/variant/sample/eligibility/run
 
         :param dict data: . (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -993,16 +993,16 @@
         PATH: /{apiVersion}/analysis/variant/sample/qc/run
 
         :param dict data: Sample QC analysis params. Mutational signature and
             genome plot are calculated for somatic samples only. In order to
             skip some metrics, use the following keywords (separated by
             commas): variant-stats, signature, signature-catalogue,
             signature-fitting, genome-plot. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -1026,16 +1026,16 @@
 
     def run_sample(self, data=None, **options):
         """
         Get samples given a set of variants.
         PATH: /{apiVersion}/analysis/variant/sample/run
 
         :param dict data: Sample variant filter params. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -1051,16 +1051,16 @@
         :param str region: List of regions, these can be just a single
             chromosome name or regions in the format chr:start-end, e.g.:
             2,3:100000-200000.
         :param str type: List of types, accepted values are SNV, MNV, INDEL,
             SV, COPY_NUMBER, COPY_NUMBER_LOSS, COPY_NUMBER_GAIN, INSERTION,
             DELETION, DUPLICATION, TANDEM_DUPLICATION, BREAKEND, e.g.
             SNV,INDEL.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str file: Filter variants from the files specified. This will
             set includeFile parameter when not provided.
         :param str filter: Specify the FILTER for any of the files. If 'file'
             filter is provided, will match the file and the filter. e.g.:
             PASS,LowGQX.
         :param str sample_data: Filter by any SampleData field from samples.
             [{sample}:]{key}{op}{value}[,;]* . If no sample is specified, will
@@ -1092,16 +1092,16 @@
         Compute sample variant stats for the selected list of samples.
         PATH: /{apiVersion}/analysis/variant/sample/stats/run
 
         :param dict data: Sample variant stats params. Use index=true and
             indexId='' to store the result in catalog sample QC. indexId=ALL
             requires an empty query. Use sample=all to compute sample stats of
             all samples in the variant storage. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -1110,18 +1110,18 @@
 
     def run_stats_export(self, data=None, **options):
         """
         Export calculated variant stats and frequencies.
         PATH: /{apiVersion}/analysis/variant/stats/export/run
 
         :param dict data: Variant stats export params. (REQUIRED)
-        :param str project: Project [user@]project where project can be either
-            the ID or the alias.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str project: Project [organization@]project where project can
+            be either the ID or the alias.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -1130,16 +1130,16 @@
 
     def run_stats(self, data=None, **options):
         """
         Compute variant stats for any cohort and any set of variants.
         PATH: /{apiVersion}/analysis/variant/stats/run
 
         :param dict data: Variant stats params. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
```

### Comparing `pyopencga-2.9.2/pyopencga/rest_clients/variant_operation_client.py` & `pyopencga-3.0.0/pyopencga/rest_clients/variant_operation_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
 WARNING: AUTOGENERATED CODE
 
     This code was generated by a tool.
-    Autogenerated on: 2023-04-18
+    Autogenerated on: 2024-03-06
     
     Manual changes to this file may cause unexpected behavior in your application.
     Manual changes to this file will be overwritten if the code is regenerated.
 """
 
 from pyopencga.rest_clients._parent_rest_clients import _ParentRestClient
 
 
 class VariantOperation(_ParentRestClient):
     """
     This class contains methods for the 'Operations - Variant Storage' webservices
-    Client version: 2.8.0-SNAPSHOT
+    Client version: 3.0.0-SNAPSHOT
     PATH: /{apiVersion}/operation
     """
 
     def __init__(self, configuration, token=None, login_handler=None, *args, **kwargs):
         super(VariantOperation, self).__init__(configuration, token, login_handler, *args, **kwargs)
 
     def configure_cellbase(self, data=None, **options):
         """
         Update Cellbase configuration.
         PATH: /{apiVersion}/operation/cellbase/configure
 
-        :param str project: Project [user@]project where project can be either
-            the ID or the alias.
+        :param str project: Project [organization@]project where project can
+            be either the ID or the alias.
         :param bool annotation_update: Create and load variant annotations
             into the database.
         :param str annotation_save_id: Save a copy of the current variant
             annotation at the database.
         :param dict data: New cellbase configuration.
         """
 
@@ -45,16 +45,16 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param dict data: Variant aggregate params.
         """
 
         return self._post(category='operation', resource='aggregate', subcategory='variant', data=data, **options)
 
     def delete_variant_annotation(self, **options):
         """
@@ -63,16 +63,16 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str project: Project [user@]project where project can be either
-            the ID or the alias.
+        :param str project: Project [organization@]project where project can
+            be either the ID or the alias.
         :param str annotation_id: Annotation identifier.
         """
 
         return self._delete(category='operation', resource='delete', subcategory='variant/annotation', **options)
 
     def index_variant_annotation(self, data=None, **options):
         """
@@ -81,18 +81,18 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str project: Project [user@]project where project can be either
-            the ID or the alias.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str project: Project [organization@]project where project can
+            be either the ID or the alias.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param dict data: Variant annotation index params.
         """
 
         return self._post(category='operation', resource='index', subcategory='variant/annotation', data=data, **options)
 
     def save_variant_annotation(self, data=None, **options):
         """
@@ -101,31 +101,31 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str project: Project [user@]project where project can be either
-            the ID or the alias.
+        :param str project: Project [organization@]project where project can
+            be either the ID or the alias.
         :param dict data: Variant annotation save params.
         """
 
         return self._post(category='operation', resource='save', subcategory='variant/annotation', data=data, **options)
 
     def configure_variant(self, data=None, **options):
         """
         Update Variant Storage Engine configuration. Can be updated at Project
             or Study level.
         PATH: /{apiVersion}/operation/variant/configure
 
-        :param str project: Project [user@]project where project can be either
-            the ID or the alias.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str project: Project [organization@]project where project can
+            be either the ID or the alias.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param dict data: Configuration params to update.
         """
 
         return self._post(category='operation', resource='configure', subcategory='variant', data=data, **options)
 
     def delete_variant(self, data=None, **options):
         """
@@ -134,16 +134,16 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param dict data: Variant delete file params.
         """
 
         return self._post(category='operation', resource='delete', subcategory='variant', data=data, **options)
 
     def aggregate_variant_family(self, data=None, **options):
         """
@@ -153,16 +153,16 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param dict data: Variant aggregate family params.
         """
 
         return self._post(category='operation', resource='aggregate', subcategory='variant/family', data=data, **options)
 
     def index_variant_family(self, data=None, **options):
         """
@@ -171,16 +171,16 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param dict data: Variant family index params.
         """
 
         return self._post(category='operation', resource='index', subcategory='variant/family', data=data, **options)
 
     def index_variant(self, data=None, **options):
         """
@@ -189,16 +189,16 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param dict data: Variant index params.
         """
 
         return self._post(category='operation', resource='index', subcategory='variant', data=data, **options)
 
     def launcher_variant_index(self, data=None, **options):
         """
@@ -208,16 +208,16 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param dict data: .
         """
 
         return self._post(category='operation', resource='launcher', subcategory='variant/index', data=data, **options)
 
     def run_variant_julie(self, data=None, **options):
         """
@@ -261,16 +261,16 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param dict data: Variant storage metadata synchronize params.
         """
 
         return self._post(category='operation', resource='synchronize', subcategory='variant/metadata', data=data, **options)
 
     def prune_variant(self, data=None, **options):
         """
@@ -296,16 +296,16 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param dict data: Variant delete sample params.
         """
 
         return self._post(category='operation', resource='delete', subcategory='variant/sample', data=data, **options)
 
     def index_variant_sample(self, data=None, **options):
         """
@@ -314,28 +314,28 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param dict data: Variant sample index params.
         """
 
         return self._post(category='operation', resource='index', subcategory='variant/sample', data=data, **options)
 
     def variant_sample_index_configure(self, data=None, **options):
         """
         DEPRECATED You should use the new sample index configure method.
         PATH: /{apiVersion}/operation/variant/sample/index/configure
 
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool skip_rebuild: Skip sample index re-build.
         :param dict data: New SampleIndexConfiguration.
         """
 
         return self._post(category='operation', resource='configure', subcategory='variant/sample/index', data=data, **options)
 
     def delete_variant_score(self, **options):
@@ -345,16 +345,16 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str name: Unique name of the score within the study.
         :param bool resume: Resume a previously failed remove.
         :param bool force: Force remove of partially indexed scores.
         """
 
         return self._delete(category='operation', resource='delete', subcategory='variant/score', **options)
 
@@ -365,16 +365,16 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param dict data: Variant score index params. scoreName: Unique name
             of the score within the study. cohort1: Cohort used to compute the
             score. Use the cohort 'ALL' if all samples from the study where
             used to compute the score. cohort2: Second cohort used to compute
             the score, typically to compare against the first cohort. If only
             one cohort was used to compute the score, leave empty.
             inputColumns: Indicate which columns to load from the input file.
@@ -399,18 +399,18 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str project: Project [user@]project where project can be either
-            the ID or the alias.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str project: Project [organization@]project where project can
+            be either the ID or the alias.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param dict data: Variant secondary annotation index params.
         """
 
         return self._post(category='operation', resource='index', subcategory='variant/secondary/annotation', data=data, **options)
 
     def variant_secondary_sample_index(self, data=None, **options):
         """
@@ -419,28 +419,28 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param dict data: Variant sample index params.
         """
 
         return self._post(category='operation', resource='index', subcategory='variant/secondary/sample', data=data, **options)
 
     def configure_variant_secondary_sample_index(self, data=None, **options):
         """
         Update SampleIndex configuration (New!).
         PATH: /{apiVersion}/operation/variant/secondary/sample/index/configure
 
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param bool skip_rebuild: Skip sample index re-build.
         :param dict data: New SampleIndexConfiguration.
         """
 
         return self._post(category='operation', resource='configure', subcategory='variant/secondary/sample/index', data=data, **options)
 
     def secondary_index_variant(self, data=None, **options):
@@ -450,18 +450,18 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str project: Project [user@]project where project can be either
-            the ID or the alias.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str project: Project [organization@]project where project can
+            be either the ID or the alias.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param dict data: Variant secondary annotation index params.
         """
 
         return self._post(category='operation', resource='secondaryIndex', subcategory='variant', data=data, **options)
 
     def delete_variant_secondary_index(self, **options):
         """
@@ -471,30 +471,30 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str samples: Samples to remove. Needs to provide all the
             samples in the secondary index.
         """
 
         return self._delete(category='operation', resource='delete', subcategory='variant/secondaryIndex', **options)
 
     def delete_variant_stats(self, data=None, **options):
         """
         Deletes the VariantStats of a cohort/s from the database.
         PATH: /{apiVersion}/operation/variant/stats/delete
 
         :param dict data: Variant stats delete params. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -504,16 +504,16 @@
     def index_variant_stats(self, data=None, **options):
         """
         Compute variant stats for any cohort and any set of variants and index
             the result in the variant storage database.
         PATH: /{apiVersion}/operation/variant/stats/index
 
         :param dict data: Variant stats params. (REQUIRED)
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
         """
@@ -527,14 +527,14 @@
 
         :param str job_id: Job ID. It must be a unique string within the
             study. An ID will be autogenerated automatically if not provided.
         :param str job_description: Job description.
         :param str job_depends_on: Comma separated list of existing job IDs
             the job will depend on.
         :param str job_tags: Job tags.
-        :param str study: Study [[user@]project:]study where study and project
-            can be either the ID or UUID.
+        :param str study: Study [[organization@]project:]study where study and
+            project can be either the ID or UUID.
         :param dict data: Variant delete study params.
         """
 
         return self._post(category='operation', resource='delete', subcategory='variant/study', data=data, **options)
```

### Comparing `pyopencga-2.9.2/pyopencga/rest_response.py` & `pyopencga-3.0.0/pyopencga/rest_response.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.9.2/pyopencga/retry.py` & `pyopencga-3.0.0/pyopencga/retry.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.9.2/pyopencga.egg-info/PKG-INFO` & `pyopencga-3.0.0/pyopencga.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencga
-Version: 2.9.2
+Version: 3.0.0
 Summary: A REST client for OpenCGA REST web services
 Home-page: https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
 Author: David Gomez-Peregrina, Pablo Marin-Garcia, Daniel Perez-Gil
 Author-email: david.gomez@mgviz.org, pmarin@kanteron.com, dp529@cam.ac.uk
 License: Apache Software License
 Project-URL: Documentation, http://docs.opencb.org/display/opencga/Python
 Project-URL: Source, https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
@@ -17,14 +17,19 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: requests>=2.7
+Requires-Dist: pip>=7.1.2
+Requires-Dist: pathlib>=1.0.1
+Requires-Dist: pyyaml>=3.12
+Requires-Dist: pandas>=1.1.5
 
 .. contents::
 
 PyOpenCGA
 ==========
 
 This Python client package makes use of the comprehensive RESTful web services API implemented for the `OpenCGA`_ platform.
```

### Comparing `pyopencga-2.9.2/pyopencga.egg-info/SOURCES.txt` & `pyopencga-3.0.0/pyopencga.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -23,13 +23,14 @@
 pyopencga/rest_clients/disease_panel_client.py
 pyopencga/rest_clients/family_client.py
 pyopencga/rest_clients/file_client.py
 pyopencga/rest_clients/ga4gh_client.py
 pyopencga/rest_clients/individual_client.py
 pyopencga/rest_clients/job_client.py
 pyopencga/rest_clients/meta_client.py
+pyopencga/rest_clients/organization_client.py
 pyopencga/rest_clients/project_client.py
 pyopencga/rest_clients/sample_client.py
 pyopencga/rest_clients/study_client.py
 pyopencga/rest_clients/user_client.py
 pyopencga/rest_clients/variant_client.py
 pyopencga/rest_clients/variant_operation_client.py
```

### Comparing `pyopencga-2.9.2/setup.py` & `pyopencga-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pyopencga',
-    version='2.9.2',
+    version='3.0.0',
     description='A REST client for OpenCGA REST web services',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     url='https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga',
     packages=['pyopencga', 'pyopencga.rest_clients'],
     license='Apache Software License',
     author='David Gomez-Peregrina, Pablo Marin-Garcia, Daniel Perez-Gil',
```

