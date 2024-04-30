# Comparing `tmp/ch9329-1.0.7.tar.gz` & `tmp/ch9329-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ch9329-1.0.7.tar", last modified: Sun Apr 28 13:40:57 2024, max compression
+gzip compressed data, was "ch9329-1.0.8.tar", last modified: Tue Apr 30 15:28:21 2024, max compression
```

## Comparing `ch9329-1.0.7.tar` & `ch9329-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:40:57.037489 ch9329-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-28 13:40:49.000000 ch9329-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-28 13:40:49.000000 ch9329-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-28 13:40:57.037489 ch9329-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-28 13:40:49.000000 ch9329-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:40:57.033489 ch9329-1.0.7/ch9329/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 13:40:49.000000 ch9329-1.0.7/ch9329/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-28 13:40:49.000000 ch9329-1.0.7/ch9329/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-28 13:40:49.000000 ch9329-1.0.7/ch9329/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13084 2024-04-28 13:40:49.000000 ch9329-1.0.7/ch9329/hid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-28 13:40:49.000000 ch9329-1.0.7/ch9329/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-28 13:40:49.000000 ch9329-1.0.7/ch9329/mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 13:40:49.000000 ch9329-1.0.7/ch9329/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-28 13:40:49.000000 ch9329-1.0.7/ch9329/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 13:40:57.033489 ch9329-1.0.7/ch9329.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-28 13:40:57.000000 ch9329-1.0.7/ch9329.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-28 13:40:57.000000 ch9329-1.0.7/ch9329.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 13:40:57.000000 ch9329-1.0.7/ch9329.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 13:40:57.000000 ch9329-1.0.7/ch9329.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-28 13:40:57.000000 ch9329-1.0.7/ch9329.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-28 13:40:49.000000 ch9329-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 13:40:57.037489 ch9329-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:28:21.601718 ch9329-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-30 15:28:12.000000 ch9329-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-30 15:28:12.000000 ch9329-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-30 15:28:21.601718 ch9329-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-30 15:28:12.000000 ch9329-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:28:21.601718 ch9329-1.0.8/ch9329/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:28:12.000000 ch9329-1.0.8/ch9329/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-30 15:28:12.000000 ch9329-1.0.8/ch9329/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-30 15:28:12.000000 ch9329-1.0.8/ch9329/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13242 2024-04-30 15:28:12.000000 ch9329-1.0.8/ch9329/hid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-30 15:28:12.000000 ch9329-1.0.8/ch9329/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-30 15:28:12.000000 ch9329-1.0.8/ch9329/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:28:12.000000 ch9329-1.0.8/ch9329/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-30 15:28:12.000000 ch9329-1.0.8/ch9329/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:28:21.601718 ch9329-1.0.8/ch9329.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-30 15:28:21.000000 ch9329-1.0.8/ch9329.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-30 15:28:21.000000 ch9329-1.0.8/ch9329.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:28:21.000000 ch9329-1.0.8/ch9329.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 15:28:21.000000 ch9329-1.0.8/ch9329.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 15:28:21.000000 ch9329-1.0.8/ch9329.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-30 15:28:12.000000 ch9329-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:28:21.601718 ch9329-1.0.8/setup.cfg
```

### Comparing `ch9329-1.0.7/LICENSE` & `ch9329-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.7/PKG-INFO` & `ch9329-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch9329
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python module to control ch9329
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `ch9329-1.0.7/README.md` & `ch9329-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.7/ch9329/config.py` & `ch9329-1.0.8/ch9329/config.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.7/ch9329/hid.py` & `ch9329-1.0.8/ch9329/hid.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,14 +250,18 @@
     "del": (HID_KEY_DELETE, None),
     "end": (HID_KEY_END, None),
     "page_down": (HID_KEY_PAGE_DOWN, None),
     "arrow_right": (HID_KEY_ARROW_RIGHT, None),
     "arrow_left": (HID_KEY_ARROW_LEFT, None),
     "arrow_down": (HID_KEY_ARROW_DOWN, None),
     "arrow_up": (HID_KEY_ARROW_UP, None),
+    "right": (HID_KEY_ARROW_RIGHT, None),
+    "left": (HID_KEY_ARROW_LEFT, None),
+    "down": (HID_KEY_ARROW_DOWN, None),
+    "up": (HID_KEY_ARROW_UP, None),
     "num_lock": (HID_KEY_NUM_LOCK, None),
     "keypad_divide": (HID_KEY_KEYPAD_DIVIDE, None),
     "keypad_multiply": (HID_KEY_KEYPAD_MULTIPLY, None),
     "keypad_subtract": (HID_KEY_KEYPAD_SUBTRACT, None),
     "keypad_add": (HID_KEY_KEYPAD_ADD, None),
     "keypad_enter": (HID_KEY_KEYPAD_ENTER, None),
     "keypad_1": (HID_KEY_KEYPAD_1, None),
```

### Comparing `ch9329-1.0.7/ch9329/keyboard.py` & `ch9329-1.0.8/ch9329/keyboard.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.7/ch9329/mouse.py` & `ch9329-1.0.8/ch9329/mouse.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.7/ch9329/utils.py` & `ch9329-1.0.8/ch9329/utils.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.7/ch9329.egg-info/PKG-INFO` & `ch9329-1.0.8/ch9329.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch9329
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python module to control ch9329
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `ch9329-1.0.7/pyproject.toml` & `ch9329-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ch9329"
-version = "1.0.7"
+version = "1.0.8"
 dependencies = ["pyserial"]
 requires-python = ">=3"
 authors = [{ name = "Pradish Bijukchhe", email = "pradish@sandbox.com.np" }]
 description = "Python module to control ch9329"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = []
```

