# Comparing `tmp/gtagora_connector-1.4.4.tar.gz` & `tmp/gtagora_connector-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtagora_connector-1.4.4.tar", last modified: Thu Apr 25 11:46:34 2024, max compression
+gzip compressed data, was "gtagora_connector-1.5.0.tar", last modified: Tue Apr 30 11:11:24 2024, max compression
```

## Comparing `gtagora_connector-1.4.4.tar` & `gtagora_connector-1.5.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:46:34.884129 gtagora_connector-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-04-25 11:46:34.884129 gtagora_connector-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11069 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:46:34.876129 gtagora_connector-1.4.4/gtagora/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13417 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/agora.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:46:34.880129 gtagora_connector-1.4.4/gtagora/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/http/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/http/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/http/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:46:34.884129 gtagora_connector-1.4.4/gtagora/models/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/breadcrumb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/datafile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/exam.py
--rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/folder_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/image_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    17335 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/import_package.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/parameter_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/patient.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/project_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/series.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/trash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/upload_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/models/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/gtagora/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:46:34.884129 gtagora_connector-1.4.4/gtagora_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-04-25 11:46:34.000000 gtagora_connector-1.4.4/gtagora_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-25 11:46:34.000000 gtagora_connector-1.4.4/gtagora_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 11:46:34.000000 gtagora_connector-1.4.4/gtagora_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-25 11:46:34.000000 gtagora_connector-1.4.4/gtagora_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 11:46:34.000000 gtagora_connector-1.4.4/gtagora_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 11:46:34.884129 gtagora_connector-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:46:34.884129 gtagora_connector-1.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-25 11:46:30.000000 gtagora_connector-1.4.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:11:24.612888 gtagora_connector-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-04-30 11:11:24.612888 gtagora_connector-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11069 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:11:24.608888 gtagora_connector-1.5.0/gtagora/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13417 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/agora.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:11:24.608888 gtagora_connector-1.5.0/gtagora/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/http/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/http/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:11:24.612888 gtagora_connector-1.5.0/gtagora/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10944 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/breadcrumb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/datafile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/exam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/folder_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/image_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17335 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/import_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/parameter_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/patient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/project_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/trash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/models/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/gtagora/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:11:24.612888 gtagora_connector-1.5.0/gtagora_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-04-30 11:11:24.000000 gtagora_connector-1.5.0/gtagora_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-30 11:11:24.000000 gtagora_connector-1.5.0/gtagora_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 11:11:24.000000 gtagora_connector-1.5.0/gtagora_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 11:11:24.000000 gtagora_connector-1.5.0/gtagora_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 11:11:24.000000 gtagora_connector-1.5.0/gtagora_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 11:11:24.612888 gtagora_connector-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:11:24.612888 gtagora_connector-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-30 11:11:18.000000 gtagora_connector-1.5.0/tests/test_utils.py
```

### Comparing `gtagora_connector-1.4.4/LICENSE` & `gtagora_connector-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/PKG-INFO` & `gtagora_connector-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtagora-connector
-Version: 1.4.4
+Version: 1.5.0
 Summary: The Agora Connector for Python
 Home-page: https://github.com/gyrotools/gtagora
 Author: Martin Bührer, Felix Eichenberger
 Author-email: info@gyrotools.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gtagora_connector-1.4.4/README.md` & `gtagora_connector-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/gtagora/agora.py` & `gtagora_connector-1.5.0/gtagora/agora.py`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/gtagora/http/auth.py` & `gtagora_connector-1.5.0/gtagora/http/auth.py`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/gtagora/http/client.py` & `gtagora_connector-1.5.0/gtagora/http/client.py`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/gtagora/http/connection.py` & `gtagora_connector-1.5.0/gtagora/http/connection.py`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/gtagora/models/base.py` & `gtagora_connector-1.5.0/gtagora/models/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -262,7 +262,66 @@
             instances = TagInstance.get_list_from_data(response.json())
             if instances:
                 return instances[0]
             else:
                 return None
 
         raise AgoraException('Could not tag the object')
