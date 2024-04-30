# Comparing `tmp/openfeature_sdk-0.6.1.tar.gz` & `tmp/openfeature_sdk-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfeature_sdk-0.6.1.tar", last modified: Wed Mar 27 13:11:53 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `openfeature_sdk-0.6.1.tar` & `openfeature_sdk-0.7.0.tar`

### file list

```diff
@@ -1,42 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:11:53.224595 openfeature_sdk-0.6.1/
--rw-r--r--   0 root         (0) root         (0)    11323 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    27713 2024-03-27 13:11:53.224595 openfeature_sdk-0.6.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14122 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:11:53.220595 openfeature_sdk-0.6.1/openfeature/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:11:53.220595 openfeature_sdk-0.6.1/openfeature/_backports/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/_backports/__init__.py
--rw-r--r--   0 root         (0) root         (0)      285 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/_backports/strenum.py
--rw-r--r--   0 root         (0) root         (0)     2574 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/_event_support.py
--rw-r--r--   0 root         (0) root         (0)     2215 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/api.py
--rw-r--r--   0 root         (0) root         (0)    15934 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/client.py
--rw-r--r--   0 root         (0) root         (0)      539 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/evaluation_context.py
--rw-r--r--   0 root         (0) root         (0)     1935 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/event.py
--rw-r--r--   0 root         (0) root         (0)     6219 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/exception.py
--rw-r--r--   0 root         (0) root         (0)     1876 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/flag_evaluation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:11:53.220595 openfeature_sdk-0.6.1/openfeature/hook/
--rw-r--r--   0 root         (0) root         (0)     3982 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/hook/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4309 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/hook/_hook_support.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:11:53.220595 openfeature_sdk-0.6.1/openfeature/immutable_dict/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/immutable_dict/__init__.py
--rw-r--r--   0 root         (0) root         (0)      955 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/immutable_dict/mapping_proxy_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:11:53.220595 openfeature_sdk-0.6.1/openfeature/provider/
--rw-r--r--   0 root         (0) root         (0)     1744 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/provider/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3709 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/provider/in_memory_provider.py
--rw-r--r--   0 root         (0) root         (0)       77 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/provider/metadata.py
--rw-r--r--   0 root         (0) root         (0)      199 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/provider/no_op_metadata.py
--rw-r--r--   0 root         (0) root         (0)     2430 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/provider/no_op_provider.py
--rw-r--r--   0 root         (0) root         (0)     2713 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/provider/provider.py
--rw-r--r--   0 root         (0) root         (0)     4044 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/provider/registry.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/openfeature/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:11:53.224595 openfeature_sdk-0.6.1/openfeature_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)    27713 2024-03-27 13:11:53.000000 openfeature_sdk-0.6.1/openfeature_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      971 2024-03-27 13:11:53.000000 openfeature_sdk-0.6.1/openfeature_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 13:11:53.000000 openfeature_sdk-0.6.1/openfeature_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-03-27 13:11:53.000000 openfeature_sdk-0.6.1/openfeature_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-03-27 13:11:53.000000 openfeature_sdk-0.6.1/openfeature_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1795 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-27 13:11:53.224595 openfeature_sdk-0.6.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 13:11:53.224595 openfeature_sdk-0.6.1/tests/
--rw-r--r--   0 root         (0) root         (0)     8289 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)    10859 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)     1394 2024-03-27 13:11:40.000000 openfeature_sdk-0.6.1/tests/test_flag_evaluation.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/.gitmodules
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/.release-please-manifest.json
+-rw-r--r--   0        0        0    21014 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/release-please-config.json
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/renovate.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/.github/codeql-config.yml
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/.github/workflows/lint-pr.yml
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/_event_support.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/api.py
+-rw-r--r--   0        0        0    16047 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/client.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/evaluation_context.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/event.py
+-rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/exception.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/flag_evaluation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/_backports/__init__.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/_backports/strenum.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/hook/__init__.py
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/hook/_hook_support.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/immutable_dict/__init__.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/immutable_dict/mapping_proxy_type.py
+-rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/provider/__init__.py
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/provider/_registry.py
+-rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/provider/in_memory_provider.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/provider/metadata.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/provider/no_op_metadata.py
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/provider/no_op_provider.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/openfeature/provider/provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0     9578 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/tests/test_api.py
+-rw-r--r--   0        0        0    10859 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/tests/test_client.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/tests/test_flag_evaluation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/tests/evaluation_context/__init__.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/tests/evaluation_context/test_evaluation_context.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/tests/features/__init__.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/tests/features/data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/tests/features/steps/__init__.py
+-rw-r--r--   0        0        0    11194 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/tests/features/steps/steps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/tests/hook/__init__.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/tests/hook/conftest.py
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/tests/hook/test_hook_support.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/tests/provider/__init__.py
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/tests/provider/test_in_memory_provider.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/tests/provider/test_no_op_provider.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/.gitignore
+-rw-r--r--   0        0        0    11323 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/LICENSE
+-rw-r--r--   0        0        0    14072 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/README.md
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    27522 2020-02-02 00:00:00.000000 openfeature_sdk-0.7.0/PKG-INFO
```

