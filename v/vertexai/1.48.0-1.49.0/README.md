# Comparing `tmp/vertexai-1.48.0.tar.gz` & `tmp/vertexai-1.49.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertexai-1.48.0.tar", last modified: Wed Apr 17 22:44:02 2024, max compression
+gzip compressed data, was "vertexai-1.49.0.tar", last modified: Tue Apr 30 17:35:22 2024, max compression
```

## Comparing `vertexai-1.48.0.tar` & `vertexai-1.49.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 wuamy    (518829) primarygroup (89939)        0 2024-04-17 22:44:02.000000 vertexai-1.48.0/
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)    11358 2023-05-05 15:54:43.000000 vertexai-1.48.0/LICENSE
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)    10471 2024-04-17 22:44:02.000000 vertexai-1.48.0/PKG-INFO
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      264 2024-03-07 21:35:24.000000 vertexai-1.48.0/README.md
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      490 2024-04-06 04:10:48.000000 vertexai-1.48.0/pyproject.toml
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)       38 2024-04-17 22:44:02.000000 vertexai-1.48.0/setup.cfg
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)     7616 2024-04-17 22:43:06.000000 vertexai-1.48.0/setup.py
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      625 2024-04-17 20:52:55.000000 vertexai-1.48.0/version.py
-drwxrwxr-x   0 wuamy    (518829) primarygroup (89939)        0 2024-04-17 22:44:02.000000 vertexai-1.48.0/vertexai.egg-info/
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)    10471 2024-04-17 22:44:02.000000 vertexai-1.48.0/vertexai.egg-info/PKG-INFO
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      242 2024-04-17 22:44:02.000000 vertexai-1.48.0/vertexai.egg-info/SOURCES.txt
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)        1 2024-04-17 22:44:02.000000 vertexai-1.48.0/vertexai.egg-info/dependency_links.txt
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)        1 2024-04-17 22:44:01.000000 vertexai-1.48.0/vertexai.egg-info/not-zip-safe
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)     4129 2024-04-17 22:44:02.000000 vertexai-1.48.0/vertexai.egg-info/requires.txt
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)        8 2024-04-17 22:44:02.000000 vertexai-1.48.0/vertexai.egg-info/top_level.txt
+drwxrwxr-x   0 wuamy    (518829) primarygroup (89939)        0 2024-04-30 17:35:22.000000 vertexai-1.49.0/
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)    11358 2023-05-05 15:54:43.000000 vertexai-1.49.0/LICENSE
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)    10471 2024-04-30 17:35:22.000000 vertexai-1.49.0/PKG-INFO
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      264 2024-03-07 21:35:24.000000 vertexai-1.49.0/README.md
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      490 2024-04-06 04:10:48.000000 vertexai-1.49.0/pyproject.toml
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)       38 2024-04-30 17:35:22.000000 vertexai-1.49.0/setup.cfg
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)     7616 2024-04-18 21:09:30.000000 vertexai-1.49.0/setup.py
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      625 2024-04-29 17:38:34.000000 vertexai-1.49.0/version.py
+drwxrwxr-x   0 wuamy    (518829) primarygroup (89939)        0 2024-04-30 17:35:22.000000 vertexai-1.49.0/vertexai.egg-info/
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)    10471 2024-04-30 17:35:21.000000 vertexai-1.49.0/vertexai.egg-info/PKG-INFO
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      242 2024-04-30 17:35:22.000000 vertexai-1.49.0/vertexai.egg-info/SOURCES.txt
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)        1 2024-04-30 17:35:21.000000 vertexai-1.49.0/vertexai.egg-info/dependency_links.txt
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)        1 2024-04-30 17:35:21.000000 vertexai-1.49.0/vertexai.egg-info/not-zip-safe
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)     4129 2024-04-30 17:35:22.000000 vertexai-1.49.0/vertexai.egg-info/requires.txt
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)        8 2024-04-30 17:35:22.000000 vertexai-1.49.0/vertexai.egg-info/top_level.txt
```

### Comparing `vertexai-1.48.0/LICENSE` & `vertexai-1.49.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vertexai-1.48.0/PKG-INFO` & `vertexai-1.49.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,96 +1,96 @@
 Metadata-Version: 2.1
 Name: vertexai
