# Comparing `tmp/npc_mvr-0.1.4.tar.gz` & `tmp/npc_mvr-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npc_mvr-0.1.4.tar", last modified: Tue Apr 23 19:10:13 2024, max compression
+gzip compressed data, was "npc_mvr-0.1.5.tar", last modified: Mon Apr 29 22:04:47 2024, max compression
```

## Comparing `npc_mvr-0.1.4.tar` & `npc_mvr-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:13.271785 npc_mvr-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-23 19:09:40.000000 npc_mvr-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-23 19:10:13.271785 npc_mvr-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-23 19:09:40.000000 npc_mvr-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-23 19:10:10.000000 npc_mvr-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:10:13.271785 npc_mvr-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:13.271785 npc_mvr-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:13.271785 npc_mvr-0.1.4/src/npc_mvr/
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-23 19:09:40.000000 npc_mvr-0.1.4/src/npc_mvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35353 2024-04-23 19:10:07.000000 npc_mvr-0.1.4/src/npc_mvr/mvr.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:09:40.000000 npc_mvr-0.1.4/src/npc_mvr/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:13.271785 npc_mvr-0.1.4/src/npc_mvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-23 19:10:13.000000 npc_mvr-0.1.4/src/npc_mvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-23 19:10:13.000000 npc_mvr-0.1.4/src/npc_mvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:10:13.000000 npc_mvr-0.1.4/src/npc_mvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-23 19:10:13.000000 npc_mvr-0.1.4/src/npc_mvr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 19:10:13.000000 npc_mvr-0.1.4/src/npc_mvr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:10:13.271785 npc_mvr-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 19:09:40.000000 npc_mvr-0.1.4/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:04:47.108709 npc_mvr-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-29 22:04:15.000000 npc_mvr-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-29 22:04:47.108709 npc_mvr-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-29 22:04:15.000000 npc_mvr-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-29 22:04:44.000000 npc_mvr-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 22:04:47.108709 npc_mvr-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:04:47.104709 npc_mvr-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:04:47.108709 npc_mvr-0.1.5/src/npc_mvr/
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-29 22:04:15.000000 npc_mvr-0.1.5/src/npc_mvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35080 2024-04-29 22:04:15.000000 npc_mvr-0.1.5/src/npc_mvr/mvr.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:04:15.000000 npc_mvr-0.1.5/src/npc_mvr/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:04:47.108709 npc_mvr-0.1.5/src/npc_mvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-29 22:04:47.000000 npc_mvr-0.1.5/src/npc_mvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-29 22:04:47.000000 npc_mvr-0.1.5/src/npc_mvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:04:47.000000 npc_mvr-0.1.5/src/npc_mvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-29 22:04:47.000000 npc_mvr-0.1.5/src/npc_mvr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 22:04:47.000000 npc_mvr-0.1.5/src/npc_mvr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:04:47.108709 npc_mvr-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 22:04:15.000000 npc_mvr-0.1.5/tests/test_core.py
```

### Comparing `npc_mvr-0.1.4/LICENSE` & `npc_mvr-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `npc_mvr-0.1.4/PKG-INFO` & `npc_mvr-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npc-mvr
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tools for reading raw video data from MindScope Neuropixels experiments, compatible with data in the cloud.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/npc_mvr
 Project-URL: Issues, https://github.com/AllenInstitute/npc_mvr/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `npc_mvr-0.1.4/README.md` & `npc_mvr-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `npc_mvr-0.1.4/pyproject.toml` & `npc_mvr-0.1.5/pyproject.toml`

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
-version = "0.1.4"
+version = "0.1.5"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
```

### Comparing `npc_mvr-0.1.4/src/npc_mvr/__init__.py` & `npc_mvr-0.1.5/src/npc_mvr/__init__.py`

 * *Files identical despite different names*

### Comparing `npc_mvr-0.1.4/src/npc_mvr/mvr.py` & `npc_mvr-0.1.5/src/npc_mvr/mvr.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,18 +459,15 @@
             key=lambda line: abs(
                 expected_duration - actual_exposure_fingerprint_durations[line]
             ),
         )
         expected_to_actual_line_mapping[get_camera_name(sync_camera_name)] = (
             get_camera_name_on_sync(actual_line)
         )
-        readout_line = f"{sync_camera_name}_cam_frame_readout"
-        assert (a := lines_sorted_by_start_time.index(exposing_line)) + 1 == (
-            b := lines_sorted_by_start_time.index(readout_line)
-        ), f"Expected {readout_line} (start index {a}) to start immediately after {exposing_line} (start index {b}) - assumption is incorrect (are lines connected to sync separately?)"
+        # readout line is coupled to exposing line (ie. they share the same plug) so the same mapping applies to both
     return expected_to_actual_line_mapping
 
 
 def get_video_frame_times(
     sync_path_or_dataset: npc_io.PathLike | npc_sync.SyncDataset,
     *video_paths: npc_io.PathLike,
     apply_correction: bool = True,
```

### Comparing `npc_mvr-0.1.4/src/npc_mvr.egg-info/PKG-INFO` & `npc_mvr-0.1.5/src/npc_mvr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npc-mvr
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tools for reading raw video data from MindScope Neuropixels experiments, compatible with data in the cloud.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitue.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/npc_mvr
 Project-URL: Issues, https://github.com/AllenInstitute/npc_mvr/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

