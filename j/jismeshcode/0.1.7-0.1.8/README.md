# Comparing `tmp/jismeshcode-0.1.7.tar.gz` & `tmp/jismeshcode-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jismeshcode-0.1.7.tar", max compression
+gzip compressed data, was "jismeshcode-0.1.8.tar", max compression
```

## Comparing `jismeshcode-0.1.7.tar` & `jismeshcode-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1249 2023-11-07 12:58:24.696554 jismeshcode-0.1.7/README.md
--rw-r--r--   0        0        0       35 2023-10-29 08:49:09.100206 jismeshcode-0.1.7/jismeshcode/__init__.py
--rw-r--r--   0        0        0     7352 2023-11-03 15:20:51.051442 jismeshcode-0.1.7/jismeshcode/jismeshcode.py
--rw-r--r--   0        0        0      322 2023-11-07 12:58:34.816554 jismeshcode-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1685 1970-01-01 00:00:00.000000 jismeshcode-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1249 2024-04-30 13:23:14.100290 jismeshcode-0.1.8/README.md
+-rw-r--r--   0        0        0       35 2024-04-30 13:23:14.100290 jismeshcode-0.1.8/jismeshcode/__init__.py
+-rw-r--r--   0        0        0     7352 2024-04-30 13:54:09.140290 jismeshcode-0.1.8/jismeshcode/jismeshcode.py
+-rw-r--r--   0        0        0      322 2024-04-30 14:05:03.850290 jismeshcode-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1736 1970-01-01 00:00:00.000000 jismeshcode-0.1.8/PKG-INFO
```

### Comparing `jismeshcode-0.1.7/README.md` & `jismeshcode-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `jismeshcode-0.1.7/jismeshcode/jismeshcode.py` & `jismeshcode-0.1.8/jismeshcode/jismeshcode.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     if mesh_level >= 8:  # Apply adjustments for third order mesh
         delta_latitude = 1/120 # 30 seconds in degrees
         delta_longitude = 3/240 # 45 seconds in degrees
         south_latitude += int(meshcode[6]) * delta_latitude
         west_longitude += int(meshcode[7]) * delta_longitude
         
-    if mesh_level == 9:  # Apply adjustments for fourth order or two times mesh
+    if mesh_level >= 9:  # Apply adjustments for fourth order or two times mesh
         if not 1 <= int(meshcode[8]) <= 5:
             raise ValueError(f"meshcode number error last number:The range of number in last number of forth meshcode must be from 1 to 5")
         
         if not int(meshcode[8]) == 5: # Apply adjustments for fourth order mesh
             delta_latitude = 15/3600 # 15 seconds in degrees
             delta_longitude = 22.5/3600 # 22.5 seconds in degrees
             south_latitude += [None, 0, 0, delta_latitude, delta_latitude][int(meshcode[8])]
```

### Comparing `jismeshcode-0.1.7/PKG-INFO` & `jismeshcode-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: jismeshcode
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: itch
 Author-email: marine.taichi@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # jismeshcode
 
 [GitHub](https://github.com/itch0323/jismeshcode)
 
 [English version](README_en.md)
```

