# Comparing `tmp/grpcio-csds-1.63.0rc1.tar.gz` & `tmp/grpcio_csds-1.63.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-csds-1.63.0rc1.tar", last modified: Fri Apr 12 06:40:48 2024, max compression
+gzip compressed data, was "grpcio_csds-1.63.0rc2.tar", last modified: Wed Apr 17 21:53:55 2024, max compression
```

## Comparing `grpcio-csds-1.63.0rc1.tar` & `grpcio_csds-1.63.0rc2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:48.947079 grpcio-csds-1.63.0rc1/
--rw-r--r--   0 root         (0) root         (0)    29687 2024-04-12 06:29:42.000000 grpcio-csds-1.63.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       94 2024-04-12 06:29:27.000000 grpcio-csds-1.63.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1087 2024-04-12 06:40:48.947079 grpcio-csds-1.63.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      511 2024-04-12 06:29:27.000000 grpcio-csds-1.63.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:48.947079 grpcio-csds-1.63.0rc1/grpc_csds/
--rw-r--r--   0 root         (0) root         (0)     2051 2024-04-12 06:29:27.000000 grpcio-csds-1.63.0rc1/grpc_csds/__init__.py
--rw-r--r--   0 root         (0) root         (0)      700 2024-04-12 06:29:27.000000 grpcio-csds-1.63.0rc1/grpc_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:48.947079 grpcio-csds-1.63.0rc1/grpcio_csds.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1087 2024-04-12 06:40:48.000000 grpcio-csds-1.63.0rc1/grpcio_csds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      275 2024-04-12 06:40:48.000000 grpcio-csds-1.63.0rc1/grpcio_csds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 06:40:48.000000 grpcio-csds-1.63.0rc1/grpcio_csds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-04-12 06:40:48.000000 grpcio-csds-1.63.0rc1/grpcio_csds.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-12 06:40:48.000000 grpcio-csds-1.63.0rc1/grpcio_csds.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 06:40:48.947079 grpcio-csds-1.63.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1953 2024-04-12 06:29:27.000000 grpcio-csds-1.63.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:55.615553 grpcio_csds-1.63.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    29687 2024-04-17 21:17:14.000000 grpcio_csds-1.63.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       94 2024-04-17 21:16:56.000000 grpcio_csds-1.63.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-17 21:53:55.615553 grpcio_csds-1.63.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      511 2024-04-17 21:16:56.000000 grpcio_csds-1.63.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:55.611553 grpcio_csds-1.63.0rc2/grpc_csds/
+-rw-r--r--   0 root         (0) root         (0)     2051 2024-04-17 21:16:56.000000 grpcio_csds-1.63.0rc2/grpc_csds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      700 2024-04-17 21:16:56.000000 grpcio_csds-1.63.0rc2/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:55.615553 grpcio_csds-1.63.0rc2/grpcio_csds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-17 21:53:55.000000 grpcio_csds-1.63.0rc2/grpcio_csds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      275 2024-04-17 21:53:55.000000 grpcio_csds-1.63.0rc2/grpcio_csds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 21:53:55.000000 grpcio_csds-1.63.0rc2/grpcio_csds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-17 21:53:55.000000 grpcio_csds-1.63.0rc2/grpcio_csds.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-17 21:53:55.000000 grpcio_csds-1.63.0rc2/grpcio_csds.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 21:53:55.615553 grpcio_csds-1.63.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1961 2024-04-17 21:16:56.000000 grpcio_csds-1.63.0rc2/setup.py
```

### Comparing `grpcio-csds-1.63.0rc1/LICENSE` & `grpcio_csds-1.63.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `grpcio-csds-1.63.0rc1/PKG-INFO` & `grpcio_csds-1.63.0rc2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: grpcio-csds
-Version: 1.63.0rc1
+Version: 1.63.0rc2
 Summary: xDS configuration dump library
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: protobuf>=4.21.6
-Requires-Dist: xds-protos==1.63.0rc1
-Requires-Dist: grpcio>=1.63.0rc1
+Requires-Dist: protobuf<6.0dev,>=5.26.1
+Requires-Dist: xds-protos==1.63.0rc2
+Requires-Dist: grpcio>=1.63.0rc2
 
 gRPC Python Client Status Discovery Service package
 ===================================================
 
 CSDS is part of the Envoy xDS protocol:
 https://www.envoyproxy.io/docs/envoy/latest/api-v3/service/status/v3/csds.proto.
 It allows the gRPC application to programmatically expose the received traffic
```

### Comparing `grpcio-csds-1.63.0rc1/grpc_csds/__init__.py` & `grpcio_csds-1.63.0rc2/grpc_csds/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-csds-1.63.0rc1/grpc_version.py` & `grpcio_csds-1.63.0rc2/grpc_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # AUTO-GENERATED FROM `$REPO_ROOT/templates/src/python/grpcio_csds/grpc_version.py.template`!!!
 
-VERSION = '1.63.0rc1'
+VERSION = '1.63.0rc2'
```

### Comparing `grpcio-csds-1.63.0rc1/grpcio_csds.egg-info/PKG-INFO` & `grpcio_csds-1.63.0rc2/grpcio_csds.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: grpcio-csds
-Version: 1.63.0rc1
+Version: 1.63.0rc2
 Summary: xDS configuration dump library
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: protobuf>=4.21.6
-Requires-Dist: xds-protos==1.63.0rc1
-Requires-Dist: grpcio>=1.63.0rc1
+Requires-Dist: protobuf<6.0dev,>=5.26.1
+Requires-Dist: xds-protos==1.63.0rc2
+Requires-Dist: grpcio>=1.63.0rc2
 
 gRPC Python Client Status Discovery Service package
 ===================================================
 
 CSDS is part of the Envoy xDS protocol:
 https://www.envoyproxy.io/docs/envoy/latest/api-v3/service/status/v3/csds.proto.
 It allows the gRPC application to programmatically expose the received traffic
```

### Comparing `grpcio-csds-1.63.0rc1/setup.py` & `grpcio_csds-1.63.0rc2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ]
 
 PACKAGE_DIRECTORIES = {
     "": ".",
 }
 
 INSTALL_REQUIRES = (
-    "protobuf>=4.21.6",
+    "protobuf>=5.26.1,<6.0dev",
     f"xds-protos=={grpc_version.VERSION}",
     f"grpcio>={grpc_version.VERSION}",
 )
 SETUP_REQUIRES = INSTALL_REQUIRES
 
 setuptools.setup(
     name="grpcio-csds",
```

