# Comparing `tmp/grpcio-testing-1.63.0rc1.tar.gz` & `tmp/grpcio_testing-1.63.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-testing-1.63.0rc1.tar", last modified: Fri Apr 12 06:40:43 2024, max compression
+gzip compressed data, was "grpcio_testing-1.63.0rc2.tar", last modified: Wed Apr 17 21:53:48 2024, max compression
```

## Comparing `grpcio-testing-1.63.0rc1.tar` & `grpcio_testing-1.63.0rc2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:43.014548 grpcio-testing-1.63.0rc1/
--rw-r--r--   0 root         (0) root         (0)    29687 2024-04-12 06:40:42.000000 grpcio-testing-1.63.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       97 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      578 2024-04-12 06:40:43.014548 grpcio-testing-1.63.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      266 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:43.006547 grpcio-testing-1.63.0rc1/grpc_testing/
--rw-r--r--   0 root         (0) root         (0)    22799 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:43.010548 grpcio-testing-1.63.0rc1/grpc_testing/_channel/
--rw-r--r--   0 root         (0) root         (0)      887 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_channel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2984 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_channel/_channel.py
--rw-r--r--   0 root         (0) root         (0)     3920 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_channel/_channel_rpc.py
--rw-r--r--   0 root         (0) root         (0)     1782 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_channel/_channel_state.py
--rw-r--r--   0 root         (0) root         (0)     8036 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_channel/_invocation.py
--rw-r--r--   0 root         (0) root         (0)     4933 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_channel/_multi_callable.py
--rw-r--r--   0 root         (0) root         (0)     7246 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_channel/_rpc_state.py
--rw-r--r--   0 root         (0) root         (0)     4406 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:43.010548 grpcio-testing-1.63.0rc1/grpc_testing/_server/
--rw-r--r--   0 root         (0) root         (0)      782 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7428 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_server/_handler.py
--rw-r--r--   0 root         (0) root         (0)     5273 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_server/_rpc.py
--rw-r--r--   0 root         (0) root         (0)     6096 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_server/_server.py
--rw-r--r--   0 root         (0) root         (0)     2460 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_server/_server_rpc.py
--rw-r--r--   0 root         (0) root         (0)     2846 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_server/_service.py
--rw-r--r--   0 root         (0) root         (0)     2631 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_server/_servicer_context.py
--rw-r--r--   0 root         (0) root         (0)     7256 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_testing/_time.py
--rw-r--r--   0 root         (0) root         (0)      700 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/grpc_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:43.014548 grpcio-testing-1.63.0rc1/grpcio_testing.egg-info/
--rw-r--r--   0 root         (0) root         (0)      578 2024-04-12 06:40:42.000000 grpcio-testing-1.63.0rc1/grpcio_testing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1416 2024-04-12 06:40:42.000000 grpcio-testing-1.63.0rc1/grpcio_testing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 06:40:42.000000 grpcio-testing-1.63.0rc1/grpcio_testing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-04-12 06:40:42.000000 grpcio-testing-1.63.0rc1/grpcio_testing.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-12 06:40:42.000000 grpcio-testing-1.63.0rc1/grpcio_testing.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 06:40:43.014548 grpcio-testing-1.63.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2320 2024-04-12 06:29:27.000000 grpcio-testing-1.63.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:48.346816 grpcio_testing-1.63.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    29687 2024-04-17 21:53:48.000000 grpcio_testing-1.63.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       97 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      586 2024-04-17 21:53:48.346816 grpcio_testing-1.63.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      266 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:48.334815 grpcio_testing-1.63.0rc2/grpc_testing/
+-rw-r--r--   0 root         (0) root         (0)    22799 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/grpc_testing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:48.334815 grpcio_testing-1.63.0rc2/grpc_testing/_channel/
+-rw-r--r--   0 root         (0) root         (0)      887 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/grpc_testing/_channel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2984 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/grpc_testing/_channel/_channel.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/grpc_testing/_channel/_channel_rpc.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/grpc_testing/_channel/_channel_state.py
+-rw-r--r--   0 root         (0) root         (0)     8036 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/grpc_testing/_channel/_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     4933 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/grpc_testing/_channel/_multi_callable.py
+-rw-r--r--   0 root         (0) root         (0)     7246 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/grpc_testing/_channel/_rpc_state.py
+-rw-r--r--   0 root         (0) root         (0)     4406 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/grpc_testing/_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:48.338815 grpcio_testing-1.63.0rc2/grpc_testing/_server/
+-rw-r--r--   0 root         (0) root         (0)      782 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/grpc_testing/_server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7428 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/grpc_testing/_server/_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5273 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/grpc_testing/_server/_rpc.py
+-rw-r--r--   0 root         (0) root         (0)     6096 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/grpc_testing/_server/_server.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/grpc_testing/_server/_server_rpc.py
+-rw-r--r--   0 root         (0) root         (0)     2846 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/grpc_testing/_server/_service.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/grpc_testing/_server/_servicer_context.py
+-rw-r--r--   0 root         (0) root         (0)     7256 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/grpc_testing/_time.py
+-rw-r--r--   0 root         (0) root         (0)      700 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:48.338815 grpcio_testing-1.63.0rc2/grpcio_testing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      586 2024-04-17 21:53:48.000000 grpcio_testing-1.63.0rc2/grpcio_testing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1416 2024-04-17 21:53:48.000000 grpcio_testing-1.63.0rc2/grpcio_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 21:53:48.000000 grpcio_testing-1.63.0rc2/grpcio_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-17 21:53:48.000000 grpcio_testing-1.63.0rc2/grpcio_testing.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-17 21:53:48.000000 grpcio_testing-1.63.0rc2/grpcio_testing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 21:53:48.346816 grpcio_testing-1.63.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2328 2024-04-17 21:16:56.000000 grpcio_testing-1.63.0rc2/setup.py
```

### Comparing `grpcio-testing-1.63.0rc1/LICENSE` & `grpcio_testing-1.63.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.63.0rc1/PKG-INFO` & `grpcio_testing-1.63.0rc2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: grpcio-testing
-Version: 1.63.0rc1
+Version: 1.63.0rc2
 Summary: Testing utilities for gRPC Python
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 License-File: LICENSE
-Requires-Dist: protobuf>=4.21.6
-Requires-Dist: grpcio>=1.63.0rc1
+Requires-Dist: protobuf<6.0dev,>=5.26.1
+Requires-Dist: grpcio>=1.63.0rc2
 
 gRPC Python Testing Package
 ===========================
 
 Testing utilities for gRPC Python
 
 Supported Python Versions
