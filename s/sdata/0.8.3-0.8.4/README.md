# Comparing `tmp/sdata-0.8.3.tar.gz` & `tmp/sdata-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sdata-0.8.3.tar", last modified: Mon Dec  7 16:46:59 2020, max compression
+gzip compressed data, was "dist/sdata-0.8.4.tar", last modified: Tue Dec  8 12:14:01 2020, max compression
```

## Comparing `sdata-0.8.3.tar` & `sdata-0.8.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2020-12-07 16:46:59.000000 sdata-0.8.3/
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     1066 2019-01-04 15:48:33.000000 sdata-0.8.3/LICENSE-MIT
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)       38 2019-01-04 15:47:58.000000 sdata-0.8.3/MANIFEST.in
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     5191 2020-12-07 16:46:59.000000 sdata-0.8.3/PKG-INFO
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     3587 2020-12-05 17:12:02.000000 sdata-0.8.3/README.md
-drwxrwxr-x   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2020-12-07 16:46:59.000000 sdata-0.8.3/sdata/
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)    26709 2020-12-07 16:46:22.000000 sdata-0.8.3/sdata/__init__.py
-drwxrwxr-x   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2020-12-07 16:46:59.000000 sdata-0.8.3/sdata/experiments/
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)      266 2019-01-04 15:48:33.000000 sdata-0.8.3/sdata/experiments/__init__.py
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)      834 2019-01-04 15:48:33.000000 sdata-0.8.3/sdata/experiments/ks2.py
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)      281 2019-01-04 15:48:33.000000 sdata-0.8.3/sdata/experiments/lapshear.py
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)      318 2019-01-04 15:48:33.000000 sdata-0.8.3/sdata/experiments/material.py
-drwxrwxr-x   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2020-12-07 16:46:59.000000 sdata-0.8.3/sdata/io/
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     1383 2019-04-09 07:39:35.000000 sdata-0.8.3/sdata/io/__init__.py
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     9157 2019-04-09 07:39:35.000000 sdata-0.8.3/sdata/io/pud.py
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)    12646 2020-12-07 16:35:40.000000 sdata-0.8.3/sdata/metadata.py
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     9256 2019-01-04 15:48:33.000000 sdata-0.8.3/sdata/timestamp.py
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)      337 2019-01-04 15:48:33.000000 sdata-0.8.3/sdata/tools.py
-drwxrwxr-x   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2020-12-07 16:46:59.000000 sdata-0.8.3/sdata.egg-info/
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     5191 2020-12-07 16:46:59.000000 sdata-0.8.3/sdata.egg-info/PKG-INFO
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)      676 2020-12-07 16:46:59.000000 sdata-0.8.3/sdata.egg-info/SOURCES.txt
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        1 2020-12-07 16:46:59.000000 sdata-0.8.3/sdata.egg-info/dependency_links.txt
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)       13 2020-12-07 16:46:59.000000 sdata-0.8.3/sdata.egg-info/requires.txt
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)       12 2020-12-07 16:46:59.000000 sdata-0.8.3/sdata.egg-info/top_level.txt
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)       63 2020-12-07 16:46:59.000000 sdata-0.8.3/setup.cfg
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     1434 2020-12-03 18:48:00.000000 sdata-0.8.3/setup.py
-drwxrwxr-x   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2020-12-07 16:46:59.000000 sdata-0.8.3/tests/
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2019-01-04 15:48:34.000000 sdata-0.8.3/tests/__init__.py
-drwxrwxr-x   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2020-12-07 16:46:59.000000 sdata-0.8.3/tests/io/
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2019-04-09 07:39:35.000000 sdata-0.8.3/tests/io/__init__.py
-drwxrwxr-x   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2020-12-07 16:46:59.000000 sdata-0.8.3/tests/io/pud/
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2019-04-09 07:39:35.000000 sdata-0.8.3/tests/io/pud/__init__.py
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)      335 2019-04-09 07:39:35.000000 sdata-0.8.3/tests/io/pud/test_pud.py
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)      504 2020-12-02 22:58:03.000000 sdata-0.8.3/tests/test_blob.py
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     2088 2020-12-07 12:33:02.000000 sdata-0.8.3/tests/test_data.py
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     8769 2020-12-04 14:29:59.000000 sdata-0.8.3/tests/test_ks2.py
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     4493 2020-12-04 13:24:02.000000 sdata-0.8.3/tests/test_metadata.py
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     1158 2019-09-05 16:40:57.000000 sdata-0.8.3/tests/test_table.py
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     7336 2020-12-07 12:34:07.000000 sdata-0.8.3/tests/test_testprogram.py
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     3868 2019-04-09 07:41:08.000000 sdata-0.8.3/tests/test_timestamp.py
--rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)      130 2019-01-04 15:48:34.000000 sdata-0.8.3/tests/test_tools.py
+drwxrwxr-x   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2020-12-08 12:14:01.000000 sdata-0.8.4/
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     1066 2019-01-04 15:48:33.000000 sdata-0.8.4/LICENSE-MIT
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)       38 2019-01-04 15:47:58.000000 sdata-0.8.4/MANIFEST.in
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     5191 2020-12-08 12:14:01.000000 sdata-0.8.4/PKG-INFO
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     3587 2020-12-05 17:12:02.000000 sdata-0.8.4/README.md
+drwxrwxr-x   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2020-12-08 12:14:01.000000 sdata-0.8.4/sdata/
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)    26967 2020-12-08 11:30:49.000000 sdata-0.8.4/sdata/__init__.py
+drwxrwxr-x   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2020-12-08 12:14:01.000000 sdata-0.8.4/sdata/experiments/
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)      266 2019-01-04 15:48:33.000000 sdata-0.8.4/sdata/experiments/__init__.py
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)      834 2019-01-04 15:48:33.000000 sdata-0.8.4/sdata/experiments/ks2.py
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)      281 2019-01-04 15:48:33.000000 sdata-0.8.4/sdata/experiments/lapshear.py
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)      318 2019-01-04 15:48:33.000000 sdata-0.8.4/sdata/experiments/material.py
+drwxrwxr-x   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2020-12-08 12:14:01.000000 sdata-0.8.4/sdata/io/
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     1383 2019-04-09 07:39:35.000000 sdata-0.8.4/sdata/io/__init__.py
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     9157 2019-04-09 07:39:35.000000 sdata-0.8.4/sdata/io/pud.py
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)    12861 2020-12-08 11:36:56.000000 sdata-0.8.4/sdata/metadata.py
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     9256 2019-01-04 15:48:33.000000 sdata-0.8.4/sdata/timestamp.py
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)      337 2019-01-04 15:48:33.000000 sdata-0.8.4/sdata/tools.py
+drwxrwxr-x   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2020-12-08 12:14:01.000000 sdata-0.8.4/sdata.egg-info/
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     5191 2020-12-08 12:14:00.000000 sdata-0.8.4/sdata.egg-info/PKG-INFO
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)      676 2020-12-08 12:14:00.000000 sdata-0.8.4/sdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        1 2020-12-08 12:14:00.000000 sdata-0.8.4/sdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)       13 2020-12-08 12:14:00.000000 sdata-0.8.4/sdata.egg-info/requires.txt
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)       12 2020-12-08 12:14:00.000000 sdata-0.8.4/sdata.egg-info/top_level.txt
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)       63 2020-12-08 12:14:01.000000 sdata-0.8.4/setup.cfg
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     1434 2020-12-03 18:48:00.000000 sdata-0.8.4/setup.py
+drwxrwxr-x   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2020-12-08 12:14:01.000000 sdata-0.8.4/tests/
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2019-01-04 15:48:34.000000 sdata-0.8.4/tests/__init__.py
+drwxrwxr-x   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2020-12-08 12:14:01.000000 sdata-0.8.4/tests/io/
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2019-04-09 07:39:35.000000 sdata-0.8.4/tests/io/__init__.py
+drwxrwxr-x   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2020-12-08 12:14:01.000000 sdata-0.8.4/tests/io/pud/
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)        0 2019-04-09 07:39:35.000000 sdata-0.8.4/tests/io/pud/__init__.py
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)      335 2019-04-09 07:39:35.000000 sdata-0.8.4/tests/io/pud/test_pud.py
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)      504 2020-12-02 22:58:03.000000 sdata-0.8.4/tests/test_blob.py
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     2088 2020-12-07 12:33:02.000000 sdata-0.8.4/tests/test_data.py
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     8769 2020-12-04 14:29:59.000000 sdata-0.8.4/tests/test_ks2.py
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     4493 2020-12-04 13:24:02.000000 sdata-0.8.4/tests/test_metadata.py
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     1158 2019-09-05 16:40:57.000000 sdata-0.8.4/tests/test_table.py
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     7336 2020-12-07 12:34:07.000000 sdata-0.8.4/tests/test_testprogram.py
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)     3868 2019-04-09 07:41:08.000000 sdata-0.8.4/tests/test_timestamp.py
+-rw-rw-r--   0 ingolf.lepenies (10010) ingolf.lepenies (10010)      130 2019-01-04 15:48:34.000000 sdata-0.8.4/tests/test_tools.py
```

### Comparing `sdata-0.8.3/LICENSE-MIT` & `sdata-0.8.4/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `sdata-0.8.3/PKG-INFO` & `sdata-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdata
-Version: 0.8.3
+Version: 0.8.4
 Summary: structured data
 Home-page: https://github.com/lepy/sdata
 Author: Lepy
 Author-email: lepy@mailbox.org
 Maintainer: Lepy
 Maintainer-email: lepy@mailbox.org
 License: MIT/Apache-2.0
```

