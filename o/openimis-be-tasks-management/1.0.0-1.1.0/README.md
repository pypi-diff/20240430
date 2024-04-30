# Comparing `tmp/openimis-be-tasks_management-1.0.0.tar.gz` & `tmp/openimis_be_tasks_management-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-tasks_management-1.0.0.tar", last modified: Sat Dec 16 01:08:30 2023, max compression
+gzip compressed data, was "openimis_be_tasks_management-1.1.0.tar", last modified: Tue Apr 30 09:00:25 2024, max compression
```

## Comparing `openimis-be-tasks_management-1.0.0.tar` & `openimis_be_tasks_management-1.1.0.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:08:30.860971 openimis-be-tasks_management-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2023-12-16 01:08:30.860971 openimis-be-tasks_management-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:08:30.860971 openimis-be-tasks_management-1.0.0/openimis_be_tasks_management.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2023-12-16 01:08:30.000000 openimis-be-tasks_management-1.0.0/openimis_be_tasks_management.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2023-12-16 01:08:30.000000 openimis-be-tasks_management-1.0.0/openimis_be_tasks_management.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 01:08:30.000000 openimis-be-tasks_management-1.0.0/openimis_be_tasks_management.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-12-16 01:08:30.000000 openimis-be-tasks_management-1.0.0/openimis_be_tasks_management.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-16 01:08:30.000000 openimis-be-tasks_management-1.0.0/openimis_be_tasks_management.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 01:08:30.860971 openimis-be-tasks_management-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-12-16 01:08:30.000000 openimis-be-tasks_management-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:08:30.856971 openimis-be-tasks_management-1.0.0/tasks_management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:08:30.856971 openimis-be-tasks_management-1.0.0/tasks_management/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/migrations/0002_add_task_triage_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/migrations/0003_historicaltaskexecutor_taskexecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/migrations/0004_auto_20230628_1404.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/migrations/0005_add_task_perms_to_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/migrations/0006_add_search_users_to_task_triage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/migrations/0007_taskmutation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    13539 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:08:30.856971 openimis-be-tasks_management-1.0.0/tasks_management/signals/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/signals/on_task_resolve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:08:30.860971 openimis-be-tasks_management-1.0.0/tasks_management/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/tests/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/tests/task_event_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/tests/task_group_service_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/tests/task_service_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 01:08:18.000000 openimis-be-tasks_management-1.0.0/tasks_management/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:25.222506 openimis_be_tasks_management-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-30 09:00:25.222506 openimis_be_tasks_management-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:25.222506 openimis_be_tasks_management-1.1.0/openimis_be_tasks_management.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-30 09:00:25.000000 openimis_be_tasks_management-1.1.0/openimis_be_tasks_management.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-30 09:00:25.000000 openimis_be_tasks_management-1.1.0/openimis_be_tasks_management.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:00:25.000000 openimis_be_tasks_management-1.1.0/openimis_be_tasks_management.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 09:00:25.000000 openimis_be_tasks_management-1.1.0/openimis_be_tasks_management.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 09:00:25.000000 openimis_be_tasks_management-1.1.0/openimis_be_tasks_management.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:00:25.222506 openimis_be_tasks_management-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-30 09:00:24.000000 openimis_be_tasks_management-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:25.218506 openimis_be_tasks_management-1.1.0/tasks_management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:25.218506 openimis_be_tasks_management-1.1.0/tasks_management/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/migrations/0002_add_task_triage_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/migrations/0003_historicaltaskexecutor_taskexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/migrations/0004_auto_20230628_1404.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/migrations/0005_add_task_perms_to_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/migrations/0006_add_search_users_to_task_triage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/migrations/0007_taskmutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/migrations/0008_auto_20240118_1510.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/migrations/0009_alter_historicaltask_business_data_serializer_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/migrations/0010_add_search_all_perms_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17915 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:25.218506 openimis_be_tasks_management-1.1.0/tasks_management/signals/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/signals/on_task_resolve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:25.222506 openimis_be_tasks_management-1.1.0/tasks_management/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/tests/task_event_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/tests/task_group_service_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/tests/task_service_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:00:16.000000 openimis_be_tasks_management-1.1.0/tasks_management/views.py
```

### Comparing `openimis-be-tasks_management-1.0.0/LICENSE.md` & `openimis_be_tasks_management-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-tasks_management-1.0.0/PKG-INFO` & `openimis_be_tasks_management-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-tasks_management
-Version: 1.0.0
+Version: 1.1.0
 Summary: The openIMIS Backend tasks_management reference module.
 Home-page: https://openimis.org/
 Author: jdolkowski
 Author-email: jdolkowski@gmail.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-tasks_management-1.0.0/README.md` & `openimis_be_tasks_management-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-tasks_management-1.0.0/openimis_be_tasks_management.egg-info/PKG-INFO` & `openimis_be_tasks_management-1.1.0/openimis_be_tasks_management.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openimis-be-tasks-management
