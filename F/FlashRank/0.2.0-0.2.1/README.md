# Comparing `tmp/FlashRank-0.2.0.tar.gz` & `tmp/FlashRank-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlashRank-0.2.0.tar", last modified: Tue Mar 19 00:46:03 2024, max compression
+gzip compressed data, was "FlashRank-0.2.1.tar", last modified: Tue Apr 30 09:27:38 2024, max compression
```

## Comparing `FlashRank-0.2.0.tar` & `FlashRank-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-03-19 00:46:03.805556 FlashRank-0.2.0/
-drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-03-19 00:46:03.804123 FlashRank-0.2.0/FlashRank.egg-info/
--rw-r--r--   0 prithivida   (501) staff       (20)    10125 2024-03-19 00:46:03.000000 FlashRank-0.2.0/FlashRank.egg-info/PKG-INFO
--rw-r--r--   0 prithivida   (501) staff       (20)      273 2024-03-19 00:46:03.000000 FlashRank-0.2.0/FlashRank.egg-info/SOURCES.txt
--rw-r--r--   0 prithivida   (501) staff       (20)        1 2024-03-19 00:46:03.000000 FlashRank-0.2.0/FlashRank.egg-info/dependency_links.txt
--rw-r--r--   0 prithivida   (501) staff       (20)       43 2024-03-19 00:46:03.000000 FlashRank-0.2.0/FlashRank.egg-info/requires.txt
--rw-r--r--   0 prithivida   (501) staff       (20)       10 2024-03-19 00:46:03.000000 FlashRank-0.2.0/FlashRank.egg-info/top_level.txt
--rw-r--r--   0 prithivida   (501) staff       (20)    11357 2023-12-04 14:24:33.000000 FlashRank-0.2.0/LICENSE
--rw-r--r--   0 prithivida   (501) staff       (20)    10125 2024-03-19 00:46:03.805383 FlashRank-0.2.0/PKG-INFO
--rw-r--r--   0 prithivida   (501) staff       (20)     9604 2024-03-19 00:44:26.000000 FlashRank-0.2.0/README.md
-drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-03-19 00:46:03.805030 FlashRank-0.2.0/flashrank/
--rw-r--r--   0 prithivida   (501) staff       (20)      534 2024-03-19 00:44:52.000000 FlashRank-0.2.0/flashrank/Config.py
--rw-r--r--   0 prithivida   (501) staff       (20)     6093 2024-01-29 14:51:57.000000 FlashRank-0.2.0/flashrank/Ranker.py
--rw-r--r--   0 prithivida   (501) staff       (20)    10457 2023-12-13 12:36:57.000000 FlashRank-0.2.0/flashrank/Rankerb.py
--rw-r--r--   0 prithivida   (501) staff       (20)       41 2023-12-13 12:36:21.000000 FlashRank-0.2.0/flashrank/__init__.py
--rw-r--r--   0 prithivida   (501) staff       (20)       38 2024-03-19 00:46:03.805599 FlashRank-0.2.0/setup.cfg
--rw-r--r--   0 prithivida   (501) staff       (20)      819 2024-03-19 00:44:21.000000 FlashRank-0.2.0/setup.py
+drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-30 09:27:38.722456 FlashRank-0.2.1/
+drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-30 09:27:38.720617 FlashRank-0.2.1/FlashRank.egg-info/
+-rw-r--r--   0 prithivida   (501) staff       (20)    10278 2024-04-30 09:27:38.000000 FlashRank-0.2.1/FlashRank.egg-info/PKG-INFO
+-rw-r--r--   0 prithivida   (501) staff       (20)      294 2024-04-30 09:27:38.000000 FlashRank-0.2.1/FlashRank.egg-info/SOURCES.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)        1 2024-04-30 09:27:38.000000 FlashRank-0.2.1/FlashRank.egg-info/dependency_links.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)       43 2024-04-30 09:27:38.000000 FlashRank-0.2.1/FlashRank.egg-info/requires.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)       10 2024-04-30 09:27:38.000000 FlashRank-0.2.1/FlashRank.egg-info/top_level.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)    11357 2023-12-04 14:24:33.000000 FlashRank-0.2.1/LICENSE
+-rw-r--r--   0 prithivida   (501) staff       (20)    10278 2024-04-30 09:27:38.722277 FlashRank-0.2.1/PKG-INFO
+-rw-r--r--   0 prithivida   (501) staff       (20)     9757 2024-03-19 01:23:34.000000 FlashRank-0.2.1/README.md
+drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-30 09:27:38.721979 FlashRank-0.2.1/flashrank/
+-rw-r--r--   0 prithivida   (501) staff       (20)      608 2024-03-19 00:50:27.000000 FlashRank-0.2.1/flashrank/Config.py
+-rw-r--r--   0 prithivida   (501) staff       (20)     7193 2024-04-30 09:24:47.000000 FlashRank-0.2.1/flashrank/Ranker.py
+-rw-r--r--   0 prithivida   (501) staff       (20)    10457 2023-12-13 12:36:57.000000 FlashRank-0.2.1/flashrank/Rankerb.py
+-rw-r--r--   0 prithivida   (501) staff       (20)     6093 2024-01-29 14:51:57.000000 FlashRank-0.2.1/flashrank/Rankerc.py
+-rw-r--r--   0 prithivida   (501) staff       (20)       41 2024-04-30 09:25:26.000000 FlashRank-0.2.1/flashrank/__init__.py
+-rw-r--r--   0 prithivida   (501) staff       (20)       38 2024-04-30 09:27:38.722492 FlashRank-0.2.1/setup.cfg
+-rw-r--r--   0 prithivida   (501) staff       (20)      819 2024-04-30 09:26:14.000000 FlashRank-0.2.1/setup.py
```

### Comparing `FlashRank-0.2.0/FlashRank.egg-info/PKG-INFO` & `FlashRank-0.2.1/FlashRank.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: FlashRank
-Version: 0.2.0
+Version: 0.2.1
 Summary: Ultra lite & Super fast SoTA cross-encoder based re-ranking for your search & retrieval pipelines.
 Home-page: https://github.com/PrithivirajDamodaran/FlashRank
 Author: Prithivi Da
 Author-email: 
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # [IMPORTANT UPDATE]
 