-Version: 1.48.0
+Version: 1.49.0
 Summary: Please run pip install vertexai to use the Vertex SDK.
 Home-page: https://github.com/googleapis/python-aiplatform
 Author: Google LLC
 Author-email: Google LLC <googleapis-packages@google.com>
 License: Apache 2.0
 Project-URL: repository, https://github.com/googleapis/python-aiplatform.git
 Platform: Posix; MacOS X; Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: google-cloud-aiplatform[all]==1.48.0
+Requires-Dist: google-cloud-aiplatform[all]==1.49.0
 Provides-Extra: endpoint
 Requires-Dist: requests>=2.28.1; extra == "endpoint"
 Provides-Extra: full
-Requires-Dist: pyarrow>=14.0.0; python_version >= "3.12" and extra == "full"
-Requires-Dist: pandas>=1.0.0; extra == "full"
-Requires-Dist: numpy>=1.15.0; extra == "full"
-Requires-Dist: httpx<0.25.0,>=0.23.0; extra == "full"
-Requires-Dist: requests>=2.28.1; extra == "full"
-Requires-Dist: pydantic<2; extra == "full"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; python_version <= "3.11" and extra == "full"
-Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "full"
-Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "full"
 Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "full"
-Requires-Dist: immutabledict; extra == "full"
+Requires-Dist: pyyaml<7,>=5.3.1; extra == "full"
+Requires-Dist: lit-nlp==0.4.0; extra == "full"
 Requires-Dist: uvicorn[standard]>=0.16.0; extra == "full"
-Requires-Dist: cloudpickle<3.0; extra == "full"
-Requires-Dist: urllib3<1.27,>=1.21.1; extra == "full"
+Requires-Dist: pyarrow>=10.0.1; python_version == "3.11" and extra == "full"
 Requires-Dist: pyarrow>=6.0.1; extra == "full"
-Requires-Dist: google-vizier>=0.1.6; extra == "full"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
+Requires-Dist: google-cloud-bigquery; extra == "full"
+Requires-Dist: docker>=5.0.3; extra == "full"
 Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
-Requires-Dist: lit-nlp==0.4.0; extra == "full"
-Requires-Dist: fastapi<=0.109.1,>=0.71.0; extra == "full"
-Requires-Dist: cloudpickle<3.0,>=2.2.1; extra == "full"
+Requires-Dist: nest_asyncio<1.6.0,>=1.0.0; extra == "full"
 Requires-Dist: pydantic<3; extra == "full"
-Requires-Dist: docker>=5.0.3; extra == "full"
-Requires-Dist: google-cloud-logging<4.0; extra == "full"
-Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "full"
-Requires-Dist: pyyaml<7,>=5.3.1; extra == "full"
-Requires-Dist: google-cloud-bigquery-storage; extra == "full"
+Requires-Dist: pyarrow>=14.0.0; python_version >= "3.12" and extra == "full"
+Requires-Dist: immutabledict; extra == "full"
 Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version == "3.11" and extra == "full"
-Requires-Dist: pyarrow>=10.0.1; python_version == "3.11" and extra == "full"
+Requires-Dist: pydantic<2; extra == "full"
+Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "full"
 Requires-Dist: starlette>=0.17.1; extra == "full"
-Requires-Dist: google-cloud-bigquery; extra == "full"
-Requires-Dist: nest_asyncio<1.6.0,>=1.0.0; extra == "full"
+Requires-Dist: google-vizier>=0.1.6; extra == "full"
+Requires-Dist: fastapi<=0.109.1,>=0.71.0; extra == "full"
+Requires-Dist: httpx<0.25.0,>=0.23.0; extra == "full"
+Requires-Dist: requests>=2.28.1; extra == "full"
 Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "full"
