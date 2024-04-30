# Comparing `tmp/ragstack_ai_colbert-1.0.0.tar.gz` & `tmp/ragstack_ai_colbert-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai_colbert-1.0.0.tar", max compression
+gzip compressed data, was "ragstack_ai_colbert-1.0.1.tar", max compression
```

## Comparing `ragstack_ai_colbert-1.0.0.tar` & `ragstack_ai_colbert-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      374 2024-04-24 10:24:28.510436 ragstack_ai_colbert-1.0.0/README.md
--rw-r--r--   0        0        0      576 2024-04-24 10:24:28.510436 ragstack_ai_colbert-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1511 2024-04-24 10:24:28.510436 ragstack_ai_colbert-1.0.0/ragstack_colbert/__init__.py
--rw-r--r--   0        0        0     2641 2024-04-24 10:24:28.510436 ragstack_ai_colbert-1.0.0/ragstack_colbert/base_embedding_model.py
--rw-r--r--   0        0        0     1853 2024-04-24 10:24:28.510436 ragstack_ai_colbert-1.0.0/ragstack_colbert/base_retriever.py
--rw-r--r--   0        0        0     2989 2024-04-24 10:24:28.510436 ragstack_ai_colbert-1.0.0/ragstack_colbert/base_vector_store.py
--rw-r--r--   0        0        0     7928 2024-04-24 10:24:28.510436 ragstack_ai_colbert-1.0.0/ragstack_colbert/cassandra_vector_store.py
--rw-r--r--   0        0        0    13411 2024-04-24 10:24:28.510436 ragstack_ai_colbert-1.0.0/ragstack_colbert/cobert_retriever.py
--rw-r--r--   0        0        0    12718 2024-04-24 10:24:28.510436 ragstack_ai_colbert-1.0.0/ragstack_colbert/colbert_embedding_model.py
--rw-r--r--   0        0        0      695 2024-04-24 10:24:28.510436 ragstack_ai_colbert-1.0.0/ragstack_colbert/constant.py
--rw-r--r--   0        0        0      154 2024-04-24 10:24:28.510436 ragstack_ai_colbert-1.0.0/ragstack_colbert/distributed/__init__.py
--rw-r--r--   0        0        0     5617 2024-04-24 10:24:28.510436 ragstack_ai_colbert-1.0.0/ragstack_colbert/distributed/chunk_encoder.py
--rw-r--r--   0        0        0     7136 2024-04-24 10:24:28.510436 ragstack_ai_colbert-1.0.0/ragstack_colbert/distributed/distributed.py
--rw-r--r--   0        0        0     6962 2024-04-24 10:24:28.510436 ragstack_ai_colbert-1.0.0/ragstack_colbert/distributed/runner.py
--rw-r--r--   0        0        0     2702 2024-04-24 10:24:28.510436 ragstack_ai_colbert-1.0.0/ragstack_colbert/objects.py
--rw-r--r--   0        0        0     1165 1970-01-01 00:00:00.000000 ragstack_ai_colbert-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      374 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/README.md
+-rw-r--r--   0        0        0      600 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1512 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/__init__.py
+-rw-r--r--   0        0        0     2641 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/base_embedding_model.py
+-rw-r--r--   0        0        0     1853 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/base_retriever.py
+-rw-r--r--   0        0        0     2989 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/base_vector_store.py
+-rw-r--r--   0        0        0     7928 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/cassandra_vector_store.py
+-rw-r--r--   0        0        0    12718 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/colbert_embedding_model.py
+-rw-r--r--   0        0        0    13608 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/colbert_retriever.py
+-rw-r--r--   0        0        0      695 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/constant.py
+-rw-r--r--   0        0        0      154 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/distributed/__init__.py
+-rw-r--r--   0        0        0     5617 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/distributed/chunk_encoder.py
+-rw-r--r--   0        0        0     7136 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/distributed/distributed.py
+-rw-r--r--   0        0        0     6962 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/distributed/runner.py
+-rw-r--r--   0        0        0     2702 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/objects.py
+-rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 ragstack_ai_colbert-1.0.1/PKG-INFO
```

### Comparing `ragstack_ai_colbert-1.0.0/pyproject.toml` & `ragstack_ai_colbert-1.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "ragstack-ai-colbert"
-version = "1.0.0"
+version = "1.0.1"
 description = "DataStax RAGStack Colbert implementation"
 license = "BUSL-1.1"
 authors = ["DataStax"]
 readme = "README.md"
 repository = "https://github.com/datastax/ragstack-ai"
 documentation = "https://docs.datastax.com/en/ragstack"
 packages = [{ include = "ragstack_colbert" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 colbert-ai = "0.2.19"
 pyarrow = "14.0.1"
 torch = "2.2.1"
 cassio = "~0.1.7"
+nest-asyncio = "^1.6.0"
 
 [tool.poetry.group.test.dependencies]
 ragstack-ai-tests-utils = { path = "../tests-utils", develop = true }
```

### Comparing `ragstack_ai_colbert-1.0.0/ragstack_colbert/__init__.py` & `ragstack_ai_colbert-1.0.1/ragstack_colbert/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 - DEFAULT_COLBERT_MODEL: The default identifier for the ColBERT model.
 - DEFAULT_COLBERT_DIM: The default dimensionality for ColBERT model embeddings.
 - EmbeddedChunk: Data class for representing a chunk of embedded text.
 - RetrievedChunk: Data class for representing a chunk of retrieved text.
 """
 
 from .cassandra_vector_store import CassandraVectorStore
-from .cobert_retriever import ColbertRetriever
+from .colbert_retriever import ColbertRetriever
 from .colbert_embedding_model import ColbertEmbeddingModel
 from .constant import DEFAULT_COLBERT_DIM, DEFAULT_COLBERT_MODEL
 from .objects import ChunkData, EmbeddedChunk, RetrievedChunk
 
 __all__ = [
     "CassandraVectorStore",
     "ChunkData",
```

### Comparing `ragstack_ai_colbert-1.0.0/ragstack_colbert/base_embedding_model.py` & `ragstack_ai_colbert-1.0.1/ragstack_colbert/base_embedding_model.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.0/ragstack_colbert/base_retriever.py` & `ragstack_ai_colbert-1.0.1/ragstack_colbert/base_retriever.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.0/ragstack_colbert/base_vector_store.py` & `ragstack_ai_colbert-1.0.1/ragstack_colbert/base_vector_store.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.0/ragstack_colbert/cassandra_vector_store.py` & `ragstack_ai_colbert-1.0.1/ragstack_colbert/cassandra_vector_store.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.0/ragstack_colbert/cobert_retriever.py` & `ragstack_ai_colbert-1.0.1/ragstack_colbert/colbert_retriever.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 to CPU computation if needed. This flexibility ensures that the retrieval system can be deployed in a
 variety of hardware environments.
 """
 
 import asyncio
 import logging
 import math
+import nest_asyncio
 from typing import Any, Dict, List, Optional, Set
 
 import torch
 from torch import Tensor
 
 from .base_embedding_model import BaseEmbeddingModel
 from .base_retriever import BaseRetriever
@@ -241,24 +242,24 @@
             if isinstance(result, Exception):
                 logging.error(f"Issue on vector_store.get_chunk_text_and_metadata(): {result} at {get_trace(result)}")
             else:
                 chunk, chunk_data = result
                 chunk_data_map[chunk] = chunk_data
 
         answers: List[RetrievedChunk] = []
-        rank = 1
-        for chunk in chunks_by_score:
+
+        for idx, chunk in enumerate(chunks_by_score):
             score = chunk_scores[chunk]
             chunk_data = chunk_data_map[chunk]
             answers.append(
                     RetrievedChunk(
                         doc_id=chunk.doc_id,
                         chunk_id=chunk.chunk_id,
                         score=score.item(),  # Ensure score is a scalar if it's a tensor
-                        rank=rank,
+                        rank=idx + 1,
                         data=chunk_data,
                     )
                 )
 
         return answers
 
     async def aretrieve(
@@ -332,9 +333,12 @@
             List[RetrievedChunk]: A list of RetrievedChunk objects, each representing a text chunk that is relevant
                                   to the query, along with its similarity score and rank.
 
         Note:
             The actual retrieval process involves encoding the query, performing an ANN search to find relevant
             embeddings, scoring these embeddings for similarity, and retrieving the corresponding text chunks.
         """
+        # nest_asyncio does not a new event loop to be created
+        # in the case there is already an event loop such as colab, it's required
+        nest_asyncio.apply()
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(self.aretrieve(query=query, k=k, query_maxlen=query_maxlen))
```

### Comparing `ragstack_ai_colbert-1.0.0/ragstack_colbert/colbert_embedding_model.py` & `ragstack_ai_colbert-1.0.1/ragstack_colbert/colbert_embedding_model.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.0/ragstack_colbert/constant.py` & `ragstack_ai_colbert-1.0.1/ragstack_colbert/constant.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.0/ragstack_colbert/distributed/chunk_encoder.py` & `ragstack_ai_colbert-1.0.1/ragstack_colbert/distributed/chunk_encoder.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.0/ragstack_colbert/distributed/distributed.py` & `ragstack_ai_colbert-1.0.1/ragstack_colbert/distributed/distributed.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.0/ragstack_colbert/distributed/runner.py` & `ragstack_ai_colbert-1.0.1/ragstack_colbert/distributed/runner.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.0/ragstack_colbert/objects.py` & `ragstack_ai_colbert-1.0.1/ragstack_colbert/objects.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.0/PKG-INFO` & `ragstack_ai_colbert-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: ragstack-ai-colbert
-Version: 1.0.0
+Version: 1.0.1
 Summary: DataStax RAGStack Colbert implementation
 Home-page: https://github.com/datastax/ragstack-ai
 License: BUSL-1.1
 Author: DataStax
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cassio (>=0.1.7,<0.2.0)
 Requires-Dist: colbert-ai (==0.2.19)
+Requires-Dist: nest-asyncio (>=1.6.0,<2.0.0)
 Requires-Dist: pyarrow (==14.0.1)
 Requires-Dist: torch (==2.2.1)
 Project-URL: Documentation, https://docs.datastax.com/en/ragstack
 Project-URL: Repository, https://github.com/datastax/ragstack-ai
 Description-Content-Type: text/markdown
 
-# RAGStack Colbert
+# RAGStack ColBERT
 
-RAGStack colbert implementation, part of [`ragstack-ai`](https://pypi.org/project/ragstack-ai/).
+RAGStack ColBERT implementation, part of [`ragstack-ai`](https://pypi.org/project/ragstack-ai/).
 
 ## Documentation
 
 [DataStax RAGStack Documentation](https://docs.datastax.com/en/ragstack/docs/index.html)
 
 [Quickstart](https://docs.datastax.com/en/ragstack/docs/quickstart.html)
```

