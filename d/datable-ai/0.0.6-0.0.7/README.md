# Comparing `tmp/datable_ai-0.0.6.tar.gz` & `tmp/datable_ai-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datable_ai-0.0.6.tar", max compression
+gzip compressed data, was "datable_ai-0.0.7.tar", max compression
```

## Comparing `datable_ai-0.0.6.tar` & `datable_ai-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2024-04-16 04:28:26.214655 datable_ai-0.0.6/LICENSE
--rw-r--r--   0        0        0       24 2024-04-16 04:28:26.214775 datable_ai-0.0.6/README.md
--rw-r--r--   0        0        0      137 2024-04-22 02:56:10.143859 datable_ai-0.0.6/datable_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 07:16:32.282582 datable_ai-0.0.6/datable_ai/core/__init__.py
--rw-r--r--   0        0        0     2276 2024-04-19 04:23:17.212551 datable_ai-0.0.6/datable_ai/core/llm.py
--rw-r--r--   0        0        0     4017 2024-04-22 04:36:14.538424 datable_ai-0.0.6/datable_ai/output.py
--rw-r--r--   0        0        0     1736 2024-04-22 00:24:12.885367 datable_ai-0.0.6/datable_ai/structured_output.py
--rw-r--r--   0        0        0      546 2024-04-22 04:36:03.633842 datable_ai-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 datable_ai-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-30 04:31:28.554459 datable_ai-0.0.7/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-30 04:31:28.554459 datable_ai-0.0.7/README.md
+-rw-r--r--   0        0        0      137 2024-04-30 04:31:28.554459 datable_ai-0.0.7/datable_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 04:31:28.554459 datable_ai-0.0.7/datable_ai/core/__init__.py
+-rw-r--r--   0        0        0     2276 2024-04-30 04:31:28.554459 datable_ai-0.0.7/datable_ai/core/llm.py
+-rw-r--r--   0        0        0     4017 2024-04-30 04:31:28.554459 datable_ai-0.0.7/datable_ai/output.py
+-rw-r--r--   0        0        0     1736 2024-04-30 04:31:28.554459 datable_ai-0.0.7/datable_ai/structured_output.py
+-rw-r--r--   0        0        0      506 2024-04-30 04:31:28.554459 datable_ai-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 datable_ai-0.0.7/PKG-INFO
```

### Comparing `datable_ai-0.0.6/LICENSE` & `datable_ai-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.6/datable_ai/core/llm.py` & `datable_ai-0.0.7/datable_ai/core/llm.py`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.6/datable_ai/output.py` & `datable_ai-0.0.7/datable_ai/output.py`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.6/datable_ai/structured_output.py` & `datable_ai-0.0.7/datable_ai/structured_output.py`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.6/PKG-INFO` & `datable_ai-0.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datable-ai
-Version: 0.0.6
+Version: 0.0.7
 Summary: datable-ai
 License: MIT
 Author: datable
 Author-email: dev@datable.jp
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,13 +13,12 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: langchain (>=0.1.16,<0.2.0)
 Requires-Dist: langchain-anthropic (>=0.1.11,<0.2.0)
 Requires-Dist: langchain-openai (>=0.1.3,<0.2.0)
 Requires-Dist: openai (>=1.23.1,<2.0.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
-Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Description-Content-Type: text/markdown
 
 # datable-ai
 datable-ai
```

