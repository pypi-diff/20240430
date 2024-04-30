# Comparing `tmp/openimis-be-workflow-1.0.0.tar.gz` & `tmp/openimis_be_workflow-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-workflow-1.0.0.tar", last modified: Sat Dec 16 01:09:46 2023, max compression
+gzip compressed data, was "openimis_be_workflow-1.0.1.tar", last modified: Tue Apr 30 09:00:21 2024, max compression
```

## Comparing `openimis-be-workflow-1.0.0.tar` & `openimis_be_workflow-1.0.1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:09:46.105867 openimis-be-workflow-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2023-12-16 01:09:46.105867 openimis-be-workflow-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:09:46.101867 openimis-be-workflow-1.0.0/openimis_be_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2023-12-16 01:09:46.000000 openimis-be-workflow-1.0.0/openimis_be_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      876 2023-12-16 01:09:46.000000 openimis-be-workflow-1.0.0/openimis_be_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-16 01:09:46.000000 openimis-be-workflow-1.0.0/openimis_be_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-12-16 01:09:46.000000 openimis-be-workflow-1.0.0/openimis_be_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-16 01:09:46.000000 openimis-be-workflow-1.0.0/openimis_be_workflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-16 01:09:46.105867 openimis-be-workflow-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2023-12-16 01:09:45.000000 openimis-be-workflow-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:09:46.101867 openimis-be-workflow-1.0.0/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:09:46.101867 openimis-be-workflow-1.0.0/workflow/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:09:46.101867 openimis-be-workflow-1.0.0/workflow/systems/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/systems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:09:46.101867 openimis-be-workflow-1.0.0/workflow/systems/base/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/systems/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/systems/base/adaptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/systems/base/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:09:46.101867 openimis-be-workflow-1.0.0/workflow/systems/lightning/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/systems/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/systems/lightning/adaptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/systems/lightning/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/systems/lightning/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-16 01:09:46.101867 openimis-be-workflow-1.0.0/workflow/systems/python/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/systems/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/systems/python/adaptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/systems/python/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-16 01:09:38.000000 openimis-be-workflow-1.0.0/workflow/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:21.438379 openimis_be_workflow-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-30 09:00:21.438379 openimis_be_workflow-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:21.438379 openimis_be_workflow-1.0.1/openimis_be_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-30 09:00:21.000000 openimis_be_workflow-1.0.1/openimis_be_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-30 09:00:21.000000 openimis_be_workflow-1.0.1/openimis_be_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:00:21.000000 openimis_be_workflow-1.0.1/openimis_be_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 09:00:21.000000 openimis_be_workflow-1.0.1/openimis_be_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 09:00:21.000000 openimis_be_workflow-1.0.1/openimis_be_workflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:00:21.438379 openimis_be_workflow-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-30 09:00:21.000000 openimis_be_workflow-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:21.438379 openimis_be_workflow-1.0.1/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:21.438379 openimis_be_workflow-1.0.1/workflow/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:21.438379 openimis_be_workflow-1.0.1/workflow/systems/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/systems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:21.438379 openimis_be_workflow-1.0.1/workflow/systems/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/systems/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/systems/base/adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/systems/base/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:21.438379 openimis_be_workflow-1.0.1/workflow/systems/lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/systems/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/systems/lightning/adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/systems/lightning/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/systems/lightning/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:21.438379 openimis_be_workflow-1.0.1/workflow/systems/python/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/systems/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/systems/python/adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/systems/python/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:00:11.000000 openimis_be_workflow-1.0.1/workflow/views.py
```

### Comparing `openimis-be-workflow-1.0.0/LICENSE.md` & `openimis_be_workflow-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-workflow-1.0.0/PKG-INFO` & `openimis_be_workflow-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-workflow
-Version: 1.0.0
+Version: 1.0.1
 Summary: The openIMIS Backend workflow reference module.
 Home-page: https://openimis.org/
 Author: Kamil Malinowski
 Author-email: kmalinowski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-workflow-1.0.0/README.md` & `openimis_be_workflow-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-workflow-1.0.0/openimis_be_workflow.egg-info/PKG-INFO` & `openimis_be_workflow-1.0.1/openimis_be_workflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-workflow
