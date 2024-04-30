# Comparing `tmp/panther_detection_helpers-0.3.0.tar.gz` & `tmp/panther_detection_helpers-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panther_detection_helpers-0.3.0.tar", last modified: Thu Mar 21 20:36:43 2024, max compression
+gzip compressed data, was "panther_detection_helpers-0.4.0.tar", last modified: Tue Apr 30 18:32:13 2024, max compression
```

## Comparing `panther_detection_helpers-0.3.0.tar` & `panther_detection_helpers-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 20:36:43.598404 panther_detection_helpers-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-03-21 20:35:53.000000 panther_detection_helpers-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-21 20:35:53.000000 panther_detection_helpers-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-21 20:36:43.598404 panther_detection_helpers-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-21 20:35:53.000000 panther_detection_helpers-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 20:36:43.594404 panther_detection_helpers-0.3.0/panther_detection_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 20:35:53.000000 panther_detection_helpers-0.3.0/panther_detection_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15896 2024-03-21 20:35:53.000000 panther_detection_helpers-0.3.0/panther_detection_helpers/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-21 20:35:53.000000 panther_detection_helpers-0.3.0/panther_detection_helpers/mocking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-03-21 20:35:53.000000 panther_detection_helpers-0.3.0/panther_detection_helpers/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 20:36:43.598404 panther_detection_helpers-0.3.0/panther_detection_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-21 20:36:43.000000 panther_detection_helpers-0.3.0/panther_detection_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-21 20:36:43.000000 panther_detection_helpers-0.3.0/panther_detection_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 20:36:43.000000 panther_detection_helpers-0.3.0/panther_detection_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-21 20:36:43.000000 panther_detection_helpers-0.3.0/panther_detection_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-21 20:36:43.000000 panther_detection_helpers-0.3.0/panther_detection_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-21 20:36:29.000000 panther_detection_helpers-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-21 20:36:43.598404 panther_detection_helpers-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-21 20:35:53.000000 panther_detection_helpers-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 20:36:43.598404 panther_detection_helpers-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    15639 2024-03-21 20:35:53.000000 panther_detection_helpers-0.3.0/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-21 20:35:53.000000 panther_detection_helpers-0.3.0/tests/test_mocking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:13.339687 panther_detection_helpers-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-04-30 18:31:20.000000 panther_detection_helpers-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 18:31:20.000000 panther_detection_helpers-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-30 18:32:13.339687 panther_detection_helpers-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-30 18:31:20.000000 panther_detection_helpers-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:13.335687 panther_detection_helpers-0.4.0/panther_detection_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:31:20.000000 panther_detection_helpers-0.4.0/panther_detection_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15896 2024-04-30 18:31:20.000000 panther_detection_helpers-0.4.0/panther_detection_helpers/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-30 18:31:20.000000 panther_detection_helpers-0.4.0/panther_detection_helpers/mocking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-30 18:31:20.000000 panther_detection_helpers-0.4.0/panther_detection_helpers/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:13.339687 panther_detection_helpers-0.4.0/panther_detection_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-30 18:32:13.000000 panther_detection_helpers-0.4.0/panther_detection_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-30 18:32:13.000000 panther_detection_helpers-0.4.0/panther_detection_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:32:13.000000 panther_detection_helpers-0.4.0/panther_detection_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 18:32:13.000000 panther_detection_helpers-0.4.0/panther_detection_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 18:32:13.000000 panther_detection_helpers-0.4.0/panther_detection_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-30 18:32:00.000000 panther_detection_helpers-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-30 18:32:13.339687 panther_detection_helpers-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-30 18:31:20.000000 panther_detection_helpers-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:32:13.339687 panther_detection_helpers-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15606 2024-04-30 18:31:20.000000 panther_detection_helpers-0.4.0/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-30 18:31:20.000000 panther_detection_helpers-0.4.0/tests/test_mocking.py
```

### Comparing `panther_detection_helpers-0.3.0/LICENSE.txt` & `panther_detection_helpers-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panther_detection_helpers-0.3.0/PKG-INFO` & `panther_detection_helpers-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: panther_detection_helpers
-Version: 0.3.0
+Version: 0.4.0
 Summary: Panther Detection Helpers Library
 Home-page: https://github.com/panther-labs/panther_detection_helpers