### Comparing `sdata-0.8.3/README.md` & `sdata-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `sdata-0.8.3/sdata/__init__.py` & `sdata-0.8.4/sdata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*-coding: utf-8-*-
 from __future__ import division
 
-__version__ = '0.8.3'
+__version__ = '0.8.4'
 __revision__ = None
 __version_info__ = tuple([int(num) for num in __version__.split('.')])
 
 '''
 basic sdata types 
 '''
 
@@ -507,15 +507,15 @@
 
         with pd.ExcelWriter(filepath) as writer:
 
             # metadata
             # dfm = pd.DataFrame.from_dict(self.metadata, orient="index", columns=["value"])
             dfm = self.metadata.to_dataframe()
 
-            dfm = dfm.sort_index()
+            # dfm = dfm.sort_index()
             dfm.index.name = "key"
             dfm.to_excel(writer, sheet_name='metadata', index=False)
             adjust_col_width('metadata', dfm, writer)
 
             # data
             if self.table is not None:
                 self.table.index.name = "index"
@@ -554,14 +554,18 @@
                 # read df
                 if "table" in sheetnames:
                     tt.table = pd.read_excel(filepath, sheet_name="table", index_col='index')
                 else:
                     logging.info("no table data in '{}'".format(filepath))
                 dfm = pd.read_excel(filepath, sheet_name="metadata")
                 dfm = dfm.set_index(dfm.name.values)