-*A clone library called **SwiftRank is pointing to our model buckets, we are working on a interim solution to avoid this stealing**. Thank you for patience and understanding.*
+~~*A clone library called **SwiftRank is pointing to our model buckets, we are working on a interim solution to avoid this stealing**. Thank you for patience and understanding.*~~
+
+This issue is resolved, the models are in HF now. **please upgrade to continue** pip install -U flashrank. Thank you for patience and understanding
 
 # 🏎️ FlashRank
 Ultra-lite &amp; Super-fast Python library to add re-ranking to your existing search &amp; retrieval pipelines. It is based on SoTA cross-encoders, with gratitude to all the model owners.
 
 1. ⚡ **Ultra-lite**: 
     - **No Torch or Transformers** needed. Runs on CPU.
     - Boasts the **tiniest reranking model in the world, ~4MB**.
```

### Comparing `FlashRank-0.2.0/LICENSE` & `FlashRank-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FlashRank-0.2.0/PKG-INFO` & `FlashRank-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: FlashRank
-Version: 0.2.0
+Version: 0.2.1
 Summary: Ultra lite & Super fast SoTA cross-encoder based re-ranking for your search & retrieval pipelines.
 Home-page: https://github.com/PrithivirajDamodaran/FlashRank
 Author: Prithivi Da
 Author-email: 
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # [IMPORTANT UPDATE]
 
-*A clone library called **SwiftRank is pointing to our model buckets, we are working on a interim solution to avoid this stealing**. Thank you for patience and understanding.*
+~~*A clone library called **SwiftRank is pointing to our model buckets, we are working on a interim solution to avoid this stealing**. Thank you for patience and understanding.*~~
+
+This issue is resolved, the models are in HF now. **please upgrade to continue** pip install -U flashrank. Thank you for patience and understanding
 
 # 🏎️ FlashRank
 Ultra-lite &amp; Super-fast Python library to add re-ranking to your existing search &amp; retrieval pipelines. It is based on SoTA cross-encoders, with gratitude to all the model owners.
 
 1. ⚡ **Ultra-lite**: 
     - **No Torch or Transformers** needed. Runs on CPU.
     - Boasts the **tiniest reranking model in the world, ~4MB**.
```

### Comparing `FlashRank-0.2.0/README.md` & `FlashRank-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # [IMPORTANT UPDATE]
 
-*A clone library called **SwiftRank is pointing to our model buckets, we are working on a interim solution to avoid this stealing**. Thank you for patience and understanding.*
+~~*A clone library called **SwiftRank is pointing to our model buckets, we are working on a interim solution to avoid this stealing**. Thank you for patience and understanding.*~~
+
+This issue is resolved, the models are in HF now. **please upgrade to continue** pip install -U flashrank. Thank you for patience and understanding
 
 # 🏎️ FlashRank
 Ultra-lite &amp; Super-fast Python library to add re-ranking to your existing search &amp; retrieval pipelines. It is based on SoTA cross-encoders, with gratitude to all the model owners.
 
 1. ⚡ **Ultra-lite**: 
     - **No Torch or Transformers** needed. Runs on CPU.
     - Boasts the **tiniest reranking model in the world, ~4MB**.
```

### Comparing `FlashRank-0.2.0/flashrank/Ranker.py` & `FlashRank-0.2.1/flashrank/Rankerc.py`

 * *Files identical despite different names*

### Comparing `FlashRank-0.2.0/flashrank/Rankerb.py` & `FlashRank-0.2.1/flashrank/Rankerb.py`

 * *Files identical despite different names*

### Comparing `FlashRank-0.2.0/setup.py` & `FlashRank-0.2.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FlashRank', 
-    version='0.2.0', 
+    version='0.2.1', 
     packages=find_packages(),
     install_requires=[
         'tokenizers',
         'onnxruntime',
         'numpy',
         'requests',
         'tqdm'
```

