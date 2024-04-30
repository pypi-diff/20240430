# Comparing `tmp/retriever_search-0.0.6.tar.gz` & `tmp/retriever_search-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retriever_search-0.0.6.tar", last modified: Tue Apr 30 05:07:14 2024, max compression
+gzip compressed data, was "retriever_search-0.0.7.tar", last modified: Tue Apr 30 05:41:49 2024, max compression
```

## Comparing `retriever_search-0.0.6.tar` & `retriever_search-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 05:07:14.939724 retriever_search-0.0.6/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.0.6/LICENSE
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1841 2024-04-30 05:07:14.939390 retriever_search-0.0.6/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1205 2024-04-30 05:04:29.000000 retriever_search-0.0.6/README.md
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 05:07:14.937301 retriever_search-0.0.6/retriever_search/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     6434 2024-04-24 08:53:52.000000 retriever_search-0.0.6/retriever_search/DocumentIngestion.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1922 2024-04-24 08:53:52.000000 retriever_search-0.0.6/retriever_search/QueryPipeline.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       85 2024-04-30 05:07:08.000000 retriever_search-0.0.6/retriever_search/__init__.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3617 2024-04-24 08:53:52.000000 retriever_search-0.0.6/retriever_search/frontend_app.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1424 2024-04-25 03:47:47.000000 retriever_search-0.0.6/retriever_search/search_app.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3381 2024-04-25 03:47:48.000000 retriever_search-0.0.6/retriever_search/search_server.py
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 05:07:14.938963 retriever_search-0.0.6/retriever_search.egg-info/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1841 2024-04-30 05:07:14.000000 retriever_search-0.0.6/retriever_search.egg-info/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      424 2024-04-30 05:07:14.000000 retriever_search-0.0.6/retriever_search.egg-info/SOURCES.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-04-30 05:07:14.000000 retriever_search-0.0.6/retriever_search.egg-info/dependency_links.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      191 2024-04-30 05:07:14.000000 retriever_search-0.0.6/retriever_search.egg-info/requires.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-04-30 05:07:14.000000 retriever_search-0.0.6/retriever_search.egg-info/top_level.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-04-30 05:07:14.939798 retriever_search-0.0.6/setup.cfg
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      834 2024-04-30 04:41:43.000000 retriever_search-0.0.6/setup.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 05:41:49.305215 retriever_search-0.0.7/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.0.7/LICENSE
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1976 2024-04-30 05:41:49.304879 retriever_search-0.0.7/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1341 2024-04-30 05:13:10.000000 retriever_search-0.0.7/README.md
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 05:41:49.302790 retriever_search-0.0.7/retriever_search/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     6493 2024-04-30 05:36:58.000000 retriever_search-0.0.7/retriever_search/DocumentIngestion.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1922 2024-04-24 08:53:52.000000 retriever_search-0.0.7/retriever_search/QueryPipeline.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       85 2024-04-30 05:41:45.000000 retriever_search-0.0.7/retriever_search/__init__.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3617 2024-04-24 08:53:52.000000 retriever_search-0.0.7/retriever_search/frontend_app.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1509 2024-04-30 05:38:18.000000 retriever_search-0.0.7/retriever_search/search_app.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3424 2024-04-30 05:40:42.000000 retriever_search-0.0.7/retriever_search/search_server.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 05:41:49.304453 retriever_search-0.0.7/retriever_search.egg-info/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1976 2024-04-30 05:41:49.000000 retriever_search-0.0.7/retriever_search.egg-info/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      424 2024-04-30 05:41:49.000000 retriever_search-0.0.7/retriever_search.egg-info/SOURCES.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-04-30 05:41:49.000000 retriever_search-0.0.7/retriever_search.egg-info/dependency_links.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      191 2024-04-30 05:41:49.000000 retriever_search-0.0.7/retriever_search.egg-info/requires.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-04-30 05:41:49.000000 retriever_search-0.0.7/retriever_search.egg-info/top_level.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-04-30 05:41:49.305291 retriever_search-0.0.7/setup.cfg
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      834 2024-04-30 04:41:43.000000 retriever_search-0.0.7/setup.py
```

### Comparing `retriever_search-0.0.6/LICENSE` & `retriever_search-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `retriever_search-0.0.6/PKG-INFO` & `retriever_search-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retriever_search
-Version: 0.0.6
+Version: 0.0.7
 Summary: Local retriever search for your use
 Home-page: https://github.com/GovML/retriever.git
 Author: Sidharth Kathpal
 Author-email: kathpal.sid@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: haystack-ai==2.0.0
@@ -58,7 +58,12 @@
 
 ```bash
 >>> from retriever_search import search_server
 >>> from retriever_search import frontend_app as fp
 >>> fp.run_frontend()
 >>> search_server.run_search_server('path_to_folder', 'save_json_path')
 ```
+
+## Where to access the frontend 
+
+Access via the following URL - http://127.0.0.1:7860 
+This URL would work for your local setup only
```

