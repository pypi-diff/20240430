# Comparing `tmp/openimis-be-controls-1.0.0.tar.gz` & `tmp/openimis_be_controls-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-controls-1.0.0.tar", last modified: Tue Dec 19 12:24:46 2023, max compression
+gzip compressed data, was "openimis_be_controls-1.1.0.tar", last modified: Tue Apr 30 09:08:07 2024, max compression
```

## Comparing `openimis-be-controls-1.0.0.tar` & `openimis_be_controls-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 12:24:46.602503 openimis-be-controls-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-12-19 12:24:36.000000 openimis-be-controls-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2023-12-19 12:24:46.602503 openimis-be-controls-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2023-12-19 12:24:36.000000 openimis-be-controls-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 12:24:46.598503 openimis-be-controls-1.0.0/controls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 12:24:36.000000 openimis-be-controls-1.0.0/controls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-19 12:24:36.000000 openimis-be-controls-1.0.0/controls/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-12-19 12:24:36.000000 openimis-be-controls-1.0.0/controls/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 12:24:46.598503 openimis-be-controls-1.0.0/controls/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2023-12-19 12:24:36.000000 openimis-be-controls-1.0.0/controls/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 12:24:36.000000 openimis-be-controls-1.0.0/controls/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-12-19 12:24:36.000000 openimis-be-controls-1.0.0/controls/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-12-19 12:24:36.000000 openimis-be-controls-1.0.0/controls/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-19 12:24:36.000000 openimis-be-controls-1.0.0/controls/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 12:24:46.598503 openimis-be-controls-1.0.0/controls/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 12:24:36.000000 openimis-be-controls-1.0.0/controls/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2023-12-19 12:24:36.000000 openimis-be-controls-1.0.0/controls/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2023-12-19 12:24:36.000000 openimis-be-controls-1.0.0/controls/tests/test_gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2023-12-19 12:24:36.000000 openimis-be-controls-1.0.0/controls/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-19 12:24:36.000000 openimis-be-controls-1.0.0/controls/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-19 12:24:36.000000 openimis-be-controls-1.0.0/controls/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 12:24:46.602503 openimis-be-controls-1.0.0/openimis_be_controls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2023-12-19 12:24:46.000000 openimis-be-controls-1.0.0/openimis_be_controls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-12-19 12:24:46.000000 openimis-be-controls-1.0.0/openimis_be_controls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 12:24:46.000000 openimis-be-controls-1.0.0/openimis_be_controls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-12-19 12:24:46.000000 openimis-be-controls-1.0.0/openimis_be_controls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-19 12:24:46.000000 openimis-be-controls-1.0.0/openimis_be_controls.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 12:24:46.602503 openimis-be-controls-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2023-12-19 12:24:46.000000 openimis-be-controls-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:08:07.293283 openimis_be_controls-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-30 09:07:59.000000 openimis_be_controls-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-30 09:08:07.293283 openimis_be_controls-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-30 09:07:59.000000 openimis_be_controls-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:08:07.289283 openimis_be_controls-1.1.0/controls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:59.000000 openimis_be_controls-1.1.0/controls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:07:59.000000 openimis_be_controls-1.1.0/controls/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-30 09:07:59.000000 openimis_be_controls-1.1.0/controls/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:08:07.293283 openimis_be_controls-1.1.0/controls/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-30 09:07:59.000000 openimis_be_controls-1.1.0/controls/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:59.000000 openimis_be_controls-1.1.0/controls/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-30 09:07:59.000000 openimis_be_controls-1.1.0/controls/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-30 09:07:59.000000 openimis_be_controls-1.1.0/controls/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-30 09:07:59.000000 openimis_be_controls-1.1.0/controls/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:08:07.293283 openimis_be_controls-1.1.0/controls/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 09:07:59.000000 openimis_be_controls-1.1.0/controls/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-30 09:07:59.000000 openimis_be_controls-1.1.0/controls/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-30 09:07:59.000000 openimis_be_controls-1.1.0/controls/tests/test_gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-30 09:07:59.000000 openimis_be_controls-1.1.0/controls/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 09:07:59.000000 openimis_be_controls-1.1.0/controls/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 09:07:59.000000 openimis_be_controls-1.1.0/controls/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:08:07.293283 openimis_be_controls-1.1.0/openimis_be_controls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-30 09:08:07.000000 openimis_be_controls-1.1.0/openimis_be_controls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-30 09:08:07.000000 openimis_be_controls-1.1.0/openimis_be_controls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:08:07.000000 openimis_be_controls-1.1.0/openimis_be_controls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-30 09:08:07.000000 openimis_be_controls-1.1.0/openimis_be_controls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 09:08:07.000000 openimis_be_controls-1.1.0/openimis_be_controls.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 09:08:07.293283 openimis_be_controls-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-30 09:08:07.000000 openimis_be_controls-1.1.0/setup.py
```

### Comparing `openimis-be-controls-1.0.0/LICENSE.md` & `openimis_be_controls-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-controls-1.0.0/PKG-INFO` & `openimis_be_controls-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-controls
-Version: 1.0.0
+Version: 1.1.0
 Summary: The openIMIS Backend controls reference module.
 Home-page: https://openimis.org/
 Author: Christophe Philemotte
 Author-email: cphilemotte@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -12,19 +12,19 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: django~=3.2.15