### Comparing `openfeature_sdk-0.6.1/LICENSE` & `openfeature_sdk-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openfeature_sdk-0.6.1/PKG-INFO` & `openfeature_sdk-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: openfeature_sdk
-Version: 0.6.1
+Version: 0.7.0
 Summary: Standardizing Feature Flagging for Everyone
+Project-URL: Homepage, https://github.com/open-feature/python-sdk
 Author-email: OpenFeature <openfeature-core@groups.io>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -200,26 +201,21 @@
                http://www.apache.org/licenses/LICENSE-2.0
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
-Project-URL: Homepage, https://github.com/open-feature/python-sdk
-Keywords: openfeature,feature,flags,toggles
+License-File: LICENSE
+Keywords: feature,flags,openfeature,toggles
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Provides-Extra: dev
-Requires-Dist: pip-tools; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
 
 <!-- markdownlint-disable MD033 -->
 <!-- x-hide-in-docs-start -->
 <p align="center">
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/open-feature/community/0e23508c163a6a1ac8c0ced3e4bd78faafe627c7/assets/logo/horizontal/white/openfeature-horizontal-white.svg" />
     <img align="center" alt="OpenFeature Logo" src="https://raw.githubusercontent.com/open-feature/community/0e23508c163a6a1ac8c0ced3e4bd78faafe627c7/assets/logo/horizontal/black/openfeature-horizontal-black.svg" />
@@ -234,16 +230,16 @@
 
   <a href="https://github.com/open-feature/spec/releases/tag/v0.8.0">
     <img alt="Specification" src="https://img.shields.io/static/v1?label=Specification&message=v0.8.0&color=red&style=for-the-badge" />
   </a>
 
   <!-- x-release-please-start-version -->
 
-  <a href="https://github.com/open-feature/python-sdk/releases/tag/v0.6.1">
-    <img alt="Latest version" src="https://img.shields.io/static/v1?label=release&message=v0.6.1&color=blue&style=for-the-badge" />
+  <a href="https://github.com/open-feature/python-sdk/releases/tag/v0.7.0">
+    <img alt="Latest version" src="https://img.shields.io/static/v1?label=release&message=v0.7.0&color=blue&style=for-the-badge" />
   </a>
 
   <!-- x-release-please-end -->
   <br/>
   <a href="https://github.com/open-feature/python-sdk/actions/workflows/merge.yml">
     <img alt="Build status" src="https://github.com/open-feature/python-sdk/actions/workflows/build.yml/badge.svg" />
   </a>
@@ -275,21 +271,21 @@
 ### Install
 
 <!---x-release-please-start-version-->
 
 #### Pip install
 
 ```bash
-pip install openfeature-sdk==0.6.1
+pip install openfeature-sdk==0.7.0
 ```
 
 #### requirements.txt
 
 ```bash
-openfeature-sdk==0.6.1
+openfeature-sdk==0.7.0
 ```
 
 ```python
 pip install -r requirements.txt
 ```
 
 <!---x-release-please-end-->
@@ -474,16 +470,15 @@
 
 ```python
 from typing import List, Optional, Union
 
 from openfeature.evaluation_context import EvaluationContext
 from openfeature.flag_evaluation import FlagResolutionDetails
 from openfeature.hook import Hook
-from openfeature.provider.metadata import Metadata
-from openfeature.provider.provider import AbstractProvider
+from openfeature.provider import AbstractProvider, Metadata
 
 class MyProvider(AbstractProvider):
     def get_metadata(self) -> Metadata:
         ...
 
     def get_provider_hooks(self) -> List[Hook]:
         return []
```