+                # dfm["value"] = dfm["value"].replace(np.nan, None)
+                dfm["description"] = dfm["description"].replace(np.nan, '')
+                dfm["label"] = dfm["label"].replace(np.nan, '')
+                # print("!data.from_xlsx", dfm)
                 tt.metadata = tt.metadata.from_dataframe(dfm)
 
                 # read description
                 if "description" in sheetnames:
                     cells = []
                     for cell in wb["description"]["A"]:
                         if cell.value is not None:
```

### Comparing `sdata-0.8.3/sdata/experiments/ks2.py` & `sdata-0.8.4/sdata/experiments/ks2.py`

 * *Files identical despite different names*

### Comparing `sdata-0.8.3/sdata/io/__init__.py` & `sdata-0.8.4/sdata/io/__init__.py`

 * *Files identical despite different names*

### Comparing `sdata-0.8.3/sdata/io/pud.py` & `sdata-0.8.4/sdata/io/pud.py`

 * *Files identical despite different names*

### Comparing `sdata-0.8.3/sdata/metadata.py` & `sdata-0.8.4/sdata/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,18 @@
 
     def _set_value(self, value):
         try:
             dtype = self.DTYPES.get(self.dtype, None)
             if dtype is None:
                 dtype = self._guess_dtype(value)
             self.dtype = dtype.__name__
