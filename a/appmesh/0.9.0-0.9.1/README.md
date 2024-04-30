# Comparing `tmp/appmesh-0.9.0-py3-none-any.whl.zip` & `tmp/appmesh-0.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 15971 bytes, number of entries: 6
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-30 11:14 appmesh/__init__.py
--rw-r--r--  2.0 unx    58527 b- defN 24-Apr-30 11:14 appmesh/appmesh_client.py
--rw-r--r--  2.0 unx    10786 b- defN 24-Apr-30 11:14 appmesh-0.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 11:14 appmesh-0.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-30 11:14 appmesh-0.9.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      455 b- defN 24-Apr-30 11:14 appmesh-0.9.0.dist-info/RECORD
-6 files, 69879 bytes uncompressed, 15149 bytes compressed:  78.3%
+Zip file size: 15969 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-30 12:14 appmesh/__init__.py
+-rw-r--r--  2.0 unx    58527 b- defN 24-Apr-30 12:14 appmesh/appmesh_client.py
+-rw-r--r--  2.0 unx    10786 b- defN 24-Apr-30 12:14 appmesh-0.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 12:14 appmesh-0.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-30 12:14 appmesh-0.9.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      455 b- defN 24-Apr-30 12:14 appmesh-0.9.1.dist-info/RECORD
+6 files, 69879 bytes uncompressed, 15147 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: appmesh/__init__.py
 Comment: 
 
 Filename: appmesh/appmesh_client.py
 Comment: 
 
-Filename: appmesh-0.9.0.dist-info/METADATA
+Filename: appmesh-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: appmesh-0.9.0.dist-info/WHEEL
+Filename: appmesh-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: appmesh-0.9.0.dist-info/top_level.txt
+Filename: appmesh-0.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: appmesh-0.9.0.dist-info/RECORD
+Filename: appmesh-0.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `appmesh-0.9.0.dist-info/METADATA` & `appmesh-0.9.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appmesh
-Version: 0.9.0
+Version: 0.9.1
 Summary: Client SDK for App Mesh
 Home-page: https://github.com/laoshanxi/app-mesh
 Author: laoshanxi
 Author-email: 178029200@qq.com
 License: MIT
 Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: appmesh Version: 0.9.0 Summary: Client SDK for App
+Metadata-Version: 2.1 Name: appmesh Version: 0.9.1 Summary: Client SDK for App
 Mesh Home-page: https://github.com/laoshanxi/app-mesh Author: laoshanxi Author-
 email: 178029200@qq.com License: MIT Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: msgpack Requires-Dist: requests-toolbelt Requires-Dist:
 aniso8601 ï»¿[![language.badge]][language.url] [![standard.badge]]
```