-Version: 1.0.0
+Name: openimis-be-tasks_management
+Version: 1.1.0
 Summary: The openIMIS Backend tasks_management reference module.
 Home-page: https://openimis.org/
 Author: jdolkowski
 Author-email: jdolkowski@gmail.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-tasks_management-1.0.0/openimis_be_tasks_management.egg-info/SOURCES.txt` & `openimis_be_tasks_management-1.1.0/openimis_be_tasks_management.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 tasks_management/apps.py
 tasks_management/gql_mutations.py
 tasks_management/gql_queries.py
 tasks_management/models.py
 tasks_management/schema.py
 tasks_management/services.py
 tasks_management/urls.py
-tasks_management/utils.py
 tasks_management/validation.py
 tasks_management/views.py
 tasks_management/migrations/0001_initial.py
 tasks_management/migrations/0002_add_task_triage_role.py
 tasks_management/migrations/0003_historicaltaskexecutor_taskexecutor.py
 tasks_management/migrations/0004_auto_20230628_1404.py
 tasks_management/migrations/0005_add_task_perms_to_admin.py
 tasks_management/migrations/0006_add_search_users_to_task_triage.py
 tasks_management/migrations/0007_taskmutation.py
+tasks_management/migrations/0008_auto_20240118_1510.py
+tasks_management/migrations/0009_alter_historicaltask_business_data_serializer_and_more.py
+tasks_management/migrations/0010_add_search_all_perms_admin.py
 tasks_management/migrations/__init__.py
 tasks_management/signals/__init__.py
 tasks_management/signals/on_task_resolve.py
 tasks_management/tests/__init__.py
 tasks_management/tests/data.py
 tasks_management/tests/helpers.py
 tasks_management/tests/task_event_tests.py
```

### Comparing `openimis-be-tasks_management-1.0.0/setup.py` & `openimis_be_tasks_management-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-tasks_management',
-    version='1.0.0',
+    version='v1.1.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend tasks_management reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

### Comparing `openimis-be-tasks_management-1.0.0/tasks_management/apps.py` & `openimis_be_tasks_management-1.1.0/tasks_management/apps.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from django.apps import AppConfig
 
 DEFAULT_CONFIG = {
     "gql_task_group_search_perms": ["190001"],
     "gql_task_group_create_perms": ["190002"],
     "gql_task_group_update_perms": ["190003"],
     "gql_task_group_delete_perms": ["190004"],
+    
     "gql_task_search_perms": ["191001"],
     "gql_task_create_perms": ["191002"],
     "gql_task_update_perms": ["191003"],
     "gql_task_delete_perms": ["191004"],
+    "gql_task_search_all_perms": ["191005"],
     # To be used if task should use generic resolver
-    "default_executor_event": "default"
+    "default_executor_event": "default",
+    "task_user_approved": "APPROVED",
 }
 
 
 class TasksManagementConfig(AppConfig):
     default_auto_field = 'django.db.models.BigAutoField'
     name = 'tasks_management'
 
@@ -22,15 +25,17 @@
     gql_task_group_create_perms = None
     gql_task_group_update_perms = None
     gql_task_group_delete_perms = None
     gql_task_search_perms = None
     gql_task_create_perms = None
     gql_task_update_perms = None
     gql_task_delete_perms = None
+    gql_task_search_all_perms = None
     default_executor_event = None
+    task_user_approved = None
 
     def ready(self):
         from core.models import ModuleConfiguration
 
         cfg = ModuleConfiguration.get_or_default(self.name, DEFAULT_CONFIG)
         self.__load_config(cfg)
```

### Comparing `openimis-be-tasks_management-1.0.0/tasks_management/gql_mutations.py` & `openimis_be_tasks_management-1.1.0/tasks_management/gql_mutations.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         ALL = TaskGroup.TaskGroupCompletionPolicy.ALL
         ANY = TaskGroup.TaskGroupCompletionPolicy.ANY
         N = TaskGroup.TaskGroupCompletionPolicy.N
 
     code = graphene.String(required=True, max_length=255)
     completion_policy = graphene.Field(TaskGroupCompletionPolicyEnum, required=True)
     user_ids = graphene.List(graphene.UUID)
+    task_sources = graphene.List(graphene.String)
 
     def resolve_completion_policy(self, info):
         return self.completion_policy
 
 
 class UpdateTaskInput(OpenIMISMutation.Input):
     class TaskStatusEnum(graphene.Enum):
@@ -39,14 +40,15 @@
 class UpdateTaskGroupInput(CreateTaskGroupInput):
     id = graphene.UUID(required=True)
 
 
 class ResolveTaskGroupInput(OpenIMISMutation.Input):
     id = graphene.UUID(required=True)
     business_status = graphene.JSONString(required=True)
+    additional_data = graphene.JSONString(required=False)
 
 
 class CreateTaskGroupMutation(BaseHistoryModelCreateMutationMixin, BaseMutation):
     _mutation_class = "CreateTaskGroupMutation"
     _mutation_module = "tasks_management"
     _model = TaskGroup
```

### Comparing `openimis-be-tasks_management-1.0.0/tasks_management/gql_queries.py` & `openimis_be_tasks_management-1.1.0/tasks_management/gql_queries.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,33 @@
-import json
+import importlib
+
 import graphene
-from uuid import UUID
+import copy
 
 from django.db.models import Q
 from graphene_django import DjangoObjectType
 
 from core import ExtendedConnection, prefix_filterset
-from core.datetimes.ad_datetime import AdDatetime
 from core.gql_queries import UserGQLType