+Requires-Dist: cloudpickle<3.0; extra == "full"
+Requires-Dist: google-cloud-logging<4.0; extra == "full"
+Requires-Dist: urllib3<1.27,>=1.21.1; extra == "full"
+Requires-Dist: pandas>=1.0.0; extra == "full"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
+Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "full"
+Requires-Dist: numpy>=1.15.0; extra == "full"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; python_version <= "3.11" and extra == "full"
+Requires-Dist: cloudpickle<3.0,>=2.2.1; extra == "full"
+Requires-Dist: google-cloud-bigquery-storage; extra == "full"
+Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "full"
 Provides-Extra: metadata
 Requires-Dist: pandas>=1.0.0; extra == "metadata"
 Requires-Dist: numpy>=1.15.0; extra == "metadata"
 Provides-Extra: tensorboard
 Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; python_version <= "3.11" and extra == "tensorboard"
 Provides-Extra: testing
-Requires-Dist: pyarrow>=14.0.0; python_version >= "3.12" and extra == "testing"
-Requires-Dist: pandas>=1.0.0; extra == "testing"
-Requires-Dist: numpy>=1.15.0; extra == "testing"
-Requires-Dist: httpx<0.25.0,>=0.23.0; extra == "testing"
-Requires-Dist: requests>=2.28.1; extra == "testing"
-Requires-Dist: pydantic<2; extra == "testing"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; python_version <= "3.11" and extra == "testing"
-Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "testing"
-Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "testing"
 Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "testing"
-Requires-Dist: immutabledict; extra == "testing"
+Requires-Dist: pyyaml<7,>=5.3.1; extra == "testing"
+Requires-Dist: lit-nlp==0.4.0; extra == "testing"
 Requires-Dist: uvicorn[standard]>=0.16.0; extra == "testing"
-Requires-Dist: cloudpickle<3.0; extra == "testing"
-Requires-Dist: urllib3<1.27,>=1.21.1; extra == "testing"
+Requires-Dist: pyarrow>=10.0.1; python_version == "3.11" and extra == "testing"
 Requires-Dist: pyarrow>=6.0.1; extra == "testing"
-Requires-Dist: google-vizier>=0.1.6; extra == "testing"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
+Requires-Dist: google-cloud-bigquery; extra == "testing"
+Requires-Dist: docker>=5.0.3; extra == "testing"
 Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
-Requires-Dist: lit-nlp==0.4.0; extra == "testing"
-Requires-Dist: fastapi<=0.109.1,>=0.71.0; extra == "testing"
-Requires-Dist: cloudpickle<3.0,>=2.2.1; extra == "testing"
+Requires-Dist: nest_asyncio<1.6.0,>=1.0.0; extra == "testing"
 Requires-Dist: pydantic<3; extra == "testing"
-Requires-Dist: docker>=5.0.3; extra == "testing"
-Requires-Dist: google-cloud-logging<4.0; extra == "testing"
-Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "testing"
-Requires-Dist: pyyaml<7,>=5.3.1; extra == "testing"
-Requires-Dist: google-cloud-bigquery-storage; extra == "testing"
+Requires-Dist: pyarrow>=14.0.0; python_version >= "3.12" and extra == "testing"
+Requires-Dist: immutabledict; extra == "testing"
 Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version == "3.11" and extra == "testing"
-Requires-Dist: pyarrow>=10.0.1; python_version == "3.11" and extra == "testing"
+Requires-Dist: pydantic<2; extra == "testing"
+Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "testing"
 Requires-Dist: starlette>=0.17.1; extra == "testing"
-Requires-Dist: google-cloud-bigquery; extra == "testing"
-Requires-Dist: nest_asyncio<1.6.0,>=1.0.0; extra == "testing"
+Requires-Dist: google-vizier>=0.1.6; extra == "testing"
+Requires-Dist: fastapi<=0.109.1,>=0.71.0; extra == "testing"
+Requires-Dist: httpx<0.25.0,>=0.23.0; extra == "testing"
+Requires-Dist: requests>=2.28.1; extra == "testing"
 Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "testing"
