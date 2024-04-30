# Comparing `tmp/focuscreen-0.7.2.tar.gz` & `tmp/focuscreen-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "focuscreen-0.7.2.tar", last modified: Sat Apr 27 21:12:38 2024, max compression
+gzip compressed data, was "focuscreen-0.7.3.tar", last modified: Mon Apr 29 17:30:12 2024, max compression
```

## Comparing `focuscreen-0.7.2.tar` & `focuscreen-0.7.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:12:38.558293 focuscreen-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-27 21:12:38.558293 focuscreen-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-27 21:12:28.000000 focuscreen-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-27 21:12:28.000000 focuscreen-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 21:12:38.558293 focuscreen-0.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:12:38.554293 focuscreen-0.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:12:38.554293 focuscreen-0.7.2/src/focuscreen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:12:28.000000 focuscreen-0.7.2/src/focuscreen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-27 21:12:28.000000 focuscreen-0.7.2/src/focuscreen/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:12:38.554293 focuscreen-0.7.2/src/focuscreen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-27 21:12:38.000000 focuscreen-0.7.2/src/focuscreen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-27 21:12:38.000000 focuscreen-0.7.2/src/focuscreen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 21:12:38.000000 focuscreen-0.7.2/src/focuscreen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-27 21:12:38.000000 focuscreen-0.7.2/src/focuscreen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 21:12:38.000000 focuscreen-0.7.2/src/focuscreen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:30:12.478626 focuscreen-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-29 17:30:12.478626 focuscreen-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-29 17:30:01.000000 focuscreen-0.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-29 17:30:01.000000 focuscreen-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 17:30:12.478626 focuscreen-0.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:30:12.478626 focuscreen-0.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:30:12.478626 focuscreen-0.7.3/src/focuscreen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:30:01.000000 focuscreen-0.7.3/src/focuscreen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-29 17:30:01.000000 focuscreen-0.7.3/src/focuscreen/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-29 17:30:01.000000 focuscreen-0.7.3/src/focuscreen/focus_region_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:30:12.478626 focuscreen-0.7.3/src/focuscreen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-29 17:30:12.000000 focuscreen-0.7.3/src/focuscreen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-29 17:30:12.000000 focuscreen-0.7.3/src/focuscreen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:30:12.000000 focuscreen-0.7.3/src/focuscreen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-29 17:30:12.000000 focuscreen-0.7.3/src/focuscreen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 17:30:12.000000 focuscreen-0.7.3/src/focuscreen.egg-info/top_level.txt
```

### Comparing `focuscreen-0.7.2/PKG-INFO` & `focuscreen-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: focuscreen
-Version: 0.7.2
+Version: 0.7.3
 Summary: Snap screen by focusing on mouse and keyboard events
 Author: Hansimov
 Project-URL: Homepage, https://github.com/Hansimov/focuscreen
 Project-URL: Issues, https://github.com/Hansimov/focuscreen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Requires-Dist: mss
 Requires-Dist: numpy
 Requires-Dist: opencv-python
 Requires-Dist: Pillow
 Requires-Dist: pynput
 Requires-Dist: tclogger
 
-# focuscreen
+# FocuScreen
 Snap screen by focusing on mouse and keyboard events.
 
 ![](https://img.shields.io/pypi/v/focuscreen?label=focuscreen&color=blue&cacheSeconds=60)
 
 ## Install
 ```sh
 pip install --upgrade focuscreen
```

### Comparing `focuscreen-0.7.2/pyproject.toml` & `focuscreen-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "focuscreen"
-version = "0.7.2"
+version = "0.7.3"
 authors = [
     { name="Hansimov" },
 ]
 description = "Snap screen by focusing on mouse and keyboard events"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `focuscreen-0.7.2/src/focuscreen/app.py` & `focuscreen-0.7.3/src/focuscreen/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import cv2
 import numpy as np
 
 from mss import mss
 from pynput import mouse
 from tclogger import logger
 
+from .focus_region_updater import FocusRegionUpdater
+
 
 class FocuScreenApp:
     def __init__(self):
         self.window_name = "FocuScreen"
-        self.ratio = 1.5
+        self.ratio = 2
         self.window_width = int(1920 / self.ratio)
         self.window_height = int(1080 / self.ratio)
         self.mouse_x, self.mouse_y = 0, 0
+        self.focus_region_updater = FocusRegionUpdater()
         self.get_monitor_bounds()
         self.setup_window()
 
     def setup_window(self):
         cv2.namedWindow(self.window_name, cv2.WINDOW_NORMAL)
         cv2.resizeWindow(self.window_name, self.window_width, self.window_height)
 
@@ -53,25 +56,28 @@
             )
             self.monitor_top_bound = combined_monitor["top"]
             self.monitor_bottom_bound = (
                 combined_monitor["top"] + combined_monitor["height"]
             )
 
     def calc_focus_region(self):
-        """calculate the region of the screen to capture based on focus"""
+        """calculate focus region to capture"""
+        self.focus_x, self.focus_y = self.focus_region_updater.calc_focus_center(
+            self.mouse_x, self.mouse_y
+        )
         self.region_x1 = min(
             max(
-                self.mouse_x - self.window_width // 2,
+                self.focus_x - self.window_width // 2,
                 self.monitor_left_bound,
             ),
             self.monitor_right_bound - self.window_width,
         )
         self.region_y1 = min(
             max(
-                self.mouse_y - self.window_height // 2,
+                self.focus_y - self.window_height // 2,
                 self.monitor_top_bound,
             ),
             self.monitor_bottom_bound - self.window_height,
         )
 
         self.mouse_region = {
             "top": self.region_y1,
```

### Comparing `focuscreen-0.7.2/src/focuscreen.egg-info/PKG-INFO` & `focuscreen-0.7.3/src/focuscreen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: focuscreen
-Version: 0.7.2
+Version: 0.7.3
 Summary: Snap screen by focusing on mouse and keyboard events
 Author: Hansimov
 Project-URL: Homepage, https://github.com/Hansimov/focuscreen
 Project-URL: Issues, https://github.com/Hansimov/focuscreen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Requires-Dist: mss
 Requires-Dist: numpy
 Requires-Dist: opencv-python
 Requires-Dist: Pillow
 Requires-Dist: pynput
 Requires-Dist: tclogger
 
-# focuscreen
+# FocuScreen
 Snap screen by focusing on mouse and keyboard events.
 
 ![](https://img.shields.io/pypi/v/focuscreen?label=focuscreen&color=blue&cacheSeconds=60)
 
 ## Install
 ```sh
 pip install --upgrade focuscreen
```