### Comparing `openfeature_sdk-0.6.1/README.md` & `openfeature_sdk-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
   <a href="https://github.com/open-feature/spec/releases/tag/v0.8.0">
     <img alt="Specification" src="https://img.shields.io/static/v1?label=Specification&message=v0.8.0&color=red&style=for-the-badge" />
   </a>
 
   <!-- x-release-please-start-version -->
 
-  <a href="https://github.com/open-feature/python-sdk/releases/tag/v0.6.1">
-    <img alt="Latest version" src="https://img.shields.io/static/v1?label=release&message=v0.6.1&color=blue&style=for-the-badge" />
+  <a href="https://github.com/open-feature/python-sdk/releases/tag/v0.7.0">
+    <img alt="Latest version" src="https://img.shields.io/static/v1?label=release&message=v0.7.0&color=blue&style=for-the-badge" />
   </a>
 
   <!-- x-release-please-end -->
   <br/>
   <a href="https://github.com/open-feature/python-sdk/actions/workflows/merge.yml">
     <img alt="Build status" src="https://github.com/open-feature/python-sdk/actions/workflows/build.yml/badge.svg" />
   </a>
@@ -56,21 +56,21 @@
 ### Install
 
 <!---x-release-please-start-version-->
 
 #### Pip install
 
 ```bash
-pip install openfeature-sdk==0.6.1
+pip install openfeature-sdk==0.7.0
 ```
 
 #### requirements.txt
 
 ```bash
-openfeature-sdk==0.6.1
+openfeature-sdk==0.7.0
 ```
 
 ```python
 pip install -r requirements.txt
 ```
 
 <!---x-release-please-end-->
@@ -255,16 +255,15 @@
 
 ```python
 from typing import List, Optional, Union
 
 from openfeature.evaluation_context import EvaluationContext
 from openfeature.flag_evaluation import FlagResolutionDetails
 from openfeature.hook import Hook
-from openfeature.provider.metadata import Metadata
-from openfeature.provider.provider import AbstractProvider
+from openfeature.provider import AbstractProvider, Metadata
 
 class MyProvider(AbstractProvider):
     def get_metadata(self) -> Metadata:
         ...
 
     def get_provider_hooks(self) -> List[Hook]:
         return []
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
                       ********** OOppeennFFeeaattuurree PPyytthhoonn SSDDKK **********
                         _[_S_p_e_c_i_f_i_c_a_t_i_o_n_]_[_L_a_t_e_s_t_ _v_e_r_s_i_o_n_]
            _[_B_u_i_l_d_ _s_t_a_t_u_s_]_[_C_o_d_e_c_o_v_]_[_M_i_n_ _p_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_R_e_p_o_ _s_t_a_t_u_s_]
 [OpenFeature](https://openfeature.dev) is an open specification that provides a
 vendor-agnostic, community-driven API for feature flagging that works with your
 favorite feature flag management tool. ## ð Quick start ### Requirements -
 Python 3.8+ ### Install #### Pip install ```bash pip install openfeature-