-Version: 1.0.0
+Version: 1.0.1
 Summary: The openIMIS Backend workflow reference module.
 Home-page: https://openimis.org/
 Author: Kamil Malinowski
 Author-email: kmalinowski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-workflow-1.0.0/openimis_be_workflow.egg-info/SOURCES.txt` & `openimis_be_workflow-1.0.1/openimis_be_workflow.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 openimis_be_workflow.egg-info/SOURCES.txt
 openimis_be_workflow.egg-info/dependency_links.txt
 openimis_be_workflow.egg-info/requires.txt
 openimis_be_workflow.egg-info/top_level.txt
 workflow/__init__.py
 workflow/admin.py
 workflow/apps.py
+workflow/exceptions.py
 workflow/gql_queries.py
 workflow/models.py
 workflow/schema.py
 workflow/services.py
 workflow/tests.py
 workflow/urls.py
 workflow/util.py
```

### Comparing `openimis-be-workflow-1.0.0/setup.py` & `openimis_be_workflow-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-workflow',
-    version='1.0.0',
+    version='v1.0.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend workflow reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

### Comparing `openimis-be-workflow-1.0.0/workflow/apps.py` & `openimis_be_workflow-1.0.1/workflow/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-workflow-1.0.0/workflow/schema.py` & `openimis_be_workflow-1.0.1/workflow/schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from workflow.gql_queries import WorkflowGQLType
 from workflow.services import WorkflowService
 
 
 class Query:
     workflow = graphene.Field(
         graphene.List(WorkflowGQLType),
-        name=graphene.String(),
-        group=graphene.String(),
+        name=graphene.Argument(graphene.String, required=False),
+        group=graphene.Argument(graphene.String, required=False),
     )
 
     def resolve_workflow(self, info, **kwargs):
         workflows = WorkflowService.get_workflows(**kwargs)
         if not workflows.get('success', False):
             raise ValueError(str(workflows))
```

### Comparing `openimis-be-workflow-1.0.0/workflow/services.py` & `openimis_be_workflow-1.0.1/workflow/services.py`

 * *Files identical despite different names*

### Comparing `openimis-be-workflow-1.0.0/workflow/systems/base/adaptor.py` & `openimis_be_workflow-1.0.1/workflow/systems/base/adaptor.py`

 * *Files identical despite different names*

### Comparing `openimis-be-workflow-1.0.0/workflow/systems/base/handler.py` & `openimis_be_workflow-1.0.1/workflow/systems/base/handler.py`

 * *Files identical despite different names*

### Comparing `openimis-be-workflow-1.0.0/workflow/systems/lightning/adaptor.py` & `openimis_be_workflow-1.0.1/workflow/systems/lightning/adaptor.py`

 * *Files identical despite different names*

### Comparing `openimis-be-workflow-1.0.0/workflow/systems/lightning/client.py` & `openimis_be_workflow-1.0.1/workflow/systems/lightning/client.py`

 * *Files identical despite different names*

### Comparing `openimis-be-workflow-1.0.0/workflow/systems/lightning/handler.py` & `openimis_be_workflow-1.0.1/workflow/systems/lightning/handler.py`

 * *Files identical despite different names*

### Comparing `openimis-be-workflow-1.0.0/workflow/systems/python/adaptor.py` & `openimis_be_workflow-1.0.1/workflow/systems/python/adaptor.py`

 * *Files identical despite different names*

### Comparing `openimis-be-workflow-1.0.0/workflow/systems/python/handler.py` & `openimis_be_workflow-1.0.1/workflow/systems/python/handler.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 import logging
 from typing import Dict
 
+from workflow.exceptions import PythonWorkflowHandlerException
 from workflow.systems.base import WorkflowHandler
 from workflow.util import result
 
 logger = logging.getLogger(__name__)
 
 
 class PythonWorkflowHandler(WorkflowHandler):
     def __init__(self, name, group, system, function):
         super().__init__(name, group, system)
         self._function = function
 
     def run(self, data: Dict):
         try:
-            output = self._function(data)
+            output = self._function(**data)
             return result(
                 success=True,
                 data=output
             )
+        # Dedicated exception handling for workflow exceptions that should have custom message
+        except PythonWorkflowHandlerException as e:
+            logging.error("Error while executing workflow %s-%s: ", self.system, self.name, exc_info=e)
+            return result(
+                success=False,
+                message=e.message,
+                details=str(e)
+            )
         except Exception as e:
             logging.error("Error while executing workflow %s-%s: ", self.system, self.name, exc_info=e)
             return result(
                 success=False,
                 message="Error while executing workflow",
                 details=str(e)
             )
```

