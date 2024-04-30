# Comparing `tmp/grpcio-status-1.63.0rc1.tar.gz` & `tmp/grpcio_status-1.63.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-status-1.63.0rc1.tar", last modified: Fri Apr 12 06:40:45 2024, max compression
+gzip compressed data, was "grpcio_status-1.63.0rc2.tar", last modified: Wed Apr 17 21:53:51 2024, max compression
```

## Comparing `grpcio-status-1.63.0rc1.tar` & `grpcio_status-1.63.0rc2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:45.626782 grpcio-status-1.63.0rc1/
--rw-r--r--   0 root         (0) root         (0)    29687 2024-04-12 06:40:45.000000 grpcio-status-1.63.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      140 2024-04-12 06:29:27.000000 grpcio-status-1.63.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1124 2024-04-12 06:40:45.622782 grpcio-status-1.63.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      284 2024-04-12 06:29:27.000000 grpcio-status-1.63.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:45.622782 grpcio-status-1.63.0rc1/grpc_status/
--rw-r--r--   0 root         (0) root         (0)      580 2024-04-12 06:29:27.000000 grpcio-status-1.63.0rc1/grpc_status/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-04-12 06:29:27.000000 grpcio-status-1.63.0rc1/grpc_status/_async.py
--rw-r--r--   0 root         (0) root         (0)      959 2024-04-12 06:29:27.000000 grpcio-status-1.63.0rc1/grpc_status/_common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:45.610780 grpcio-status-1.63.0rc1/grpc_status/google/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:45.622782 grpcio-status-1.63.0rc1/grpc_status/google/rpc/
--rw-r--r--   0 root         (0) root         (0)     1924 2024-04-12 06:40:45.000000 grpcio-status-1.63.0rc1/grpc_status/google/rpc/status.proto
--rw-r--r--   0 root         (0) root         (0)     2992 2024-04-12 06:29:27.000000 grpcio-status-1.63.0rc1/grpc_status/rpc_status.py
--rw-r--r--   0 root         (0) root         (0)      702 2024-04-12 06:29:27.000000 grpcio-status-1.63.0rc1/grpc_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:45.622782 grpcio-status-1.63.0rc1/grpcio_status.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1124 2024-04-12 06:40:45.000000 grpcio-status-1.63.0rc1/grpcio_status.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      473 2024-04-12 06:40:45.000000 grpcio-status-1.63.0rc1/grpcio_status.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 06:40:45.000000 grpcio-status-1.63.0rc1/grpcio_status.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-12 06:40:45.000000 grpcio-status-1.63.0rc1/grpcio_status.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-12 06:40:45.000000 grpcio-status-1.63.0rc1/grpcio_status.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 06:40:45.626782 grpcio-status-1.63.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2940 2024-04-12 06:29:27.000000 grpcio-status-1.63.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:51.487134 grpcio_status-1.63.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    29687 2024-04-17 21:53:51.000000 grpcio_status-1.63.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      140 2024-04-17 21:16:56.000000 grpcio_status-1.63.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-04-17 21:53:51.483134 grpcio_status-1.63.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      284 2024-04-17 21:16:56.000000 grpcio_status-1.63.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:51.483134 grpcio_status-1.63.0rc2/grpc_status/
+-rw-r--r--   0 root         (0) root         (0)      580 2024-04-17 21:16:56.000000 grpcio_status-1.63.0rc2/grpc_status/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-17 21:16:56.000000 grpcio_status-1.63.0rc2/grpc_status/_async.py
+-rw-r--r--   0 root         (0) root         (0)      959 2024-04-17 21:16:56.000000 grpcio_status-1.63.0rc2/grpc_status/_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:51.471133 grpcio_status-1.63.0rc2/grpc_status/google/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:51.483134 grpcio_status-1.63.0rc2/grpc_status/google/rpc/
+-rw-r--r--   0 root         (0) root         (0)     1924 2024-04-17 21:53:51.000000 grpcio_status-1.63.0rc2/grpc_status/google/rpc/status.proto
+-rw-r--r--   0 root         (0) root         (0)     2992 2024-04-17 21:16:56.000000 grpcio_status-1.63.0rc2/grpc_status/rpc_status.py
+-rw-r--r--   0 root         (0) root         (0)      702 2024-04-17 21:16:56.000000 grpcio_status-1.63.0rc2/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:51.483134 grpcio_status-1.63.0rc2/grpcio_status.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-04-17 21:53:51.000000 grpcio_status-1.63.0rc2/grpcio_status.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      473 2024-04-17 21:53:51.000000 grpcio_status-1.63.0rc2/grpcio_status.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 21:53:51.000000 grpcio_status-1.63.0rc2/grpcio_status.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       75 2024-04-17 21:53:51.000000 grpcio_status-1.63.0rc2/grpcio_status.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-17 21:53:51.000000 grpcio_status-1.63.0rc2/grpcio_status.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 21:53:51.487134 grpcio_status-1.63.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2948 2024-04-17 21:16:56.000000 grpcio_status-1.63.0rc2/setup.py
```

### Comparing `grpcio-status-1.63.0rc1/LICENSE` & `grpcio_status-1.63.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.63.0rc1/PKG-INFO` & `grpcio_status-1.63.0rc2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-status
-Version: 1.63.0rc1
+Version: 1.63.0rc2
 Summary: Status proto mapping for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: protobuf>=4.21.6
