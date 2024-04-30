# Comparing `tmp/python-MotionMount-1.0.0.tar.gz` & `tmp/python_motionmount-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-MotionMount-1.0.0.tar", last modified: Mon Jan 22 15:08:27 2024, max compression
+gzip compressed data, was "python_motionmount-1.0.1.tar", last modified: Tue Apr 30 11:50:17 2024, max compression
```

## Comparing `python-MotionMount-1.0.0.tar` & `python_motionmount-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 remcopoelstra   (501) staff       (20)        0 2024-01-22 15:08:27.485103 python-MotionMount-1.0.0/
--rw-r--r--   0 remcopoelstra   (501) staff       (20)     1073 2023-10-27 08:23:06.000000 python-MotionMount-1.0.0/LICENSE.txt
--rw-r--r--   0 remcopoelstra   (501) staff       (20)     3149 2024-01-22 15:08:27.484952 python-MotionMount-1.0.0/PKG-INFO
--rw-r--r--   0 remcopoelstra   (501) staff       (20)     1464 2023-10-27 08:23:06.000000 python-MotionMount-1.0.0/README.md
--rw-r--r--   0 remcopoelstra   (501) staff       (20)       85 2023-10-27 08:23:06.000000 python-MotionMount-1.0.0/pyproject.toml
--rw-r--r--   0 remcopoelstra   (501) staff       (20)      852 2024-01-22 15:08:27.485678 python-MotionMount-1.0.0/setup.cfg
-drwxr-xr-x   0 remcopoelstra   (501) staff       (20)        0 2024-01-22 15:08:27.480357 python-MotionMount-1.0.0/src/
-drwxr-xr-x   0 remcopoelstra   (501) staff       (20)        0 2024-01-22 15:08:27.482743 python-MotionMount-1.0.0/src/motionmount/
--rw-r--r--   0 remcopoelstra   (501) staff       (20)      203 2023-10-27 08:23:06.000000 python-MotionMount-1.0.0/src/motionmount/__init__.py
--rw-r--r--   0 remcopoelstra   (501) staff       (20)    16803 2024-01-22 14:58:47.000000 python-MotionMount-1.0.0/src/motionmount/motionmount.py
--rw-r--r--   0 remcopoelstra   (501) staff       (20)        0 2023-11-06 15:45:57.000000 python-MotionMount-1.0.0/src/motionmount/py.typed
-drwxr-xr-x   0 remcopoelstra   (501) staff       (20)        0 2024-01-22 15:08:27.484446 python-MotionMount-1.0.0/src/python_MotionMount.egg-info/
--rw-r--r--   0 remcopoelstra   (501) staff       (20)     3149 2024-01-22 15:08:27.000000 python-MotionMount-1.0.0/src/python_MotionMount.egg-info/PKG-INFO
--rw-r--r--   0 remcopoelstra   (501) staff       (20)      314 2024-01-22 15:08:27.000000 python-MotionMount-1.0.0/src/python_MotionMount.egg-info/SOURCES.txt
--rw-r--r--   0 remcopoelstra   (501) staff       (20)        1 2024-01-22 15:08:27.000000 python-MotionMount-1.0.0/src/python_MotionMount.egg-info/dependency_links.txt
--rw-r--r--   0 remcopoelstra   (501) staff       (20)       12 2024-01-22 15:08:27.000000 python-MotionMount-1.0.0/src/python_MotionMount.egg-info/top_level.txt
+drwxr-xr-x   0 remcopoelstra   (501) staff       (20)        0 2024-04-30 11:50:17.002947 python_motionmount-1.0.1/
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)     1073 2023-10-27 08:23:06.000000 python_motionmount-1.0.1/LICENSE.txt
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)     3204 2024-04-30 11:50:17.002781 python_motionmount-1.0.1/PKG-INFO
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)     1521 2024-04-30 11:48:02.000000 python_motionmount-1.0.1/README.md
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)       85 2023-10-27 08:23:06.000000 python_motionmount-1.0.1/pyproject.toml
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)      852 2024-04-30 11:50:17.003750 python_motionmount-1.0.1/setup.cfg
+drwxr-xr-x   0 remcopoelstra   (501) staff       (20)        0 2024-04-30 11:50:16.997402 python_motionmount-1.0.1/src/
+drwxr-xr-x   0 remcopoelstra   (501) staff       (20)        0 2024-04-30 11:50:17.000400 python_motionmount-1.0.1/src/motionmount/
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)      203 2023-10-27 08:23:06.000000 python_motionmount-1.0.1/src/motionmount/__init__.py
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)    16803 2024-04-30 11:48:02.000000 python_motionmount-1.0.1/src/motionmount/motionmount.py
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)        0 2023-11-06 15:45:57.000000 python_motionmount-1.0.1/src/motionmount/py.typed
+drwxr-xr-x   0 remcopoelstra   (501) staff       (20)        0 2024-04-30 11:50:17.002240 python_motionmount-1.0.1/src/python_MotionMount.egg-info/
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)     3204 2024-04-30 11:50:16.000000 python_motionmount-1.0.1/src/python_MotionMount.egg-info/PKG-INFO
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)      314 2024-04-30 11:50:16.000000 python_motionmount-1.0.1/src/python_MotionMount.egg-info/SOURCES.txt
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)        1 2024-04-30 11:50:16.000000 python_motionmount-1.0.1/src/python_MotionMount.egg-info/dependency_links.txt
+-rw-r--r--   0 remcopoelstra   (501) staff       (20)       12 2024-04-30 11:50:16.000000 python_motionmount-1.0.1/src/python_MotionMount.egg-info/top_level.txt
```

### Comparing `python-MotionMount-1.0.0/LICENSE.txt` & `python_motionmount-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-MotionMount-1.0.0/PKG-INFO` & `python_motionmount-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-MotionMount
-Version: 1.0.0
+Version: 1.0.1
 Summary: Control your MotionMount Signature TVM7675 Pro using Python
 Home-page: https://github.com/vogelsproducts/python-MotionMount
 Author: Remco Poelstra
 Author-email: r.poelstra@vogels.com
 Project-URL: Bug Tracker, https://github.com/vogelsproducts/python-MotionMount/issues
 Project-URL: repository, https://github.com/vogelsproducts/python-MotionMount
 Classifier: Programming Language :: Python :: 3
