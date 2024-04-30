# Comparing `tmp/grpcio-admin-1.63.0rc1.tar.gz` & `tmp/grpcio_admin-1.63.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-admin-1.63.0rc1.tar", last modified: Fri Apr 12 06:40:51 2024, max compression
+gzip compressed data, was "grpcio_admin-1.63.0rc2.tar", last modified: Wed Apr 17 21:53:58 2024, max compression
```

## Comparing `grpcio-admin-1.63.0rc1.tar` & `grpcio_admin-1.63.0rc2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:51.743329 grpcio-admin-1.63.0rc1/
--rw-r--r--   0 root         (0) root         (0)    29687 2024-04-12 06:29:42.000000 grpcio-admin-1.63.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       95 2024-04-12 06:29:27.000000 grpcio-admin-1.63.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1420 2024-04-12 06:40:51.743329 grpcio-admin-1.63.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      865 2024-04-12 06:29:27.000000 grpcio-admin-1.63.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:51.739329 grpcio-admin-1.63.0rc1/grpc_admin/
--rw-r--r--   0 root         (0) root         (0)     1620 2024-04-12 06:29:27.000000 grpcio-admin-1.63.0rc1/grpc_admin/__init__.py
--rw-r--r--   0 root         (0) root         (0)      701 2024-04-12 06:29:27.000000 grpcio-admin-1.63.0rc1/grpc_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:40:51.739329 grpcio-admin-1.63.0rc1/grpcio_admin.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1420 2024-04-12 06:40:51.000000 grpcio-admin-1.63.0rc1/grpcio_admin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      282 2024-04-12 06:40:51.000000 grpcio-admin-1.63.0rc1/grpcio_admin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 06:40:51.000000 grpcio-admin-1.63.0rc1/grpcio_admin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2024-04-12 06:40:51.000000 grpcio-admin-1.63.0rc1/grpcio_admin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-12 06:40:51.000000 grpcio-admin-1.63.0rc1/grpcio_admin.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 06:40:51.743329 grpcio-admin-1.63.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1997 2024-04-12 06:29:27.000000 grpcio-admin-1.63.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:58.635860 grpcio_admin-1.63.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    29687 2024-04-17 21:17:14.000000 grpcio_admin-1.63.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       95 2024-04-17 21:16:56.000000 grpcio_admin-1.63.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1420 2024-04-17 21:53:58.635860 grpcio_admin-1.63.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      865 2024-04-17 21:16:56.000000 grpcio_admin-1.63.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:58.631859 grpcio_admin-1.63.0rc2/grpc_admin/
+-rw-r--r--   0 root         (0) root         (0)     1620 2024-04-17 21:16:56.000000 grpcio_admin-1.63.0rc2/grpc_admin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      701 2024-04-17 21:16:56.000000 grpcio_admin-1.63.0rc2/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:53:58.635860 grpcio_admin-1.63.0rc2/grpcio_admin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1420 2024-04-17 21:53:58.000000 grpcio_admin-1.63.0rc2/grpcio_admin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      282 2024-04-17 21:53:58.000000 grpcio_admin-1.63.0rc2/grpcio_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 21:53:58.000000 grpcio_admin-1.63.0rc2/grpcio_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-04-17 21:53:58.000000 grpcio_admin-1.63.0rc2/grpcio_admin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-17 21:53:58.000000 grpcio_admin-1.63.0rc2/grpcio_admin.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 21:53:58.635860 grpcio_admin-1.63.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1997 2024-04-17 21:16:56.000000 grpcio_admin-1.63.0rc2/setup.py
```

### Comparing `grpcio-admin-1.63.0rc1/LICENSE` & `grpcio_admin-1.63.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `grpcio-admin-1.63.0rc1/PKG-INFO` & `grpcio_admin-1.63.0rc2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: grpcio-admin
-Version: 1.63.0rc1
+Version: 1.63.0rc2
 Summary: a collection of admin services
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
-Requires-Dist: grpcio-channelz>=1.63.0rc1
-Requires-Dist: grpcio-csds>=1.63.0rc1
+Requires-Dist: grpcio-channelz>=1.63.0rc2
+Requires-Dist: grpcio-csds>=1.63.0rc2
 
 gRPC Python Admin Interface Package
 ===================================
 
 Debugging gRPC library can be a complex task. There are many configurations and
 internal states, which will affect the behavior of the library. This Python
 package will be the collection of admin services that are exposing debug
```

### Comparing `grpcio-admin-1.63.0rc1/README.rst` & `grpcio_admin-1.63.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `grpcio-admin-1.63.0rc1/grpc_admin/__init__.py` & `grpcio_admin-1.63.0rc2/grpc_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-admin-1.63.0rc1/grpc_version.py` & `grpcio_admin-1.63.0rc2/grpc_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # AUTO-GENERATED FROM `$REPO_ROOT/templates/src/python/grpcio_admin/grpc_version.py.template`!!!
 
-VERSION = '1.63.0rc1'
+VERSION = '1.63.0rc2'
```

### Comparing `grpcio-admin-1.63.0rc1/grpcio_admin.egg-info/PKG-INFO` & `grpcio_admin-1.63.0rc2/grpcio_admin.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: grpcio-admin
-Version: 1.63.0rc1
+Version: 1.63.0rc2
 Summary: a collection of admin services
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
-Requires-Dist: grpcio-channelz>=1.63.0rc1
-Requires-Dist: grpcio-csds>=1.63.0rc1
+Requires-Dist: grpcio-channelz>=1.63.0rc2
+Requires-Dist: grpcio-csds>=1.63.0rc2
 
 gRPC Python Admin Interface Package
 ===================================
 
 Debugging gRPC library can be a complex task. There are many configurations and
 internal states, which will affect the behavior of the library. This Python
 package will be the collection of admin services that are exposing debug
```

### Comparing `grpcio-admin-1.63.0rc1/setup.py` & `grpcio_admin-1.63.0rc2/setup.py`

 * *Files identical despite different names*