-sdk==0.6.1 ``` #### requirements.txt ```bash openfeature-sdk==0.6.1 ```
+sdk==0.7.0 ``` #### requirements.txt ```bash openfeature-sdk==0.7.0 ```
 ```python pip install -r requirements.txt ``` ### Usage ```python from
 openfeature import api from openfeature.provider.in_memory_provider import
 InMemoryFlag, InMemoryProvider # flags defined in memory my_flags =
 { "v2_enabled": InMemoryFlag("on", {"on": True, "off": False}) } # configure a
 provider api.set_provider(InMemoryProvider(my_flags)) # create a client client
 = api.get_client() # get a bool flag value flag_value =
 client.get_boolean_value("v2_enabled", False) print("Value: " + str
@@ -102,17 +102,16 @@
 dependency. This can be a new repository or included in [the existing contrib
 repository](https://github.com/open-feature/python-sdk-contrib) available under
 the OpenFeature organization. Youâll then need to write the provider by
 implementing the `AbstractProvider` class exported by the OpenFeature SDK.
 ```python from typing import List, Optional, Union from
 openfeature.evaluation_context import EvaluationContext from
 openfeature.flag_evaluation import FlagResolutionDetails from openfeature.hook
-import Hook from openfeature.provider.metadata import Metadata from
-openfeature.provider.provider import AbstractProvider class MyProvider
-(AbstractProvider): def get_metadata(self) -> Metadata: ... def
+import Hook from openfeature.provider import AbstractProvider, Metadata class
+MyProvider(AbstractProvider): def get_metadata(self) -> Metadata: ... def
 get_provider_hooks(self) -> List[Hook]: return [] def resolve_boolean_details
 ( self, flag_key: str, default_value: bool, evaluation_context: Optional
 [EvaluationContext] = None, ) -> FlagResolutionDetails[bool]: ... def
 resolve_string_details( self, flag_key: str, default_value: str,
 evaluation_context: Optional[EvaluationContext] = None, ) -
 > FlagResolutionDetails[str]: ... def resolve_integer_details( self, flag_key:
 str, default_value: int, evaluation_context: Optional[EvaluationContext] =
```

### Comparing `openfeature_sdk-0.6.1/openfeature/_event_support.py` & `openfeature_sdk-0.7.0/openfeature/_event_support.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from openfeature.event import (
     EventDetails,
     EventHandler,
     ProviderEvent,
     ProviderEventDetails,
 )
-from openfeature.provider import FeatureProvider
+from openfeature.provider import FeatureProvider, ProviderStatus
 
 if TYPE_CHECKING:
     from openfeature.client import OpenFeatureClient
 
 
 _global_handlers: Dict[ProviderEvent, List[EventHandler]] = defaultdict(list)
 _client_handlers: Dict[OpenFeatureClient, Dict[ProviderEvent, List[EventHandler]]] = (
@@ -76,14 +76,20 @@
         if client.provider == provider:
             run_client_handlers(client, event, details)
 
 
 def _run_immediate_handler(
     client: OpenFeatureClient, event: ProviderEvent, handler: EventHandler
 ) -> None:
-    if event == ProviderEvent.from_provider_status(client.get_provider_status()):
+    status_to_event = {
+        ProviderStatus.READY: ProviderEvent.PROVIDER_READY,
+        ProviderStatus.ERROR: ProviderEvent.PROVIDER_ERROR,
+        ProviderStatus.FATAL: ProviderEvent.PROVIDER_ERROR,
+        ProviderStatus.STALE: ProviderEvent.PROVIDER_STALE,
+    }
+    if event == status_to_event.get(client.get_provider_status()):
         handler(EventDetails(provider_name=client.provider.get_metadata().name))
 
 
 def clear() -> None:
     _global_handlers.clear()
     _client_handlers.clear()
```

### Comparing `openfeature_sdk-0.6.1/openfeature/api.py` & `openfeature_sdk-0.7.0/openfeature/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,46 +6,59 @@
 from openfeature.event import (
     EventHandler,
     ProviderEvent,
 )
 from openfeature.exception import GeneralError
 from openfeature.hook import Hook
 from openfeature.provider import FeatureProvider
+from openfeature.provider._registry import provider_registry
 from openfeature.provider.metadata import Metadata
-from openfeature.provider.registry import ProviderRegistry
+
+__all__ = [
+    "get_client",
+    "set_provider",
+    "clear_providers",
+    "get_provider_metadata",
+    "get_evaluation_context",
+    "set_evaluation_context",
+    "add_hooks",
+    "clear_hooks",
+    "get_hooks",
+    "shutdown",
+    "add_handler",
+    "remove_handler",
+]
 
 _evaluation_context = EvaluationContext()
 
 _hooks: typing.List[Hook] = []
 
-_provider_registry: ProviderRegistry = ProviderRegistry()
-
 
 def get_client(
     domain: typing.Optional[str] = None, version: typing.Optional[str] = None
 ) -> OpenFeatureClient:
     return OpenFeatureClient(domain=domain, version=version)
 
 
 def set_provider(
     provider: FeatureProvider, domain: typing.Optional[str] = None
 ) -> None:
     if domain is None:
-        _provider_registry.set_default_provider(provider)
+        provider_registry.set_default_provider(provider)
     else:
-        _provider_registry.set_provider(domain, provider)
+        provider_registry.set_provider(domain, provider)
 
 
 def clear_providers() -> None:
-    _provider_registry.clear_providers()
+    provider_registry.clear_providers()
     _event_support.clear()
 
 
 def get_provider_metadata(domain: typing.Optional[str] = None) -> Metadata:
-    return _provider_registry.get_provider(domain).get_metadata()
+    return provider_registry.get_provider(domain).get_metadata()
 
 
 def get_evaluation_context() -> EvaluationContext:
     global _evaluation_context
     return _evaluation_context
 
 
@@ -68,15 +81,15 @@
 
 def get_hooks() -> typing.List[Hook]:
     global _hooks
     return _hooks
 
 
 def shutdown() -> None:
-    _provider_registry.shutdown()
+    provider_registry.shutdown()
 
 
 def add_handler(event: ProviderEvent, handler: EventHandler) -> None:
     _event_support.add_global_handler(event, handler)
 
 
 def remove_handler(event: ProviderEvent, handler: EventHandler) -> None:
```

### Comparing `openfeature_sdk-0.6.1/openfeature/client.py` & `openfeature_sdk-0.7.0/openfeature/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 from openfeature.hook._hook_support import (
     after_all_hooks,
     after_hooks,
     before_hooks,
     error_hooks,
 )
 from openfeature.provider import FeatureProvider, ProviderStatus
+from openfeature.provider._registry import provider_registry
+
+__all__ = [
+    "ClientMetadata",
+    "OpenFeatureClient",
+]
 
 logger = logging.getLogger("openfeature")
 
 GetDetailCallable = typing.Union[
     typing.Callable[
         [str, bool, typing.Optional[EvaluationContext]], FlagResolutionDetails[bool]
     ],
@@ -78,18 +84,18 @@
         self.domain = domain
         self.version = version
         self.context = context or EvaluationContext()
         self.hooks = hooks or []
 
     @property
     def provider(self) -> FeatureProvider:
-        return api._provider_registry.get_provider(self.domain)
+        return provider_registry.get_provider(self.domain)
 
     def get_provider_status(self) -> ProviderStatus:
-        return api._provider_registry.get_provider_status(self.provider)
+        return provider_registry.get_provider_status(self.provider)
 
     def get_metadata(self) -> ClientMetadata:
         return ClientMetadata(domain=self.domain)
 
     def add_hooks(self, hooks: typing.List[Hook]) -> None:
         self.hooks = self.hooks + hooks
```

### Comparing `openfeature_sdk-0.6.1/openfeature/evaluation_context.py` & `openfeature_sdk-0.7.0/openfeature/evaluation_context.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import typing
 from dataclasses import dataclass, field
 
+__all__ = ["EvaluationContext"]
+
 
 @dataclass
 class EvaluationContext:
     targeting_key: typing.Optional[str] = None
     attributes: dict = field(default_factory=dict)
 
     def merge(self, ctx2: "EvaluationContext") -> "EvaluationContext":
```

### Comparing `openfeature_sdk-0.6.1/openfeature/event.py` & `openfeature_sdk-0.7.0/openfeature/event.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,24 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import Callable, ClassVar, Dict, List, Optional, Union
+from typing import Callable, Dict, List, Optional, Union
 
 from openfeature.exception import ErrorCode
-from openfeature.provider import ProviderStatus
+
+__all__ = ["ProviderEvent", "ProviderEventDetails", "EventDetails", "EventHandler"]
 
 
 class ProviderEvent(Enum):
     PROVIDER_READY = "PROVIDER_READY"
     PROVIDER_CONFIGURATION_CHANGED = "PROVIDER_CONFIGURATION_CHANGED"
     PROVIDER_ERROR = "PROVIDER_ERROR"
-    PROVIDER_FATAL = "PROVIDER_FATAL"
     PROVIDER_STALE = "PROVIDER_STALE"
 
-    __status__: ClassVar[Dict[ProviderStatus, str]] = {
-        ProviderStatus.READY: PROVIDER_READY,
-        ProviderStatus.ERROR: PROVIDER_ERROR,
-        ProviderStatus.FATAL: PROVIDER_FATAL,
-        ProviderStatus.STALE: PROVIDER_STALE,
-    }
-
-    @classmethod
-    def from_provider_status(cls, status: ProviderStatus) -> Optional[ProviderEvent]:
-        value = ProviderEvent.__status__.get(status)
-        return ProviderEvent[value] if value else None
-
 
 @dataclass
 class ProviderEventDetails:
     flags_changed: Optional[List[str]] = None
     message: Optional[str] = None
     error_code: Optional[ErrorCode] = None
     metadata: Dict[str, Union[bool, str, int, float]] = field(default_factory=dict)
```

### Comparing `openfeature_sdk-0.6.1/openfeature/exception.py` & `openfeature_sdk-0.7.0/openfeature/exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 from __future__ import annotations
 
 import typing
 from collections.abc import Mapping
 from enum import Enum
 
+__all__ = [
+    "OpenFeatureError",
+    "ProviderNotReadyError",
+    "ProviderFatalError",
+    "FlagNotFoundError",
+    "GeneralError",
+    "ParseError",
+    "TypeMismatchError",
+    "TargetingKeyMissingError",
+    "InvalidContextError",
+    "ErrorCode",
+]
+
 
 class OpenFeatureError(Exception):
     """
     A generic open feature exception, this exception should not be raised. Instead
     the more specific exceptions extending this one should be used.
     """
```

### Comparing `openfeature_sdk-0.6.1/openfeature/flag_evaluation.py` & `openfeature_sdk-0.7.0/openfeature/flag_evaluation.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,24 @@
 from openfeature.exception import ErrorCode
 
 if typing.TYPE_CHECKING:  # pragma: no cover
     # resolves a circular dependency in type annotations
     from openfeature.hook import Hook, HookHints
 
 
+__all__ = [
+    "FlagType",
+    "Reason",
+    "FlagMetadata",
+    "FlagEvaluationDetails",
+    "FlagEvaluationOptions",
+    "FlagResolutionDetails",
+]
+
+
 class FlagType(StrEnum):
     BOOLEAN = "BOOLEAN"
     STRING = "STRING"
     OBJECT = "OBJECT"
     FLOAT = "FLOAT"
     INTEGER = "INTEGER"
```

### Comparing `openfeature_sdk-0.6.1/openfeature/hook/__init__.py` & `openfeature_sdk-0.7.0/openfeature/hook/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from openfeature.evaluation_context import EvaluationContext
 from openfeature.flag_evaluation import FlagEvaluationDetails, FlagType
 
 if TYPE_CHECKING:
     from openfeature.client import ClientMetadata
     from openfeature.provider.metadata import Metadata
 
+__all__ = ["HookType", "HookContext", "HookHints", "Hook"]
+
 
 class HookType(Enum):
     BEFORE = "before"
     AFTER = "after"
     FINALLY_AFTER = "finally_after"
     ERROR = "error"
```

### Comparing `openfeature_sdk-0.6.1/openfeature/hook/_hook_support.py` & `openfeature_sdk-0.7.0/openfeature/hook/_hook_support.py`

 * *Files identical despite different names*

### Comparing `openfeature_sdk-0.6.1/openfeature/immutable_dict/mapping_proxy_type.py` & `openfeature_sdk-0.7.0/openfeature/immutable_dict/mapping_proxy_type.py`

 * *Files identical despite different names*

### Comparing `openfeature_sdk-0.6.1/openfeature/provider/__init__.py` & `openfeature_sdk-0.7.0/openfeature/provider/no_op_provider.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,77 @@
 import typing
-from enum import Enum
 
 from openfeature.evaluation_context import EvaluationContext
-from openfeature.flag_evaluation import FlagResolutionDetails
+from openfeature.flag_evaluation import FlagResolutionDetails, Reason
 from openfeature.hook import Hook
+from openfeature.provider import AbstractProvider, Metadata
+from openfeature.provider.no_op_metadata import NoOpMetadata
 
-from .metadata import Metadata
+PASSED_IN_DEFAULT = "Passed in default"
 
 
-class ProviderStatus(Enum):
-    NOT_READY = "NOT_READY"
-    READY = "READY"
-    ERROR = "ERROR"
-    STALE = "STALE"
-    FATAL = "FATAL"
+class NoOpProvider(AbstractProvider):
+    def get_metadata(self) -> Metadata:
+        return NoOpMetadata()
 
-
-class FeatureProvider(typing.Protocol):  # pragma: no cover
-    def initialize(self, evaluation_context: EvaluationContext) -> None: ...
-
-    def shutdown(self) -> None: ...
-
-    def get_metadata(self) -> Metadata: ...
-
-    def get_provider_hooks(self) -> typing.List[Hook]: ...
+    def get_provider_hooks(self) -> typing.List[Hook]:
+        return []
 
     def resolve_boolean_details(
         self,
         flag_key: str,
         default_value: bool,
         evaluation_context: typing.Optional[EvaluationContext] = None,
-    ) -> FlagResolutionDetails[bool]: ...
+    ) -> FlagResolutionDetails[bool]:
+        return FlagResolutionDetails(
+            value=default_value,
+            reason=Reason.DEFAULT,
+            variant=PASSED_IN_DEFAULT,
+        )
 
     def resolve_string_details(
         self,
         flag_key: str,
         default_value: str,
         evaluation_context: typing.Optional[EvaluationContext] = None,
-    ) -> FlagResolutionDetails[str]: ...
+    ) -> FlagResolutionDetails[str]:
+        return FlagResolutionDetails(
+            value=default_value,
+            reason=Reason.DEFAULT,
+            variant=PASSED_IN_DEFAULT,
+        )
 
     def resolve_integer_details(
         self,
         flag_key: str,
         default_value: int,
         evaluation_context: typing.Optional[EvaluationContext] = None,
-    ) -> FlagResolutionDetails[int]: ...
+    ) -> FlagResolutionDetails[int]:
+        return FlagResolutionDetails(
+            value=default_value,
+            reason=Reason.DEFAULT,
+            variant=PASSED_IN_DEFAULT,
+        )
 
     def resolve_float_details(
         self,
         flag_key: str,
         default_value: float,
         evaluation_context: typing.Optional[EvaluationContext] = None,
-    ) -> FlagResolutionDetails[float]: ...
+    ) -> FlagResolutionDetails[float]:
+        return FlagResolutionDetails(
+            value=default_value,
+            reason=Reason.DEFAULT,
+            variant=PASSED_IN_DEFAULT,
+        )
 
     def resolve_object_details(
         self,
         flag_key: str,
         default_value: typing.Union[dict, list],
         evaluation_context: typing.Optional[EvaluationContext] = None,
-    ) -> FlagResolutionDetails[typing.Union[dict, list]]: ...
+    ) -> FlagResolutionDetails[typing.Union[dict, list]]:
+        return FlagResolutionDetails(
+            value=default_value,
+            reason=Reason.DEFAULT,
+            variant=PASSED_IN_DEFAULT,
+        )
```

### Comparing `openfeature_sdk-0.6.1/openfeature/provider/in_memory_provider.py` & `openfeature_sdk-0.7.0/openfeature/provider/in_memory_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from dataclasses import dataclass, field
 
 from openfeature._backports.strenum import StrEnum
 from openfeature.evaluation_context import EvaluationContext
 from openfeature.exception import FlagNotFoundError
 from openfeature.flag_evaluation import FlagMetadata, FlagResolutionDetails, Reason
 from openfeature.hook import Hook