@@ -53,14 +53,16 @@
     asyncio.run(main())
 ```
 
 To get the IP address of the MotionMount you can use [pyzeroconf](https://github.com/paulsm/pyzeroconf) or you can use a manual tool like `dns-sd` in the macOS Terminal or a GUI tool like [Discovery](https://apps.apple.com/nl/app/discovery-dns-sd-browser/id1381004916?mt=12) (macOS) or [Bonjour Browser](https://hobbyistsoftware.com/bonjourbrowser) (Windows)
   
 A simple example using `pyzeroconf` is included in the `examples` folder.
     
+# Changelog
+1.0.1: - Fix bug in allowed preset indices
 
 MIT License
 
 Copyright (c) 2023 Vogel's Products
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `python-MotionMount-1.0.0/README.md` & `python_motionmount-1.0.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -37,7 +37,9 @@
     asyncio.run(main())
 ```
 
 To get the IP address of the MotionMount you can use [pyzeroconf](https://github.com/paulsm/pyzeroconf) or you can use a manual tool like `dns-sd` in the macOS Terminal or a GUI tool like [Discovery](https://apps.apple.com/nl/app/discovery-dns-sd-browser/id1381004916?mt=12) (macOS) or [Bonjour Browser](https://hobbyistsoftware.com/bonjourbrowser) (Windows)
   
 A simple example using `pyzeroconf` is included in the `examples` folder.
     
+# Changelog
+1.0.1: - Fix bug in allowed preset indices
```

### Comparing `python-MotionMount-1.0.0/setup.cfg` & `python_motionmount-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-MotionMount
-version = 1.0.0
+version = 1.0.1
 author = Remco Poelstra
 author_email = r.poelstra@vogels.com
 description = Control your MotionMount Signature TVM7675 Pro using Python
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/vogelsproducts/python-MotionMount
 project_urls =
```

### Comparing `python-MotionMount-1.0.0/src/motionmount/motionmount.py` & `python_motionmount-1.0.1/src/motionmount/motionmount.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,21 +310,21 @@
         
     async def go_to_preset(self, position: int):
         """
         Go to a preset position.
         Preset 0 is the (fixed) Wall position.
 
         Args:
-            position (int): The preset position to go to (0 - 9).
+            position (int): The preset position to go to (0 - 7).
 
         Raises:
             ValueError: If the position is out of range.
         """
-        if position < 0 or position > 9:
-            raise ValueError("position must be in the range [0...9]")
+        if position < 0 or position > 7:
+            raise ValueError("position must be in the range [0...7]")
 
         await self._request(Request(f"mount/preset/index = {position}", MotionMountValueType.Void))
 
     async def go_to_position(self, extension: int, turn: int):
         """
         Go to a specific position.
```

### Comparing `python-MotionMount-1.0.0/src/python_MotionMount.egg-info/PKG-INFO` & `python_motionmount-1.0.1/src/python_MotionMount.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-MotionMount
-Version: 1.0.0
+Version: 1.0.1
 Summary: Control your MotionMount Signature TVM7675 Pro using Python
 Home-page: https://github.com/vogelsproducts/python-MotionMount
 Author: Remco Poelstra
 Author-email: r.poelstra@vogels.com
 Project-URL: Bug Tracker, https://github.com/vogelsproducts/python-MotionMount/issues
 Project-URL: repository, https://github.com/vogelsproducts/python-MotionMount
 Classifier: Programming Language :: Python :: 3
@@ -53,14 +53,16 @@
     asyncio.run(main())
 ```
 
 To get the IP address of the MotionMount you can use [pyzeroconf](https://github.com/paulsm/pyzeroconf) or you can use a manual tool like `dns-sd` in the macOS Terminal or a GUI tool like [Discovery](https://apps.apple.com/nl/app/discovery-dns-sd-browser/id1381004916?mt=12) (macOS) or [Bonjour Browser](https://hobbyistsoftware.com/bonjourbrowser) (Windows)
   
 A simple example using `pyzeroconf` is included in the `examples` folder.
     
+# Changelog
+1.0.1: - Fix bug in allowed preset indices
 
 MIT License
 
 Copyright (c) 2023 Vogel's Products
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

