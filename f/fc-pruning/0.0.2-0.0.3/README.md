# Comparing `tmp/fc_pruning-0.0.2.tar.gz` & `tmp/fc_pruning-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fc_pruning-0.0.2.tar", last modified: Tue Apr 23 17:25:08 2024, max compression
+gzip compressed data, was "fc_pruning-0.0.3.tar", last modified: Tue Apr 30 12:15:20 2024, max compression
```

## Comparing `fc_pruning-0.0.2.tar` & `fc_pruning-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-04-23 17:25:08.252511 fc_pruning-0.0.2/
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-04-23 17:25:08.251247 fc_pruning-0.0.2/Compress/
--rw-r--r--   0 aidamehammed   (501) staff       (20)        0 2024-04-23 17:07:18.000000 fc_pruning-0.0.2/Compress/__init__.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)     5617 2024-04-19 19:55:07.000000 fc_pruning-0.0.2/Compress/compress.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)     4071 2024-04-19 19:55:07.000000 fc_pruning-0.0.2/Compress/utils.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)    11352 2024-03-22 14:55:37.000000 fc_pruning-0.0.2/LICENSE
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1044 2024-04-23 17:25:08.252384 fc_pruning-0.0.2/PKG-INFO
--rw-r--r--   0 aidamehammed   (501) staff       (20)      556 2024-04-15 22:17:45.000000 fc_pruning-0.0.2/README.md
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-04-23 17:25:08.252096 fc_pruning-0.0.2/fc_pruning.egg-info/
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1044 2024-04-23 17:25:08.000000 fc_pruning-0.0.2/fc_pruning.egg-info/PKG-INFO
--rw-r--r--   0 aidamehammed   (501) staff       (20)      255 2024-04-23 17:25:08.000000 fc_pruning-0.0.2/fc_pruning.egg-info/SOURCES.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)        1 2024-04-23 17:25:08.000000 fc_pruning-0.0.2/fc_pruning.egg-info/dependency_links.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       27 2024-04-23 17:25:08.000000 fc_pruning-0.0.2/fc_pruning.egg-info/requires.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)        9 2024-04-23 17:25:08.000000 fc_pruning-0.0.2/fc_pruning.egg-info/top_level.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       38 2024-04-23 17:25:08.252563 fc_pruning-0.0.2/setup.cfg
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1052 2024-04-23 17:22:45.000000 fc_pruning-0.0.2/setup.py
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-04-30 12:15:20.817951 fc_pruning-0.0.3/
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-04-30 12:15:20.816445 fc_pruning-0.0.3/Compress/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)        0 2024-04-23 17:07:18.000000 fc_pruning-0.0.3/Compress/__init__.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     5665 2024-04-23 18:22:16.000000 fc_pruning-0.0.3/Compress/compress.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     4112 2024-04-23 17:35:47.000000 fc_pruning-0.0.3/Compress/utils.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)    11352 2024-03-22 14:55:37.000000 fc_pruning-0.0.3/LICENSE
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1044 2024-04-30 12:15:20.817802 fc_pruning-0.0.3/PKG-INFO
+-rw-r--r--   0 aidamehammed   (501) staff       (20)      556 2024-04-15 22:17:45.000000 fc_pruning-0.0.3/README.md
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-04-30 12:15:20.817386 fc_pruning-0.0.3/fc_pruning.egg-info/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1044 2024-04-30 12:15:20.000000 fc_pruning-0.0.3/fc_pruning.egg-info/PKG-INFO
+-rw-r--r--   0 aidamehammed   (501) staff       (20)      272 2024-04-30 12:15:20.000000 fc_pruning-0.0.3/fc_pruning.egg-info/SOURCES.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)        1 2024-04-30 12:15:20.000000 fc_pruning-0.0.3/fc_pruning.egg-info/dependency_links.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       27 2024-04-30 12:15:20.000000 fc_pruning-0.0.3/fc_pruning.egg-info/requires.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)        9 2024-04-30 12:15:20.000000 fc_pruning-0.0.3/fc_pruning.egg-info/top_level.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       38 2024-04-30 12:15:20.818025 fc_pruning-0.0.3/setup.cfg
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1052 2024-04-30 12:15:12.000000 fc_pruning-0.0.3/setup.py
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-04-30 12:15:20.817523 fc_pruning-0.0.3/test/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)      128 2024-04-23 17:35:47.000000 fc_pruning-0.0.3/test/testcase.py
```

### Comparing `fc_pruning-0.0.2/Compress/compress.py` & `fc_pruning-0.0.3/Compress/compress.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from FeatureCloud.app.engine.app import AppState
 from typing import TypedDict, Union, List, Type
 import torch
 import torch_pruning as tp
-import utils as pf
+import fc_pruning.Compress.utils as pf
+import sys
+print('running')
 
 class PruningType(TypedDict):
     model: torch.nn.Module
     reference_model: Union[List[torch.nn.Module], None]
     imp: Type[tp.pruner.importance.Importance]
     ignored_layers: Union[List[torch.nn.Module], None]
     pruning_ratio: float
```

### Comparing `fc_pruning-0.0.2/Compress/utils.py` & `fc_pruning-0.0.3/Compress/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import torch_pruning as tp
 import torch
 import torch.nn as nn
 import copy
 import os
 
-
+def print_test():
+    print(' It works ')
 def get_weights(model):
     return [param.data for param in model.parameters()]
 
 def get_last_layer(model):
     last_layer = None
     for layer in model.modules():
         if isinstance(layer, nn.Linear):
```

### Comparing `fc_pruning-0.0.2/LICENSE` & `fc_pruning-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fc_pruning-0.0.2/PKG-INFO` & `fc_pruning-0.0.3/fc_pruning.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fc_pruning
-Version: 0.0.2
+Name: fc-pruning
+Version: 0.0.3
 Summary: FC Pruning
 Home-page: https://github.com/AidaMehammed/fc_pruning
 Author: Aida Mehammed
 Author-email: aida.mehammed@studium.uni-hamburg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AidaMehammed/fc_pruning
 Platform: UNKNOWN
```

### Comparing `fc_pruning-0.0.2/README.md` & `fc_pruning-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fc_pruning-0.0.2/fc_pruning.egg-info/PKG-INFO` & `fc_pruning-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fc-pruning
-Version: 0.0.2
+Name: fc_pruning
+Version: 0.0.3
 Summary: FC Pruning
 Home-page: https://github.com/AidaMehammed/fc_pruning
 Author: Aida Mehammed
 Author-email: aida.mehammed@studium.uni-hamburg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AidaMehammed/fc_pruning
 Platform: UNKNOWN
```

### Comparing `fc_pruning-0.0.2/setup.py` & `fc_pruning-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(name="fc_pruning",
-                 version="0.0.2",
+                 version="0.0.3",
                  author="Aida Mehammed",
                  author_email="aida.mehammed@studium.uni-hamburg.de",
                  description="FC Pruning",
                  long_description=long_description,
                  long_description_content_type="text/markdown",
                  url="https://github.com/AidaMehammed/fc_pruning",
                  project_urls={
```