-from core.models import HistoryModel, Role
-from core.services.utils import model_representation
 from tasks_management.apps import TasksManagementConfig
 from tasks_management.models import TaskGroup, TaskExecutor, Task
 
 DICT_STRING = "{}"
 
 
-def _convert_to_serializable_json(entity):
-    converted_dict = {}
-    model_fields = set([field.name for field in entity._meta.fields])
-    history_fields = set([field.name for field in HistoryModel._meta.fields])
-    fields_to_exclude = history_fields.intersection(model_fields)
-
-    for key, value in model_representation(entity).items():
-        if key in fields_to_exclude:
-            continue
-
-        if isinstance(value, AdDatetime):
-            ad_datetime_str = value.strftime('%Y-%m-%d %H:%M:%S')
-            value = ad_datetime_str
-
-        if isinstance(value, UUID):
-            value = str(value)
-
-        converted_dict[key] = value
-
-    return json.dumps(converted_dict)
-
-
 def is_task_triage(user):
     return user.has_perms(TasksManagementConfig.gql_task_group_create_perms
                           + TasksManagementConfig.gql_task_group_search_perms
                           + TasksManagementConfig.gql_task_group_update_perms
                           + TasksManagementConfig.gql_task_group_delete_perms)
 
 
 class TaskGQLType(DjangoObjectType):
     uuid = graphene.String(source='uuid')
-    current_entity_data = graphene.JSONString()
+    business_data = graphene.JSONString()
     entity_string = graphene.String()
 
     class Meta:
         model = Task
         interfaces = (graphene.relay.Node,)
         filter_fields = {
             "id": ["exact"],
@@ -66,20 +42,41 @@
             "date_created": ["exact", "lt", "lte", "gt", "gte"],
             "date_updated": ["exact", "lt", "lte", "gt", "gte"],
             "is_deleted": ["exact"],
             "version": ["exact"],
         }
         connection_class = ExtendedConnection
 
-    def resolve_current_entity_data(self, info):
-        entity = self.entity
-        if entity:
-            serialized_json = _convert_to_serializable_json(entity)
-            return serialized_json
-        return DICT_STRING
+    def resolve_business_data(self, info):
+        data = self.data
+        serializer_path = self.business_data_serializer
+        serialized_data = copy.deepcopy(data)
+        if serializer_path:
+            module_path, class_name, method_name = serializer_path.rsplit('.', 2)
+
+            try:
+                service_module = importlib.import_module(module_path)
+
+                if hasattr(service_module, class_name):
+                    service_class = getattr(service_module, class_name)
+                    instance = service_class(info.context.user)
+
+                    serializer_method = getattr(instance, method_name, None)
+
+                    if callable(serializer_method):
+                        serialized_data = serializer_method(serialized_data)
+
+            except ImportError:
+                return f"Error: Module '{module_path}' not found."
+            except AttributeError:
+                return f"Error: Attribute not found in the module or class."
+            except Exception as e:
+                return f"Error: {str(e)}"
+
+        return serialized_data
 
     def resolve_entity_string(self, info):
         return self.entity.__str__()
 
     @classmethod
     def get_queryset(cls, queryset, info):
         user = info.context.user
```

### Comparing `openimis-be-tasks_management-1.0.0/tasks_management/migrations/0001_initial.py` & `openimis_be_tasks_management-1.1.0/tasks_management/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tasks_management-1.0.0/tasks_management/migrations/0002_add_task_triage_role.py` & `openimis_be_tasks_management-1.1.0/tasks_management/migrations/0002_add_task_triage_role.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tasks_management-1.0.0/tasks_management/migrations/0003_historicaltaskexecutor_taskexecutor.py` & `openimis_be_tasks_management-1.1.0/tasks_management/migrations/0003_historicaltaskexecutor_taskexecutor.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tasks_management-1.0.0/tasks_management/migrations/0004_auto_20230628_1404.py` & `openimis_be_tasks_management-1.1.0/tasks_management/migrations/0004_auto_20230628_1404.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tasks_management-1.0.0/tasks_management/migrations/0005_add_task_perms_to_admin.py` & `openimis_be_tasks_management-1.1.0/tasks_management/migrations/0005_add_task_perms_to_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tasks_management-1.0.0/tasks_management/migrations/0006_add_search_users_to_task_triage.py` & `openimis_be_tasks_management-1.1.0/tasks_management/migrations/0006_add_search_users_to_task_triage.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tasks_management-1.0.0/tasks_management/migrations/0007_taskmutation.py` & `openimis_be_tasks_management-1.1.0/tasks_management/migrations/0007_taskmutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tasks_management-1.0.0/tasks_management/models.py` & `openimis_be_tasks_management-1.1.0/tasks_management/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,22 +27,23 @@
 class Task(HistoryModel):
     class Status(models.TextChoices):
         RECEIVED = 'RECEIVED', _('Received')
         ACCEPTED = 'ACCEPTED', _('Accepted')
         COMPLETED = 'COMPLETED', _('Completed')
         FAILED = 'FAILED', _('Failed')
 
