# Comparing `tmp/retroapi-0.8.0.tar.gz` & `tmp/retroapi-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retroapi-0.8.0.tar", last modified: Fri Dec 15 01:04:53 2023, max compression
+gzip compressed data, was "retroapi-0.8.2.tar", last modified: Tue Apr 30 08:09:06 2024, max compression
```

## Comparing `retroapi-0.8.0.tar` & `retroapi-0.8.2.tar`

### file list

```diff
@@ -1,25 +1,21 @@
-drwxr-xr-x   0 bruce      (501) staff       (20)        0 2023-12-15 01:04:53.818360 retroapi-0.8.0/
--rw-r--r--   0 bruce      (501) staff       (20)       58 2023-10-13 13:09:00.000000 retroapi-0.8.0/MANIFEST.in
--rw-r--r--   0 bruce      (501) staff       (20)     4525 2023-12-15 01:04:53.818144 retroapi-0.8.0/PKG-INFO
--rw-r--r--   0 bruce      (501) staff       (20)     3308 2023-12-15 01:02:11.000000 retroapi-0.8.0/README.md
--rw-r--r--   0 bruce      (501) staff       (20)      805 2023-10-12 13:16:15.000000 retroapi-0.8.0/pyproject.toml
-drwxr-xr-x   0 bruce      (501) staff       (20)        0 2023-12-15 01:04:53.815547 retroapi-0.8.0/retroapi/
--rw-r--r--   0 bruce      (501) staff       (20)       77 2023-10-13 09:08:56.000000 retroapi-0.8.0/retroapi/__init__.py
-drwxr-xr-x   0 bruce      (501) staff       (20)        0 2023-12-15 01:04:53.817000 retroapi-0.8.0/retroapi/__pycache__/
--rw-r--r--   0 bruce      (501) staff       (20)      303 2023-10-13 09:08:57.000000 retroapi-0.8.0/retroapi/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 bruce      (501) staff       (20)     2176 2023-10-31 11:24:08.000000 retroapi-0.8.0/retroapi/__pycache__/convert_name2smiles.cpython-311.pyc
--rw-r--r--   0 bruce      (501) staff       (20)    13334 2023-12-15 00:49:57.000000 retroapi-0.8.0/retroapi/__pycache__/retro_api.cpython-311.pyc
--rw-r--r--   0 bruce      (501) staff       (20)      691 2023-10-31 11:23:21.000000 retroapi-0.8.0/retroapi/convert_name2smiles.py
--rw-r--r--   0 bruce      (501) staff       (20)     6878 2023-12-15 00:59:57.000000 retroapi-0.8.0/retroapi/retro_api.py
-drwxr-xr-x   0 bruce      (501) staff       (20)        0 2023-12-15 01:04:53.817922 retroapi-0.8.0/retroapi.egg-info/
--rw-r--r--   0 bruce      (501) staff       (20)     4525 2023-12-15 01:04:53.000000 retroapi-0.8.0/retroapi.egg-info/PKG-INFO
--rw-r--r--   0 bruce      (501) staff       (20)      497 2023-12-15 01:04:53.000000 retroapi-0.8.0/retroapi.egg-info/SOURCES.txt
--rw-r--r--   0 bruce      (501) staff       (20)        1 2023-12-15 01:04:53.000000 retroapi-0.8.0/retroapi.egg-info/dependency_links.txt
--rw-r--r--   0 bruce      (501) staff       (20)       17 2023-12-15 01:04:53.000000 retroapi-0.8.0/retroapi.egg-info/requires.txt
--rw-r--r--   0 bruce      (501) staff       (20)       15 2023-12-15 01:04:53.000000 retroapi-0.8.0/retroapi.egg-info/top_level.txt
--rw-r--r--   0 bruce      (501) staff       (20)       38 2023-12-15 01:04:53.818409 retroapi-0.8.0/setup.cfg
--rw-r--r--   0 bruce      (501) staff       (20)     1462 2023-12-15 01:02:28.000000 retroapi-0.8.0/setup.py
-drwxr-xr-x   0 bruce      (501) staff       (20)        0 2023-12-15 01:04:53.817716 retroapi-0.8.0/tests/
--rw-r--r--   0 bruce      (501) staff       (20)        0 2023-10-12 13:25:36.000000 retroapi-0.8.0/tests/__init__.py
--rw-r--r--   0 bruce      (501) staff       (20)      861 2023-10-31 11:26:57.000000 retroapi-0.8.0/tests/test_name2smiles.py
--rw-r--r--   0 bruce      (501) staff       (20)     2960 2023-12-15 00:51:02.000000 retroapi-0.8.0/tests/test_retro_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:09:06.847035 retroapi-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 08:08:46.000000 retroapi-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-30 08:09:06.847035 retroapi-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-30 08:08:46.000000 retroapi-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-30 08:08:46.000000 retroapi-0.8.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:09:06.847035 retroapi-0.8.2/retroapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-30 08:08:46.000000 retroapi-0.8.2/retroapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-30 08:08:46.000000 retroapi-0.8.2/retroapi/convert_name2smiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-30 08:08:46.000000 retroapi-0.8.2/retroapi/retro_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:09:06.847035 retroapi-0.8.2/retroapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-30 08:09:06.000000 retroapi-0.8.2/retroapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-30 08:09:06.000000 retroapi-0.8.2/retroapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:09:06.000000 retroapi-0.8.2/retroapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 08:09:06.000000 retroapi-0.8.2/retroapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 08:09:06.000000 retroapi-0.8.2/retroapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 08:09:06.847035 retroapi-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-30 08:08:46.000000 retroapi-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:09:06.847035 retroapi-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 08:08:46.000000 retroapi-0.8.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-30 08:08:46.000000 retroapi-0.8.2/tests/test_name2smiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-30 08:08:46.000000 retroapi-0.8.2/tests/test_retro_api.py
```

### Comparing `retroapi-0.8.0/PKG-INFO` & `retroapi-0.8.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retroapi
-Version: 0.8.0
+Version: 0.8.2
 Summary: A wrap retroapi package for retrosynthesis routes and exploring reaction conditions
 Home-page: https://github.com/bruceunx/retrosynthesis
 Author: Bruceunx
 Author-email: bruceunx@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/bruceunx/retrosynthesis
 Classifier: Intended Audience :: Science/Research
