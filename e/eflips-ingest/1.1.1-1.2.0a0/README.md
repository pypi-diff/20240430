# Comparing `tmp/eflips_ingest-1.1.1.tar.gz` & `tmp/eflips_ingest-1.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eflips_ingest-1.1.1.tar", max compression
+gzip compressed data, was "eflips_ingest-1.2.0a0.tar", max compression
```

## Comparing `eflips_ingest-1.1.1.tar` & `eflips_ingest-1.2.0a0.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0    34143 2024-04-09 15:53:38.121598 eflips_ingest-1.1.1/LICENSE.md
--rw-r--r--   0        0        0     7014 2024-04-09 15:53:38.121598 eflips_ingest-1.1.1/README.md
--rw-r--r--   0        0        0      207 2024-04-09 15:53:38.125598 eflips_ingest-1.1.1/eflips/ingest/__init__.py
--rw-r--r--   0        0        0     5978 2024-04-09 15:53:38.125598 eflips_ingest-1.1.1/eflips/ingest/base.py
--rw-r--r--   0        0        0    16283 2024-04-09 15:53:38.125598 eflips_ingest-1.1.1/eflips/ingest/dummy.py
--rw-r--r--   0        0        0        0 2024-04-09 15:53:38.125598 eflips_ingest-1.1.1/eflips/ingest/legacy/__init__.py
--rw-r--r--   0        0        0    63454 2024-04-09 15:53:38.125598 eflips_ingest-1.1.1/eflips/ingest/legacy/bvgxml.py
--rw-r--r--   0        0        0      383 2024-04-09 15:53:38.125598 eflips_ingest-1.1.1/eflips/ingest/legacy/xmldata/README.md
--rw-r--r--   0        0        0     1065 2024-04-09 15:53:38.125598 eflips_ingest-1.1.1/eflips/ingest/legacy/xmldata/__init__.py
--rw-r--r--   0        0        0    47033 2024-04-09 15:53:38.125598 eflips_ingest-1.1.1/eflips/ingest/legacy/xmldata/bvg_xml.py
--rw-r--r--   0        0        0     3049 2024-04-09 15:53:38.125598 eflips_ingest-1.1.1/eflips/ingest/util.py
--rw-r--r--   0        0        0     1120 2024-04-09 15:53:38.125598 eflips_ingest-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     8056 1970-01-01 00:00:00.000000 eflips_ingest-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34143 2024-02-13 18:24:50.048548 eflips_ingest-1.2.0a0/LICENSE.md
+-rw-r--r--   0        0        0     7014 2024-04-01 14:04:27.651157 eflips_ingest-1.2.0a0/README.md
+-rw-r--r--   0        0        0      207 2024-04-01 14:04:27.651494 eflips_ingest-1.2.0a0/eflips/ingest/__init__.py
+-rw-r--r--   0        0        0     5978 2024-04-19 12:42:52.197526 eflips_ingest-1.2.0a0/eflips/ingest/base.py
+-rw-r--r--   0        0        0    16283 2024-04-19 12:42:52.197795 eflips_ingest-1.2.0a0/eflips/ingest/dummy.py
+-rw-r--r--   0        0        0        0 2024-04-01 14:16:33.464380 eflips_ingest-1.2.0a0/eflips/ingest/legacy/__init__.py
+-rw-r--r--   0        0        0    63454 2024-04-01 14:16:33.465214 eflips_ingest-1.2.0a0/eflips/ingest/legacy/bvgxml.py
+-rw-r--r--   0        0        0      549 2024-04-29 11:48:41.323942 eflips_ingest-1.2.0a0/eflips/ingest/legacy/vdv452/vdv2.py
+-rw-r--r--   0        0        0      383 2024-04-01 14:16:33.465541 eflips_ingest-1.2.0a0/eflips/ingest/legacy/xmldata/README.md
+-rw-r--r--   0        0        0     1065 2024-04-01 14:16:33.465853 eflips_ingest-1.2.0a0/eflips/ingest/legacy/xmldata/__init__.py
+-rw-r--r--   0        0        0    47033 2024-04-01 14:16:33.466102 eflips_ingest-1.2.0a0/eflips/ingest/legacy/xmldata/bvg_xml.py
+-rw-r--r--   0        0        0     3049 2024-04-01 14:16:33.466569 eflips_ingest-1.2.0a0/eflips/ingest/util.py
+-rw-r--r--   0        0        0    46557 2024-04-30 19:00:38.473490 eflips_ingest-1.2.0a0/eflips/ingest/vdv.py
+-rw-r--r--   0        0        0      618 2024-04-29 12:47:00.182773 eflips_ingest-1.2.0a0/eflips/ingest/vdv452data/__init__.py
+-rw-r--r--   0        0        0    45974 2024-04-30 19:00:38.477621 eflips_ingest-1.2.0a0/eflips/ingest/vdv452data/vdv452_v1_5.py
+-rw-r--r--   0        0        0     1126 2024-04-30 19:00:47.173640 eflips_ingest-1.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0     8058 1970-01-01 00:00:00.000000 eflips_ingest-1.2.0a0/PKG-INFO
```

### Comparing `eflips_ingest-1.1.1/LICENSE.md` & `eflips_ingest-1.2.0a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.1.1/README.md` & `eflips_ingest-1.2.0a0/README.md`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.1.1/eflips/ingest/base.py` & `eflips_ingest-1.2.0a0/eflips/ingest/base.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.1.1/eflips/ingest/dummy.py` & `eflips_ingest-1.2.0a0/eflips/ingest/dummy.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.1.1/eflips/ingest/legacy/bvgxml.py` & `eflips_ingest-1.2.0a0/eflips/ingest/legacy/bvgxml.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.1.1/eflips/ingest/legacy/xmldata/__init__.py` & `eflips_ingest-1.2.0a0/eflips/ingest/legacy/xmldata/__init__.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.1.1/eflips/ingest/legacy/xmldata/bvg_xml.py` & `eflips_ingest-1.2.0a0/eflips/ingest/legacy/xmldata/bvg_xml.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.1.1/eflips/ingest/util.py` & `eflips_ingest-1.2.0a0/eflips/ingest/util.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.1.1/pyproject.toml` & `eflips_ingest-1.2.0a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eflips-ingest"
-version = "1.1.1"
+version = "1.2.0-alpha"
 description = "A collection of import scripts for converting bus schedule data into the [eflips-model](https://github.com/mpm-tu-berlin/eflips-model) data format."
 authors = [
     "Ludger Heide <ludger.heide@lhtechnologies.de>"
 ]
 readme = "README.md"
 license = "AGPL-3.0-or-later"
 homepage = "https://github.com/mpm-tu-berlin/eflips-import"
```

### Comparing `eflips_ingest-1.1.1/PKG-INFO` & `eflips_ingest-1.2.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eflips-ingest
-Version: 1.1.1
+Version: 1.2.0a0
 Summary: A collection of import scripts for converting bus schedule data into the [eflips-model](https://github.com/mpm-tu-berlin/eflips-model) data format.
 Home-page: https://github.com/mpm-tu-berlin/eflips-import
 License: AGPL-3.0-or-later
 Author: Ludger Heide
 Author-email: ludger.heide@lhtechnologies.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