+Requires-Dist: cloudpickle<3.0; extra == "testing"
+Requires-Dist: google-cloud-logging<4.0; extra == "testing"
+Requires-Dist: urllib3<1.27,>=1.21.1; extra == "testing"
+Requires-Dist: pandas>=1.0.0; extra == "testing"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
+Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "testing"
+Requires-Dist: numpy>=1.15.0; extra == "testing"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; python_version <= "3.11" and extra == "testing"
+Requires-Dist: cloudpickle<3.0,>=2.2.1; extra == "testing"
+Requires-Dist: google-cloud-bigquery-storage; extra == "testing"
+Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "testing"
 Requires-Dist: tensorboard-plugin-profile<3.0.0dev,>=2.4.0; extra == "testing"
 Requires-Dist: werkzeug<2.1.0dev,>=2.0.0; extra == "testing"
 Requires-Dist: tensorflow<3.0.0dev,>=2.4.0; extra == "testing"
 Requires-Dist: bigframes; python_version >= "3.10" and extra == "testing"
 Requires-Dist: google-api-core<3.0.0,>=2.11; extra == "testing"
 Requires-Dist: grpcio-testing; extra == "testing"
 Requires-Dist: ipython; extra == "testing"
```

### Comparing `vertexai-1.48.0/setup.py` & `vertexai-1.49.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2022 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertexai-1.48.0/version.py` & `vertexai-1.49.0/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "1.48.0"
+__version__ = "1.49.0"
```

### Comparing `vertexai-1.48.0/vertexai.egg-info/PKG-INFO` & `vertexai-1.49.0/vertexai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,96 +1,96 @@
 Metadata-Version: 2.1
 Name: vertexai
-Version: 1.48.0
+Version: 1.49.0
 Summary: Please run pip install vertexai to use the Vertex SDK.
 Home-page: https://github.com/googleapis/python-aiplatform
 Author: Google LLC
 Author-email: Google LLC <googleapis-packages@google.com>
 License: Apache 2.0
 Project-URL: repository, https://github.com/googleapis/python-aiplatform.git
 Platform: Posix; MacOS X; Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: google-cloud-aiplatform[all]==1.48.0
+Requires-Dist: google-cloud-aiplatform[all]==1.49.0
 Provides-Extra: endpoint
 Requires-Dist: requests>=2.28.1; extra == "endpoint"
 Provides-Extra: full
-Requires-Dist: pyarrow>=14.0.0; python_version >= "3.12" and extra == "full"
-Requires-Dist: pandas>=1.0.0; extra == "full"
-Requires-Dist: numpy>=1.15.0; extra == "full"
-Requires-Dist: httpx<0.25.0,>=0.23.0; extra == "full"
-Requires-Dist: requests>=2.28.1; extra == "full"
-Requires-Dist: pydantic<2; extra == "full"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; python_version <= "3.11" and extra == "full"
-Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "full"
-Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "full"
 Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "full"
-Requires-Dist: immutabledict; extra == "full"
+Requires-Dist: pyyaml<7,>=5.3.1; extra == "full"
+Requires-Dist: lit-nlp==0.4.0; extra == "full"
 Requires-Dist: uvicorn[standard]>=0.16.0; extra == "full"
-Requires-Dist: cloudpickle<3.0; extra == "full"
-Requires-Dist: urllib3<1.27,>=1.21.1; extra == "full"
+Requires-Dist: pyarrow>=10.0.1; python_version == "3.11" and extra == "full"
 Requires-Dist: pyarrow>=6.0.1; extra == "full"
-Requires-Dist: google-vizier>=0.1.6; extra == "full"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
+Requires-Dist: google-cloud-bigquery; extra == "full"
+Requires-Dist: docker>=5.0.3; extra == "full"
 Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
-Requires-Dist: lit-nlp==0.4.0; extra == "full"
-Requires-Dist: fastapi<=0.109.1,>=0.71.0; extra == "full"
-Requires-Dist: cloudpickle<3.0,>=2.2.1; extra == "full"
+Requires-Dist: nest_asyncio<1.6.0,>=1.0.0; extra == "full"
 Requires-Dist: pydantic<3; extra == "full"
