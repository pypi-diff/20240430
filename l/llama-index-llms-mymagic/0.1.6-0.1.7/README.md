# Comparing `tmp/llama_index_llms_mymagic-0.1.6.tar.gz` & `tmp/llama_index_llms_mymagic-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_mymagic-0.1.6.tar", max compression
+gzip compressed data, was "llama_index_llms_mymagic-0.1.7.tar", max compression
```

## Comparing `llama_index_llms_mymagic-0.1.6.tar` & `llama_index_llms_mymagic-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       39 2024-03-19 15:40:11.936803 llama_index_llms_mymagic-0.1.6/README.md
--rw-r--r--   0        0        0       78 2024-03-19 15:40:11.936803 llama_index_llms_mymagic-0.1.6/llama_index/llms/mymagic/__init__.py
--rw-r--r--   0        0        0     7829 2024-03-19 15:40:11.936803 llama_index_llms_mymagic-0.1.6/llama_index/llms/mymagic/base.py
--rw-r--r--   0        0        0     1434 2024-03-19 15:40:11.936803 llama_index_llms_mymagic-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 llama_index_llms_mymagic-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-04-29 23:54:26.988645 llama_index_llms_mymagic-0.1.7/README.md
+-rw-r--r--   0        0        0       78 2024-04-29 23:54:26.988645 llama_index_llms_mymagic-0.1.7/llama_index/llms/mymagic/__init__.py
+-rw-r--r--   0        0        0     9562 2024-04-29 23:54:26.988645 llama_index_llms_mymagic-0.1.7/llama_index/llms/mymagic/base.py
+-rw-r--r--   0        0        0     1434 2024-04-29 23:54:26.988645 llama_index_llms_mymagic-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 llama_index_llms_mymagic-0.1.7/PKG-INFO
```

### Comparing `llama_index_llms_mymagic-0.1.6/pyproject.toml` & `llama_index_llms_mymagic-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Vitali Avagyan <vitali@mymagic.ai>"]
 description = "llama-index llms mymagic integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-mymagic"
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_llms_mymagic-0.1.6/PKG-INFO` & `llama_index_llms_mymagic-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-mymagic
-Version: 0.1.6
+Version: 0.1.7
 Summary: llama-index llms mymagic integration
 License: MIT
 Author: Vitali Avagyan
 Author-email: vitali@mymagic.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

