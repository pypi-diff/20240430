# Comparing `tmp/npc_mvr-0.1.5.tar.gz` & `tmp/npc_mvr-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npc_mvr-0.1.5.tar", last modified: Mon Apr 29 22:04:47 2024, max compression
+gzip compressed data, was "npc_mvr-0.1.6.tar", last modified: Tue Apr 30 01:15:17 2024, max compression
```

## Comparing `npc_mvr-0.1.5.tar` & `npc_mvr-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:04:47.108709 npc_mvr-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-29 22:04:15.000000 npc_mvr-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-29 22:04:47.108709 npc_mvr-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-29 22:04:15.000000 npc_mvr-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-29 22:04:44.000000 npc_mvr-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 22:04:47.108709 npc_mvr-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:04:47.104709 npc_mvr-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:04:47.108709 npc_mvr-0.1.5/src/npc_mvr/
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-29 22:04:15.000000 npc_mvr-0.1.5/src/npc_mvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35080 2024-04-29 22:04:15.000000 npc_mvr-0.1.5/src/npc_mvr/mvr.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:04:15.000000 npc_mvr-0.1.5/src/npc_mvr/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:04:47.108709 npc_mvr-0.1.5/src/npc_mvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-29 22:04:47.000000 npc_mvr-0.1.5/src/npc_mvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-29 22:04:47.000000 npc_mvr-0.1.5/src/npc_mvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:04:47.000000 npc_mvr-0.1.5/src/npc_mvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-29 22:04:47.000000 npc_mvr-0.1.5/src/npc_mvr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 22:04:47.000000 npc_mvr-0.1.5/src/npc_mvr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:04:47.108709 npc_mvr-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 22:04:15.000000 npc_mvr-0.1.5/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:15:17.482252 npc_mvr-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-30 01:14:45.000000 npc_mvr-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-30 01:15:17.482252 npc_mvr-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-30 01:14:45.000000 npc_mvr-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-30 01:15:15.000000 npc_mvr-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 01:15:17.482252 npc_mvr-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:15:17.478252 npc_mvr-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:15:17.478252 npc_mvr-0.1.6/src/npc_mvr/
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-30 01:14:45.000000 npc_mvr-0.1.6/src/npc_mvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35180 2024-04-30 01:15:11.000000 npc_mvr-0.1.6/src/npc_mvr/mvr.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 01:14:45.000000 npc_mvr-0.1.6/src/npc_mvr/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:15:17.482252 npc_mvr-0.1.6/src/npc_mvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-30 01:15:17.000000 npc_mvr-0.1.6/src/npc_mvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-30 01:15:17.000000 npc_mvr-0.1.6/src/npc_mvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 01:15:17.000000 npc_mvr-0.1.6/src/npc_mvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-30 01:15:17.000000 npc_mvr-0.1.6/src/npc_mvr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 01:15:17.000000 npc_mvr-0.1.6/src/npc_mvr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:15:17.482252 npc_mvr-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 01:14:45.000000 npc_mvr-0.1.6/tests/test_core.py
```

### Comparing `npc_mvr-0.1.5/LICENSE` & `npc_mvr-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `npc_mvr-0.1.5/PKG-INFO` & `npc_mvr-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npc-mvr
-Version: 0.1.5
+Version: 0.1.6
 Summary: Tools for reading raw video data from MindScope Neuropixels experiments, compatible with data in the cloud.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/npc_mvr
 Project-URL: Issues, https://github.com/AllenInstitute/npc_mvr/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `npc_mvr-0.1.5/README.md` & `npc_mvr-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `npc_mvr-0.1.5/pyproject.toml` & `npc_mvr-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 requires-python = ">=3.9"
 dependencies = [
     "npc-io>=0.1.20",
     "npc-sync>=0.1.5",
     "opencv-python-headless>=4.9.0.80",
     "typing-extensions>=4.9.0",
 ]
-version = "0.1.5"
+version = "0.1.6"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
```

### Comparing `npc_mvr-0.1.5/src/npc_mvr/__init__.py` & `npc_mvr-0.1.6/src/npc_mvr/__init__.py`

 * *Files identical despite different names*

### Comparing `npc_mvr-0.1.5/src/npc_mvr/mvr.py` & `npc_mvr-0.1.6/src/npc_mvr/mvr.py`

 * *Files 0% similar despite different names*

```diff
@@ -506,24 +506,28 @@
     """
     videos = get_video_file_paths(*video_paths)
     jsons = get_video_info_file_paths(*video_paths)
     camera_to_video_path = {get_camera_name(path.stem): path for path in videos}
     camera_to_json_data = {
         get_camera_name(path.stem): get_video_info_data(path) for path in jsons
     }
-    correct_sync_line_names = get_camera_sync_line_name_mapping(
+    correct_sync_line_name_mapping = get_camera_sync_line_name_mapping(
         sync_path_or_dataset, *videos
     )
-    if tuple(correct_sync_line_names.keys()) != tuple(correct_sync_line_names.values()):
+    if tuple(
+        get_camera_name_on_sync(c) for c in correct_sync_line_name_mapping
+    ) != tuple(correct_sync_line_name_mapping.values()):
         logger.warning(
-            f"Camera lines are plugged into sync incorrectly - we'll accommodate for this, but if this is a recent session check the rig: {correct_sync_line_names}"
+            f"Camera lines are plugged into sync incorrectly - we'll accommodate for this, but if this is a recent session check the rig: {correct_sync_line_name_mapping}"
         )
     camera_exposing_times = get_cam_exposing_times_on_sync(sync_path_or_dataset)
     camera_exposing_times = {
-        camera: camera_exposing_times[get_camera_name(correct_sync_line_names[camera])]
+        camera: camera_exposing_times[
+            get_camera_name(correct_sync_line_name_mapping[camera])
+        ]
         for camera in camera_exposing_times
     }
     frame_times: dict[upath.UPath, npt.NDArray[np.floating]] = {}
     for camera in camera_exposing_times:
         if camera in camera_to_video_path:
             num_frames_in_video = get_total_frames_in_video(
                 camera_to_video_path[camera]
```

### Comparing `npc_mvr-0.1.5/src/npc_mvr.egg-info/PKG-INFO` & `npc_mvr-0.1.6/src/npc_mvr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npc-mvr
-Version: 0.1.5
+Version: 0.1.6
 Summary: Tools for reading raw video data from MindScope Neuropixels experiments, compatible with data in the cloud.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/npc_mvr
 Project-URL: Issues, https://github.com/AllenInstitute/npc_mvr/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

