# Comparing `tmp/mecoda-minka-1.6.0.tar.gz` & `tmp/mecoda-minka-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecoda-minka-1.6.0.tar", last modified: Tue Apr  9 13:23:04 2024, max compression
+gzip compressed data, was "mecoda-minka-1.6.1.tar", last modified: Tue Apr 30 15:01:44 2024, max compression
```

## Comparing `mecoda-minka-1.6.0.tar` & `mecoda-minka-1.6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-04-09 13:23:04.125319 mecoda-minka-1.6.0/
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    35149 2022-12-22 16:17:43.000000 mecoda-minka-1.6.0/LICENSE
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    11399 2024-04-09 13:23:04.125319 mecoda-minka-1.6.0/PKG-INFO
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    10346 2024-04-09 13:15:47.000000 mecoda-minka-1.6.0/README.md
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)       38 2024-04-09 13:23:04.125319 mecoda-minka-1.6.0/setup.cfg
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     1522 2024-04-09 13:18:01.000000 mecoda-minka-1.6.0/setup.py
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-04-09 13:23:04.113319 mecoda-minka-1.6.0/src/
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-04-09 13:23:04.117319 mecoda-minka-1.6.0/src/mecoda_minka/
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)      566 2022-12-22 16:17:43.000000 mecoda-minka-1.6.0/src/mecoda_minka/__init__.py
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-04-09 13:23:04.117319 mecoda-minka-1.6.0/src/mecoda_minka/data/
--rw-r--r--   0 anomalia  (1000) anomalia  (1000) 10910030 2023-10-04 12:19:58.000000 mecoda-minka-1.6.0/src/mecoda_minka/data/taxon_tree.csv
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    20644 2024-04-09 12:53:35.000000 mecoda-minka-1.6.0/src/mecoda_minka/mecoda_minka.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     2716 2024-04-09 09:38:38.000000 mecoda-minka-1.6.0/src/mecoda_minka/models.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)        0 2022-12-22 16:17:43.000000 mecoda-minka-1.6.0/src/mecoda_minka/py.typed
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     1720 2023-03-01 13:46:13.000000 mecoda-minka-1.6.0/src/mecoda_minka/views.py
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-04-09 13:23:04.121319 mecoda-minka-1.6.0/src/mecoda_minka.egg-info/
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    11399 2024-04-09 13:23:04.000000 mecoda-minka-1.6.0/src/mecoda_minka.egg-info/PKG-INFO
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)      423 2024-04-09 13:23:04.000000 mecoda-minka-1.6.0/src/mecoda_minka.egg-info/SOURCES.txt
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)        1 2024-04-09 13:23:04.000000 mecoda-minka-1.6.0/src/mecoda_minka.egg-info/dependency_links.txt
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)       32 2024-04-09 13:23:04.000000 mecoda-minka-1.6.0/src/mecoda_minka.egg-info/requires.txt
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)       13 2024-04-09 13:23:04.000000 mecoda-minka-1.6.0/src/mecoda_minka.egg-info/top_level.txt
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-04-09 13:23:04.121319 mecoda-minka-1.6.0/tests/
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    27869 2024-03-13 14:37:53.000000 mecoda-minka-1.6.0/tests/test_minka.py
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-04-30 15:01:44.503698 mecoda-minka-1.6.1/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    35149 2022-12-22 16:17:43.000000 mecoda-minka-1.6.1/LICENSE
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    11399 2024-04-30 15:01:44.503698 mecoda-minka-1.6.1/PKG-INFO
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    10346 2024-04-09 13:15:47.000000 mecoda-minka-1.6.1/README.md
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)       38 2024-04-30 15:01:44.503698 mecoda-minka-1.6.1/setup.cfg
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     1522 2024-04-30 14:59:50.000000 mecoda-minka-1.6.1/setup.py
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-04-30 15:01:44.495698 mecoda-minka-1.6.1/src/
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-04-30 15:01:44.495698 mecoda-minka-1.6.1/src/mecoda_minka/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)      566 2022-12-22 16:17:43.000000 mecoda-minka-1.6.1/src/mecoda_minka/__init__.py
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-04-30 15:01:44.495698 mecoda-minka-1.6.1/src/mecoda_minka/data/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000) 10910030 2023-10-04 12:19:58.000000 mecoda-minka-1.6.1/src/mecoda_minka/data/taxon_tree.csv
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    21409 2024-04-30 14:58:30.000000 mecoda-minka-1.6.1/src/mecoda_minka/mecoda_minka.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     2716 2024-04-09 09:38:38.000000 mecoda-minka-1.6.1/src/mecoda_minka/models.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)        0 2022-12-22 16:17:43.000000 mecoda-minka-1.6.1/src/mecoda_minka/py.typed
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     1720 2023-03-01 13:46:13.000000 mecoda-minka-1.6.1/src/mecoda_minka/views.py
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-04-30 15:01:44.503698 mecoda-minka-1.6.1/src/mecoda_minka.egg-info/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    11399 2024-04-30 15:01:44.000000 mecoda-minka-1.6.1/src/mecoda_minka.egg-info/PKG-INFO
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)      423 2024-04-30 15:01:44.000000 mecoda-minka-1.6.1/src/mecoda_minka.egg-info/SOURCES.txt
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)        1 2024-04-30 15:01:44.000000 mecoda-minka-1.6.1/src/mecoda_minka.egg-info/dependency_links.txt
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)       32 2024-04-30 15:01:44.000000 mecoda-minka-1.6.1/src/mecoda_minka.egg-info/requires.txt
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)       13 2024-04-30 15:01:44.000000 mecoda-minka-1.6.1/src/mecoda_minka.egg-info/top_level.txt
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-04-30 15:01:44.503698 mecoda-minka-1.6.1/tests/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    27869 2024-03-13 14:37:53.000000 mecoda-minka-1.6.1/tests/test_minka.py
```

### Comparing `mecoda-minka-1.6.0/LICENSE` & `mecoda-minka-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mecoda-minka-1.6.0/PKG-INFO` & `mecoda-minka-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecoda-minka
-Version: 1.6.0
+Version: 1.6.1
 Summary: Library to download information using Minka API.
 Home-page: https://github.com/pynomaly/mecoda-minka
 Author: Ana Alvarez
 Author-email: ana.alvarez@icm.csic.es
 License: GNU General Public License v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `mecoda-minka-1.6.0/README.md` & `mecoda-minka-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `mecoda-minka-1.6.0/setup.py` & `mecoda-minka-1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="mecoda-minka",