-from openfeature.provider.metadata import Metadata
-from openfeature.provider.provider import AbstractProvider
+from openfeature.provider import AbstractProvider, Metadata
 
 PASSED_IN_DEFAULT = "Passed in default"
 
 
 @dataclass
 class InMemoryMetadata(Metadata):
     name: str = "In-Memory Provider"
```

### Comparing `openfeature_sdk-0.6.1/pyproject.toml` & `openfeature_sdk-0.7.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pyproject.toml
 [build-system]
-requires      = ["setuptools>=61.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
 [project]
 name = "openfeature_sdk"
-version = "0.6.1"
+version = "0.7.0"
 description = "Standardizing Feature Flagging for Everyone"
 readme = "README.md"
 authors = [{ name = "OpenFeature", email = "openfeature-core@groups.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
@@ -20,20 +20,53 @@
     "feature",
     "flags",
     "toggles",
 ]
 dependencies = []
 requires-python = ">=3.8"
 
-[project.optional-dependencies]
-dev = ["pip-tools", "pytest", "pre-commit"]
-
 [project.urls]
 Homepage = "https://github.com/open-feature/python-sdk"
 
+[tool.hatch]
+
+[tool.hatch.envs.default]
+dependencies = [
+    "behave",
+    "coverage[toml]>=6.5",
+    "pytest",
+]
+
+[tool.hatch.envs.default.scripts]
+test = "pytest {args:tests}"
+test-cov = "coverage run -m pytest {args:tests}"
+cov-report = [
+    "coverage xml",
+]
+cov = [
+    "test-cov",
+    "cov-report",
+]
+e2e = [
+    "git submodule update --init",
+    "cp test-harness/features/evaluation.feature tests/features/",
+    "behave tests/features/",
+    "rm tests/features/*.feature",
+]
+
+[tool.hatch.build.targets.sdist]
+exclude = [
+    ".gitignore",
+    "test-harness",
+    "venv",
+]
+
+[tool.hatch.build.targets.wheel]
+packages = ["openfeature"]
+
 [tool.mypy]
 files = "openfeature"
 namespace_packages = true
 explicit_package_bases = true
 local_partial_types = true # will become the new default from version 2
 pretty = true
 strict = true
@@ -85,10 +118,7 @@
 [tool.ruff.lint.pylint]
 max-args = 6
 max-statements = 30
 
 [tool.ruff.lint.pyupgrade]
 # Preserve types, even if a file imports `from __future__ import annotations`.
 keep-runtime-typing = true
-
-[tool.setuptools.package-data]
-openfeature = ["py.typed"]
```

### Comparing `openfeature_sdk-0.6.1/tests/test_api.py` & `openfeature_sdk-0.7.0/tests/test_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     remove_handler,
     set_evaluation_context,
     set_provider,
     shutdown,
 )
 from openfeature.evaluation_context import EvaluationContext
 from openfeature.event import EventDetails, ProviderEvent, ProviderEventDetails
-from openfeature.exception import ErrorCode, GeneralError
+from openfeature.exception import ErrorCode, GeneralError, ProviderFatalError
 from openfeature.hook import Hook
-from openfeature.provider import FeatureProvider, Metadata
+from openfeature.provider import FeatureProvider, Metadata, ProviderStatus
 from openfeature.provider.no_op_provider import NoOpProvider
 
 
 def test_should_not_raise_exception_with_noop_client():
     # Given
     # No provider has been set
     # When
@@ -299,17 +299,61 @@
     # Then
     spy.provider_ready.assert_called_once()
 
 
 def test_provider_ready_handlers_run_if_provider_initialize_function_terminates_normally():
     # Given
     provider = NoOpProvider()
-    set_provider(provider)
 
     spy = MagicMock()
     add_handler(ProviderEvent.PROVIDER_READY, spy.provider_ready)
+    spy.reset_mock()  # reset the mock to avoid counting the immediate call on subscribe
 
     # When
-    provider.initialize(get_evaluation_context())
+    set_provider(provider)
 
     # Then
     spy.provider_ready.assert_called_once()
+
+
+def test_provider_error_handlers_run_if_provider_initialize_function_terminates_abnormally():
+    # Given
+    provider = MagicMock(spec=FeatureProvider)
+    provider.initialize.side_effect = ProviderFatalError()
+
+    spy = MagicMock()
+    add_handler(ProviderEvent.PROVIDER_ERROR, spy.provider_error)
+
+    # When
+    set_provider(provider)
+
+    # Then
+    spy.provider_error.assert_called_once()
+
+
+def test_provider_status_is_updated_after_provider_emits_event():
+    # Given
+    provider = NoOpProvider()
+    set_provider(provider)
+    client = get_client()
+
+    # When
+    provider.emit_provider_error(ProviderEventDetails(error_code=ErrorCode.GENERAL))
+    # Then
+    assert client.get_provider_status() == ProviderStatus.ERROR
+
+    # When
+    provider.emit_provider_error(
+        ProviderEventDetails(error_code=ErrorCode.PROVIDER_FATAL)
+    )
+    # Then
+    assert client.get_provider_status() == ProviderStatus.FATAL
+
+    # When
+    provider.emit_provider_stale(ProviderEventDetails())
+    # Then
+    assert client.get_provider_status() == ProviderStatus.STALE
+
+    # When
+    provider.emit_provider_ready(ProviderEventDetails())
+    # Then
+    assert client.get_provider_status() == ProviderStatus.READY
```

### Comparing `openfeature_sdk-0.6.1/tests/test_client.py` & `openfeature_sdk-0.7.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `openfeature_sdk-0.6.1/tests/test_flag_evaluation.py` & `openfeature_sdk-0.7.0/tests/test_flag_evaluation.py`

 * *Files identical despite different names*

