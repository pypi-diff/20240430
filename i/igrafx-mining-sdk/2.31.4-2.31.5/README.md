# Comparing `tmp/igrafx_mining_sdk-2.31.4.tar.gz` & `tmp/igrafx_mining_sdk-2.31.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igrafx_mining_sdk-2.31.4.tar", last modified: Fri Apr 19 12:43:55 2024, max compression
+gzip compressed data, was "igrafx_mining_sdk-2.31.5.tar", last modified: Tue Apr 30 15:25:46 2024, max compression
```

## Comparing `igrafx_mining_sdk-2.31.4.tar` & `igrafx_mining_sdk-2.31.5.tar`

### file list

```diff
@@ -1,37 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:43:55.110100 igrafx_mining_sdk-2.31.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-19 12:43:55.110100 igrafx_mining_sdk-2.31.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:43:55.106099 igrafx_mining_sdk-2.31.4/igrafx_mining_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/igrafx_mining_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/igrafx_mining_sdk/api_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    17408 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/igrafx_mining_sdk/column_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/igrafx_mining_sdk/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/igrafx_mining_sdk/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/igrafx_mining_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/igrafx_mining_sdk/workgroup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:43:55.106099 igrafx_mining_sdk-2.31.4/igrafx_mining_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-19 12:43:55.000000 igrafx_mining_sdk-2.31.4/igrafx_mining_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-19 12:43:55.000000 igrafx_mining_sdk-2.31.4/igrafx_mining_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:43:55.000000 igrafx_mining_sdk-2.31.4/igrafx_mining_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 12:43:55.000000 igrafx_mining_sdk-2.31.4/igrafx_mining_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 12:43:55.110100 igrafx_mining_sdk-2.31.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 12:43:41.000000 igrafx_mining_sdk-2.31.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:43:55.110100 igrafx_mining_sdk-2.31.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:43:55.106099 igrafx_mining_sdk-2.31.4/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:43:55.110100 igrafx_mining_sdk-2.31.4/tests/data/graphs/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/tests/data/graphs/graph.json
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/tests/data/graphs/graph_with_invalid_edges.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:43:55.110100 igrafx_mining_sdk-2.31.4/tests/data/tables/
--rw-r--r--   0 runner    (1001) docker     (127)    27136 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/tests/data/tables/p2pShortExcel.xls
--rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/tests/data/tables/p2pShortExcel.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/tests/data/tables/testdata.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/tests/test_00_workgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/tests/test_01_column_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    35094 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/tests/test_02_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/tests/test_03_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/tests/test_04_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-19 12:43:32.000000 igrafx_mining_sdk-2.31.4/tests/test_05_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:25:46.698876 igrafx_mining_sdk-2.31.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-30 15:25:46.698876 igrafx_mining_sdk-2.31.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:25:46.698876 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/api_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17408 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/column_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/datasource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:25:46.698876 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/dtos/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/dtos/PredictionErrorStatusDto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/dtos/PredictionLaunchErrorStatusDto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/dtos/PredictionPossibilityDto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/dtos/PredictionStatusDto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/dtos/PredictionTaskTypeDto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/dtos/WorkflowStatusDto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/dtos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23177 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/workgroup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:25:46.698876 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-30 15:25:46.000000 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-30 15:25:46.000000 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:25:46.000000 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 15:25:46.000000 igrafx_mining_sdk-2.31.5/igrafx_mining_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:25:46.698876 igrafx_mining_sdk-2.31.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-30 15:25:29.000000 igrafx_mining_sdk-2.31.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:25:46.698876 igrafx_mining_sdk-2.31.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:25:46.694877 igrafx_mining_sdk-2.31.5/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:25:46.698876 igrafx_mining_sdk-2.31.5/tests/data/graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/tests/data/graphs/graph.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/tests/data/graphs/graph_with_invalid_edges.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:25:46.698876 igrafx_mining_sdk-2.31.5/tests/data/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)    27136 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/tests/data/tables/p2pShortExcel.xls
+-rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/tests/data/tables/p2pShortExcel.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/tests/data/tables/testdata.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/tests/test_00_workgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/tests/test_01_column_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34953 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/tests/test_02_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/tests/test_03_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/tests/test_04_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-30 15:25:20.000000 igrafx_mining_sdk-2.31.5/tests/test_05_delete.py
```

### Comparing `igrafx_mining_sdk-2.31.4/LICENSE` & `igrafx_mining_sdk-2.31.5/LICENSE`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.4/PKG-INFO` & `igrafx_mining_sdk-2.31.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igrafx_mining_sdk
-Version: 2.31.4
+Version: 2.31.5
 Summary: The iGrafx P360 Live Mining SDK is an open source application that can be used to manage your mining projects.
 Home-page: https://www.igrafx.com
 Author: iGrafx
 Author-email: contact@igrafx.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `igrafx_mining_sdk-2.31.4/README.md` & `igrafx_mining_sdk-2.31.5/README.md`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.4/igrafx_mining_sdk/__init__.py` & `igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.4/igrafx_mining_sdk/api_connector.py` & `igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/api_connector.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.4/igrafx_mining_sdk/column_mapping.py` & `igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/column_mapping.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.4/igrafx_mining_sdk/datasource.py` & `igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/datasource.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.4/igrafx_mining_sdk/graph.py` & `igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/graph.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.4/igrafx_mining_sdk/project.py` & `igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import json
 import os
 import random
 from igrafx_mining_sdk.graph import Graph, GraphInstance
 from igrafx_mining_sdk.column_mapping import FileStructure, ColumnMapping
 from igrafx_mining_sdk.datasource import Datasource
 from igrafx_mining_sdk.api_connector import APIConnector
-from igrafx_mining_sdk.dtos.PredictionStatusDto import PredictionStatusDto
-from igrafx_mining_sdk.dtos.PredictionTaskTypeDto import PredictionTaskTypeDto
-from igrafx_mining_sdk.dtos.PredictionLaunchErrorStatusDto import PredictionLaunchErrorStatusDto
-from igrafx_mining_sdk.dtos.PredictionPossibilityDto import PredictionPossibilityDto
-from igrafx_mining_sdk.dtos.PredictionErrorStatusDto import PredictionErrorStatusDto
-from igrafx_mining_sdk.dtos.WorkflowStatusDto import WorkflowStatusDto
+from igrafx_mining_sdk.dtos import PredictionStatusDto
+from igrafx_mining_sdk.dtos import PredictionTaskTypeDto
+from igrafx_mining_sdk.dtos import PredictionLaunchErrorStatusDto
+from igrafx_mining_sdk.dtos import PredictionPossibilityDto
+from igrafx_mining_sdk.dtos import PredictionErrorStatusDto
+from igrafx_mining_sdk.dtos import WorkflowStatusDto
 import uuid
 from enum import Enum
 from datetime import datetime
 from typing import List, Optional, Dict, Union
 from collections import OrderedDict
```