-Requires-Dist: docker>=5.0.3; extra == "full"
-Requires-Dist: google-cloud-logging<4.0; extra == "full"
-Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "full"
-Requires-Dist: pyyaml<7,>=5.3.1; extra == "full"
-Requires-Dist: google-cloud-bigquery-storage; extra == "full"
+Requires-Dist: pyarrow>=14.0.0; python_version >= "3.12" and extra == "full"
+Requires-Dist: immutabledict; extra == "full"
 Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version == "3.11" and extra == "full"
-Requires-Dist: pyarrow>=10.0.1; python_version == "3.11" and extra == "full"
+Requires-Dist: pydantic<2; extra == "full"
+Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "full"
 Requires-Dist: starlette>=0.17.1; extra == "full"
-Requires-Dist: google-cloud-bigquery; extra == "full"
-Requires-Dist: nest_asyncio<1.6.0,>=1.0.0; extra == "full"
+Requires-Dist: google-vizier>=0.1.6; extra == "full"
+Requires-Dist: fastapi<=0.109.1,>=0.71.0; extra == "full"
+Requires-Dist: httpx<0.25.0,>=0.23.0; extra == "full"
+Requires-Dist: requests>=2.28.1; extra == "full"
 Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "full"
+Requires-Dist: cloudpickle<3.0; extra == "full"
+Requires-Dist: google-cloud-logging<4.0; extra == "full"
+Requires-Dist: urllib3<1.27,>=1.21.1; extra == "full"
+Requires-Dist: pandas>=1.0.0; extra == "full"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
+Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "full"
+Requires-Dist: numpy>=1.15.0; extra == "full"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; python_version <= "3.11" and extra == "full"
+Requires-Dist: cloudpickle<3.0,>=2.2.1; extra == "full"
+Requires-Dist: google-cloud-bigquery-storage; extra == "full"
+Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "full"
 Provides-Extra: metadata
 Requires-Dist: pandas>=1.0.0; extra == "metadata"
 Requires-Dist: numpy>=1.15.0; extra == "metadata"
 Provides-Extra: tensorboard
 Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; python_version <= "3.11" and extra == "tensorboard"
 Provides-Extra: testing
-Requires-Dist: pyarrow>=14.0.0; python_version >= "3.12" and extra == "testing"
-Requires-Dist: pandas>=1.0.0; extra == "testing"
-Requires-Dist: numpy>=1.15.0; extra == "testing"
-Requires-Dist: httpx<0.25.0,>=0.23.0; extra == "testing"
-Requires-Dist: requests>=2.28.1; extra == "testing"
-Requires-Dist: pydantic<2; extra == "testing"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; python_version <= "3.11" and extra == "testing"
-Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "testing"
-Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "testing"
 Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "testing"
-Requires-Dist: immutabledict; extra == "testing"
+Requires-Dist: pyyaml<7,>=5.3.1; extra == "testing"
+Requires-Dist: lit-nlp==0.4.0; extra == "testing"
 Requires-Dist: uvicorn[standard]>=0.16.0; extra == "testing"
-Requires-Dist: cloudpickle<3.0; extra == "testing"
-Requires-Dist: urllib3<1.27,>=1.21.1; extra == "testing"
+Requires-Dist: pyarrow>=10.0.1; python_version == "3.11" and extra == "testing"
 Requires-Dist: pyarrow>=6.0.1; extra == "testing"
-Requires-Dist: google-vizier>=0.1.6; extra == "testing"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
+Requires-Dist: google-cloud-bigquery; extra == "testing"
+Requires-Dist: docker>=5.0.3; extra == "testing"
 Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
-Requires-Dist: lit-nlp==0.4.0; extra == "testing"
-Requires-Dist: fastapi<=0.109.1,>=0.71.0; extra == "testing"
-Requires-Dist: cloudpickle<3.0,>=2.2.1; extra == "testing"
+Requires-Dist: nest_asyncio<1.6.0,>=1.0.0; extra == "testing"
 Requires-Dist: pydantic<3; extra == "testing"
