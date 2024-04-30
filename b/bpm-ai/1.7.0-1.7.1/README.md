# Comparing `tmp/bpm_ai-1.7.0.tar.gz` & `tmp/bpm_ai-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai-1.7.0.tar", max compression
+gzip compressed data, was "bpm_ai-1.7.1.tar", max compression
```

## Comparing `bpm_ai-1.7.0.tar` & `bpm_ai-1.7.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      726 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/README.md
--rw-r--r--   0        0        0        0 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/common/__init__.py
--rw-r--r--   0        0        0      195 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/common/errors.py
--rw-r--r--   0        0        0     1668 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/common/multimodal.py
--rw-r--r--   0        0        0        0 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/compose/__init__.py
--rw-r--r--   0        0        0     1595 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/compose/compose.anthropic.prompt
--rw-r--r--   0        0        0     1369 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/compose/compose.openai.prompt
--rw-r--r--   0        0        0     1699 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/compose/compose.prompt
--rw-r--r--   0        0        0     3644 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/compose/compose.py
--rw-r--r--   0        0        0      950 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/compose/util.py
--rw-r--r--   0        0        0        0 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/decide/__init__.py
--rw-r--r--   0        0        0     8786 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/decide/decide.anthropic.prompt
--rw-r--r--   0        0        0     8181 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/decide/decide.openai.prompt
--rw-r--r--   0        0        0     8459 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/decide/decide.prompt
--rw-r--r--   0        0        0     6170 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/decide/decide.py
--rw-r--r--   0        0        0     3044 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/decide/schema.py
--rw-r--r--   0        0        0        0 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/extract/__init__.py
--rw-r--r--   0        0        0     1485 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/extract/extract.anthropic.prompt
--rw-r--r--   0        0        0     1286 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/extract/extract.openai.prompt
--rw-r--r--   0        0        0     1466 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/extract/extract.prompt
--rw-r--r--   0        0        0     7495 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/extract/extract.py
--rw-r--r--   0        0        0     2578 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/extract/util.py
--rw-r--r--   0        0        0        0 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/generic/__init__.py
--rw-r--r--   0        0        0      690 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/generic/generic.anthropic.prompt
--rw-r--r--   0        0        0      544 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/generic/generic.openai.prompt
--rw-r--r--   0        0        0      738 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/generic/generic.prompt
--rw-r--r--   0        0        0     1631 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/generic/generic.py
--rw-r--r--   0        0        0        0 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/translate/__init__.py
--rw-r--r--   0        0        0      632 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/translate/translate.anthropic.prompt
--rw-r--r--   0        0        0      611 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/translate/translate.openai.prompt
--rw-r--r--   0        0        0      688 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/translate/translate.prompt
--rw-r--r--   0        0        0     3138 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/translate/translate.py
--rw-r--r--   0        0        0      680 2024-04-29 16:12:29.954361 bpm_ai-1.7.0/bpm_ai/translate/util.py
--rw-r--r--   0        0        0      900 2024-04-29 16:12:29.958361 bpm_ai-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 bpm_ai-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0      726 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/common/__init__.py
+-rw-r--r--   0        0        0      195 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/common/errors.py
+-rw-r--r--   0        0        0     1668 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/common/multimodal.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/compose/__init__.py
+-rw-r--r--   0        0        0     1595 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/compose/compose.anthropic.prompt
+-rw-r--r--   0        0        0     1369 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/compose/compose.openai.prompt
+-rw-r--r--   0        0        0     1699 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/compose/compose.prompt
+-rw-r--r--   0        0        0     3644 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/compose/compose.py
+-rw-r--r--   0        0        0      950 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/compose/util.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/decide/__init__.py
+-rw-r--r--   0        0        0     8786 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/decide/decide.anthropic.prompt
+-rw-r--r--   0        0        0     8181 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/decide/decide.openai.prompt
+-rw-r--r--   0        0        0     8459 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/decide/decide.prompt
+-rw-r--r--   0        0        0     6221 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/decide/decide.py
+-rw-r--r--   0        0        0     3044 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/decide/schema.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/extract/__init__.py
+-rw-r--r--   0        0        0     1485 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/extract/extract.anthropic.prompt
+-rw-r--r--   0        0        0     1286 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/extract/extract.openai.prompt
+-rw-r--r--   0        0        0     1466 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/extract/extract.prompt
+-rw-r--r--   0        0        0     7495 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/extract/extract.py
+-rw-r--r--   0        0        0     2578 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/extract/util.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/generic/__init__.py
+-rw-r--r--   0        0        0      690 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/generic/generic.anthropic.prompt
+-rw-r--r--   0        0        0      544 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/generic/generic.openai.prompt
+-rw-r--r--   0        0        0      738 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/generic/generic.prompt
+-rw-r--r--   0        0        0     1631 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/generic/generic.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/translate/__init__.py
+-rw-r--r--   0        0        0      632 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/translate/translate.anthropic.prompt
+-rw-r--r--   0        0        0      611 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/translate/translate.openai.prompt
+-rw-r--r--   0        0        0      688 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/translate/translate.prompt
+-rw-r--r--   0        0        0     3138 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/translate/translate.py
+-rw-r--r--   0        0        0      680 2024-04-30 09:46:16.004526 bpm_ai-1.7.1/bpm_ai/translate/util.py
+-rw-r--r--   0        0        0      900 2024-04-30 09:46:16.008526 bpm_ai-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 bpm_ai-1.7.1/PKG-INFO
```

### Comparing `bpm_ai-1.7.0/README.md` & `bpm_ai-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/common/multimodal.py` & `bpm_ai-1.7.1/bpm_ai/common/multimodal.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/compose/compose.anthropic.prompt` & `bpm_ai-1.7.1/bpm_ai/compose/compose.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/compose/compose.openai.prompt` & `bpm_ai-1.7.1/bpm_ai/compose/compose.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/compose/compose.prompt` & `bpm_ai-1.7.1/bpm_ai/compose/compose.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/compose/compose.py` & `bpm_ai-1.7.1/bpm_ai/compose/compose.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/compose/util.py` & `bpm_ai-1.7.1/bpm_ai/compose/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/decide/decide.anthropic.prompt` & `bpm_ai-1.7.1/bpm_ai/decide/decide.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/decide/decide.openai.prompt` & `bpm_ai-1.7.1/bpm_ai/decide/decide.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/decide/decide.prompt` & `bpm_ai-1.7.1/bpm_ai/decide/decide.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/decide/decide.py` & `bpm_ai-1.7.1/bpm_ai/decide/decide.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,17 @@
         elif output_type == "integer":
             return int(raw) if raw else None
         elif output_type == "number":
             return float(raw) if raw else None
         else:
             return raw
 