### Comparing `igrafx_mining_sdk-2.31.4/igrafx_mining_sdk/workgroup.py` & `igrafx_mining_sdk-2.31.5/igrafx_mining_sdk/workgroup.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.4/igrafx_mining_sdk.egg-info/PKG-INFO` & `igrafx_mining_sdk-2.31.5/igrafx_mining_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igrafx-mining-sdk
-Version: 2.31.4
+Version: 2.31.5
 Summary: The iGrafx P360 Live Mining SDK is an open source application that can be used to manage your mining projects.
 Home-page: https://www.igrafx.com
 Author: iGrafx
 Author-email: contact@igrafx.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `igrafx_mining_sdk-2.31.4/pyproject.toml` & `igrafx_mining_sdk-2.31.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "igrafx_mining_sdk"
-version = "2.31.4"
+version = "2.31.5"
 description = "The iGrafx P360 Live Mining SDK is an open source application that can be used to manage your mining projects."
 authors = ["iGrafx <contact@igrafx.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.grafx.com/"
 repository = "https://github.com/igrafx/mining-python-sdk"
 keywords = ["process mining"]
```

### Comparing `igrafx_mining_sdk-2.31.4/setup.py` & `igrafx_mining_sdk-2.31.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 }
 
 # Extract requirements
 requirements = list(pyproject_data['tool']['poetry']['dependencies'].values())
 
 setup(
     name="igrafx_mining_sdk",
-    version='2.31.4',
+    version='2.31.5',
     description=package_infos['__doc__'],
     long_description=open("README.md", 'r').read(),
     long_description_content_type='text/markdown',
     url="https://www.igrafx.com",
     author=package_infos['__author__'],
     author_email=package_infos['__email__'],
     packages=find_packages(),
```

### Comparing `igrafx_mining_sdk-2.31.4/tests/data/graphs/graph.json` & `igrafx_mining_sdk-2.31.5/tests/data/graphs/graph.json`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.4/tests/data/graphs/graph_with_invalid_edges.json` & `igrafx_mining_sdk-2.31.5/tests/data/graphs/graph_with_invalid_edges.json`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.4/tests/data/tables/p2pShortExcel.xls` & `igrafx_mining_sdk-2.31.5/tests/data/tables/p2pShortExcel.xls`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.4/tests/data/tables/p2pShortExcel.xlsx` & `igrafx_mining_sdk-2.31.5/tests/data/tables/p2pShortExcel.xlsx`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.4/tests/test_00_workgroup.py` & `igrafx_mining_sdk-2.31.5/tests/test_00_workgroup.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.4/tests/test_01_column_mapping.py` & `igrafx_mining_sdk-2.31.5/tests/test_01_column_mapping.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.4/tests/test_02_project.py` & `igrafx_mining_sdk-2.31.5/tests/test_02_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 # https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
 import time
 import pytest
 from pathlib import Path
 from igrafx_mining_sdk.project import FileStructure
 from igrafx_mining_sdk.column_mapping import Column, ColumnType, ColumnMapping, FileType
 from igrafx_mining_sdk.datasource import Datasource
-from igrafx_mining_sdk.dtos.PredictionStatusDto import PredictionStatusDto
-from igrafx_mining_sdk.dtos.PredictionTaskTypeDto import PredictionTaskTypeDto
-from igrafx_mining_sdk.dtos.PredictionLaunchErrorStatusDto import PredictionLaunchErrorStatusDto
-from igrafx_mining_sdk.dtos.PredictionPossibilityDto import PredictionPossibilityDto
-from igrafx_mining_sdk.dtos.PredictionErrorStatusDto import PredictionErrorStatusDto
-from igrafx_mining_sdk.dtos.WorkflowStatusDto import WorkflowStatusDto
+from igrafx_mining_sdk.dtos import PredictionStatusDto
+from igrafx_mining_sdk.dtos import PredictionTaskTypeDto
+from igrafx_mining_sdk.dtos import PredictionLaunchErrorStatusDto
+from igrafx_mining_sdk.dtos import PredictionPossibilityDto
+from igrafx_mining_sdk.dtos import PredictionErrorStatusDto
+from igrafx_mining_sdk.dtos import WorkflowStatusDto
 from igrafx_mining_sdk.api_connector import APIConnector
 from unittest.mock import MagicMock
 import uuid
 from datetime import datetime
 
 
 class TestProject:
```

### Comparing `igrafx_mining_sdk-2.31.4/tests/test_03_datasource.py` & `igrafx_mining_sdk-2.31.5/tests/test_03_datasource.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.4/tests/test_04_graph.py` & `igrafx_mining_sdk-2.31.5/tests/test_04_graph.py`

 * *Files identical despite different names*

