# Comparing `tmp/neutron-ai-1.0.0b6.tar.gz` & `tmp/neutron_ai-1.0.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neutron-ai-1.0.0b6.tar", last modified: Tue Apr  2 20:07:03 2024, max compression
+gzip compressed data, was "neutron_ai-1.0.0b7.tar", last modified: Tue Apr 30 21:06:32 2024, max compression
```

## Comparing `neutron-ai-1.0.0b6.tar` & `neutron_ai-1.0.0b7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:07:03.387123 neutron-ai-1.0.0b6/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-02 20:06:38.000000 neutron-ai-1.0.0b6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-02 20:07:03.387123 neutron-ai-1.0.0b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-02 20:06:38.000000 neutron-ai-1.0.0b6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-02 20:06:38.000000 neutron-ai-1.0.0b6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 20:07:03.387123 neutron-ai-1.0.0b6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-02 20:06:50.000000 neutron-ai-1.0.0b6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:07:03.387123 neutron-ai-1.0.0b6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:07:03.387123 neutron-ai-1.0.0b6/src/neutron/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:06:38.000000 neutron-ai-1.0.0b6/src/neutron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-02 20:06:38.000000 neutron-ai-1.0.0b6/src/neutron/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-02 20:06:38.000000 neutron-ai-1.0.0b6/src/neutron/interactive_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-02 20:06:38.000000 neutron-ai-1.0.0b6/src/neutron/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-02 20:06:38.000000 neutron-ai-1.0.0b6/src/neutron/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:07:03.387123 neutron-ai-1.0.0b6/src/neutron_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-02 20:07:03.000000 neutron-ai-1.0.0b6/src/neutron_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-02 20:07:03.000000 neutron-ai-1.0.0b6/src/neutron_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:07:03.000000 neutron-ai-1.0.0b6/src/neutron_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-02 20:07:03.000000 neutron-ai-1.0.0b6/src/neutron_ai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 20:07:03.000000 neutron-ai-1.0.0b6/src/neutron_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 20:07:03.000000 neutron-ai-1.0.0b6/src/neutron_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:06:32.052285 neutron_ai-1.0.0b7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-30 21:06:17.000000 neutron_ai-1.0.0b7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-30 21:06:32.052285 neutron_ai-1.0.0b7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-30 21:06:17.000000 neutron_ai-1.0.0b7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-30 21:06:17.000000 neutron_ai-1.0.0b7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 21:06:32.052285 neutron_ai-1.0.0b7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-30 21:06:27.000000 neutron_ai-1.0.0b7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:06:32.048285 neutron_ai-1.0.0b7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:06:32.048285 neutron_ai-1.0.0b7/src/neutron/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 21:06:17.000000 neutron_ai-1.0.0b7/src/neutron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-30 21:06:17.000000 neutron_ai-1.0.0b7/src/neutron/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-30 21:06:17.000000 neutron_ai-1.0.0b7/src/neutron/interactive_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-30 21:06:17.000000 neutron_ai-1.0.0b7/src/neutron/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-30 21:06:17.000000 neutron_ai-1.0.0b7/src/neutron/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:06:32.052285 neutron_ai-1.0.0b7/src/neutron_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-30 21:06:32.000000 neutron_ai-1.0.0b7/src/neutron_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-30 21:06:32.000000 neutron_ai-1.0.0b7/src/neutron_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 21:06:32.000000 neutron_ai-1.0.0b7/src/neutron_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-30 21:06:32.000000 neutron_ai-1.0.0b7/src/neutron_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-30 21:06:32.000000 neutron_ai-1.0.0b7/src/neutron_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 21:06:32.000000 neutron_ai-1.0.0b7/src/neutron_ai.egg-info/top_level.txt
```

### Comparing `neutron-ai-1.0.0b6/LICENSE.md` & `neutron_ai-1.0.0b7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neutron-ai-1.0.0b6/PKG-INFO` & `neutron_ai-1.0.0b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neutron-ai
-Version: 1.0.0b6
+Version: 1.0.0b7
 Summary: AI Powered Ethical Hacking Assistant
 Home-page: https://github.com/berylliumsec/neutron
 Author: David I
 Author-email: david@berylliumsec.com
 License: BSD
 Keywords: AI,Ethical Hacking
 Classifier: Development Status :: 4 - Beta
```

### Comparing `neutron-ai-1.0.0b6/README.md` & `neutron_ai-1.0.0b7/README.md`

 * *Files identical despite different names*

### Comparing `neutron-ai-1.0.0b6/setup.py` & `neutron_ai-1.0.0b7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="neutron-ai",
-    version="1.0.0b6",
+    version="1.0.0b7",
     description="AI Powered Ethical Hacking Assistant",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="David I",
     author_email="david@berylliumsec.com",
     url="https://github.com/berylliumsec/neutron",
     classifiers=[
@@ -32,17 +32,15 @@
         "transformers>=4.34.0",
         "fastapi",
         "uvicorn",
         "pydantic",
         "langchain",
         "regex",
         "argparse",
-        "typing-extensions"
-    
-
+        "typing-extensions",
     ],
     entry_points={
         "console_scripts": [
             # Allows users to type 'neutron-client' in the command line to interact with the server
             "neutron-client=neutron.client:main",
             # Allows users to start the server by typing 'neutron-server'
             "neutron-server=neutron.server:main",
```

### Comparing `neutron-ai-1.0.0b6/src/neutron/client.py` & `neutron_ai-1.0.0b7/src/neutron/client.py`

 * *Files identical despite different names*

### Comparing `neutron-ai-1.0.0b6/src/neutron/server.py` & `neutron_ai-1.0.0b7/src/neutron/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import os
 from typing import Any, Dict
-import torch
+
 import psutil
+import torch
 from fastapi import FastAPI, HTTPException, Request, status
 from fastapi.middleware.cors import CORSMiddleware
 from pydantic import BaseModel
 
 from neutron.interactive_model import InteractiveModel
 
 # Set up argument parsing
```

### Comparing `neutron-ai-1.0.0b6/src/neutron/utilities.py` & `neutron_ai-1.0.0b7/src/neutron/utilities.py`

 * *Files identical despite different names*

### Comparing `neutron-ai-1.0.0b6/src/neutron_ai.egg-info/PKG-INFO` & `neutron_ai-1.0.0b7/src/neutron_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neutron-ai
-Version: 1.0.0b6
+Version: 1.0.0b7
 Summary: AI Powered Ethical Hacking Assistant
 Home-page: https://github.com/berylliumsec/neutron
 Author: David I
 Author-email: david@berylliumsec.com
 License: BSD
 Keywords: AI,Ethical Hacking
 Classifier: Development Status :: 4 - Beta
```

