# Comparing `tmp/np_aind_metadata-0.1.6.tar.gz` & `tmp/np_aind_metadata-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_aind_metadata-0.1.6.tar", last modified: Tue Apr 23 19:34:04 2024, max compression
+gzip compressed data, was "np_aind_metadata-0.1.7.tar", last modified: Tue Apr 30 00:32:52 2024, max compression
```

## Comparing `np_aind_metadata-0.1.6.tar` & `np_aind_metadata-0.1.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:04.831829 np_aind_metadata-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-23 19:33:27.000000 np_aind_metadata-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-23 19:34:04.831829 np_aind_metadata-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-23 19:33:27.000000 np_aind_metadata-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-23 19:34:02.000000 np_aind_metadata-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:34:04.831829 np_aind_metadata-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:04.827829 np_aind_metadata-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:04.827829 np_aind_metadata-0.1.6/src/np_aind_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-23 19:33:27.000000 np_aind_metadata-0.1.6/src/np_aind_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-23 19:33:58.000000 np_aind_metadata-0.1.6/src/np_aind_metadata/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:04.831829 np_aind_metadata-0.1.6/src/np_aind_metadata/init/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:33:27.000000 np_aind_metadata-0.1.6/src/np_aind_metadata/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22049 2024-04-23 19:33:58.000000 np_aind_metadata-0.1.6/src/np_aind_metadata/init/neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-23 19:33:27.000000 np_aind_metadata-0.1.6/src/np_aind_metadata/np.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-23 19:33:58.000000 np_aind_metadata-0.1.6/src/np_aind_metadata/np_codeocean.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:33:27.000000 np_aind_metadata-0.1.6/src/np_aind_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:04.831829 np_aind_metadata-0.1.6/src/np_aind_metadata/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-23 19:33:27.000000 np_aind_metadata-0.1.6/src/np_aind_metadata/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-23 19:33:27.000000 np_aind_metadata-0.1.6/src/np_aind_metadata/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:04.831829 np_aind_metadata-0.1.6/src/np_aind_metadata/update/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:33:27.000000 np_aind_metadata-0.1.6/src/np_aind_metadata/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-23 19:33:59.000000 np_aind_metadata-0.1.6/src/np_aind_metadata/update/dynamic_routing_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-04-23 19:33:27.000000 np_aind_metadata-0.1.6/src/np_aind_metadata/update/dynamic_routing_task_etl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-23 19:33:27.000000 np_aind_metadata-0.1.6/src/np_aind_metadata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:04.831829 np_aind_metadata-0.1.6/src/np_aind_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-23 19:34:04.000000 np_aind_metadata-0.1.6/src/np_aind_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-23 19:34:04.000000 np_aind_metadata-0.1.6/src/np_aind_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:04.000000 np_aind_metadata-0.1.6/src/np_aind_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 19:34:04.000000 np_aind_metadata-0.1.6/src/np_aind_metadata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-23 19:34:04.000000 np_aind_metadata-0.1.6/src/np_aind_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-23 19:34:04.000000 np_aind_metadata-0.1.6/src/np_aind_metadata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:04.831829 np_aind_metadata-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 19:33:27.000000 np_aind_metadata-0.1.6/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-23 19:33:27.000000 np_aind_metadata-0.1.6/tests/test_np.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-23 19:33:27.000000 np_aind_metadata-0.1.6/tests/test_np_codeocean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-23 19:33:27.000000 np_aind_metadata-0.1.6/tests/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:52.959532 np_aind_metadata-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-30 00:32:52.959532 np_aind_metadata-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-30 00:32:50.000000 np_aind_metadata-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 00:32:52.959532 np_aind_metadata-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:52.955531 np_aind_metadata-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:52.959532 np_aind_metadata-0.1.7/src/np_aind_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:52.959532 np_aind_metadata-0.1.7/src/np_aind_metadata/init/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22049 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/init/neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/np.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-30 00:32:47.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/np_codeocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:52.959532 np_aind_metadata-0.1.7/src/np_aind_metadata/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:52.959532 np_aind_metadata-0.1.7/src/np_aind_metadata/update/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/update/dynamic_routing_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/update/dynamic_routing_task_etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/src/np_aind_metadata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:52.959532 np_aind_metadata-0.1.7/src/np_aind_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-30 00:32:52.000000 np_aind_metadata-0.1.7/src/np_aind_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-30 00:32:52.000000 np_aind_metadata-0.1.7/src/np_aind_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 00:32:52.000000 np_aind_metadata-0.1.7/src/np_aind_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-30 00:32:52.000000 np_aind_metadata-0.1.7/src/np_aind_metadata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-30 00:32:52.000000 np_aind_metadata-0.1.7/src/np_aind_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 00:32:52.000000 np_aind_metadata-0.1.7/src/np_aind_metadata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 00:32:52.959532 np_aind_metadata-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/tests/test_np.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/tests/test_np_codeocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-30 00:32:16.000000 np_aind_metadata-0.1.7/tests/test_storage.py
```

### Comparing `np_aind_metadata-0.1.6/LICENSE` & `np_aind_metadata-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.6/PKG-INFO` & `np_aind_metadata-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-aind-metadata
-Version: 0.1.6
+Version: 0.1.7
 Author-email: Christopher Mochizuki <chrism@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/np-aind-metadata
 Project-URL: Issues, https://github.com/AllenInstitute/np-aind-metadata/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `np_aind_metadata-0.1.6/README.md` & `np_aind_metadata-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.6/pyproject.toml` & `np_aind_metadata-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 dependencies = [
     "h5py>=3.10.0",
     "pyyaml>=6.0.1",
     "np-session>=0.6.40",
     "np-config>=0.4.27",
     "aind-metadata-mapper==0.6.2",
 ]
