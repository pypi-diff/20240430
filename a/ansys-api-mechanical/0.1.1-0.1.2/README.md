# Comparing `tmp/ansys-api-mechanical-0.1.1.tar.gz` & `tmp/ansys_api_mechanical-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-mechanical-0.1.1.tar", last modified: Fri Oct  6 13:31:41 2023, max compression
+gzip compressed data, was "ansys_api_mechanical-0.1.2.tar", last modified: Tue Apr 30 14:21:03 2024, max compression
```

## Comparing `ansys-api-mechanical-0.1.1.tar` & `ansys_api_mechanical-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:31:41.702946 ansys-api-mechanical-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-10-06 13:31:22.000000 ansys-api-mechanical-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2023-10-06 13:31:41.702946 ansys-api-mechanical-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2023-10-06 13:31:22.000000 ansys-api-mechanical-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-10-06 13:31:22.000000 ansys-api-mechanical-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-06 13:31:41.702946 ansys-api-mechanical-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2023-10-06 13:31:22.000000 ansys-api-mechanical-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:31:41.698946 ansys-api-mechanical-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:31:41.698946 ansys-api-mechanical-0.1.1/src/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:31:41.698946 ansys-api-mechanical-0.1.1/src/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:31:41.702946 ansys-api-mechanical-0.1.1/src/ansys/api/mechanical/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-06 13:31:22.000000 ansys-api-mechanical-0.1.1/src/ansys/api/mechanical/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-10-06 13:31:22.000000 ansys-api-mechanical-0.1.1/src/ansys/api/mechanical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 13:31:22.000000 ansys-api-mechanical-0.1.1/src/ansys/api/mechanical/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:31:41.702946 ansys-api-mechanical-0.1.1/src/ansys/api/mechanical/v0/
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2023-10-06 13:31:22.000000 ansys-api-mechanical-0.1.1/src/ansys/api/mechanical/v0/mechanical.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 13:31:41.702946 ansys-api-mechanical-0.1.1/src/ansys_api_mechanical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2023-10-06 13:31:41.000000 ansys-api-mechanical-0.1.1/src/ansys_api_mechanical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      480 2023-10-06 13:31:41.000000 ansys-api-mechanical-0.1.1/src/ansys_api_mechanical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 13:31:41.000000 ansys-api-mechanical-0.1.1/src/ansys_api_mechanical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-10-06 13:31:41.000000 ansys-api-mechanical-0.1.1/src/ansys_api_mechanical.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-10-06 13:31:41.000000 ansys-api-mechanical-0.1.1/src/ansys_api_mechanical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-06 13:31:41.000000 ansys-api-mechanical-0.1.1/src/ansys_api_mechanical.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:21:03.247810 ansys_api_mechanical-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-30 14:20:55.000000 ansys_api_mechanical-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-30 14:21:03.247810 ansys_api_mechanical-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-30 14:20:55.000000 ansys_api_mechanical-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-30 14:20:55.000000 ansys_api_mechanical-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 14:21:03.247810 ansys_api_mechanical-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-30 14:20:55.000000 ansys_api_mechanical-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:21:03.243810 ansys_api_mechanical-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:21:03.243810 ansys_api_mechanical-0.1.2/src/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:21:03.243810 ansys_api_mechanical-0.1.2/src/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:21:03.247810 ansys_api_mechanical-0.1.2/src/ansys/api/mechanical/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 14:20:55.000000 ansys_api_mechanical-0.1.2/src/ansys/api/mechanical/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-30 14:20:55.000000 ansys_api_mechanical-0.1.2/src/ansys/api/mechanical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:20:55.000000 ansys_api_mechanical-0.1.2/src/ansys/api/mechanical/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:21:03.247810 ansys_api_mechanical-0.1.2/src/ansys/api/mechanical/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-30 14:20:55.000000 ansys_api_mechanical-0.1.2/src/ansys/api/mechanical/v0/mechanical.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:21:03.247810 ansys_api_mechanical-0.1.2/src/ansys_api_mechanical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-30 14:21:03.000000 ansys_api_mechanical-0.1.2/src/ansys_api_mechanical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-30 14:21:03.000000 ansys_api_mechanical-0.1.2/src/ansys_api_mechanical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:21:03.000000 ansys_api_mechanical-0.1.2/src/ansys_api_mechanical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-30 14:21:03.000000 ansys_api_mechanical-0.1.2/src/ansys_api_mechanical.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-30 14:21:03.000000 ansys_api_mechanical-0.1.2/src/ansys_api_mechanical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 14:21:03.000000 ansys_api_mechanical-0.1.2/src/ansys_api_mechanical.egg-info/top_level.txt
```

### Comparing `ansys-api-mechanical-0.1.1/LICENSE` & `ansys_api_mechanical-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-api-mechanical-0.1.1/PKG-INFO` & `ansys_api_mechanical-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: ansys-api-mechanical
-Version: 0.1.1
-Summary: Autogenerated python gRPC interface package for ansys-api-mechanical, built on 13:31:41 on 06 October 2023
+Version: 0.1.2
+Summary: Autogenerated python gRPC interface package for ansys-api-mechanical, built on 14:21:03 on 30 April 2024
 Home-page: https://github.com/ansys/ansys-api-mechanical
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: grpcio~=1.30
-Requires-Dist: protobuf<5,>=3.19
+Requires-Dist: protobuf<6,>=3.19
 
 ### ansys-api-mechanical gRPC Interface Package
 
 This Python package contains the auto-generated gRPC Python interface files for
 Mechanical.
```

### Comparing `ansys-api-mechanical-0.1.1/README.md` & `ansys_api_mechanical-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ansys-api-mechanical-0.1.1/setup.py` & `ansys_api_mechanical-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         author_email='support@ansys.com',
         description=description,
         long_description=long_description,
         long_description_content_type='text/markdown',
         url=f"https://github.com/ansys/{package_name}",
         license="MIT",
         python_requires=">=3.7",
-        install_requires=["grpcio~=1.30", "protobuf>=3.19,<5"],
+        install_requires=["grpcio~=1.30", "protobuf>=3.19,<6"],
         package_dir = {"": "src"},
         packages=setuptools.find_namespace_packages("src", include=("ansys.*",)),
         package_data={
             "": ["*.proto", "*.pyi", "py.typed", "VERSION"],
         },
         entry_points={
             "ansys.tools.protoc_helper.proto_provider": [
```

### Comparing `ansys-api-mechanical-0.1.1/src/ansys/api/mechanical/v0/mechanical.proto` & `ansys_api_mechanical-0.1.2/src/ansys/api/mechanical/v0/mechanical.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-mechanical-0.1.1/src/ansys_api_mechanical.egg-info/PKG-INFO` & `ansys_api_mechanical-0.1.2/src/ansys_api_mechanical.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: ansys-api-mechanical
-Version: 0.1.1
-Summary: Autogenerated python gRPC interface package for ansys-api-mechanical, built on 13:31:41 on 06 October 2023
+Version: 0.1.2
+Summary: Autogenerated python gRPC interface package for ansys-api-mechanical, built on 14:21:03 on 30 April 2024
 Home-page: https://github.com/ansys/ansys-api-mechanical
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: grpcio~=1.30
-Requires-Dist: protobuf<5,>=3.19
+Requires-Dist: protobuf<6,>=3.19
 
 ### ansys-api-mechanical gRPC Interface Package
 
 This Python package contains the auto-generated gRPC Python interface files for
 Mechanical.
```