+
+    def get_tags(self):
+        from gtagora.models.tag import Tag
+
+        url = f'{self.BASE_URL_V2}{self.id}/tags/'
+        response = self.http_client.get(url)
+        if response.status_code == 200:
+            list = Tag.get_list_from_data(response.json())
+            return list
+        else:
+            raise AgoraException(f'Cannot get the tags: {response.text}')
+
+
+class RatingMixin:
+    def rate(self, value):
+        from gtagora.models.tag import RatingInstance
+
+        if value < 0 or value > 5:
+            raise AgoraException('The rating must be between 0 and 5')
+
+        # check if the object already has a rating
+        rating = self.get_rating()
+        url = RatingInstance.BASE_URL
+
+        if rating:
+            if value == 0:
+                # delete rating
+                response = self.http_client.delete(f'{url}{rating.id}/')
+            else:
+                # update rating
+                put_data = {'id': rating.id, 'value': value, 'rated_object_content_type': self.content_type(), 'rated_object_id': self.id}
+                response = self.http_client.put(f'{url}{rating.id}/', put_data)
+        else:
+            # create rating
+            post_data = {'value': value, 'rated_object_content_type': self.content_type(), 'rated_object_id': self.id}
+            response = self.http_client.post(url, post_data)
+
+        if response.status_code == 204:
+            return None
+
+        if response.status_code < 400:
+            return RatingInstance.from_response(response.json(), http_client=self.http_client)
+
+        raise AgoraException('Could not rate the object')
+
+    def get_rating(self):
+        from gtagora.models.tag import RatingInstance
+
+        url = f'{self.BASE_URL_V2}{self.id}/rating/'
+        response = self.http_client.get(url)
+        if response.status_code == 200:
+            ratings = RatingInstance.get_list_from_data(response.json())
+            if ratings:
+                return ratings[0]
+            else:
+                return None
+
+
+        raise AgoraException(f'Cannot get the rating: {response.text}')
```

### Comparing `gtagora_connector-1.4.4/gtagora/models/datafile.py` & `gtagora_connector-1.5.0/gtagora/models/datafile.py`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/gtagora/models/dataset.py` & `gtagora_connector-1.5.0/gtagora/models/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 from gtagora.exception import AgoraException
-from gtagora.models.base import BaseModel, LinkToFolderMixin, TagMixin
+from gtagora.models.base import BaseModel, LinkToFolderMixin, TagMixin, RatingMixin
 from gtagora.models.datafile import Datafile
 from gtagora.models.image_info import ImageInfo
 from gtagora.models.parameter import Parameter
 from gtagora.models.parameter_set import ParameterSet
 
 
 class DatasetType:
@@ -24,15 +24,15 @@
     NIFTI2 = 601
     NIFTI_ANALYZE75 = 602
     JMRUI_SPECTRO = 700
     QUERY = 10000
     OTHER = 100000
 
 
-class Dataset(LinkToFolderMixin, TagMixin, BaseModel):
+class Dataset(LinkToFolderMixin, TagMixin, RatingMixin, BaseModel):
     BASE_URL = '/api/v1/dataset/'
     BASE_URL_V2 = '/api/v2/dataset/'
 
     def _set_values(self, model_dict):
         for key, value in model_dict.items():
             if key == 'datafiles':
                 datafiles = []
```

### Comparing `gtagora_connector-1.4.4/gtagora/models/exam.py` & `gtagora_connector-1.5.0/gtagora/models/exam.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import List
 
 from gtagora.exception import AgoraException
-from gtagora.models.base import BaseModel, LinkToFolderMixin, DownloadDatasetMixin, TagMixin
+from gtagora.models.base import BaseModel, LinkToFolderMixin, DownloadDatasetMixin, TagMixin, RatingMixin
 from gtagora.models.dataset import Dataset
 from gtagora.models.import_package import import_data
 from gtagora.models.series import Series
 from gtagora.models.timeline import TimelineItem
 from gtagora.utils import remove_illegal_chars
 
 from pathlib import Path
 
 
-class Exam(LinkToFolderMixin, DownloadDatasetMixin, TagMixin, BaseModel):
+class Exam(LinkToFolderMixin, DownloadDatasetMixin, TagMixin, RatingMixin, BaseModel):
     BASE_URL = '/api/v1/exam/'
     BASE_URL_V2 = '/api/v2/exam/'
 
     def set_name(self, name):
         url = self.BASE_URL + str(self.id) + '/'
         data = {"name": name}
         response = self.http_client.put(url, data)
```

### Comparing `gtagora_connector-1.4.4/gtagora/models/folder.py` & `gtagora_connector-1.5.0/gtagora/models/folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from gtagora.exception import AgoraException
-from gtagora.models.base import LinkToFolderMixin, BaseModel, TagMixin
+from gtagora.models.base import LinkToFolderMixin, BaseModel, TagMixin, RatingMixin
 from gtagora.models.breadcrumb import Breadcrumb
 from gtagora.models.dataset import Dataset
 from gtagora.models.datafile import Datafile
 from gtagora.models.exam import Exam
 from gtagora.models.folder_item import FolderItem
 from gtagora.models.import_package import import_data
 from gtagora.models.series import Series
 from gtagora.utils import remove_illegal_chars
 
 from pathlib import Path
 from typing import List
 from functools import partial
 
 
-class Folder(LinkToFolderMixin, TagMixin, BaseModel):
+class Folder(LinkToFolderMixin, TagMixin, RatingMixin, BaseModel):
     BASE_URL = '/api/v1/folder/'
+    BASE_URL_V2 = '/api/v2/folder/'
 
     def get_items(self):
         items = []
 
         url = self.BASE_URL + str(self.id) + '/items/?limit=10000000000'
         response = self.http_client.get(url)