-    source = models.CharField(max_length=255, null=True)
-    entity_type = models.ForeignKey(ContentType, models.DO_NOTHING, null=True, unique=False)
-    entity_id = models.CharField(max_length=255, null=True)
+    source = models.CharField(max_length=255,  blank=True, null=True)
+    entity_type = models.ForeignKey(ContentType, models.DO_NOTHING, blank=True, null=True, unique=False)
+    entity_id = models.CharField(max_length=255,  blank=True, null=True)
     entity = GenericForeignKey('entity_type', 'entity_id')
     status = models.CharField(max_length=255, choices=Status.choices, default=Status.RECEIVED)
-    executor_action_event = models.CharField(max_length=255, null=True)
-    business_status = models.JSONField(default=dict)
-    business_event = models.CharField(max_length=255, null=True)
-    task_group = models.ForeignKey(TaskGroup, on_delete=models.DO_NOTHING, null=True)
-    data = models.JSONField(default=dict)
+    executor_action_event = models.CharField(max_length=255, blank=True, null=True)
+    business_status = models.JSONField( blank=True,default=dict)
+    business_event = models.CharField(max_length=255, blank=True, null=True)
+    task_group = models.ForeignKey(TaskGroup, on_delete=models.DO_NOTHING,  blank=True, null=True)
+    data = models.JSONField(blank=True, default=dict)
+    business_data_serializer = models.CharField(max_length=255, blank=True, null=True)
 
 
 class TaskMutation(UUIDModel, ObjectMutation):
     task = models.ForeignKey(Task, models.DO_NOTHING, related_name='mutations')
     mutation = models.ForeignKey(MutationLog, models.DO_NOTHING, related_name='task')
```

### Comparing `openimis-be-tasks_management-1.0.0/tasks_management/schema.py` & `openimis_be_tasks_management-1.1.0/tasks_management/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import graphene
+import json
 import graphene_django_optimizer as gql_optimizer
 
 from django.contrib.auth.models import AnonymousUser
 from django.db.models import Q
 
 from core.schema import OrderedDjangoFilterConnectionField
 from core.utils import append_validity_filter
@@ -36,29 +37,42 @@
     task = OrderedDjangoFilterConnectionField(
         TaskGQLType,
         orderBy=graphene.List(of_type=graphene.String),
         applyDefaultValidityFilter=graphene.Boolean(),
         client_mutation_id=graphene.String(),
         groupId=graphene.String(),
         customFilters=graphene.List(of_type=graphene.String),
-        taskGroupId=graphene.String()
+        taskGroupId=graphene.String(),
+        entityIds=graphene.List(graphene.UUID),
+        entityString__Icontains=graphene.String(),
     )
 
     def resolve_task(self, info, **kwargs):
         filters = append_validity_filter(**kwargs)
 
         client_mutation_id = kwargs.get("client_mutation_id")
         if client_mutation_id:
             filters.append(Q(mutations__mutation__client_mutation_id=client_mutation_id))
 
         taskGroupId = kwargs.get("taskGroupId")
         if taskGroupId:
             filters.append(Q(task_group__id=taskGroupId))
+
+        entityIds = kwargs.get("entityIds")
+        if entityIds:
+            filters.append(Q(entity_id__in=entityIds))
+
         # not checking perms because get_queryset filters tasks assigned to user
         query = Task.objects.filter(*filters)
+
+        entity_string = kwargs.get("entityString__Icontains")
+        if entity_string:
+            task_ids = [task.id for task in query if entity_string.lower() in str(task.entity).lower()]
+            query = query.filter(id__in=task_ids)
+
         return gql_optimizer.query(query, info)
 
     def resolve_task_group(self, info, **kwargs):
         filters = append_validity_filter(**kwargs)
 
         client_mutation_id = kwargs.get("client_mutation_id", None)
         if client_mutation_id:
```

### Comparing `openimis-be-tasks_management-1.0.0/tasks_management/services.py` & `openimis_be_tasks_management-1.1.0/tasks_management/services.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 import copy
 import datetime
 import decimal
 import logging
-import json
 import uuid
 from abc import abstractmethod, ABC
 from typing import Dict, Type
-from uuid import UUID
-
 from django.contrib.contenttypes.models import ContentType
 from django.db import transaction
 
+from django.core.exceptions import ValidationError
+from core.datetimes.ad_datetime import AdDate, AdDatetime
 from core.forms import User
 from core.services import BaseService
 from core.signals import register_service_signal
 from core.services.utils import check_authentication, output_exception, output_result_success, model_representation
 from tasks_management.apps import TasksManagementConfig
-
 from tasks_management.models import TaskGroup, TaskExecutor, Task
 from tasks_management.validation import TaskGroupValidation, TaskExecutorValidation, TaskValidation
 
 logger = logging.getLogger(__name__)
 
+non_serializable_types = (
+    uuid.UUID,
+    datetime.date,
+    AdDate,
+    AdDatetime,
+    decimal.Decimal,
+)
+
 
 class TaskService(BaseService):
     OBJECT_TYPE = Task
 
     def __init__(self, user, validation_class=TaskValidation):
         super().__init__(user, validation_class)
 
+    @transaction.atomic
     @register_service_signal('task_service.create')
     def create(self, obj_data):
