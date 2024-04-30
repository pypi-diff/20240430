# Comparing `tmp/pyartifactory-2.1.3.tar.gz` & `tmp/pyartifactory-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyartifactory-2.1.3.tar", max compression
+gzip compressed data, was "pyartifactory-2.1.4.tar", max compression
```

## Comparing `pyartifactory-2.1.3.tar` & `pyartifactory-2.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1108 2023-10-31 20:25:04.083388 pyartifactory-2.1.3/LICENSE
--rw-r--r--   0        0        0    14598 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/README.md
--rw-r--r--   0        0        0      954 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/__init__.py
--rw-r--r--   0        0        0     1279 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/exception.py
--rw-r--r--   0        0        0     1719 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/models/__init__.py
--rw-r--r--   0        0        0     2543 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/models/artifact.py
--rw-r--r--   0        0        0      780 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/models/auth.py
--rw-r--r--   0        0        0      609 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/models/group.py
--rw-r--r--   0        0        0     2862 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/models/permission.py
--rw-r--r--   0        0        0     9622 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/models/repository.py
--rw-r--r--   0        0        0     1254 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/models/user.py
--rw-r--r--   0        0        0       35 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/objects/__init__.py
--rw-r--r--   0        0        0    14517 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/objects/artifact.py
--rw-r--r--   0        0        0     1264 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/objects/artifactory.py
--rw-r--r--   0        0        0     2980 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/objects/group.py
--rw-r--r--   0        0        0     2812 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/objects/object.py
--rw-r--r--   0        0        0     4284 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/objects/permission.py
--rw-r--r--   0        0        0     5157 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/objects/repository.py
--rw-r--r--   0        0        0     4763 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/objects/security.py
--rw-r--r--   0        0        0     3318 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/objects/user.py
--rw-r--r--   0        0        0        0 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/py.typed
--rw-r--r--   0        0        0      507 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyartifactory/utils.py
--rw-r--r--   0        0        0     4064 2023-10-31 20:25:04.087388 pyartifactory-2.1.3/pyproject.toml
--rw-r--r--   0        0        0    15941 1970-01-01 00:00:00.000000 pyartifactory-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1108 2024-03-13 22:08:36.494686 pyartifactory-2.1.4/LICENSE
+-rw-r--r--   0        0        0    14598 2024-03-13 22:08:36.494686 pyartifactory-2.1.4/README.md
+-rw-r--r--   0        0        0      954 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/__init__.py
+-rw-r--r--   0        0        0     1279 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/exception.py
+-rw-r--r--   0        0        0     1719 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/models/__init__.py
+-rw-r--r--   0        0        0     2543 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/models/artifact.py
+-rw-r--r--   0        0        0      780 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/models/auth.py
+-rw-r--r--   0        0        0      609 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/models/group.py
+-rw-r--r--   0        0        0     2862 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/models/permission.py
+-rw-r--r--   0        0        0     9622 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/models/repository.py
+-rw-r--r--   0        0        0     1254 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/models/user.py
+-rw-r--r--   0        0        0       35 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/objects/__init__.py
+-rw-r--r--   0        0        0    14713 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/objects/artifact.py
+-rw-r--r--   0        0        0     1264 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/objects/artifactory.py
+-rw-r--r--   0        0        0     2980 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/objects/group.py
+-rw-r--r--   0        0        0     2812 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/objects/object.py
+-rw-r--r--   0        0        0     4284 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/objects/permission.py
+-rw-r--r--   0        0        0     5157 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/objects/repository.py
+-rw-r--r--   0        0        0     4763 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/objects/security.py
+-rw-r--r--   0        0        0     3318 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/objects/user.py
+-rw-r--r--   0        0        0        0 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/py.typed
+-rw-r--r--   0        0        0      507 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyartifactory/utils.py
+-rw-r--r--   0        0        0     4064 2024-03-13 22:08:36.498686 pyartifactory-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0    15992 1970-01-01 00:00:00.000000 pyartifactory-2.1.4/PKG-INFO
```

### Comparing `pyartifactory-2.1.3/LICENSE` & `pyartifactory-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyartifactory-2.1.3/README.md` & `pyartifactory-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyartifactory-2.1.3/pyartifactory/__init__.py` & `pyartifactory-2.1.4/pyartifactory/__init__.py`

 * *Files identical despite different names*

### Comparing `pyartifactory-2.1.3/pyartifactory/exception.py` & `pyartifactory-2.1.4/pyartifactory/exception.py`

 * *Files identical despite different names*

### Comparing `pyartifactory-2.1.3/pyartifactory/models/__init__.py` & `pyartifactory-2.1.4/pyartifactory/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyartifactory-2.1.3/pyartifactory/models/artifact.py` & `pyartifactory-2.1.4/pyartifactory/models/artifact.py`

 * *Files identical despite different names*

### Comparing `pyartifactory-2.1.3/pyartifactory/models/auth.py` & `pyartifactory-2.1.4/pyartifactory/models/auth.py`

 * *Files identical despite different names*

### Comparing `pyartifactory-2.1.3/pyartifactory/models/group.py` & `pyartifactory-2.1.4/pyartifactory/models/group.py`

 * *Files identical despite different names*

### Comparing `pyartifactory-2.1.3/pyartifactory/models/permission.py` & `pyartifactory-2.1.4/pyartifactory/models/permission.py`

 * *Files identical despite different names*

### Comparing `pyartifactory-2.1.3/pyartifactory/models/repository.py` & `pyartifactory-2.1.4/pyartifactory/models/repository.py`

 * *Files identical despite different names*

### Comparing `pyartifactory-2.1.3/pyartifactory/models/user.py` & `pyartifactory-2.1.4/pyartifactory/models/user.py`

 * *Files identical despite different names*

### Comparing `pyartifactory-2.1.3/pyartifactory/objects/artifact.py` & `pyartifactory-2.1.4/pyartifactory/objects/artifact.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import logging
 import os
