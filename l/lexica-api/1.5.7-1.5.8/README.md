# Comparing `tmp/lexica-api-1.5.7.tar.gz` & `tmp/lexica-api-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexica-api-1.5.7.tar", last modified: Sun Mar  3 11:20:50 2024, max compression
+gzip compressed data, was "lexica-api-1.5.8.tar", last modified: Tue Apr 30 20:36:52 2024, max compression
```

## Comparing `lexica-api-1.5.7.tar` & `lexica-api-1.5.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-03 11:20:50.512321 lexica-api-1.5.7/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1065 2024-02-17 12:02:32.000000 lexica-api-1.5.7/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1588 2024-03-03 11:20:50.512321 lexica-api-1.5.7/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      974 2024-01-22 14:56:08.000000 lexica-api-1.5.7/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-03 11:20:50.512321 lexica-api-1.5.7/lexica/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      297 2024-03-03 11:18:25.000000 lexica-api-1.5.7/lexica/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      950 2024-02-17 12:00:36.000000 lexica-api-1.5.7/lexica/constants.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9339 2024-03-03 11:19:57.000000 lexica-api-1.5.7/lexica/core.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9873 2024-03-03 11:19:40.000000 lexica-api-1.5.7/lexica/core_async.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      130 2023-09-10 07:01:14.000000 lexica-api-1.5.7/lexica/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-03 11:20:50.512321 lexica-api-1.5.7/lexica_api.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1588 2024-03-03 11:20:50.000000 lexica-api-1.5.7/lexica_api.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      286 2024-03-03 11:20:50.000000 lexica-api-1.5.7/lexica_api.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-03-03 11:20:50.000000 lexica-api-1.5.7/lexica_api.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       21 2024-03-03 11:20:50.000000 lexica-api-1.5.7/lexica_api.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2024-03-03 11:20:50.000000 lexica-api-1.5.7/lexica_api.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-03-03 11:20:50.512321 lexica-api-1.5.7/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1378 2024-01-22 14:48:28.000000 lexica-api-1.5.7/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-30 20:36:52.440300 lexica-api-1.5.8/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1065 2024-02-17 12:02:32.000000 lexica-api-1.5.8/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2647 2024-04-30 20:36:52.436300 lexica-api-1.5.8/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2032 2024-04-20 07:14:21.000000 lexica-api-1.5.8/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-30 20:36:52.436300 lexica-api-1.5.8/lexica/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      297 2024-04-30 20:36:12.000000 lexica-api-1.5.8/lexica/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      916 2024-04-30 20:35:07.000000 lexica-api-1.5.8/lexica/constants.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9339 2024-03-03 11:19:57.000000 lexica-api-1.5.8/lexica/core.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9873 2024-03-03 11:19:40.000000 lexica-api-1.5.8/lexica/core_async.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      130 2023-09-10 07:01:14.000000 lexica-api-1.5.8/lexica/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-30 20:36:52.436300 lexica-api-1.5.8/lexica_api.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2647 2024-04-30 20:36:52.000000 lexica-api-1.5.8/lexica_api.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      286 2024-04-30 20:36:52.000000 lexica-api-1.5.8/lexica_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-30 20:36:52.000000 lexica-api-1.5.8/lexica_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2024-04-30 20:36:52.000000 lexica-api-1.5.8/lexica_api.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2024-04-30 20:36:52.000000 lexica-api-1.5.8/lexica_api.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-04-30 20:36:52.440300 lexica-api-1.5.8/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1360 2024-04-30 20:35:19.000000 lexica-api-1.5.8/setup.py
```

### Comparing `lexica-api-1.5.7/LICENSE` & `lexica-api-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lexica-api-1.5.7/lexica/core.py` & `lexica-api-1.5.8/lexica/core.py`

 * *Files identical despite different names*

### Comparing `lexica-api-1.5.7/lexica/core_async.py` & `lexica-api-1.5.8/lexica/core_async.py`

 * *Files identical despite different names*

### Comparing `lexica-api-1.5.7/setup.py` & `lexica-api-1.5.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,23 +18,22 @@
         return long_description
 
 setup(
     name="lexica-api",
     version=get_version(),
     author="Qewertyy",
     author_email="Qewertyy.irl@gmail.com",
-    description="The python package for api.qewertyy.me",
+    description="The python package for api.qewertyy.dev",
     url="https://github.com/Qewertyy/LexicaAPI",
     python_requires=">=3.8",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
-        "httpx[http2]",
-        "asyncio"
+        "httpx[http2]"
     ],
     keywords="Python, API, Bard, Google Bard, Large Language Model, Chatbot API, Google API, Chatbot, Image Generations, Latent Diffusion, State of Art, Image Reverse Search, Reverse Image Search",
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
     ]
```