+        source = obj_data.get('source')
+        task_group_query = TaskGroup.objects.filter(json_ext__contains={"task_sources": [source]})
+        if task_group_query.exists():
+            obj_data = {**obj_data, "task_group": task_group_query.first(), "status": Task.Status.ACCEPTED}
         return super().create(obj_data)
 
     @register_service_signal('task_service.update')
     def update(self, obj_data):
         return super().update(obj_data)
 
     @register_service_signal('task_service.delete')
@@ -54,37 +65,73 @@
 
     @register_service_signal('task_service.resolve_task')
     def resolve_task(self, obj_data):
         try:
             self.validation_class.validate_update(self.user, **obj_data)
             obj = self.OBJECT_TYPE.objects.get(id=obj_data['id'])
             incoming_status = obj_data.get('business_status')
-            self._update_task_business_status(obj, incoming_status)
+            additional_data = obj_data.get('additional_data')
+            self._update_task_business_status(obj, incoming_status, additional_data)
+            self._insert_additional_data_to_json_ext(obj, additional_data)
             return output_result_success({'task': model_representation(obj), 'user': {'id': f"{self.user.id}"}})
         except Exception as exc:
             return output_exception(model_name=self.OBJECT_TYPE.__name__, method="resolve", exception=exc)
 
-    def _update_task_business_status(self, task, incoming_status):
-        task.business_status = {**task.business_status, **incoming_status}
-        task.save(username=self.user.login_name)
+    def _update_task_business_status(self, task, incoming_status, additional_data):
+        try:
+            task.business_status = self.__deep_merge(task.business_status, incoming_status)
+            self._insert_additional_data_to_json_ext(task, additional_data)
+            task.save(username=self.user.login_name)
+        except ValidationError as e:
+            if e.message == 'Record has not be updated - there are no changes in fields':
+                return None
+
+    def _insert_additional_data_to_json_ext(self, obj, additional_data):
+        if not additional_data:
+            return
+
+        obj.json_ext = obj.json_ext or {}
+
+        existing_additional_data = obj.json_ext.get("additional_resolve_data", {})
+        existing_additional_data[str(self.user.id)] = additional_data
+
+        obj.json_ext["additional_resolve_data"] = existing_additional_data
+
+    def __deep_merge(self, dict1, dict2):
+        """
+        Merges two dictionaries, deeply combining them.
+        """
+        result = copy.deepcopy(dict1)
+
+        for key, value in dict2.items():
+            if key in result and isinstance(result[key], dict) and isinstance(value, dict):
+                result[key] = self.__deep_merge(result[key], value)
+            elif key in result and isinstance(result[key], list) and isinstance(value, list):
+                result[key] = result[key] + value
+            else:
+                result[key] = copy.deepcopy(value)
+
+        return result
 
 
 class TaskGroupService(BaseService):
     OBJECT_TYPE: Type[TaskGroup] = TaskGroup
 
     def __init__(self, user, validation_class=TaskGroupValidation):
         super().__init__(user, validation_class)
 
     @check_authentication
-    @transaction.atomic
     def create(self, obj_data: Dict[str, any]):
         try:
             with transaction.atomic():
                 user_ids = obj_data.pop('user_ids')
+                obj_data = self._adjust_update_payload(obj_data)
                 self.validation_class.validate_create(self.user, **obj_data)
+                task_sources = obj_data.pop('task_sources')
+                obj_data = {**obj_data, "json_ext": {"task_sources": list(task_sources)}}
                 obj_: TaskGroup = self.OBJECT_TYPE(**obj_data)
                 task_group_output = self.save_instance(obj_)
                 task_group_id = task_group_output['data']['id']
                 task_executor_service = TaskExecutorService(self.user)
                 # TODO: it would be good to override bulk_create and use it here
                 for user_id in user_ids:
                     task_executor_service.create({
@@ -93,22 +140,31 @@
                     })
                 return task_group_output
         except Exception as exc:
             return output_exception(model_name=self.OBJECT_TYPE.__name__, method="create", exception=exc)
 
     @check_authentication
     def update(self, obj_data: Dict[str, any]):
-        user_ids = obj_data.pop('user_ids')
-        task_group_id = obj_data.get('id')
-        task_group = TaskGroup.objects.get(id=task_group_id)
-        current_task_executors = task_group.taskexecutor_set.filter(is_deleted=False)
-        current_user_ids = current_task_executors.values_list('user__id', flat=True)
-        if set(current_user_ids) != set(user_ids):
-            self._update_task_group_task_executors(task_group, user_ids)
-        return super().update(obj_data)
+        try:
+            with transaction.atomic():
+                user_ids = obj_data.pop('user_ids')
+                obj_data = self._adjust_update_payload(obj_data)
+                self.validation_class.validate_update(self.user, **obj_data)
+                task_sources = obj_data.pop('task_sources')
+                task_group_id = obj_data.get('id')
+                task_group = TaskGroup.objects.get(id=task_group_id)
+                json_ext = task_group.json_ext if task_group.json_ext else dict()
+                obj_data = {**obj_data, "json_ext": {**json_ext, "task_sources": list(task_sources)}}
+                current_task_executors = task_group.taskexecutor_set.filter(is_deleted=False)
+                current_user_ids = current_task_executors.values_list('user__id', flat=True)
+                if set(current_user_ids) != set(user_ids):
+                    self._update_task_group_task_executors(task_group, user_ids)
+                return super().update(obj_data)
+        except Exception as exc:
+            return output_exception(model_name=self.OBJECT_TYPE.__name__, method="update", exception=exc)
 
     @transaction.atomic
     def _update_task_group_task_executors(self, task_group, user_ids):
         try:
             task_group.taskexecutor_set.all().delete()
             service = TaskExecutorService(self.user)
             for user_id in user_ids:
@@ -120,50 +176,50 @@
     def delete(self, obj_data: Dict[str, any]):
         id = obj_data.get("id")
         if id:
             task_group = TaskGroup.objects.filter(id=id).first()
             task_group.taskexecutor_set.all().delete()
         return super().delete(obj_data)
 
+    def _base_payload_adjust(self, obj_data):
+        task_sources = obj_data.pop('task_sources', [])
+        if task_sources:
+            task_sources = set(task_sources)
+        return {**obj_data, 'task_sources': task_sources}
+
 
 class TaskExecutorService(BaseService):
     OBJECT_TYPE: Type[TaskExecutor] = TaskExecutor
 
     def __init__(self, user, validation_class=TaskExecutorValidation):
         super().__init__(user, validation_class)
 
 
-non_serializable_types = (
-    uuid.UUID,
-    datetime.date,
-    decimal.Decimal,
-)
-
-
 class CreateCheckerLogicServiceMixin(ABC):
     """
     Provides default implementation for creating a create task for maker-checker logic.
     To be used in implementations of core.services.BaseService.
     """
 
     @property
     @abstractmethod
     def OBJECT_TYPE(self):
         pass
 
     def create_create_task(self, obj_data):
         try:
             with transaction.atomic():
+                self.validation_class.validate_create(self.user, **obj_data)
                 task_service = TaskService(self.user)
                 task_data = {
                     'source': self._create_source,
+                    'business_data_serializer': self._get_business_data_serializer(),
                     'executor_action_event': self._create_executor_event,
                     'business_event': self._create_business_event,
-                    'data': self._adjust_create_task_data(copy.deepcopy(obj_data)),
-                    'json_ext': self._data_for_json_ext_create(obj_data)
+                    'data': self._adjust_create_task_data(None, copy.deepcopy(obj_data)),
                 }
                 return task_service.create(task_data)
         except Exception as exc:
             return output_exception(model_name=self.OBJECT_TYPE.__name__, method="create_create_task", exception=exc)
 
     @property
     def _create_source(self):
@@ -173,48 +229,49 @@
     def _create_business_event(self):
         return f'{self.__class__.__name__}.create'
 
     @property
     def _create_executor_event(self):
         return TasksManagementConfig.default_executor_event
 
-    def _adjust_create_task_data(self, obj_data):
-        for key in obj_data:
-            if any(map(lambda t: isinstance(obj_data[key], t), non_serializable_types)):
-                obj_data[key] = str(obj_data[key])
-        return obj_data
+    def _adjust_create_task_data(self, entity, obj_data):
+        return _get_std_crud_task_data_payload(entity, obj_data)
+
+    def _get_business_data_serializer(self):
+        return f'{self.__class__.__module__}.{self.__class__.__name__}._business_data_serializer'
 
-    def _data_for_json_ext_create(self, obj_data):
-        return {}
+    def _business_data_serializer(self, data):
+        return data
 
 
 class UpdateCheckerLogicServiceMixin(ABC):
     """
-    Provides default implementation for creating a update task for maker-checker logic.
+    Provides default implementation for creating an update task for maker-checker logic.
     To be used in implementations of core.services.BaseService.
     """
 
     @property
     @abstractmethod
     def OBJECT_TYPE(self):
         pass
 
     def create_update_task(self, obj_data):
         try:
             with transaction.atomic():
+                self.validation_class.validate_update(self.user, **obj_data)
                 task_service = TaskService(self.user)
                 obj = self.OBJECT_TYPE.objects.get(id=obj_data['id'])
                 task_data = {
                     'source': self._update_source,
+                    'business_data_serializer': self._get_business_data_serializer(),
                     'entity_id': obj.id,
                     'entity_type': ContentType.objects.get_for_model(self.OBJECT_TYPE),
                     'executor_action_event': self._update_executor_event,
                     'business_event': self._update_business_event,
-                    'data': self._adjust_update_task_data(copy.deepcopy(obj_data)),
-                    'json_ext': self._data_for_json_ext_update(obj_data)
+                    'data': self._adjust_update_task_data(obj, copy.deepcopy(obj_data)),
                 }
                 return task_service.create(task_data)
         except Exception as exc:
             return output_exception(model_name=self.OBJECT_TYPE.__name__, method="create_update_task", exception=exc)
 
     @property
     def _update_source(self):
@@ -224,22 +281,22 @@
     def _update_business_event(self):
         return f'{self.__class__.__name__}.update'
 
     @property
     def _update_executor_event(self):
         return TasksManagementConfig.default_executor_event
 
-    def _adjust_update_task_data(self, obj_data):
-        for key in obj_data:
-            if any(map(lambda t: isinstance(obj_data[key], t), non_serializable_types)):
-                obj_data[key] = str(obj_data[key])
-        return obj_data
+    def _adjust_update_task_data(self, entity, obj_data):
+        return _get_std_crud_task_data_payload(entity, obj_data)
 