-Download-URL: https://github.com/panther-labs/panther_detection_helpers/archive/refs/tags/v0.3.0.tar.gz
+Download-URL: https://github.com/panther-labs/panther_detection_helpers/archive/refs/tags/v0.4.0.tar.gz
 Author: Panther Labs Inc
 Author-email: pypi@runpanther.io
 License: AGPL-3.0
 Keywords: Security,CLI
 Classifier: Topic :: Security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 License-File: LICENSE.txt
 Requires-Dist: jsonpath-ng
 Requires-Dist: datadog
```

### Comparing `panther_detection_helpers-0.3.0/panther_detection_helpers/caching.py` & `panther_detection_helpers-0.4.0/panther_detection_helpers/caching.py`

 * *Files identical despite different names*

### Comparing `panther_detection_helpers-0.3.0/panther_detection_helpers/monitoring.py` & `panther_detection_helpers-0.4.0/panther_detection_helpers/monitoring.py`

 * *Files identical despite different names*

### Comparing `panther_detection_helpers-0.3.0/panther_detection_helpers.egg-info/PKG-INFO` & `panther_detection_helpers-0.4.0/panther_detection_helpers.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: panther_detection_helpers
-Version: 0.3.0
+Version: 0.4.0
 Summary: Panther Detection Helpers Library
 Home-page: https://github.com/panther-labs/panther_detection_helpers
-Download-URL: https://github.com/panther-labs/panther_detection_helpers/archive/refs/tags/v0.3.0.tar.gz
+Download-URL: https://github.com/panther-labs/panther_detection_helpers/archive/refs/tags/v0.4.0.tar.gz
 Author: Panther Labs Inc
 Author-email: pypi@runpanther.io
 License: AGPL-3.0
 Keywords: Security,CLI
 Classifier: Topic :: Security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 License-File: LICENSE.txt
 Requires-Dist: jsonpath-ng
 Requires-Dist: datadog
```

### Comparing `panther_detection_helpers-0.3.0/setup.py` & `panther_detection_helpers-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from distutils.core import setup
 
 
-VERSION = "0.3.0"
+VERSION = "0.4.0"
 
 
 install_requires = [
     'jsonpath-ng',
     'datadog',
 ]
 
@@ -30,11 +30,11 @@
     download_url=f'https://github.com/panther-labs/panther_detection_helpers/archive/refs/tags/v{VERSION}.tar.gz',
     keywords=['Security', 'CLI'],
     install_requires=install_requires,
     classifiers=[
         'Topic :: Security',
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
-        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: GNU Affero General Public License v3',
     ],
 )
```

### Comparing `panther_detection_helpers-0.3.0/tests/test_caching.py` & `panther_detection_helpers-0.4.0/tests/test_caching.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import datetime
 import json
 import os
 import unittest
 from abc import ABC
 
 import boto3
-from moto import mock_dynamodb
+from moto import mock_aws
 
 from panther_detection_helpers import caching
 
 
-@mock_dynamodb
+@mock_aws
 class DynamoBaseTest(ABC):
     # pylint: disable=protected-access,assignment-from-no-return
     def setUp(self):
         os.environ["AWS_DEFAULT_REGION"] = "us-west-2"
         self._temp_dynamo = boto3.resource("dynamodb")
         self._temp_table = self._temp_dynamo.create_table(
             TableName="panther-kv-store",
@@ -37,16 +37,15 @@
         )
         caching._KV_TABLE = self._temp_table
         caching.reset_counter("panther")
         caching.reset_counter("labs")
         caching.put_string_set("strs", ["a", "b"])
         caching.put_dictionary("d", {"z": "y"})
 