```

### Comparing `grpcio-testing-1.63.0rc1/grpc_testing/__init__.py` & `grpcio_testing-1.63.0rc2/grpc_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.63.0rc1/grpc_testing/_channel/__init__.py` & `grpcio_testing-1.63.0rc2/grpc_testing/_channel/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.63.0rc1/grpc_testing/_channel/_channel.py` & `grpcio_testing-1.63.0rc2/grpc_testing/_channel/_channel.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.63.0rc1/grpc_testing/_channel/_channel_rpc.py` & `grpcio_testing-1.63.0rc2/grpc_testing/_channel/_channel_rpc.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.63.0rc1/grpc_testing/_channel/_channel_state.py` & `grpcio_testing-1.63.0rc2/grpc_testing/_channel/_channel_state.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.63.0rc1/grpc_testing/_channel/_invocation.py` & `grpcio_testing-1.63.0rc2/grpc_testing/_channel/_invocation.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.63.0rc1/grpc_testing/_channel/_multi_callable.py` & `grpcio_testing-1.63.0rc2/grpc_testing/_channel/_multi_callable.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.63.0rc1/grpc_testing/_channel/_rpc_state.py` & `grpcio_testing-1.63.0rc2/grpc_testing/_channel/_rpc_state.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.63.0rc1/grpc_testing/_common.py` & `grpcio_testing-1.63.0rc2/grpc_testing/_common.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.63.0rc1/grpc_testing/_server/__init__.py` & `grpcio_testing-1.63.0rc2/grpc_testing/_server/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.63.0rc1/grpc_testing/_server/_handler.py` & `grpcio_testing-1.63.0rc2/grpc_testing/_server/_handler.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.63.0rc1/grpc_testing/_server/_rpc.py` & `grpcio_testing-1.63.0rc2/grpc_testing/_server/_rpc.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.63.0rc1/grpc_testing/_server/_server.py` & `grpcio_testing-1.63.0rc2/grpc_testing/_server/_server.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.63.0rc1/grpc_testing/_server/_server_rpc.py` & `grpcio_testing-1.63.0rc2/grpc_testing/_server/_server_rpc.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.63.0rc1/grpc_testing/_server/_service.py` & `grpcio_testing-1.63.0rc2/grpc_testing/_server/_service.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.63.0rc1/grpc_testing/_server/_servicer_context.py` & `grpcio_testing-1.63.0rc2/grpc_testing/_server/_servicer_context.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.63.0rc1/grpc_testing/_time.py` & `grpcio_testing-1.63.0rc2/grpc_testing/_time.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.63.0rc1/grpc_version.py` & `grpcio_testing-1.63.0rc2/grpc_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # AUTO-GENERATED FROM `$REPO_ROOT/templates/src/python/grpcio_testing/grpc_version.py.template`!!!
 
-VERSION = '1.63.0rc1'
+VERSION = '1.63.0rc2'
```

### Comparing `grpcio-testing-1.63.0rc1/grpcio_testing.egg-info/PKG-INFO` & `grpcio_testing-1.63.0rc2/grpcio_testing.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: grpcio-testing
-Version: 1.63.0rc1
+Version: 1.63.0rc2
 Summary: Testing utilities for gRPC Python
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 License-File: LICENSE
-Requires-Dist: protobuf>=4.21.6
-Requires-Dist: grpcio>=1.63.0rc1
+Requires-Dist: protobuf<6.0dev,>=5.26.1
+Requires-Dist: grpcio>=1.63.0rc2
 
 gRPC Python Testing Package
 ===========================
 
 Testing utilities for gRPC Python
 
 Supported Python Versions
```

### Comparing `grpcio-testing-1.63.0rc1/grpcio_testing.egg-info/SOURCES.txt` & `grpcio_testing-1.63.0rc2/grpcio_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.63.0rc1/setup.py` & `grpcio_testing-1.63.0rc2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 
 PACKAGE_DIRECTORIES = {
     "": ".",
 }
 
 INSTALL_REQUIRES = (
-    "protobuf>=4.21.6",
+    "protobuf>=5.26.1,<6.0dev",
     "grpcio>={version}".format(version=grpc_version.VERSION),
 )
 
 try:
     import testing_commands as _testing_commands
 
     # we are in the build environment, otherwise the above import fails
```