-    def _data_for_json_ext_update(self, obj_data):
-        return {}
+    def _get_business_data_serializer(self):
+        return f'{self.__class__.__module__}.{self.__class__.__name__}._business_data_serializer'
+
+    def _business_data_serializer(self, data):
+        return data
 
 
 class DeleteCheckerLogicServiceMixin(ABC):
     """
     Provides default implementation for creating a delete task for maker-checker logic.
     To be used in implementations of core.services.BaseService.
     """
@@ -248,24 +305,25 @@
     @abstractmethod
     def OBJECT_TYPE(self):
         pass
 
     def create_delete_task(self, obj_data):
         try:
             with transaction.atomic():
+                self.validation_class.validate_delete(self.user, **obj_data)
                 task_service = TaskService(self.user)
                 obj = self.OBJECT_TYPE.objects.get(id=obj_data['id'])
                 task_data = {
                     'source': self._delete_source,
+                    'business_data_serializer': self._get_business_data_serializer(),
                     'entity_id': obj.id,
                     'entity_type': ContentType.objects.get_for_model(self.OBJECT_TYPE),
                     'executor_action_event': self._delete_executor_event,
                     'business_event': self._delete_business_event,
-                    'data': self._adjust_delete_task_data(copy.deepcopy(obj_data)),
-                    'json_ext': self._data_for_json_ext_delete(obj_data)
+                    'data': self._adjust_delete_task_data(None, copy.deepcopy(obj_data)),
                 }
                 return task_service.create(task_data)
         except Exception as exc:
             return output_exception(model_name=self.OBJECT_TYPE.__name__, method="create_delete_task", exception=exc)
 
     @property
     def _delete_source(self):
@@ -275,30 +333,30 @@
     def _delete_business_event(self):
         return f'{self.__class__.__name__}.delete'
 
     @property
     def _delete_executor_event(self):
         return TasksManagementConfig.default_executor_event
 
-    def _adjust_delete_task_data(self, obj_data):
-        for key in obj_data:
-            if any(map(lambda t: isinstance(obj_data[key], t), non_serializable_types)):
-                obj_data[key] = str(obj_data[key])
-        return obj_data
+    def _adjust_delete_task_data(self, entity, obj_data):
+        return _get_std_crud_task_data_payload(entity, obj_data)
+
+    def _get_business_data_serializer(self):
+        return f'{self.__class__.__module__}.{self.__class__.__name__}._business_data_serializer'
 