-version = "0.1.6"
+version = "0.1.7"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
```

### Comparing `np_aind_metadata-0.1.6/src/np_aind_metadata/__init__.py` & `np_aind_metadata-0.1.7/src/np_aind_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.6/src/np_aind_metadata/init/neuropixels_rig.py` & `np_aind_metadata-0.1.7/src/np_aind_metadata/init/neuropixels_rig.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.6/src/np_aind_metadata/np.py` & `np_aind_metadata-0.1.7/src/np_aind_metadata/np.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.6/src/np_aind_metadata/np_codeocean.py` & `np_aind_metadata-0.1.7/src/np_aind_metadata/np_codeocean.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import logging
 import pathlib
 import shutil
 import tempfile
 
 from aind_data_schema.core import rig, session
 
@@ -16,14 +17,30 @@
     directory.
     """
     matches = list(session_directory.glob("*session.json"))
     logger.debug("Scraped session model paths: %s" % matches)
     return matches[0]
 
 
+def _update_rig_modification_date(
+    current: rig.Rig,
+    modification_date: datetime.date,
+    output_path: pathlib.Path,
+) -> pathlib.Path:
+    id_parts = current.rig_id.split("_")
+    id_parts[-1] = modification_date.strftime("%y%m%d")
+    current.rig_id = "_".join(id_parts)
+    current.modification_date = modification_date
+    with tempfile.TemporaryDirectory() as temp_dir:
+        current.write_standard_file(temp_dir)
+        temp_path = pathlib.Path(temp_dir) / current.default_filename()
+        assert temp_path.exists()
+        return pathlib.Path(shutil.copy2(temp_path, output_path))
+
+
 def _update_session_rig_id(
     session: session.Session,
     rig_id: str,
     output_path: pathlib.Path,
 ) -> pathlib.Path:
     """Updates session rig id and copies it to `output_path`."""
     session.rig_id = rig_id
@@ -33,14 +50,15 @@
         assert temp_session_path.exists()
         return pathlib.Path(shutil.copy2(temp_session_path, output_path))
 
 
 def add_rig_to_dynamic_routing_session_dir(
     session_dir: pathlib.Path,
     rig_model_dir: pathlib.Path,
+    modification_date: datetime.date,
 ) -> pathlib.Path:
     """Direct support for np_codeocean. Adds an aind-metadata rig model
     rig.json to a dynamic routing session directory. If rig_id is updated,
      will update the associated session json.
 
     Notes
     -----
@@ -73,14 +91,19 @@
             session_rig_path.exists()
         ), "Session rig path should exist where we expect."
         updated_model_path = dynamic_routing_task_update.update_rig(
             session_rig_path,
             open_ephys_settings_sources=settings_sources,
             output_path=session_rig_path,
         )
+        updated_model_path = _update_rig_modification_date(
+            rig.Rig.model_validate_json(updated_model_path.read_text()),
+            modification_date,
+            updated_model_path,
+        )
         updated_model = rig.Rig.model_validate_json(updated_model_path.read_text())
         if updated_model.rig_id != scraped_rig_id:
             logger.debug("Rig model rig_id has changed. Updating session rig_id.")
             _update_session_rig_id(
                 scraped_session,
                 updated_model.rig_id,
                 scraped_session_model_path,
```

### Comparing `np_aind_metadata-0.1.6/src/np_aind_metadata/scripts/main.py` & `np_aind_metadata-0.1.7/src/np_aind_metadata/scripts/main.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.6/src/np_aind_metadata/storage.py` & `np_aind_metadata-0.1.7/src/np_aind_metadata/storage.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.6/src/np_aind_metadata/update/dynamic_routing_task.py` & `np_aind_metadata-0.1.7/src/np_aind_metadata/update/dynamic_routing_task.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.6/src/np_aind_metadata/update/dynamic_routing_task_etl.py` & `np_aind_metadata-0.1.7/src/np_aind_metadata/update/dynamic_routing_task_etl.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.6/src/np_aind_metadata/utils.py` & `np_aind_metadata-0.1.7/src/np_aind_metadata/utils.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.6/src/np_aind_metadata.egg-info/PKG-INFO` & `np_aind_metadata-0.1.7/src/np_aind_metadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-aind-metadata
-Version: 0.1.6
+Version: 0.1.7
 Author-email: Christopher Mochizuki <chrism@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/np-aind-metadata
 Project-URL: Issues, https://github.com/AllenInstitute/np-aind-metadata/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `np_aind_metadata-0.1.6/src/np_aind_metadata.egg-info/SOURCES.txt` & `np_aind_metadata-0.1.7/src/np_aind_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.6/tests/test_np_codeocean.py` & `np_aind_metadata-0.1.7/tests/test_np_codeocean.py`

 * *Files identical despite different names*

### Comparing `np_aind_metadata-0.1.6/tests/test_storage.py` & `np_aind_metadata-0.1.7/tests/test_storage.py`

 * *Files identical despite different names*

