# Comparing `tmp/ragstack_ai_llamaindex-1.0.0.tar.gz` & `tmp/ragstack_ai_llamaindex-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai_llamaindex-1.0.0.tar", max compression
+gzip compressed data, was "ragstack_ai_llamaindex-1.0.1.tar", max compression
```

## Comparing `ragstack_ai_llamaindex-1.0.0.tar` & `ragstack_ai_llamaindex-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      374 2024-04-24 13:31:31.936711 ragstack_ai_llamaindex-1.0.0/README.md
--rw-r--r--   0        0        0     1802 2024-04-24 13:31:31.936711 ragstack_ai_llamaindex-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      271 2024-04-24 13:31:31.936711 ragstack_ai_llamaindex-1.0.0/ragstack_llamaindex/__init__.py
--rw-r--r--   0        0        0      345 2024-04-24 13:31:31.936711 ragstack_ai_llamaindex-1.0.0/ragstack_llamaindex/colbert/__init__.py
--rw-r--r--   0        0        0     1809 2024-04-24 13:31:31.936711 ragstack_ai_llamaindex-1.0.0/ragstack_llamaindex/colbert/retriever.py
--rw-r--r--   0        0        0     2136 1970-01-01 00:00:00.000000 ragstack_ai_llamaindex-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      374 2024-04-30 16:33:53.855756 ragstack_ai_llamaindex-1.0.1/README.md
+-rw-r--r--   0        0        0     1802 2024-04-30 16:33:53.855756 ragstack_ai_llamaindex-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      271 2024-04-30 16:33:53.855756 ragstack_ai_llamaindex-1.0.1/ragstack_llamaindex/__init__.py
+-rw-r--r--   0        0        0      345 2024-04-30 16:33:53.855756 ragstack_ai_llamaindex-1.0.1/ragstack_llamaindex/colbert/__init__.py
+-rw-r--r--   0        0        0     1809 2024-04-30 16:33:53.855756 ragstack_ai_llamaindex-1.0.1/ragstack_llamaindex/colbert/retriever.py
+-rw-r--r--   0        0        0     2136 1970-01-01 00:00:00.000000 ragstack_ai_llamaindex-1.0.1/PKG-INFO
```

### Comparing `ragstack_ai_llamaindex-1.0.0/pyproject.toml` & `ragstack_ai_llamaindex-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "ragstack-ai-llamaindex"
-version = "1.0.0"
+version = "1.0.1"
 description = "DataStax RAGStack Llama Index"
 license = "BUSL-1.1"
 authors = ["DataStax"]
 readme = "README.md"
 repository = "https://github.com/datastax/ragstack-ai"
 documentation = "https://docs.datastax.com/en/ragstack"
 packages = [{ include = "ragstack_llamaindex" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 astrapy = "^1"
 cassio = "~0.1.4"
 unstructured = "0.12.5"
-ragstack-ai-colbert = "1.0.0"
+ragstack-ai-colbert = "1.0.1"
 
 # llama-index
 llama-index = "0.10.31"
 llama-index-vector-stores-astra-db = "0.1.7"
 llama-index-vector-stores-cassandra = "0.1.3"
 llama-index-embeddings-langchain = "0.1.2"
 llama-parse = "0.4.1"
```

### Comparing `ragstack_ai_llamaindex-1.0.0/ragstack_llamaindex/colbert/retriever.py` & `ragstack_ai_llamaindex-1.0.1/ragstack_llamaindex/colbert/retriever.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_llamaindex-1.0.0/PKG-INFO` & `ragstack_ai_llamaindex-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragstack-ai-llamaindex
-Version: 1.0.0
+Version: 1.0.1
 Summary: DataStax RAGStack Llama Index
 Home-page: https://github.com/datastax/ragstack-ai
 License: BUSL-1.1
 Author: DataStax
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
 Requires-Dist: llama-index-llms-bedrock (==0.1.7) ; extra == "bedrock"
 Requires-Dist: llama-index-llms-gemini (==0.1.7) ; extra == "google"
 Requires-Dist: llama-index-llms-vertex (==0.1.5) ; extra == "google"
 Requires-Dist: llama-index-multi-modal-llms-gemini (==0.1.5) ; extra == "google"
 Requires-Dist: llama-index-vector-stores-astra-db (==0.1.7)
 Requires-Dist: llama-index-vector-stores-cassandra (==0.1.3)
 Requires-Dist: llama-parse (==0.4.1)
-Requires-Dist: ragstack-ai-colbert (==1.0.0) ; extra == "colbert"
+Requires-Dist: ragstack-ai-colbert (==1.0.1) ; extra == "colbert"
 Requires-Dist: unstructured (==0.12.5)
 Project-URL: Documentation, https://docs.datastax.com/en/ragstack
 Project-URL: Repository, https://github.com/datastax/ragstack-ai
 Description-Content-Type: text/markdown
 
 # RAGStack LLamaIndex
```