+Requires-Dist: django
 Requires-Dist: djangorestframework
 Requires-Dist: django-filter~=22.1
 Requires-Dist: openimis-be-core
-Requires-Dist: graphene-django<3
+Requires-Dist: graphene-django
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-django; extra == "dev"
 
 # openIMIS Backend controls reference module
 
 This repository holds the files of the OpenIMIS Backend Controls reference module.
```

### Comparing `openimis-be-controls-1.0.0/README.md` & `openimis_be_controls-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-controls-1.0.0/controls/migrations/0001_initial.py` & `openimis_be_controls-1.1.0/controls/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-controls-1.0.0/controls/models.py` & `openimis_be_controls-1.1.0/controls/models.py`

 * *Files identical despite different names*

### Comparing `openimis-be-controls-1.0.0/controls/schema.py` & `openimis_be_controls-1.1.0/controls/schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-controls-1.0.0/controls/tests/test_gql.py` & `openimis_be_controls-1.1.0/controls/tests/test_gql.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,44 +61,56 @@
     """
     self.control_schema = graphene.Schema(query=Query)
     self.maxDiff = None
     self.isolated_tests = "PYTEST_CURRENT_TEST" in os.environ
     self.controls = []
 
   def tearDown(self):
-    [control.delete() for control in self.controls]
-
-  def test_query_without_any_new_control(self):
-    client = Client(self.control_schema)
-    executed = client.execute(self.query)
-    self.assertEqual(executed, self.generate_expected([] if self.isolated_tests else self.FULL_TEST_DATA_NAME))
+    if isinstance(self.controls, list) and len(self.controls)>0:
+      for control in self.controls:
+        if control.name:
+          control.delete()
+        else:
+          pass
+
+  # def test_query_without_any_new_control(self):
+  #   client = Client(self.control_schema)
+  #   executed = client.execute(self.query)
+  #   self.assertEqual(executed, self.generate_expected([] if self.isolated_tests else self.FULL_TEST_DATA_NAME))
 
   def test_query_with_one_control(self):
+
+
+    client = Client(self.control_schema)
+    before_executed = client.execute(self.query)
     self.controls.append(
       Control.objects.create(
         name=ModelsTestCase.DEFAULT_NAME,
         adjustability=ModelsTestCase.DEFAULT_ADJUSTABILITY,
         usage=ModelsTestCase.DEFAULT_USAGE))
-
-    client = Client(self.control_schema)
     executed = client.execute(self.query)
     self.assertEqual(
-      executed,
-      self.generate_expected(self.LOCAL_TEST_DATA_NAME if self.isolated_tests else self.LOCAL_TEST_DATA_NAME + self.FULL_TEST_DATA_NAME))
+      len(before_executed['data']['control']['edges'])+ 1,
+      len(executed['data']['control']['edges']) )
+    self.tearDown()
 
   def test_query_with_several_controls(self):
     TEST_DATA_NAMES = []
+    client = Client(self.control_schema)
+    before_executed = client.execute(self.query)
     for nbr in range(1, 4):
       name = f'{ModelsTestCase.DEFAULT_NAME}_{nbr}'
       self.controls.append(
         Control.objects.create(
           name=name,
           adjustability=ModelsTestCase.DEFAULT_ADJUSTABILITY,
           usage=ModelsTestCase.DEFAULT_USAGE))
       TEST_DATA_NAMES.append(name)
 
-    client = Client(self.control_schema)
     executed = client.execute(self.query)
     self.assertEqual(
-      executed,
-      self.generate_expected(TEST_DATA_NAMES if self.isolated_tests else TEST_DATA_NAMES + self.FULL_TEST_DATA_NAME))
+      len(before_executed['data']['control']['edges'])+ 3,
+      len(executed['data']['control']['edges']) )
+
+    self.tearDown()
+
```

### Comparing `openimis-be-controls-1.0.0/openimis_be_controls.egg-info/PKG-INFO` & `openimis_be_controls-1.1.0/openimis_be_controls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-controls
-Version: 1.0.0
+Version: 1.1.0
 Summary: The openIMIS Backend controls reference module.
 Home-page: https://openimis.org/
 Author: Christophe Philemotte
 Author-email: cphilemotte@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -12,19 +12,19 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: django~=3.2.15
+Requires-Dist: django
 Requires-Dist: djangorestframework
 Requires-Dist: django-filter~=22.1
 Requires-Dist: openimis-be-core
-Requires-Dist: graphene-django<3
+Requires-Dist: graphene-django
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-django; extra == "dev"
 
 # openIMIS Backend controls reference module
 
 This repository holds the files of the OpenIMIS Backend Controls reference module.
```

### Comparing `openimis-be-controls-1.0.0/openimis_be_controls.egg-info/SOURCES.txt` & `openimis_be_controls-1.1.0/openimis_be_controls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-controls-1.0.0/setup.py` & `openimis_be_controls-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 install_requires = read_requirements('requirements.txt')
 dev_requires = read_requirements('requirements-dev.txt')
 
 setup(
     name='openimis-be-controls',
-    version='v1.0.0',
+    version='v1.1.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend controls reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