+import urllib
 from collections.abc import Iterator
 from pathlib import Path
 from typing import Dict, List, Optional, Union
 
 import requests
 from pydantic import ValidationError
 from requests import Response
@@ -55,15 +56,17 @@
 
         :param artifact_path: Path to file or folder in Artifactory
         """
         if isinstance(artifact_path, str):
             artifact_path = Path(artifact_path.lstrip("/"))
 
         try:
-            response = self._get(f"api/storage/{artifact_path.as_posix()}")
+            artifact_as_posix = artifact_path.as_posix()
+            artifact_as_url = urllib.parse.quote(artifact_as_posix)
+            response = self._get(f"api/storage/{artifact_as_url}")
             try:
                 artifact_info: ArtifactInfoResponse = ArtifactFolderInfoResponse.model_validate(response.json())
             except ValidationError:
                 artifact_info = ArtifactFileInfoResponse.model_validate(response.json())
             return artifact_info
         except requests.exceptions.HTTPError as error:
             http_response: Union[Response, None] = error.response
@@ -116,15 +119,16 @@
 
         if local_directory_path:
             local_directory_path.mkdir(parents=True, exist_ok=True)
             local_file_full_path = local_directory_path / local_filename
         else:
             local_file_full_path = Path(local_filename)
 
-        with self._get(f"{artifact_path}", stream=True) as response, local_file_full_path.open("wb") as file:
+        artifact_path_url = urllib.parse.quote(artifact_path)
+        with self._get(f"{artifact_path_url}", stream=True) as response, local_file_full_path.open("wb") as file:
             for chunk in response.iter_content(chunk_size=8192):
                 if chunk:  # filter out keep-alive new chunks
                     file.write(chunk)
         logger.debug("Artifact %s successfully downloaded", local_filename)
         return local_file_full_path
 
     def download(self, artifact_path: str, local_directory_path: str = ".") -> Path:
```

### Comparing `pyartifactory-2.1.3/pyartifactory/objects/artifactory.py` & `pyartifactory-2.1.4/pyartifactory/objects/artifactory.py`

 * *Files identical despite different names*

### Comparing `pyartifactory-2.1.3/pyartifactory/objects/group.py` & `pyartifactory-2.1.4/pyartifactory/objects/group.py`

 * *Files identical despite different names*

### Comparing `pyartifactory-2.1.3/pyartifactory/objects/object.py` & `pyartifactory-2.1.4/pyartifactory/objects/object.py`

 * *Files identical despite different names*

### Comparing `pyartifactory-2.1.3/pyartifactory/objects/permission.py` & `pyartifactory-2.1.4/pyartifactory/objects/permission.py`

 * *Files identical despite different names*

### Comparing `pyartifactory-2.1.3/pyartifactory/objects/repository.py` & `pyartifactory-2.1.4/pyartifactory/objects/repository.py`

 * *Files identical despite different names*

### Comparing `pyartifactory-2.1.3/pyartifactory/objects/security.py` & `pyartifactory-2.1.4/pyartifactory/objects/security.py`

 * *Files identical despite different names*

### Comparing `pyartifactory-2.1.3/pyartifactory/objects/user.py` & `pyartifactory-2.1.4/pyartifactory/objects/user.py`

 * *Files identical despite different names*

### Comparing `pyartifactory-2.1.3/pyproject.toml` & `pyartifactory-2.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyArtifactory"
-version = "2.1.3"
+version = "2.1.4"
 description = "Typed interactions with the Jfrog Artifactory REST API"
 authors = [
     "Ananias CARVALHO <carvalhoananias@hotmail.com>",
     "Thomas GAUDIN <thomas.gaudin@centraliens-lille.org>",
     "Helio Chissini de Castro <heliocastro@gmail.com"
 ]
 license = "MIT"
```

### Comparing `pyartifactory-2.1.3/PKG-INFO` & `pyartifactory-2.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyArtifactory
-Version: 2.1.3
+Version: 2.1.4
 Summary: Typed interactions with the Jfrog Artifactory REST API
 Home-page: https://github.com/anancarv/python-artifactory
 License: MIT
 Keywords: artifactory
 Author: Ananias CARVALHO
 Author-email: carvalhoananias@hotmail.com
 Requires-Python: >=3.8,<4.0
@@ -14,14 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Filesystems
 Classifier: Typing :: Typed
 Requires-Dist: pydantic[email] (>=2.4.0,<3.0.0)
 Requires-Dist: requests (>=2.31,<3.0)
 Requires-Dist: typing_extensions (>=4.7.1,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/anancarv/python-artifactory/issues
```