-
-@mock_dynamodb
+@mock_aws
 class TestCachingCounter(DynamoBaseTest, unittest.TestCase):
     def test_unset_counter(self):
         self.assertEqual(caching.get_counter("panther"), 0)
 
     def test_simple_increment(self):
         self.assertEqual(caching.increment_counter("panther"), 1)
         self.assertEqual(caching.get_counter("panther"), 1)
@@ -153,16 +152,15 @@
         panther_item = self._temp_table.get_item(
             Key={"key": "panther"}, ProjectionExpression=f"{caching._COUNT_COL}, {caching._TTL_COL}"
         )
         self.assertGreater(panther_item["Item"][caching._TTL_COL], int(datetime.datetime.now().timestamp()) + caching._EPOCH_SECONDS_DELTA_DEFAULT - 10)
         self.assertLess(panther_item["Item"][caching._TTL_COL], int(datetime.datetime.now().timestamp()) + caching._EPOCH_SECONDS_DELTA_DEFAULT + 10)
         self.assertEqual(panther_item["Item"][caching._COUNT_COL], 1)
 
-
-@mock_dynamodb
+@mock_aws
 class TestCachingStringSet(DynamoBaseTest, unittest.TestCase):
     def test_new_add(self):
         self.assertEqual(caching.get_string_set("strs2"), set())
         self.assertEqual(caching.add_to_string_set("strs2", ["b", "a"]), {"a", "b"})
         self.assertEqual(caching.get_string_set("strs2"), {"a", "b"})
 
     def test_existing_add(self):
@@ -277,16 +275,15 @@
             Key={"key": "strs"}, ProjectionExpression=f"{caching._STRING_SET_COL}, {caching._TTL_COL}"
         )
         # Check TTL
         self.assertGreater(strs_item["Item"][caching._TTL_COL], int(datetime.datetime.now().timestamp()) + caching._EPOCH_SECONDS_DELTA_DEFAULT - 10)
         self.assertLess(strs_item["Item"][caching._TTL_COL], int(datetime.datetime.now().timestamp()) + caching._EPOCH_SECONDS_DELTA_DEFAULT + 10)
         self.assertEqual(strs_item["Item"][caching._STRING_SET_COL], {"w", "y"})
 
-
-@mock_dynamodb
+@mock_aws
 class TestCachingDictionary(DynamoBaseTest, unittest.TestCase):
     def test_new(self):
         self.assertEqual(caching.get_dictionary("dict"), dict())
         caching.put_dictionary("dict", {"b": "a"})
         self.assertEqual(caching.get_dictionary("dict"), {"b": "a"})
 
     def test_overwrite(self):
@@ -317,13 +314,12 @@
             Key={"key": "d"}, ProjectionExpression=f"{caching._DICT_COL}, {caching._TTL_COL}"
         )
         # Check TTL
         self.assertGreater(dict_item["Item"][caching._TTL_COL], int(datetime.datetime.now().timestamp()) + caching._EPOCH_SECONDS_DELTA_DEFAULT - 10)
         self.assertLess(dict_item["Item"][caching._TTL_COL], int(datetime.datetime.now().timestamp()) + caching._EPOCH_SECONDS_DELTA_DEFAULT + 10)
         self.assertEqual(json.loads(dict_item["Item"][caching._DICT_COL]), {"w": "y"})
 
-
-@mock_dynamodb
+@mock_aws
 class TestUsingMonitoring(DynamoBaseTest, unittest.TestCase):
     def test_monitoring_does_not_explode(self) -> None:
         caching.monitoring.USE_MONITORING = True
-        self.assertEqual(caching.get_string_set("strs"), {"a", "b"})
+        self.assertEqual(caching.get_string_set("strs"), {"a", "b"})
```

