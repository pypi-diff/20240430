# Comparing `tmp/gym_jiminy_rllib-1.8.5-py3-none-any.whl.zip` & `tmp/gym_jiminy_rllib-1.8.5.post1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 25704 bytes, number of entries: 10
--rw-r--r--  2.0 unx      264 b- defN 24-Apr-28 20:51 gym_jiminy/rllib/__init__.py
--rw-r--r--  2.0 unx     3162 b- defN 24-Apr-28 20:51 gym_jiminy/rllib/callbacks.py
--rw-r--r--  2.0 unx    12290 b- defN 24-Apr-28 20:51 gym_jiminy/rllib/curriculum.py
--rw-r--r--  2.0 unx    28124 b- defN 24-Apr-28 20:51 gym_jiminy/rllib/ppo.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-28 20:51 gym_jiminy/rllib/py.typed
--rw-r--r--  2.0 unx    46565 b- defN 24-Apr-28 20:51 gym_jiminy/rllib/utilities.py
--rw-r--r--  2.0 unx      954 b- defN 24-Apr-28 20:52 gym_jiminy_rllib-1.8.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-28 20:52 gym_jiminy_rllib-1.8.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-28 20:52 gym_jiminy_rllib-1.8.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      838 b- defN 24-Apr-28 20:52 gym_jiminy_rllib-1.8.5.dist-info/RECORD
-10 files, 92300 bytes uncompressed, 24266 bytes compressed:  73.7%
+Zip file size: 25761 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      264 b- defN 24-Apr-30 00:34 gym_jiminy/rllib/__init__.py
+-rw-r--r--  2.0 unx     3162 b- defN 24-Apr-30 00:34 gym_jiminy/rllib/callbacks.py
+-rw-r--r--  2.0 unx    12290 b- defN 24-Apr-30 00:34 gym_jiminy/rllib/curriculum.py
+-rw-r--r--  2.0 unx    28124 b- defN 24-Apr-30 00:34 gym_jiminy/rllib/ppo.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-30 00:34 gym_jiminy/rllib/py.typed
+-rw-r--r--  2.0 unx    46565 b- defN 24-Apr-30 00:34 gym_jiminy/rllib/utilities.py
+-rw-r--r--  2.0 unx      966 b- defN 24-Apr-30 00:35 gym_jiminy_rllib-1.8.5.post1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 00:35 gym_jiminy_rllib-1.8.5.post1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-30 00:35 gym_jiminy_rllib-1.8.5.post1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      862 b- defN 24-Apr-30 00:35 gym_jiminy_rllib-1.8.5.post1.dist-info/RECORD
+10 files, 92336 bytes uncompressed, 24275 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: gym_jiminy/rllib/py.typed
 Comment: 
 
 Filename: gym_jiminy/rllib/utilities.py
 Comment: 
 
-Filename: gym_jiminy_rllib-1.8.5.dist-info/METADATA
+Filename: gym_jiminy_rllib-1.8.5.post1.dist-info/METADATA
 Comment: 
 
-Filename: gym_jiminy_rllib-1.8.5.dist-info/WHEEL
+Filename: gym_jiminy_rllib-1.8.5.post1.dist-info/WHEEL
 Comment: 
 
-Filename: gym_jiminy_rllib-1.8.5.dist-info/top_level.txt
+Filename: gym_jiminy_rllib-1.8.5.post1.dist-info/top_level.txt
 Comment: 
 
-Filename: gym_jiminy_rllib-1.8.5.dist-info/RECORD
+Filename: gym_jiminy_rllib-1.8.5.post1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gym_jiminy_rllib-1.8.5.dist-info/METADATA` & `gym_jiminy_rllib-1.8.5.post1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-jiminy-rllib
-Version: 1.8.5
+Version: 1.8.5.post1
 Summary: Specialized Reinforcement learning toolbox based on Ray RLlib for Gym Jiminy.
 Author: Alexis Duburcq
 Author-email: alexis.duburcq@gmail.com
 Maintainer: Alexis Duburcq
 License: MIT
 Keywords: reinforcement-learning robotics gym jiminy
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,12 +13,12 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8,<3.12
-Requires-Dist: gym-jiminy ~=1.8.5
+Requires-Dist: gym-jiminy ~=1.8.5.post1
 Requires-Dist: ray[rllib] ~=2.9.0
 Requires-Dist: tensorboardX
 Requires-Dist: plotext >=5.0.0
```