-    version="1.6.0",
+    version="1.6.1",
     description="Library to download information using Minka API.",
     author="Ana Alvarez",
     author_email="ana.alvarez@icm.csic.es",
     license="GNU General Public License v3",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/pynomaly/mecoda-minka",
```

### Comparing `mecoda-minka-1.6.0/src/mecoda_minka/__init__.py` & `mecoda-minka-1.6.1/src/mecoda_minka/__init__.py`

 * *Files identical despite different names*

### Comparing `mecoda-minka-1.6.0/src/mecoda_minka/data/taxon_tree.csv` & `mecoda-minka-1.6.1/src/mecoda_minka/data/taxon_tree.csv`

 * *Files identical despite different names*

### Comparing `mecoda-minka-1.6.0/src/mecoda_minka/mecoda_minka.py` & `mecoda-minka-1.6.1/src/mecoda_minka/mecoda_minka.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,16 +80,33 @@
         created_on,
         created_d1,
         created_d2,
         grade,
         id_above,
         id_below,
     )
-
-    observations = _request(url, num_max)
+    session = requests.Session()
+    total_obs = session.get(url).json()["total_results"]
+    print("Total observations to download:", total_obs)
+    if total_obs <= 10000:
+        observations = _request(url, num_max)
+    else:
+        observations = []
+        # download obs using bins of 10000 ids
+        for n in range(1, 31):
+            batch_url = f"{url}&id_above={(n-1)*10000}&id_below={(n*10000)+1}"
+            print(batch_url)
+            obs_batch = _request(batch_url, num_max)
+            if len(obs_batch) > 0:
+                observations.extend(obs_batch)
+                # stop when num_max is exceeded
+                if num_max is not None:
+                    if len(observations) > num_max:
+                        observations = observations[:num_max]
+                        break
 
     return observations
 
 
 def _build_url(
     query: Optional[str] = None,
     id_project: Optional[int] = None,
```

### Comparing `mecoda-minka-1.6.0/src/mecoda_minka/models.py` & `mecoda-minka-1.6.1/src/mecoda_minka/models.py`

 * *Files identical despite different names*

### Comparing `mecoda-minka-1.6.0/src/mecoda_minka/views.py` & `mecoda-minka-1.6.1/src/mecoda_minka/views.py`

 * *Files identical despite different names*

### Comparing `mecoda-minka-1.6.0/src/mecoda_minka.egg-info/PKG-INFO` & `mecoda-minka-1.6.1/src/mecoda_minka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecoda-minka
-Version: 1.6.0
+Version: 1.6.1
 Summary: Library to download information using Minka API.
 Home-page: https://github.com/pynomaly/mecoda-minka
 Author: Ana Alvarez
 Author-email: ana.alvarez@icm.csic.es
 License: GNU General Public License v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `mecoda-minka-1.6.0/tests/test_minka.py` & `mecoda-minka-1.6.1/tests/test_minka.py`

 * *Files identical despite different names*

