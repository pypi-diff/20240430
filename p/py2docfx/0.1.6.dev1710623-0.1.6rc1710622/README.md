# Comparing `tmp/py2docfx-0.1.6.dev1710623-py3-none-any.whl.zip` & `tmp/py2docfx-0.1.6rc1710622-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 108794 bytes, number of entries: 129
+Zip file size: 108774 bytes, number of entries: 129
 -rw-rw-rw-  2.0 fat       72 b- defN 24-Apr-29 09:33 py2docfx/__init__.py
 -rw-rw-rw-  2.0 fat    10747 b- defN 24-Apr-29 09:33 py2docfx/__main__.py
 -rw-rw-rw-  2.0 fat       11 b- defN 24-Apr-29 09:33 py2docfx/convert_prepare/__init__.py
 -rw-rw-rw-  2.0 fat      894 b- defN 24-Apr-29 09:33 py2docfx/convert_prepare/environment.py
 -rw-rw-rw-  2.0 fat     2295 b- defN 24-Apr-29 09:33 py2docfx/convert_prepare/generate_conf.py
 -rw-rw-rw-  2.0 fat     2432 b- defN 24-Apr-29 09:33 py2docfx/convert_prepare/generate_document.py
 -rw-rw-rw-  2.0 fat     4872 b- defN 24-Apr-29 09:33 py2docfx/convert_prepare/get_source.py
@@ -120,12 +120,12 @@
 -rw-rw-rw-  2.0 fat      574 b- defN 24-Apr-29 09:33 py2docfx/docfx_yaml/tests/roots/test-writer-table/code_with_table_desc.py
 -rw-rw-rw-  2.0 fat      260 b- defN 24-Apr-29 09:33 py2docfx/docfx_yaml/tests/roots/test-writer-table/conf.py
 -rw-rw-rw-  2.0 fat      537 b- defN 24-Apr-29 09:33 py2docfx/docfx_yaml/tests/roots/test-writer-uri/code_with_uri.py
 -rw-rw-rw-  2.0 fat      260 b- defN 24-Apr-29 09:33 py2docfx/docfx_yaml/tests/roots/test-writer-uri/conf.py
 -rw-rw-rw-  2.0 fat     1030 b- defN 24-Apr-29 09:33 py2docfx/docfx_yaml/tests/roots/test-writer-versions/code_with_version_directives.py
 -rw-rw-rw-  2.0 fat      404 b- defN 24-Apr-29 09:33 py2docfx/docfx_yaml/tests/roots/test-writer-versions/conf.py
 -rw-rw-rw-  2.0 fat     3383 b- defN 24-Apr-29 09:33 py2docfx/docfx_yaml/tests/utils/test_utils.py
--rw-rw-rw-  2.0 fat      601 b- defN 24-Apr-29 09:39 py2docfx-0.1.6.dev1710623.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-29 09:39 py2docfx-0.1.6.dev1710623.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-29 09:39 py2docfx-0.1.6.dev1710623.dist-info/top_level.txt
--rw-rw-r--  2.0 fat    14635 b- defN 24-Apr-29 09:39 py2docfx-0.1.6.dev1710623.dist-info/RECORD
-129 files, 303766 bytes uncompressed, 84080 bytes compressed:  72.3%
+-rw-rw-rw-  2.0 fat      599 b- defN 24-Apr-29 09:40 py2docfx-0.1.6rc1710622.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-29 09:40 py2docfx-0.1.6rc1710622.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-29 09:40 py2docfx-0.1.6rc1710622.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat    14627 b- defN 24-Apr-29 09:40 py2docfx-0.1.6rc1710622.dist-info/RECORD
+129 files, 303756 bytes uncompressed, 84076 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -369,20 +369,20 @@
 
 Filename: py2docfx/docfx_yaml/tests/roots/test-writer-versions/conf.py
 Comment: 
 
 Filename: py2docfx/docfx_yaml/tests/utils/test_utils.py
 Comment: 
 
-Filename: py2docfx-0.1.6.dev1710623.dist-info/METADATA
+Filename: py2docfx-0.1.6rc1710622.dist-info/METADATA
 Comment: 
 
-Filename: py2docfx-0.1.6.dev1710623.dist-info/WHEEL
+Filename: py2docfx-0.1.6rc1710622.dist-info/WHEEL
 Comment: 
 
-Filename: py2docfx-0.1.6.dev1710623.dist-info/top_level.txt
+Filename: py2docfx-0.1.6rc1710622.dist-info/top_level.txt
 Comment: 
 
-Filename: py2docfx-0.1.6.dev1710623.dist-info/RECORD
+Filename: py2docfx-0.1.6rc1710622.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `py2docfx-0.1.6.dev1710623.dist-info/METADATA` & `py2docfx-0.1.6rc1710622.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2docfx
-Version: 0.1.6.dev1710623
+Version: 0.1.6rc1710622
 Summary: A package built based on Sphinx which download source code package and generate yaml files supported by docfx.
 Author: Microsoft Corporation
 License: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

## Comparing `py2docfx-0.1.6.dev1710623.dist-info/RECORD` & `py2docfx-0.1.6rc1710622.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -119,11 +119,11 @@
 py2docfx/docfx_yaml/tests/roots/test-writer-table/code_with_table_desc.py,sha256=J4eFvXsymgFvjnwVUY0APtUGwuxvt-AFJjTaEaQ7zMQ,574
 py2docfx/docfx_yaml/tests/roots/test-writer-table/conf.py,sha256=avcbnIOV2mlGQwhMQJZC4W6UGRBRhnq1QBxjPWlySxQ,260
 py2docfx/docfx_yaml/tests/roots/test-writer-uri/code_with_uri.py,sha256=bzWTZpY2yf_By2bOSl1GFaY3BsZpkAvwQuGztlcHKkQ,537
 py2docfx/docfx_yaml/tests/roots/test-writer-uri/conf.py,sha256=avcbnIOV2mlGQwhMQJZC4W6UGRBRhnq1QBxjPWlySxQ,260
 py2docfx/docfx_yaml/tests/roots/test-writer-versions/code_with_version_directives.py,sha256=UuizbrJPaG_PcaH18BvbI9KQevOaLd4SslpnzMSqcrE,1030
 py2docfx/docfx_yaml/tests/roots/test-writer-versions/conf.py,sha256=SCEKrm9VigArfdgf-GAieJD-40d0ctT6urmGIjFOZLM,404
 py2docfx/docfx_yaml/tests/utils/test_utils.py,sha256=d0OYSUQ6NyoZx5mlLdNGGNhiNmmQhjVT4hQ6jY3VE_M,3383
-py2docfx-0.1.6.dev1710623.dist-info/METADATA,sha256=-ycDOpn6F9v_odV8P5ZzOIcWiiVI181r4KmYaex2d2E,601
-py2docfx-0.1.6.dev1710623.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-py2docfx-0.1.6.dev1710623.dist-info/top_level.txt,sha256=5dH2uP81dczt_qQJ38wiZ-gzoVWasfiJALWRSjdbnYU,9
-py2docfx-0.1.6.dev1710623.dist-info/RECORD,,
+py2docfx-0.1.6rc1710622.dist-info/METADATA,sha256=koFUni3WE9ZE-QvYkFENMvUd_mNkPM7cwXXXaLyBtFM,599
+py2docfx-0.1.6rc1710622.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+py2docfx-0.1.6rc1710622.dist-info/top_level.txt,sha256=5dH2uP81dczt_qQJ38wiZ-gzoVWasfiJALWRSjdbnYU,9
+py2docfx-0.1.6rc1710622.dist-info/RECORD,,
```