-Requires-Dist: docker>=5.0.3; extra == "testing"
-Requires-Dist: google-cloud-logging<4.0; extra == "testing"
-Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "testing"
-Requires-Dist: pyyaml<7,>=5.3.1; extra == "testing"
-Requires-Dist: google-cloud-bigquery-storage; extra == "testing"
+Requires-Dist: pyarrow>=14.0.0; python_version >= "3.12" and extra == "testing"
+Requires-Dist: immutabledict; extra == "testing"
 Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version == "3.11" and extra == "testing"
-Requires-Dist: pyarrow>=10.0.1; python_version == "3.11" and extra == "testing"
+Requires-Dist: pydantic<2; extra == "testing"
+Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "testing"
 Requires-Dist: starlette>=0.17.1; extra == "testing"
-Requires-Dist: google-cloud-bigquery; extra == "testing"
-Requires-Dist: nest_asyncio<1.6.0,>=1.0.0; extra == "testing"
+Requires-Dist: google-vizier>=0.1.6; extra == "testing"
+Requires-Dist: fastapi<=0.109.1,>=0.71.0; extra == "testing"
+Requires-Dist: httpx<0.25.0,>=0.23.0; extra == "testing"
+Requires-Dist: requests>=2.28.1; extra == "testing"
 Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "testing"
+Requires-Dist: cloudpickle<3.0; extra == "testing"
+Requires-Dist: google-cloud-logging<4.0; extra == "testing"
+Requires-Dist: urllib3<1.27,>=1.21.1; extra == "testing"
+Requires-Dist: pandas>=1.0.0; extra == "testing"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
+Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "testing"
+Requires-Dist: numpy>=1.15.0; extra == "testing"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; python_version <= "3.11" and extra == "testing"
+Requires-Dist: cloudpickle<3.0,>=2.2.1; extra == "testing"
+Requires-Dist: google-cloud-bigquery-storage; extra == "testing"
+Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "testing"
 Requires-Dist: tensorboard-plugin-profile<3.0.0dev,>=2.4.0; extra == "testing"
 Requires-Dist: werkzeug<2.1.0dev,>=2.0.0; extra == "testing"
 Requires-Dist: tensorflow<3.0.0dev,>=2.4.0; extra == "testing"
 Requires-Dist: bigframes; python_version >= "3.10" and extra == "testing"
 Requires-Dist: google-api-core<3.0.0,>=2.11; extra == "testing"
 Requires-Dist: grpcio-testing; extra == "testing"
 Requires-Dist: ipython; extra == "testing"
```

### Comparing `vertexai-1.48.0/vertexai.egg-info/requires.txt` & `vertexai-1.49.0/vertexai.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-google-cloud-aiplatform[all]==1.48.0
+google-cloud-aiplatform[all]==1.49.0
 
 [autologging]
 mlflow<=2.1.1,>=1.27.0
 
 [cloud_profiler]
 tensorboard-plugin-profile<3.0.0dev,>=2.4.0
 werkzeug<2.1.0dev,>=2.0.0
@@ -19,51 +19,51 @@
 [datasets:python_version >= "3.12"]
 pyarrow>=14.0.0
 
 [endpoint]
 requests>=2.28.1
 
 [full]
-pandas>=1.0.0
-numpy>=1.15.0
-httpx<0.25.0,>=0.23.0
-requests>=2.28.1
-pydantic<2
-pandas<2.2.0,>=1.0.0
-mlflow<=2.1.1,>=1.27.0
-immutabledict
+pyyaml<7,>=5.3.1
+lit-nlp==0.4.0
 uvicorn[standard]>=0.16.0
-cloudpickle<3.0
-urllib3<1.27,>=1.21.1
 pyarrow>=6.0.1
-google-vizier>=0.1.6
+google-cloud-bigquery
+docker>=5.0.3
 tensorflow<3.0.0dev,>=2.3.0
-lit-nlp==0.4.0
-fastapi<=0.109.1,>=0.71.0
-cloudpickle<3.0,>=2.2.1
+nest_asyncio<1.6.0,>=1.0.0
 pydantic<3
-docker>=5.0.3
-google-cloud-logging<4.0
+immutabledict
+pydantic<2
 explainable-ai-sdk>=1.0.0
-pyyaml<7,>=5.3.1
-google-cloud-bigquery-storage
 starlette>=0.17.1