-    def _data_for_json_ext_delete(self, obj_data):
-        return {}
+    def _business_data_serializer(self, data):
+        return data
 
 
 class CheckerLogicServiceMixin(CreateCheckerLogicServiceMixin,
                                UpdateCheckerLogicServiceMixin,
                                DeleteCheckerLogicServiceMixin,
                                ABC):
     """
-    Provides default implementation for creating create, update, and delete tasks for maker-checker logic
+    Provides default implementation for creating "create", "update", and "delete" tasks for maker-checker logic
     To be used in implementations of core.services.BaseService.
     """
     pass
 
 
 def on_task_complete_service_handler(service_type: Type[BaseService]):
     """
@@ -320,27 +378,65 @@
     def service_operation_handler(operation, user, data):
         # Run the operation form a service by name
         # getattr(ExampleService(user), 'update')(data)
         return getattr(service_type(user), operation)(data)
 
     def func(**kwargs):
         try:
-            result = kwargs.get('result', None)
+            result = kwargs.get('result', {})
             task = result['data']['task']
             business_event = task['business_event']
             # Tasks generated with CheckerLogicServiceMixin use naming scheme `ServiceName.operation` as business event.
             # Checking if the task was generated by the mixin and if the service provided for the handler match
             service_match = business_event.startswith(f"{service_type.__name__}.")
             if result and result['success'] \
                     and task['status'] == Task.Status.COMPLETED \
                     and service_match:
                 # Extracting `operation` part from `ServiceName.operation`
                 operation = business_event.split(".")[1]
                 if operation in operations:
                     user = User.objects.get(id=result['data']['user']['id'])
-                    data = task['data']
+                    data = task['data']['incoming_data']
                     service_operation_handler(operation, user, data)
         except Exception as e:
             logger.error("Error while executing on_task_complete", exc_info=e)
             return [str(e)]
 
     return func
+
+
+def serialize_value(value):
+    return str(value) if any(isinstance(value, t) for t in non_serializable_types) else value
+
+
+def _get_std_crud_task_data_payload(entity, payload):
+    incoming_data = {}
+    current_data = {}
+
+    for key in payload:
+        incoming_value = serialize_value(payload[key])
+        incoming_data[key] = incoming_value
+
+        if entity:
+            entity_value = getattr(entity, key)
+            current_data[key] = serialize_value(entity_value) if entity_value else entity_value
+
+    return {"incoming_data": incoming_data, "current_data": current_data}
+
+
+def _get_std_task_data_payload(payload):
+    incoming_data = {}
+
+    for key in payload:
+        incoming_value = serialize_value(payload[key])
+        incoming_data[key] = incoming_value
+
+    return incoming_data
+
+
+def crud_business_data_builder(data, serializer):
+    serialized_data = copy.deepcopy(data)
+    for data_key, data_value in data.items():
+        serialized_data[data_key] = {
+            key: serializer(key, value) for key, value in data_value.items()
+        }
+    return serialized_data
```

### Comparing `openimis-be-tasks_management-1.0.0/tasks_management/signals/on_task_resolve.py` & `openimis_be_tasks_management-1.1.0/tasks_management/signals/on_task_resolve.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tasks_management-1.0.0/tasks_management/tests/data.py` & `openimis_be_tasks_management-1.1.0/tasks_management/tests/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from core.models import InteractiveUser
 from tasks_management.models import Task
 from tasks_management.models import TaskGroup
 
 
-
 class TaskDataMixin:
-    
-    
-
     task_group_add_payload_any = {
         "code": "example_any",
         "completion_policy": TaskGroup.TaskGroupCompletionPolicy.ANY,
     }
     task_group_add_payload_all = {
         "code": "example_all",
         "completion_policy": TaskGroup.TaskGroupCompletionPolicy.ALL,
@@ -56,17 +52,15 @@
         'entity': None,
         'status': Task.Status.RECEIVED,
         'executor_action_event': 'approve_n',
         'business_status': dict(),
         'business_event': 'test_business_action_n',
         'data': dict()
     }
-    
+
     @classmethod
     def init_data(cls):
         entity = InteractiveUser.objects.first()
         cls.task_payload_resolve_n['entity'] = entity
         cls.task_payload_resolve_all['entity'] = entity
         cls.task_payload_resolve_any['entity'] = entity
         cls.task_payload['entity'] = entity
-
-
```

### Comparing `openimis-be-tasks_management-1.0.0/tasks_management/tests/helpers.py` & `openimis_be_tasks_management-1.1.0/tasks_management/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tasks_management-1.0.0/tasks_management/tests/task_event_tests.py` & `openimis_be_tasks_management-1.1.0/tasks_management/tests/task_event_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tasks_management-1.0.0/tasks_management/tests/task_group_service_tests.py` & `openimis_be_tasks_management-1.1.0/tasks_management/tests/task_group_service_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-tasks_management-1.0.0/tasks_management/tests/task_service_tests.py` & `openimis_be_tasks_management-1.1.0/tasks_management/tests/task_service_tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import copy
 from unittest import skip
 
 from django.test import TestCase
 
-from core.test_helpers import create_test_interactive_user
+from tasks_management.apps import TasksManagementConfig
 from tasks_management.tests.data import TaskDataMixin
 from tasks_management.services import TaskService, TaskGroupService
-from tasks_management.models import Task, TaskGroup
+from tasks_management.models import Task
 from tasks_management.tests.helpers import LogInHelper
-from tasks_management.utils import APPROVED
 
 
 class TaskServiceTestCase(TestCase, TaskDataMixin):
     user = None
     task_executor = None
     service = None
     taskgroup_all = None
@@ -108,15 +107,16 @@
         result = self.service.create(create_payload)
 
         self.assertTrue(result)
         self.assertTrue(result['success'])
         obj_id = result['data']['id']
         self.assertTrue(Task.objects.filter(id=obj_id).exists())
 
-        resolve_payload = {"id": result["data"]["uuid"], "business_status": {"Jan Kowalski": APPROVED}}
+        resolve_payload = {"id": result["data"]["uuid"],
+                           "business_status": {"Jan Kowalski": TasksManagementConfig.task_user_approved}}
         result = self.service.resolve_task(resolve_payload)
 
         self.assertTrue(result)
         self.assertTrue(result['success'])
         self.assertEqual(Task.objects.filter(id=obj_id).first().status, Task.Status.COMPLETED)
 
     @skip('To be redeveloped')
@@ -129,15 +129,16 @@
 
         self.assertTrue(result)
         self.assertTrue(result['success'])
         obj_id = result['data']['id']
         self.assertTrue(Task.objects.filter(id=obj_id).exists())
 
         resolve_payload = {"id": result["data"]["uuid"],
-                           "business_status": {"Jan Kowalski": APPROVED, "Adam Kowal": APPROVED}}
+                           "business_status": {"Jan Kowalski": TasksManagementConfig.task_user_approved,
+                                               "Adam Kowal": TasksManagementConfig.task_user_approved}}
         result = self.service.resolve_task(resolve_payload)
 
         self.assertTrue(result)
         self.assertTrue(result['success'])
         self.assertEqual(Task.objects.filter(id=obj_id).first().status, Task.Status.COMPLETED)
 
     @skip('To be redeveloped')
@@ -149,15 +150,16 @@
         result = self.service.create(create_payload)
 
         self.assertTrue(result)
         self.assertTrue(result['success'])
         obj_id = result['data']['id']
         self.assertTrue(Task.objects.filter(id=obj_id).exists())
 
-        resolve_payload = {"id": result["data"]["uuid"], "business_status": {"Jan Kowalski": APPROVED}}
+        resolve_payload = {"id": result["data"]["uuid"],
+                           "business_status": {"Jan Kowalski": TasksManagementConfig.task_user_approved}}
         result = self.service.resolve_task(resolve_payload)
 
         self.assertTrue(result)
         self.assertTrue(result['success'])
         self.assertEqual(Task.objects.filter(id=obj_id).first().status, Task.Status.COMPLETED)
 
     @classmethod
```