-Requires-Dist: grpcio>=1.63.0rc1
+Requires-Dist: protobuf<6.0dev,>=5.26.1
+Requires-Dist: grpcio>=1.63.0rc2
 Requires-Dist: googleapis-common-protos>=1.5.5
 
 gRPC Python Status Proto
 ===========================
 
 Reference package for GRPC Python status proto mapping.
```

### Comparing `grpcio-status-1.63.0rc1/grpc_status/__init__.py` & `grpcio_status-1.63.0rc2/grpc_status/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.63.0rc1/grpc_status/_async.py` & `grpcio_status-1.63.0rc2/grpc_status/_async.py`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.63.0rc1/grpc_status/_common.py` & `grpcio_status-1.63.0rc2/grpc_status/_common.py`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.63.0rc1/grpc_status/google/rpc/status.proto` & `grpcio_status-1.63.0rc2/grpc_status/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.63.0rc1/grpc_status/rpc_status.py` & `grpcio_status-1.63.0rc2/grpc_status/rpc_status.py`

 * *Files identical despite different names*

### Comparing `grpcio-status-1.63.0rc1/grpc_version.py` & `grpcio_status-1.63.0rc2/grpc_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # AUTO-GENERATED FROM `$REPO_ROOT/templates/src/python/grpcio_status/grpc_version.py.template`!!!
 
-VERSION = '1.63.0rc1'
+VERSION = '1.63.0rc2'
```

### Comparing `grpcio-status-1.63.0rc1/grpcio_status.egg-info/PKG-INFO` & `grpcio_status-1.63.0rc2/grpcio_status.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-status
-Version: 1.63.0rc1
+Version: 1.63.0rc2
 Summary: Status proto mapping for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: protobuf>=4.21.6
-Requires-Dist: grpcio>=1.63.0rc1
+Requires-Dist: protobuf<6.0dev,>=5.26.1
+Requires-Dist: grpcio>=1.63.0rc2
 Requires-Dist: googleapis-common-protos>=1.5.5
 
 gRPC Python Status Proto
 ===========================
 
 Reference package for GRPC Python status proto mapping.
```

### Comparing `grpcio-status-1.63.0rc1/setup.py` & `grpcio_status-1.63.0rc2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 ]
 
 PACKAGE_DIRECTORIES = {
     "": ".",
 }
 
 INSTALL_REQUIRES = (
-    "protobuf>=4.21.6",
+    "protobuf>=5.26.1,<6.0dev",
     "grpcio>={version}".format(version=grpc_version.VERSION),
     "googleapis-common-protos>=1.5.5",
 )
 
 try:
     import status_commands as _status_commands
```