-google-cloud-bigquery
-nest_asyncio<1.6.0,>=1.0.0
+google-vizier>=0.1.6
+fastapi<=0.109.1,>=0.71.0
+httpx<0.25.0,>=0.23.0
+requests>=2.28.1
+cloudpickle<3.0
+google-cloud-logging<4.0
+urllib3<1.27,>=1.21.1
+pandas>=1.0.0
+mlflow<=2.1.1,>=1.27.0
+numpy>=1.15.0
+cloudpickle<3.0,>=2.2.1
+google-cloud-bigquery-storage
+pandas<2.2.0,>=1.0.0
 
 [full:python_version < "3.11"]
 pyarrow<8.0dev,>=3.0.0
 ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4
 
 [full:python_version <= "3.11"]
 tensorflow<3.0.0dev,>=2.3.0
 
 [full:python_version == "3.11"]
-ray[default]<=2.9.3,>=2.5
 pyarrow>=10.0.1
+ray[default]<=2.9.3,>=2.5
 
 [full:python_version >= "3.12"]
 pyarrow>=14.0.0
 
 [langchain]
 langchain<0.2,>=0.1.13
 langchain-core<0.2
@@ -148,40 +148,40 @@
 
 [tensorboard]
 
 [tensorboard:python_version <= "3.11"]
 tensorflow<3.0.0dev,>=2.3.0
 
 [testing]
-pandas>=1.0.0
-numpy>=1.15.0
-httpx<0.25.0,>=0.23.0
-requests>=2.28.1
-pydantic<2
-pandas<2.2.0,>=1.0.0
-mlflow<=2.1.1,>=1.27.0
-immutabledict
+pyyaml<7,>=5.3.1
+lit-nlp==0.4.0
 uvicorn[standard]>=0.16.0
-cloudpickle<3.0
-urllib3<1.27,>=1.21.1
 pyarrow>=6.0.1
-google-vizier>=0.1.6
+google-cloud-bigquery
+docker>=5.0.3
 tensorflow<3.0.0dev,>=2.3.0
-lit-nlp==0.4.0
-fastapi<=0.109.1,>=0.71.0
-cloudpickle<3.0,>=2.2.1
+nest_asyncio<1.6.0,>=1.0.0
 pydantic<3
-docker>=5.0.3
-google-cloud-logging<4.0
+immutabledict
+pydantic<2
 explainable-ai-sdk>=1.0.0
-pyyaml<7,>=5.3.1
-google-cloud-bigquery-storage
 starlette>=0.17.1
-google-cloud-bigquery
-nest_asyncio<1.6.0,>=1.0.0
+google-vizier>=0.1.6
+fastapi<=0.109.1,>=0.71.0
+httpx<0.25.0,>=0.23.0
+requests>=2.28.1
+cloudpickle<3.0
+google-cloud-logging<4.0
+urllib3<1.27,>=1.21.1
+pandas>=1.0.0
+mlflow<=2.1.1,>=1.27.0
+numpy>=1.15.0
+cloudpickle<3.0,>=2.2.1
+google-cloud-bigquery-storage
+pandas<2.2.0,>=1.0.0
 tensorboard-plugin-profile<3.0.0dev,>=2.4.0
 werkzeug<2.1.0dev,>=2.0.0
 tensorflow<3.0.0dev,>=2.4.0
 google-api-core<3.0.0,>=2.11
 grpcio-testing
 ipython
 kfp<3.0.0,>=2.6.0
@@ -198,16 +198,16 @@
 
 [testing:python_version <= "3.11"]
 tensorflow<3.0.0dev,>=2.3.0
 tensorflow==2.13.0
 torch<2.1.0,>=2.0.0
 
 [testing:python_version == "3.11"]
-ray[default]<=2.9.3,>=2.5
 pyarrow>=10.0.1
+ray[default]<=2.9.3,>=2.5
 
 [testing:python_version > "3.11"]
 tensorflow==2.16.1
 torch>=2.2.0
 
 [testing:python_version >= "3.10"]
 bigframes
```

