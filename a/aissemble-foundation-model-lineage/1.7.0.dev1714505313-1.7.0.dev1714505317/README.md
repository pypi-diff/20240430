# Comparing `tmp/aissemble_foundation_model_lineage-1.7.0.dev1714505313.tar.gz` & `tmp/aissemble_foundation_model_lineage-1.7.0.dev1714505317.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_foundation_model_lineage-1.7.0.dev1714505313.tar", max compression
+gzip compressed data, was "aissemble_foundation_model_lineage-1.7.0.dev1714505317.tar", max compression
```

## Comparing `aissemble_foundation_model_lineage-1.7.0.dev1714505313.tar` & `aissemble_foundation_model_lineage-1.7.0.dev1714505317.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     9580 2024-04-30 19:28:20.795441 aissemble_foundation_model_lineage-1.7.0.dev1714505313/LICENSE
--rw-r--r--   0        0        0      318 2024-04-30 19:23:29.288274 aissemble_foundation_model_lineage-1.7.0.dev1714505313/LICENSE.txt
--rw-r--r--   0        0        0      514 2024-04-30 19:23:29.288274 aissemble_foundation_model_lineage-1.7.0.dev1714505313/README.md
--rw-r--r--   0        0        0      765 2024-04-30 19:28:34.007450 aissemble_foundation_model_lineage-1.7.0.dev1714505313/pyproject.toml
--rw-r--r--   0        0        0      470 2024-04-30 19:23:29.288274 aissemble_foundation_model_lineage-1.7.0.dev1714505313/src/aissemble_model_lineage/__init__.py
--rw-r--r--   0        0        0     8674 2024-04-30 19:23:29.288274 aissemble_foundation_model_lineage-1.7.0.dev1714505313/src/aissemble_model_lineage/builder.py
--rw-r--r--   0        0        0     4273 2024-04-30 19:23:29.288274 aissemble_foundation_model_lineage-1.7.0.dev1714505313/src/aissemble_model_lineage/facets.py
--rw-r--r--   0        0        0      993 1970-01-01 00:00:00.000000 aissemble_foundation_model_lineage-1.7.0.dev1714505313/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-04-30 19:28:23.329999 aissemble_foundation_model_lineage-1.7.0.dev1714505317/LICENSE
+-rw-r--r--   0        0        0      318 2024-04-30 19:23:29.257568 aissemble_foundation_model_lineage-1.7.0.dev1714505317/LICENSE.txt
+-rw-r--r--   0        0        0      514 2024-04-30 19:23:29.257568 aissemble_foundation_model_lineage-1.7.0.dev1714505317/README.md
+-rw-r--r--   0        0        0      765 2024-04-30 19:28:37.849624 aissemble_foundation_model_lineage-1.7.0.dev1714505317/pyproject.toml
+-rw-r--r--   0        0        0      470 2024-04-30 19:23:29.257568 aissemble_foundation_model_lineage-1.7.0.dev1714505317/src/aissemble_model_lineage/__init__.py
+-rw-r--r--   0        0        0     8674 2024-04-30 19:23:29.257568 aissemble_foundation_model_lineage-1.7.0.dev1714505317/src/aissemble_model_lineage/builder.py
+-rw-r--r--   0        0        0     4273 2024-04-30 19:23:29.257568 aissemble_foundation_model_lineage-1.7.0.dev1714505317/src/aissemble_model_lineage/facets.py
+-rw-r--r--   0        0        0      993 1970-01-01 00:00:00.000000 aissemble_foundation_model_lineage-1.7.0.dev1714505317/PKG-INFO
```

### Comparing `aissemble_foundation_model_lineage-1.7.0.dev1714505313/LICENSE` & `aissemble_foundation_model_lineage-1.7.0.dev1714505317/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_model_lineage-1.7.0.dev1714505313/README.md` & `aissemble_foundation_model_lineage-1.7.0.dev1714505317/README.md`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_model_lineage-1.7.0.dev1714505313/pyproject.toml` & `aissemble_foundation_model_lineage-1.7.0.dev1714505317/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-foundation-model-lineage"
-version = "1.7.0.dev1714505313"
+version = "1.7.0.dev1714505317"
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 description = "Model lineage API"
 readme = "README.md"
 packages = [
     {include = "aissemble_model_lineage", from = "src"}
 ]
```

### Comparing `aissemble_foundation_model_lineage-1.7.0.dev1714505313/src/aissemble_model_lineage/builder.py` & `aissemble_foundation_model_lineage-1.7.0.dev1714505317/src/aissemble_model_lineage/builder.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_model_lineage-1.7.0.dev1714505313/src/aissemble_model_lineage/facets.py` & `aissemble_foundation_model_lineage-1.7.0.dev1714505317/src/aissemble_model_lineage/facets.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_model_lineage-1.7.0.dev1714505313/PKG-INFO` & `aissemble_foundation_model_lineage-1.7.0.dev1714505317/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-foundation-model-lineage
-Version: 1.7.0.dev1714505313
+Version: 1.7.0.dev1714505317
 Summary: Model lineage API
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aissemble-foundation-data-lineage-python (==1.7.0.*)
```