### Comparing `retriever_search-0.0.6/retriever_search/DocumentIngestion.py` & `retriever_search-0.0.7/retriever_search/DocumentIngestion.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 from haystack.components.embedders import SentenceTransformersDocumentEmbedder
 from sentence_transformers import SentenceTransformer
 from sklearn.manifold import TSNE
 import numpy as np
 import umap.umap_ as umap
 
 class DocumentIngestion:
-    def __init__(self, path, model = None, max_docs = float("inf")):
+    def __init__(self, path, model = None, device = 'cpu', max_docs = float("inf")):
         self.path = path
         self.documents = []
         self.max_docs = max_docs
-        print(path)
+        self.device = device
+        print(path, device)
         if path.endswith('.pdf'):
             # Handle single PDF file
             if model == None:
                 assert False, 'Specify a model to embed the document.'
             self.ingest_pdf(path)
             
         elif path.endswith('.json'):
@@ -117,15 +118,15 @@
         # Convert all PDFs in a directory to documents
         for file_name in tqdm(os.listdir(self.path)):
             if file_name.endswith('.pdf'):
                 pdf_path = os.path.join(self.path, file_name)
                 self.ingest_pdf(pdf_path)
 
     def create_embeddings(self, model):
-        model = SentenceTransformer(model, device = 'mps')
+        model = SentenceTransformer(model, device = self.device)
    
         content = []
         for doc in tqdm(self.documents):
             content.append(doc.content)
         embeddings = model.encode(content, batch_size = 128, show_progress_bar = True)
         for i, doc in enumerate(tqdm(self.documents)):
             doc.embedding = embeddings[i].tolist()
```

### Comparing `retriever_search-0.0.6/retriever_search/QueryPipeline.py` & `retriever_search-0.0.7/retriever_search/QueryPipeline.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.0.6/retriever_search/frontend_app.py` & `retriever_search-0.0.7/retriever_search/frontend_app.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.0.6/retriever_search/search_app.py` & `retriever_search-0.0.7/retriever_search/search_app.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 import os
 from retriever_search.DocumentIngestion import DocumentIngestion
 from retriever_search.QueryPipeline import QueryPipeline
 from haystack_integrations.document_stores.qdrant import QdrantDocumentStore
 
 
 class search_app:
-    def __init__(self, inputDirectory, json_save_path, embedding_2d = "red_emb_1K.npy"):
+    def __init__(self, inputDirectory, json_save_path, embedding_2d = "red_emb_1K.npy", device = 'cpu'):
         self.embedding_2d = embedding_2d
         self.json_path = json_save_path
         self.inputDirectory = inputDirectory
+        self.device = device
 
     def new_search_run(self):
         #model = 'sentence-transformers/all-mpnet-base-v2'
         model = 'sentence-transformers/allenai-specter'
         #model = 'Dagar/t5-small-science-papers'
         if os.path.exists(self.json_path):
-            ingestion = DocumentIngestion(self.json_path, model = None)
+            ingestion = DocumentIngestion(self.json_path, model = None, device=self.device)
         else:
-            ingestion = DocumentIngestion(self.inputDirectory, model = model)
+            ingestion = DocumentIngestion(self.inputDirectory, model = model, device=self.device)
             ingestion.to_json(self.json_path)
 
         document_store = document_store = QdrantDocumentStore(
             ":memory:",
             embedding_dim=768,  # the embedding_dim should match that of the embedding model
         )
```

### Comparing `retriever_search-0.0.6/retriever_search/search_server.py` & `retriever_search-0.0.7/retriever_search/search_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,12 +89,13 @@
         embedding_2d.append({"doc_ids" : doc_id, "embeddings" : emb_2d})
         doc_ids.append(doc_id)
 
     df = pd.DataFrame(list(zip(titles, abstracts, arxiv_links)), columns = ['Title','Content','Link'])
     return df, doc_ids, embedding_2d, qa_answer
 
 
-def run_search_server(inputDirectory, json_save_path):
+def run_search_server(inputDirectory, json_save_path, device):
     global main_pipe
-    search_obj = search_app(inputDirectory, json_save_path)
+    print(device)
+    search_obj = search_app(inputDirectory, json_save_path, device = device)
     main_pipe = search_obj.new_search_run()
     app.run(debug=False, host='127.0.0.1', threaded=True)
```

### Comparing `retriever_search-0.0.6/retriever_search.egg-info/PKG-INFO` & `retriever_search-0.0.7/retriever_search.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retriever_search
-Version: 0.0.6
+Version: 0.0.7
 Summary: Local retriever search for your use
 Home-page: https://github.com/GovML/retriever.git
 Author: Sidharth Kathpal
 Author-email: kathpal.sid@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: haystack-ai==2.0.0
@@ -58,7 +58,12 @@
 
 ```bash
 >>> from retriever_search import search_server
 >>> from retriever_search import frontend_app as fp
 >>> fp.run_frontend()
 >>> search_server.run_search_server('path_to_folder', 'save_json_path')
 ```
+
+## Where to access the frontend 
+
+Access via the following URL - http://127.0.0.1:7860 
+This URL would work for your local setup only
```

### Comparing `retriever_search-0.0.6/setup.py` & `retriever_search-0.0.7/setup.py`

 * *Files identical despite different names*

