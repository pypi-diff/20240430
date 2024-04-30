# Comparing `tmp/ragstack_ai_langchain-1.0.0.tar.gz` & `tmp/ragstack_ai_langchain-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai_langchain-1.0.0.tar", max compression
+gzip compressed data, was "ragstack_ai_langchain-1.0.1.tar", max compression
```

## Comparing `ragstack_ai_langchain-1.0.0.tar` & `ragstack_ai_langchain-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      371 2024-04-24 13:25:38.581902 ragstack_ai_langchain-1.0.0/README.md
--rw-r--r--   0        0        0     1153 2024-04-24 13:25:38.581902 ragstack_ai_langchain-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      271 2024-04-24 13:25:38.581902 ragstack_ai_langchain-1.0.0/ragstack_langchain/__init__.py
--rw-r--r--   0        0        0      344 2024-04-24 13:25:38.581902 ragstack_ai_langchain-1.0.0/ragstack_langchain/colbert/__init__.py
--rw-r--r--   0        0        0     1797 2024-04-24 13:25:38.581902 ragstack_ai_langchain-1.0.0/ragstack_langchain/colbert/retriever.py
--rw-r--r--   0        0        0     1679 1970-01-01 00:00:00.000000 ragstack_ai_langchain-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      371 2024-04-30 16:33:43.850771 ragstack_ai_langchain-1.0.1/README.md
+-rw-r--r--   0        0        0     1153 2024-04-30 16:33:43.850771 ragstack_ai_langchain-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      271 2024-04-30 16:33:43.850771 ragstack_ai_langchain-1.0.1/ragstack_langchain/__init__.py
+-rw-r--r--   0        0        0      344 2024-04-30 16:33:43.850771 ragstack_ai_langchain-1.0.1/ragstack_langchain/colbert/__init__.py
+-rw-r--r--   0        0        0     1797 2024-04-30 16:33:43.850771 ragstack_ai_langchain-1.0.1/ragstack_langchain/colbert/retriever.py
+-rw-r--r--   0        0        0     1679 1970-01-01 00:00:00.000000 ragstack_ai_langchain-1.0.1/PKG-INFO
```

### Comparing `ragstack_ai_langchain-1.0.0/pyproject.toml` & `ragstack_ai_langchain-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "ragstack-ai-langchain"
-version = "1.0.0"
+version = "1.0.1"
 description = "DataStax RAGStack Langchain"
 license = "BUSL-1.1"
 authors = ["DataStax"]
 readme = "README.md"
 repository = "https://github.com/datastax/ragstack-ai"
 documentation = "https://docs.datastax.com/en/ragstack"
 packages = [{ include = "ragstack_langchain" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 astrapy = "^1"
 cassio = "~0.1.4"
 unstructured = "0.12.5"
-ragstack-ai-colbert = "1.0.0"
+ragstack-ai-colbert = "1.0.1"
 
 # langchain
 langchain = "0.1.16"
 langchain-core = "0.1.45"
 langchain-community = "0.0.34"
 langchain-astradb = "0.2.0"
 langchain-openai = "0.1.3"
```

### Comparing `ragstack_ai_langchain-1.0.0/ragstack_langchain/colbert/retriever.py` & `ragstack_ai_langchain-1.0.1/ragstack_langchain/colbert/retriever.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_langchain-1.0.0/PKG-INFO` & `ragstack_ai_langchain-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragstack-ai-langchain
-Version: 1.0.0
+Version: 1.0.1
 Summary: DataStax RAGStack Langchain
 Home-page: https://github.com/datastax/ragstack-ai
 License: BUSL-1.1
 Author: DataStax
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 Requires-Dist: langchain-astradb (==0.2.0)
 Requires-Dist: langchain-community (==0.0.34)
 Requires-Dist: langchain-core (==0.1.45)
 Requires-Dist: langchain-google-genai (==0.0.11) ; extra == "google"
 Requires-Dist: langchain-google-vertexai (==1.0.1) ; extra == "google"
 Requires-Dist: langchain-nvidia-ai-endpoints (==0.0.9) ; extra == "nvidia"
 Requires-Dist: langchain-openai (==0.1.3)
-Requires-Dist: ragstack-ai-colbert (==1.0.0) ; extra == "colbert"
+Requires-Dist: ragstack-ai-colbert (==1.0.1) ; extra == "colbert"
 Requires-Dist: unstructured (==0.12.5)
 Project-URL: Documentation, https://docs.datastax.com/en/ragstack
 Project-URL: Repository, https://github.com/datastax/ragstack-ai
 Description-Content-Type: text/markdown
 
 # RAGStack LangChain
```