-    if multiple_decision_values:
+    if not classification:
+        result = None
+    elif multiple_decision_values:
         result = [raw_to_output_type(label) for label, _ in classification.labels_scores]
     else:
         result = raw_to_output_type(classification.max_label)
 
     return {
         "decision": result,
         "reasoning": ""
```

### Comparing `bpm_ai-1.7.0/bpm_ai/decide/schema.py` & `bpm_ai-1.7.1/bpm_ai/decide/schema.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/extract/extract.anthropic.prompt` & `bpm_ai-1.7.1/bpm_ai/extract/extract.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/extract/extract.openai.prompt` & `bpm_ai-1.7.1/bpm_ai/extract/extract.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/extract/extract.prompt` & `bpm_ai-1.7.1/bpm_ai/extract/extract.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/extract/extract.py` & `bpm_ai-1.7.1/bpm_ai/extract/extract.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/extract/util.py` & `bpm_ai-1.7.1/bpm_ai/extract/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/generic/generic.anthropic.prompt` & `bpm_ai-1.7.1/bpm_ai/generic/generic.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/generic/generic.openai.prompt` & `bpm_ai-1.7.1/bpm_ai/generic/generic.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/generic/generic.prompt` & `bpm_ai-1.7.1/bpm_ai/generic/generic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/generic/generic.py` & `bpm_ai-1.7.1/bpm_ai/generic/generic.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/translate/translate.anthropic.prompt` & `bpm_ai-1.7.1/bpm_ai/translate/translate.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/translate/translate.openai.prompt` & `bpm_ai-1.7.1/bpm_ai/translate/translate.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/translate/translate.prompt` & `bpm_ai-1.7.1/bpm_ai/translate/translate.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/translate/translate.py` & `bpm_ai-1.7.1/bpm_ai/translate/translate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/bpm_ai/translate/util.py` & `bpm_ai-1.7.1/bpm_ai/translate/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.0/pyproject.toml` & `bpm_ai-1.7.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpm-ai"
-version = "1.7.0"
+version = "1.7.1"
 description = "AI task automation for BPM engines."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai"
 homepage = "https://www.holisticon.de/"
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `bpm_ai-1.7.0/PKG-INFO` & `bpm_ai-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpm-ai
-Version: 1.7.0
+Version: 1.7.1
 Summary: AI task automation for BPM engines.
 Home-page: https://www.holisticon.de/
 License: Apache-2.0
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

