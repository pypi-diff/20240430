# Comparing `tmp/flowkit_jwt_generator-1.25.0-py3-none-any.whl.zip` & `tmp/flowkit_jwt_generator-1.25.0.post0.dev1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8398 bytes, number of entries: 10
--rw-r--r--  2.0 unx      507 b- defN 24-Apr-24 12:17 flowkit_jwt_generator/__init__.py
--rw-r--r--  2.0 unx      498 b- defN 24-Apr-24 12:17 flowkit_jwt_generator/_version.py
--rw-r--r--  2.0 unx     1591 b- defN 24-Apr-24 12:17 flowkit_jwt_generator/cli.py
--rw-r--r--  2.0 unx     3405 b- defN 24-Apr-24 12:17 flowkit_jwt_generator/fixtures.py
--rw-r--r--  2.0 unx     9215 b- defN 24-Apr-24 12:17 flowkit_jwt_generator/jwt.py
--rw-r--r--  2.0 unx     1322 b- defN 24-Apr-24 12:17 flowkit_jwt_generator-1.25.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 12:17 flowkit_jwt_generator-1.25.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      138 b- defN 24-Apr-24 12:17 flowkit_jwt_generator-1.25.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-24 12:17 flowkit_jwt_generator-1.25.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      907 b- defN 24-Apr-24 12:17 flowkit_jwt_generator-1.25.0.dist-info/RECORD
-10 files, 17697 bytes uncompressed, 6820 bytes compressed:  61.5%
+Zip file size: 8532 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      507 b- defN 24-Apr-30 11:54 flowkit_jwt_generator/__init__.py
+-rw-r--r--  2.0 unx      509 b- defN 24-Apr-30 11:54 flowkit_jwt_generator/_version.py
+-rw-r--r--  2.0 unx     1591 b- defN 24-Apr-30 11:54 flowkit_jwt_generator/cli.py
+-rw-r--r--  2.0 unx     3405 b- defN 24-Apr-30 11:54 flowkit_jwt_generator/fixtures.py
+-rw-r--r--  2.0 unx     9215 b- defN 24-Apr-30 11:54 flowkit_jwt_generator/jwt.py
+-rw-r--r--  2.0 unx     1333 b- defN 24-Apr-30 11:54 flowkit_jwt_generator-1.25.0.post0.dev1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 11:54 flowkit_jwt_generator-1.25.0.post0.dev1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      138 b- defN 24-Apr-30 11:54 flowkit_jwt_generator-1.25.0.post0.dev1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-30 11:54 flowkit_jwt_generator-1.25.0.post0.dev1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      962 b- defN 24-Apr-30 11:54 flowkit_jwt_generator-1.25.0.post0.dev1.dist-info/RECORD
+10 files, 17774 bytes uncompressed, 6844 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: flowkit_jwt_generator/fixtures.py
 Comment: 
 
 Filename: flowkit_jwt_generator/jwt.py
 Comment: 
 
-Filename: flowkit_jwt_generator-1.25.0.dist-info/METADATA
+Filename: flowkit_jwt_generator-1.25.0.post0.dev1.dist-info/METADATA
 Comment: 
 
-Filename: flowkit_jwt_generator-1.25.0.dist-info/WHEEL
+Filename: flowkit_jwt_generator-1.25.0.post0.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: flowkit_jwt_generator-1.25.0.dist-info/entry_points.txt
+Filename: flowkit_jwt_generator-1.25.0.post0.dev1.dist-info/entry_points.txt
 Comment: 
 
-Filename: flowkit_jwt_generator-1.25.0.dist-info/top_level.txt
+Filename: flowkit_jwt_generator-1.25.0.post0.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: flowkit_jwt_generator-1.25.0.dist-info/RECORD
+Filename: flowkit_jwt_generator-1.25.0.post0.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flowkit_jwt_generator/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2024-04-24T13:12:09+0100",
+ "date": "2024-04-30T12:38:53+0100",
  "dirty": false,
  "error": null,
- "full-revisionid": "03ed8a73811b32c7ba0b8a9d6076d50d7f550c6d",
- "version": "1.25.0"
+ "full-revisionid": "035b70b0ac23476bef32cbc4010e799f6df2f279",
+ "version": "1.25.0.post0.dev1"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## Comparing `flowkit_jwt_generator-1.25.0.dist-info/METADATA` & `flowkit_jwt_generator-1.25.0.post0.dev1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowkit_jwt_generator
-Version: 1.25.0
+Version: 1.25.0.post0.dev1
 Summary: Common test JWT generator for FlowKit.
 Home-page: https://github.com/Flowminder/FlowKit
 Author: Flowminder Foundation
 Author-email: flowkit@flowminder.org
 Keywords: mobile telecommunications analysis
 Platform: MacOS X
 Platform: Linux
```