```

### Comparing `gtagora_connector-1.4.4/gtagora/models/folder_item.py` & `gtagora_connector-1.5.0/gtagora/models/folder_item.py`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/gtagora/models/group.py` & `gtagora_connector-1.5.0/gtagora/models/group.py`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/gtagora/models/host.py` & `gtagora_connector-1.5.0/gtagora/models/host.py`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/gtagora/models/import_package.py` & `gtagora_connector-1.5.0/gtagora/models/import_package.py`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/gtagora/models/parameter_set.py` & `gtagora_connector-1.5.0/gtagora/models/parameter_set.py`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/gtagora/models/patient.py` & `gtagora_connector-1.5.0/gtagora/models/patient.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from gtagora.exception import AgoraException
-from gtagora.models.base import BaseModel, DownloadDatasetMixin, TagMixin
+from gtagora.models.base import BaseModel, DownloadDatasetMixin, TagMixin, RatingMixin
 from gtagora.models.exam import Exam
 
 
-class Patient(BaseModel, TagMixin, DownloadDatasetMixin):
+class Patient(BaseModel, TagMixin, RatingMixin, DownloadDatasetMixin):
 
     BASE_URL = '/api/v1/patient/'
+    BASE_URL_V2 = '/api/v2/patient/'
 
     def get_exams(self, filters=None):
         if filters and not isinstance(filters, dict):
             raise AgoraException('The filter must be a dict')
 
         url = f'{self.BASE_URL}{self.id}/exams/?limit=10000000000'
         return self._get_object_list(url, filters, Exam)
```

### Comparing `gtagora_connector-1.4.4/gtagora/models/project.py` & `gtagora_connector-1.5.0/gtagora/models/project.py`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/gtagora/models/series.py` & `gtagora_connector-1.5.0/gtagora/models/series.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from pathlib import Path
 from typing import List
 
 from gtagora.exception import AgoraException
-from gtagora.models.base import LinkToFolderMixin, BaseModel, DownloadDatasetMixin, SearchMixin, TagMixin
+from gtagora.models.base import LinkToFolderMixin, BaseModel, DownloadDatasetMixin, SearchMixin, TagMixin, RatingMixin
 from gtagora.models.dataset import Dataset
 from gtagora.models.import_package import import_data
 from gtagora.models.timeline import TimelineItem
 
 
-class Series(LinkToFolderMixin, DownloadDatasetMixin, TagMixin, BaseModel, SearchMixin):
+class Series(LinkToFolderMixin, DownloadDatasetMixin, TagMixin, RatingMixin, BaseModel, SearchMixin):
     BASE_URL = '/api/v1/serie/'
     BASE_URL_V2 = '/api/v2/series/'
 
     def get_datasets(self, filters=None):
         if filters and not isinstance(filters, dict):
             raise AgoraException('The filter must be a dict')
```

### Comparing `gtagora_connector-1.4.4/gtagora/models/tag.py` & `gtagora_connector-1.5.0/gtagora/models/tag.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,7 +31,12 @@
         else:
             return None
 
 
 class TagInstance(BaseModel):
 
     BASE_URL = '/api/v2/tag-instance/'
+
+
+class RatingInstance(BaseModel):
+
+    BASE_URL = '/api/v2/rating/'
```

### Comparing `gtagora_connector-1.4.4/gtagora/models/task.py` & `gtagora_connector-1.5.0/gtagora/models/task.py`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/gtagora/models/timeline.py` & `gtagora_connector-1.5.0/gtagora/models/timeline.py`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/gtagora/models/trash.py` & `gtagora_connector-1.5.0/gtagora/models/trash.py`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/gtagora/models/upload_session.py` & `gtagora_connector-1.5.0/gtagora/models/upload_session.py`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/gtagora/models/user.py` & `gtagora_connector-1.5.0/gtagora/models/user.py`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/gtagora/models/version.py` & `gtagora_connector-1.5.0/gtagora/models/version.py`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/gtagora/utils.py` & `gtagora_connector-1.5.0/gtagora/utils.py`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/gtagora_connector.egg-info/PKG-INFO` & `gtagora_connector-1.5.0/gtagora_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtagora-connector
-Version: 1.4.4
+Version: 1.5.0
 Summary: The Agora Connector for Python
 Home-page: https://github.com/gyrotools/gtagora
 Author: Martin Bührer, Felix Eichenberger
 Author-email: info@gyrotools.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gtagora_connector-1.4.4/gtagora_connector.egg-info/SOURCES.txt` & `gtagora_connector-1.5.0/gtagora_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gtagora_connector-1.4.4/setup.py` & `gtagora_connector-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gtagora-connector",
-    version="1.4.4",
+    version="1.5.0",
     author="Martin Bührer, Felix Eichenberger",
     author_email="info@gyrotools.com",
     description="The Agora Connector for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gyrotools/gtagora",
     packages=setuptools.find_packages(),
```

### Comparing `gtagora_connector-1.4.4/tests/test_utils.py` & `gtagora_connector-1.5.0/tests/test_utils.py`

 * *Files identical despite different names*