@@ -18,15 +18,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<3.13
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: aiohttp
 
 ## RetroSynthesis API
 
 ![test](https://github.com/bruceunx/retroapi/actions/workflows/python-app.yml/badge.svg)
@@ -35,14 +35,35 @@
 
 - supply plausible value for all predicts.
 
 - predict conditions base on one reaction.
 
 - add aync support
 
+- deploy your backend server with **torchserve** (if api failed)
+
+  > install torchserve and other libraries from requirements.txt
+  > run download_models.sh
+  > run
+
+  ```bash
+  torchserve --start --foreground --ncs --model-store=mars --models reaxys=reaxys.mar
+
+  ```
+
+  > test server
+
+  ```bash
+
+   curl http://127.0.0.1:8080/predictions/reaxys \                                                                                                            (base)
+                --header "Content-Type: application/json" \
+                --request POST \
+                --data '{"smiles": ["CC(C)(C)OC(=O)N1CCC(OCCO)CC1"]}'
+  ```
+
 ### Install
 
 - using pip
 
 ```bash
 pip install retroapi
 
@@ -134,23 +155,26 @@
     if conds is not None:
         # check reaction condition with plausible
         pass
 ```
 
 ## Change log:
 
+### 2023-12-30 Extract condition recommend code from ASKCOS to notebook for local test.
+
+### 2023-12-25 Run backend server with torchserve
+
 ### Add try_times in predict_routes and process_reaction w/ async
 
 ```python
 
 routes = await retro_api.apredict_routes(smiles, try_num=20)
 
 ```
 
-
 ### **Need Token** to use this package
 
 > It's wrap package for askcos.mit.edu API, so you can get token from website first.
 
 ### add aync for package
 
 > with function name prefix with 'a', for example get_smile -> aget_smile
```

### Comparing `retroapi-0.8.0/README.md` & `retroapi-0.8.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,35 @@
 
 - supply plausible value for all predicts.
 
 - predict conditions base on one reaction.
 
 - add aync support
 
+- deploy your backend server with **torchserve** (if api failed)
+
+  > install torchserve and other libraries from requirements.txt
+  > run download_models.sh
+  > run
+
+  ```bash
+  torchserve --start --foreground --ncs --model-store=mars --models reaxys=reaxys.mar
+
+  ```
+
+  > test server
+
+  ```bash
+
+   curl http://127.0.0.1:8080/predictions/reaxys \                                                                                                            (base)
+                --header "Content-Type: application/json" \
+                --request POST \
+                --data '{"smiles": ["CC(C)(C)OC(=O)N1CCC(OCCO)CC1"]}'
+  ```
+
 ### Install
 
 - using pip
 
 ```bash
 pip install retroapi
 
@@ -105,23 +126,26 @@
     if conds is not None:
         # check reaction condition with plausible
         pass
 ```
 
 ## Change log:
 
+### 2023-12-30 Extract condition recommend code from ASKCOS to notebook for local test.
+
+### 2023-12-25 Run backend server with torchserve
+
 ### Add try_times in predict_routes and process_reaction w/ async
 
 ```python
 
 routes = await retro_api.apredict_routes(smiles, try_num=20)
 
 ```
 
-
 ### **Need Token** to use this package
 
 > It's wrap package for askcos.mit.edu API, so you can get token from website first.
 
 ### add aync for package
 
 > with function name prefix with 'a', for example get_smile -> aget_smile
```

### Comparing `retroapi-0.8.0/pyproject.toml` & `retroapi-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `retroapi-0.8.0/retroapi/convert_name2smiles.py` & `retroapi-0.8.2/retroapi/convert_name2smiles.py`

 * *Files identical despite different names*

### Comparing `retroapi-0.8.0/retroapi/retro_api.py` & `retroapi-0.8.2/retroapi/retro_api.py`

 * *Files identical despite different names*

### Comparing `retroapi-0.8.0/retroapi.egg-info/PKG-INFO` & `retroapi-0.8.2/retroapi.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retroapi
-Version: 0.8.0
+Version: 0.8.2
 Summary: A wrap retroapi package for retrosynthesis routes and exploring reaction conditions
 Home-page: https://github.com/bruceunx/retrosynthesis
 Author: Bruceunx
 Author-email: bruceunx@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/bruceunx/retrosynthesis
 Classifier: Intended Audience :: Science/Research
@@ -18,15 +18,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<3.13
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: aiohttp
 
 ## RetroSynthesis API
 
 ![test](https://github.com/bruceunx/retroapi/actions/workflows/python-app.yml/badge.svg)
@@ -35,14 +35,35 @@
 
 - supply plausible value for all predicts.
 
 - predict conditions base on one reaction.
 
 - add aync support
 
+- deploy your backend server with **torchserve** (if api failed)
+
+  > install torchserve and other libraries from requirements.txt
+  > run download_models.sh
+  > run
+
+  ```bash
+  torchserve --start --foreground --ncs --model-store=mars --models reaxys=reaxys.mar
+
+  ```
+
+  > test server
+
+  ```bash
+
+   curl http://127.0.0.1:8080/predictions/reaxys \                                                                                                            (base)
+                --header "Content-Type: application/json" \
+                --request POST \
+                --data '{"smiles": ["CC(C)(C)OC(=O)N1CCC(OCCO)CC1"]}'
+  ```
+
 ### Install
 
 - using pip
 
 ```bash
 pip install retroapi
 
@@ -134,23 +155,26 @@
     if conds is not None:
         # check reaction condition with plausible
         pass
 ```
 
 ## Change log:
 
+### 2023-12-30 Extract condition recommend code from ASKCOS to notebook for local test.
+
+### 2023-12-25 Run backend server with torchserve
+
 ### Add try_times in predict_routes and process_reaction w/ async
 
 ```python
 
 routes = await retro_api.apredict_routes(smiles, try_num=20)
 
 ```
 
-
 ### **Need Token** to use this package
 
 > It's wrap package for askcos.mit.edu API, so you can get token from website first.
 
 ### add aync for package
 
 > with function name prefix with 'a', for example get_smile -> aget_smile
```

### Comparing `retroapi-0.8.0/setup.py` & `retroapi-0.8.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pathlib import Path
 from setuptools import find_packages, setup
 
 setup(
     name="retroapi",
-    version="0.8.0",
-    description="A wrap retroapi package for retrosynthesis routes and exploring reaction conditions",
+    version="0.8.2",
+    description=
+    "A wrap retroapi package for retrosynthesis routes and exploring reaction conditions",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/bruceunx/retrosynthesis",
     author="Bruceunx",
     author_email="bruceunx@gmail.com",
     license="MIT License",
     project_urls={"Source": "https://github.com/bruceunx/retrosynthesis"},
@@ -25,12 +26,11 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
-    python_requires=">=3.8,<3.12",
+    python_requires=">=3.8,<3.13",
     install_requires=["requests", "aiohttp"],
     packages=find_packages(),
-    include_package_data=True
-)
+    include_package_data=True)
```

### Comparing `retroapi-0.8.0/tests/test_name2smiles.py` & `retroapi-0.8.2/tests/test_name2smiles.py`

 * *Files identical despite different names*

### Comparing `retroapi-0.8.0/tests/test_retro_api.py` & `retroapi-0.8.2/tests/test_retro_api.py`

 * *Files identical despite different names*

