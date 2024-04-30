# Comparing `tmp/FlashRank-0.2.2.tar.gz` & `tmp/FlashRank-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlashRank-0.2.2.tar", last modified: Tue Apr 30 10:27:08 2024, max compression
+gzip compressed data, was "FlashRank-0.2.3.tar", last modified: Tue Apr 30 10:31:30 2024, max compression
```

## Comparing `FlashRank-0.2.2.tar` & `FlashRank-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-30 10:27:08.467244 FlashRank-0.2.2/
-drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-30 10:27:08.465731 FlashRank-0.2.2/FlashRank.egg-info/
--rw-r--r--   0 prithivida   (501) staff       (20)    10278 2024-04-30 10:27:08.000000 FlashRank-0.2.2/FlashRank.egg-info/PKG-INFO
--rw-r--r--   0 prithivida   (501) staff       (20)      294 2024-04-30 10:27:08.000000 FlashRank-0.2.2/FlashRank.egg-info/SOURCES.txt
--rw-r--r--   0 prithivida   (501) staff       (20)        1 2024-04-30 10:27:08.000000 FlashRank-0.2.2/FlashRank.egg-info/dependency_links.txt
--rw-r--r--   0 prithivida   (501) staff       (20)       68 2024-04-30 10:27:08.000000 FlashRank-0.2.2/FlashRank.egg-info/requires.txt
--rw-r--r--   0 prithivida   (501) staff       (20)       10 2024-04-30 10:27:08.000000 FlashRank-0.2.2/FlashRank.egg-info/top_level.txt
--rw-r--r--   0 prithivida   (501) staff       (20)    11357 2023-12-04 14:24:33.000000 FlashRank-0.2.2/LICENSE
--rw-r--r--   0 prithivida   (501) staff       (20)    10278 2024-04-30 10:27:08.467045 FlashRank-0.2.2/PKG-INFO
--rw-r--r--   0 prithivida   (501) staff       (20)     9757 2024-03-19 01:23:34.000000 FlashRank-0.2.2/README.md
-drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-30 10:27:08.466722 FlashRank-0.2.2/flashrank/
--rw-r--r--   0 prithivida   (501) staff       (20)      724 2024-04-30 10:04:33.000000 FlashRank-0.2.2/flashrank/Config.py
--rw-r--r--   0 prithivida   (501) staff       (20)     9893 2024-04-30 10:26:09.000000 FlashRank-0.2.2/flashrank/Ranker.py
--rw-r--r--   0 prithivida   (501) staff       (20)    10457 2023-12-13 12:36:57.000000 FlashRank-0.2.2/flashrank/Rankerb.py
--rw-r--r--   0 prithivida   (501) staff       (20)     6093 2024-01-29 14:51:57.000000 FlashRank-0.2.2/flashrank/Rankerc.py
--rw-r--r--   0 prithivida   (501) staff       (20)       41 2024-04-30 09:25:26.000000 FlashRank-0.2.2/flashrank/__init__.py
--rw-r--r--   0 prithivida   (501) staff       (20)       38 2024-04-30 10:27:08.467286 FlashRank-0.2.2/setup.cfg
--rw-r--r--   0 prithivida   (501) staff       (20)      855 2024-04-30 10:22:38.000000 FlashRank-0.2.2/setup.py
+drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-30 10:31:30.392667 FlashRank-0.2.3/
+drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-30 10:31:30.390753 FlashRank-0.2.3/FlashRank.egg-info/
+-rw-r--r--   0 prithivida   (501) staff       (20)    10278 2024-04-30 10:31:30.000000 FlashRank-0.2.3/FlashRank.egg-info/PKG-INFO
+-rw-r--r--   0 prithivida   (501) staff       (20)      294 2024-04-30 10:31:30.000000 FlashRank-0.2.3/FlashRank.egg-info/SOURCES.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)        1 2024-04-30 10:31:30.000000 FlashRank-0.2.3/FlashRank.egg-info/dependency_links.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)       68 2024-04-30 10:31:30.000000 FlashRank-0.2.3/FlashRank.egg-info/requires.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)       10 2024-04-30 10:31:30.000000 FlashRank-0.2.3/FlashRank.egg-info/top_level.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)    11357 2023-12-04 14:24:33.000000 FlashRank-0.2.3/LICENSE
+-rw-r--r--   0 prithivida   (501) staff       (20)    10278 2024-04-30 10:31:30.392352 FlashRank-0.2.3/PKG-INFO
+-rw-r--r--   0 prithivida   (501) staff       (20)     9757 2024-03-19 01:23:34.000000 FlashRank-0.2.3/README.md
+drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-30 10:31:30.392032 FlashRank-0.2.3/flashrank/
+-rw-r--r--   0 prithivida   (501) staff       (20)      724 2024-04-30 10:04:33.000000 FlashRank-0.2.3/flashrank/Config.py
+-rw-r--r--   0 prithivida   (501) staff       (20)     9923 2024-04-30 10:30:51.000000 FlashRank-0.2.3/flashrank/Ranker.py
+-rw-r--r--   0 prithivida   (501) staff       (20)    10457 2023-12-13 12:36:57.000000 FlashRank-0.2.3/flashrank/Rankerb.py
+-rw-r--r--   0 prithivida   (501) staff       (20)     6093 2024-01-29 14:51:57.000000 FlashRank-0.2.3/flashrank/Rankerc.py
+-rw-r--r--   0 prithivida   (501) staff       (20)       41 2024-04-30 09:25:26.000000 FlashRank-0.2.3/flashrank/__init__.py
+-rw-r--r--   0 prithivida   (501) staff       (20)       38 2024-04-30 10:31:30.392715 FlashRank-0.2.3/setup.cfg
+-rw-r--r--   0 prithivida   (501) staff       (20)      855 2024-04-30 10:30:57.000000 FlashRank-0.2.3/setup.py
```

### Comparing `FlashRank-0.2.2/FlashRank.egg-info/PKG-INFO` & `FlashRank-0.2.3/FlashRank.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlashRank
-Version: 0.2.2
+Version: 0.2.3
 Summary: Ultra lite & Super fast SoTA cross-encoder based re-ranking for your search & retrieval pipelines.
 Home-page: https://github.com/PrithivirajDamodaran/FlashRank
 Author: Prithivi Da
 Author-email: 
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `FlashRank-0.2.2/LICENSE` & `FlashRank-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FlashRank-0.2.2/PKG-INFO` & `FlashRank-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlashRank
-Version: 0.2.2
+Version: 0.2.3
 Summary: Ultra lite & Super fast SoTA cross-encoder based re-ranking for your search & retrieval pipelines.
 Home-page: https://github.com/PrithivirajDamodaran/FlashRank
 Author: Prithivi Da
 Author-email: 
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `FlashRank-0.2.2/README.md` & `FlashRank-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `FlashRank-0.2.2/flashrank/Config.py` & `FlashRank-0.2.3/flashrank/Config.py`

 * *Files identical despite different names*

