# Comparing `tmp/eodc-2024.4.5.tar.gz` & `tmp/eodc-2024.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2024.4.5.tar", max compression
+gzip compressed data, was "eodc-2024.4.6.tar", max compression
```

## Comparing `eodc-2024.4.5.tar` & `eodc-2024.4.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      676 2024-04-25 15:41:13.790220 eodc-2024.4.5/README.md
--rw-r--r--   0        0        0      195 2024-04-25 15:41:13.790220 eodc-2024.4.5/eodc/__init__.py
--rw-r--r--   0        0        0     1794 2024-04-25 15:41:13.790220 eodc-2024.4.5/eodc/auth.py
--rw-r--r--   0        0        0     1311 2024-04-25 15:41:13.794220 eodc-2024.4.5/eodc/dask.py
--rw-r--r--   0        0        0    13711 2024-04-25 15:41:13.794220 eodc-2024.4.5/eodc/faas.py
--rw-r--r--   0        0        0     1183 2024-04-25 15:41:13.794220 eodc-2024.4.5/eodc/settings.py
--rw-r--r--   0        0        0     2240 2024-04-25 15:41:13.794220 eodc-2024.4.5/eodc/storage.py
--rw-r--r--   0        0        0        0 2024-04-25 15:41:13.794220 eodc-2024.4.5/eodc/visualisation/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 15:41:13.794220 eodc-2024.4.5/eodc/visualisation/vessel_detection/__init__.py
--rwxr-xr-x   0        0        0    15080 2024-04-25 15:41:13.794220 eodc-2024.4.5/eodc/visualisation/vessel_detection/app.py
--rw-r--r--   0        0        0      261 2024-04-25 15:41:13.794220 eodc-2024.4.5/eodc/visualisation/vessel_detection/assets/app.css
--rw-r--r--   0        0        0     2539 2024-04-25 15:41:13.794220 eodc-2024.4.5/eodc/visualisation/vessel_detection/cards.py
--rw-r--r--   0        0        0     8522 2024-04-25 15:41:13.794220 eodc-2024.4.5/eodc/visualisation/vessel_detection/navbar.py
--rw-r--r--   0        0        0     2867 2024-04-25 15:41:13.794220 eodc-2024.4.5/eodc/visualisation/vessel_detection/utils.py
--rw-r--r--   0        0        0    32206 2024-04-25 15:41:13.794220 eodc-2024.4.5/eodc/workspace.py
--rw-r--r--   0        0        0     1890 2024-04-25 15:41:13.798220 eodc-2024.4.5/pyproject.toml
--rw-r--r--   0        0        0     2802 1970-01-01 00:00:00.000000 eodc-2024.4.5/PKG-INFO
+-rw-r--r--   0        0        0      676 2024-04-30 13:16:50.862928 eodc-2024.4.6/README.md
+-rw-r--r--   0        0        0      195 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/__init__.py
+-rw-r--r--   0        0        0     1794 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/auth.py
+-rw-r--r--   0        0        0     1311 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/dask.py
+-rw-r--r--   0        0        0    13711 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/faas.py
+-rw-r--r--   0        0        0     1183 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/settings.py
+-rw-r--r--   0        0        0     2240 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/storage.py
+-rw-r--r--   0        0        0        0 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/visualisation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/visualisation/vessel_detection/__init__.py
+-rwxr-xr-x   0        0        0    15080 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/visualisation/vessel_detection/app.py
+-rw-r--r--   0        0        0      261 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/visualisation/vessel_detection/assets/app.css
+-rw-r--r--   0        0        0     2539 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/visualisation/vessel_detection/cards.py
+-rw-r--r--   0        0        0     8522 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/visualisation/vessel_detection/navbar.py
+-rw-r--r--   0        0        0     2867 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/visualisation/vessel_detection/utils.py
+-rw-r--r--   0        0        0    32166 2024-04-30 13:16:50.862928 eodc-2024.4.6/eodc/workspace.py
+-rw-r--r--   0        0        0     1890 2024-04-30 13:16:50.866928 eodc-2024.4.6/pyproject.toml
+-rw-r--r--   0        0        0     2802 1970-01-01 00:00:00.000000 eodc-2024.4.6/PKG-INFO
```

### Comparing `eodc-2024.4.5/README.md` & `eodc-2024.4.6/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.5/eodc/auth.py` & `eodc-2024.4.6/eodc/auth.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.5/eodc/dask.py` & `eodc-2024.4.6/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.5/eodc/faas.py` & `eodc-2024.4.6/eodc/faas.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.5/eodc/settings.py` & `eodc-2024.4.6/eodc/settings.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.5/eodc/storage.py` & `eodc-2024.4.6/eodc/storage.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.5/eodc/visualisation/vessel_detection/app.py` & `eodc-2024.4.6/eodc/visualisation/vessel_detection/app.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.5/eodc/visualisation/vessel_detection/cards.py` & `eodc-2024.4.6/eodc/visualisation/vessel_detection/cards.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.5/eodc/visualisation/vessel_detection/navbar.py` & `eodc-2024.4.6/eodc/visualisation/vessel_detection/navbar.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.5/eodc/visualisation/vessel_detection/utils.py` & `eodc-2024.4.6/eodc/visualisation/vessel_detection/utils.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.4.5/eodc/workspace.py` & `eodc-2024.4.6/eodc/workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,15 +413,14 @@
         files = self.s3_client.list_objects(Bucket=f"{tenant_name}{workspace_name}")
         return files["Contents"]
 
     def upload_file(
         self, workspace_name: str, file_path: str, path_in_workspace: str = ""
     ):
         path_in_workspace = path_in_workspace.removesuffix("/")
-        self.s3_client.put_object_acl()
         self.s3_client.upload_file(
             file_path,
             workspace_name,
             os.path.join(path_in_workspace, file_path.split("/")[-1]),
         )
 
     def upload_path(
```

### Comparing `eodc-2024.4.5/pyproject.toml` & `eodc-2024.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "eodc"
 
-version = "2024.4.5"
+version = "2024.4.6"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Gerald Irsiegler <gerald.irsiegler@eodc.eu>", "Christoph Reimer <christoph.reimer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `eodc-2024.4.5/PKG-INFO` & `eodc-2024.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2024.4.5
+Version: 2024.4.6
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
```