-            if value is None:
+            if not value and self.dtype not in ["int", "float"]:
                 self._value = None
+            elif not value and self.dtype in ["int", "float"]:
+                self._value = np.nan
             elif dtype.__name__ == "bool" and value in [0, "0", "False", "false"]:
                 self._value = False
             elif dtype.__name__ == "bool" and value in [1, "1", "true", "True"]:
                 self._value = True
             else:
                 self._value = dtype(value)
         except ValueError as exp:
@@ -249,20 +251,23 @@
     def from_dict(cls, d):
         """setup metadata from dict"""
         metadata = cls()
         for k, v in d.items():
             if isinstance(v, (str,)):
                 v = {"name":k, "value":v, "dtype":"str", "unit":"", "description":"", "label":""}
             elif hasattr(v, "keys"):
-                v = {"name":k, "value":v.get("value"), "dtype":v.get("dtype"),
-                     "unit":v.get("unit"), "description":v.get("description"),
-                     "label":v.get("label")}
+
+                dtype = v.get("dtype", "str")
+                value = v.get("value")
+
+                v = {"name":k, "value":value, "dtype":dtype,
+                     "unit":v.get("unit", ""), "description":v.get("description", ""),
+                     "label":v.get("label", "")}
             else:
                 v = {"name":k, "value":v, "dtype":"", "unit":"", "description":"", "label":""}
-
             metadata.set_attr(**v)
         return metadata
 
     def to_dataframe(self):
         """create dataframe"""
         d = self.to_dict()
         if len(d) == 0:
```

### Comparing `sdata-0.8.3/sdata/timestamp.py` & `sdata-0.8.4/sdata/timestamp.py`

 * *Files identical despite different names*

### Comparing `sdata-0.8.3/sdata.egg-info/PKG-INFO` & `sdata-0.8.4/sdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdata
-Version: 0.8.3
+Version: 0.8.4
 Summary: structured data
 Home-page: https://github.com/lepy/sdata
 Author: Lepy
 Author-email: lepy@mailbox.org
 Maintainer: Lepy
 Maintainer-email: lepy@mailbox.org
 License: MIT/Apache-2.0
```

### Comparing `sdata-0.8.3/sdata.egg-info/SOURCES.txt` & `sdata-0.8.4/sdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdata-0.8.3/setup.py` & `sdata-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `sdata-0.8.3/tests/test_data.py` & `sdata-0.8.4/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `sdata-0.8.3/tests/test_ks2.py` & `sdata-0.8.4/tests/test_ks2.py`

 * *Files identical despite different names*

### Comparing `sdata-0.8.3/tests/test_metadata.py` & `sdata-0.8.4/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `sdata-0.8.3/tests/test_table.py` & `sdata-0.8.4/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `sdata-0.8.3/tests/test_testprogram.py` & `sdata-0.8.4/tests/test_testprogram.py`

 * *Files identical despite different names*

### Comparing `sdata-0.8.3/tests/test_timestamp.py` & `sdata-0.8.4/tests/test_timestamp.py`

 * *Files identical despite different names*