### Comparing `FlashRank-0.2.2/flashrank/Ranker.py` & `FlashRank-0.2.3/flashrank/Ranker.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
             max_length (int): The maximum length of the tokens.
         """
         self.cache_dir: Path = Path(cache_dir)
         self.model_dir: Path = self.cache_dir / model_name
         self._prepare_model_dir(model_name)
         model_file = model_file_map[model_name]
 
+        self.llm_model = None
         if model_name in listwise_rankers:
             self.llm_model = Llama(
               model_path=str(self.model_dir / model_file),
               n_ctx=max_length,  
               n_threads=8,          
             ) 
         else:
```

### Comparing `FlashRank-0.2.2/flashrank/Rankerb.py` & `FlashRank-0.2.3/flashrank/Rankerb.py`

 * *Files identical despite different names*

### Comparing `FlashRank-0.2.2/flashrank/Rankerc.py` & `FlashRank-0.2.3/flashrank/Rankerc.py`

 * *Files identical despite different names*

### Comparing `FlashRank-0.2.2/setup.py` & `FlashRank-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FlashRank', 
-    version='0.2.2', 
+    version='0.2.3', 
     packages=find_packages(),
     install_requires=[
         'tokenizers',
         'onnxruntime',
         'numpy',
         'requests',
         'tqdm',
```

