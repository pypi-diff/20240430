# Comparing `tmp/retriever_search-0.0.8.tar.gz` & `tmp/retriever_search-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retriever_search-0.0.8.tar", last modified: Tue Apr 30 05:47:14 2024, max compression
+gzip compressed data, was "retriever_search-0.0.9.tar", last modified: Tue Apr 30 17:06:15 2024, max compression
```

## Comparing `retriever_search-0.0.8.tar` & `retriever_search-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 05:47:14.076521 retriever_search-0.0.8/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.0.8/LICENSE
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1990 2024-04-30 05:47:14.076160 retriever_search-0.0.8/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1355 2024-04-30 05:46:26.000000 retriever_search-0.0.8/README.md
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 05:47:14.073933 retriever_search-0.0.8/retriever_search/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     6493 2024-04-30 05:36:58.000000 retriever_search-0.0.8/retriever_search/DocumentIngestion.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1922 2024-04-24 08:53:52.000000 retriever_search-0.0.8/retriever_search/QueryPipeline.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       85 2024-04-30 05:46:05.000000 retriever_search-0.0.8/retriever_search/__init__.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3617 2024-04-24 08:53:52.000000 retriever_search-0.0.8/retriever_search/frontend_app.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1509 2024-04-30 05:38:18.000000 retriever_search-0.0.8/retriever_search/search_app.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3424 2024-04-30 05:40:42.000000 retriever_search-0.0.8/retriever_search/search_server.py
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 05:47:14.075727 retriever_search-0.0.8/retriever_search.egg-info/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1990 2024-04-30 05:47:14.000000 retriever_search-0.0.8/retriever_search.egg-info/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      424 2024-04-30 05:47:14.000000 retriever_search-0.0.8/retriever_search.egg-info/SOURCES.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-04-30 05:47:14.000000 retriever_search-0.0.8/retriever_search.egg-info/dependency_links.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      191 2024-04-30 05:47:14.000000 retriever_search-0.0.8/retriever_search.egg-info/requires.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-04-30 05:47:14.000000 retriever_search-0.0.8/retriever_search.egg-info/top_level.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-04-30 05:47:14.076600 retriever_search-0.0.8/setup.cfg
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      834 2024-04-30 04:41:43.000000 retriever_search-0.0.8/setup.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 17:06:15.192411 retriever_search-0.0.9/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.0.9/LICENSE
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1990 2024-04-30 17:06:15.192050 retriever_search-0.0.9/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1355 2024-04-30 05:46:26.000000 retriever_search-0.0.9/README.md
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 17:06:15.190132 retriever_search-0.0.9/retriever_search/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     6508 2024-04-30 16:55:53.000000 retriever_search-0.0.9/retriever_search/DocumentIngestion.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1922 2024-04-24 08:53:52.000000 retriever_search-0.0.9/retriever_search/QueryPipeline.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       85 2024-04-30 17:05:14.000000 retriever_search-0.0.9/retriever_search/__init__.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3617 2024-04-24 08:53:52.000000 retriever_search-0.0.9/retriever_search/frontend_app.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1509 2024-04-30 05:38:18.000000 retriever_search-0.0.9/retriever_search/search_app.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3457 2024-04-30 16:57:19.000000 retriever_search-0.0.9/retriever_search/search_server.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-04-30 17:06:15.191615 retriever_search-0.0.9/retriever_search.egg-info/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1990 2024-04-30 17:06:15.000000 retriever_search-0.0.9/retriever_search.egg-info/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      424 2024-04-30 17:06:15.000000 retriever_search-0.0.9/retriever_search.egg-info/SOURCES.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-04-30 17:06:15.000000 retriever_search-0.0.9/retriever_search.egg-info/dependency_links.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      191 2024-04-30 17:06:15.000000 retriever_search-0.0.9/retriever_search.egg-info/requires.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-04-30 17:06:15.000000 retriever_search-0.0.9/retriever_search.egg-info/top_level.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-04-30 17:06:15.192499 retriever_search-0.0.9/setup.cfg
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      834 2024-04-30 04:41:43.000000 retriever_search-0.0.9/setup.py
```

### Comparing `retriever_search-0.0.8/LICENSE` & `retriever_search-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `retriever_search-0.0.8/PKG-INFO` & `retriever_search-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retriever_search
-Version: 0.0.8
+Version: 0.0.9
 Summary: Local retriever search for your use
 Home-page: https://github.com/GovML/retriever.git
 Author: Sidharth Kathpal
 Author-email: kathpal.sid@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: haystack-ai==2.0.0
```

### Comparing `retriever_search-0.0.8/README.md` & `retriever_search-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `retriever_search-0.0.8/retriever_search/DocumentIngestion.py` & `retriever_search-0.0.9/retriever_search/DocumentIngestion.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             if len(self.documents) >= self.max_docs:
                 print('Hit max documents allowed by your instantiation of max_docs. No more documents to be added.')
                 return
             else:
                 self.documents.append(Document(id = file_name, 
                                             content= content[0:4000],
                                             embedding = None,
-                                            meta = {'embedding_2d': None}
+                                            meta = {'embedding_2d': None, 'title': None}
                                             ))
         except:
             file_name = os.path.basename(pdf_path)
             print(file_name)
         
 
     def load_json(self, json_path):
```

### Comparing `retriever_search-0.0.8/retriever_search/QueryPipeline.py` & `retriever_search-0.0.9/retriever_search/QueryPipeline.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.0.8/retriever_search/frontend_app.py` & `retriever_search-0.0.9/retriever_search/frontend_app.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.0.8/retriever_search/search_app.py` & `retriever_search-0.0.9/retriever_search/search_app.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.0.8/retriever_search/search_server.py` & `retriever_search-0.0.9/retriever_search/search_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     arxiv_links = []
     embedding_2d = []
     print('new search code: ', qa_answer)
 
     for i in range(min(len(documents), len(documents))):
         doc = documents[i]
         doc_id = doc.id
+        print(doc.meta['title'])
         if doc.meta['title'] is not None:
             title = doc.meta['title']
             arxiv_link = f'https://arxiv.org/abs/{doc_id}'
         else:
             title = doc.id.rstrip('.pdf')
             arxiv_link = doc_id
         abstract = doc.content
```

### Comparing `retriever_search-0.0.8/retriever_search.egg-info/PKG-INFO` & `retriever_search-0.0.9/retriever_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retriever_search
-Version: 0.0.8
+Version: 0.0.9
 Summary: Local retriever search for your use
 Home-page: https://github.com/GovML/retriever.git
 Author: Sidharth Kathpal
 Author-email: kathpal.sid@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: haystack-ai==2.0.0
```

### Comparing `retriever_search-0.0.8/setup.py` & `retriever_search-0.0.9/setup.py`

 * *Files identical despite different names*

