# Comparing `tmp/suql-1.1.5.tar.gz` & `tmp/suql-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suql-1.1.5.tar", last modified: Thu Apr 25 17:52:14 2024, max compression
+gzip compressed data, was "suql-1.1.6.tar", last modified: Tue Apr 30 04:29:06 2024, max compression
```

## Comparing `suql-1.1.5.tar` & `suql-1.1.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwx------   0 oval      (1000) users      (100)        0 2024-04-25 17:52:14.590216 suql-1.1.5/
--rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.5/LICENSE
--rw-------   0 oval      (1000) users      (100)     4882 2024-04-25 17:52:14.590216 suql-1.1.5/PKG-INFO
--rw-------   0 oval      (1000) users      (100)     4278 2024-04-15 19:06:57.000000 suql-1.1.5/README.md
--rw-------   0 oval      (1000) users      (100)       38 2024-04-25 17:52:14.590216 suql-1.1.5/setup.cfg
--rw-------   0 oval      (1000) users      (100)     1512 2024-04-25 17:52:02.000000 suql-1.1.5/setup.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-25 17:52:14.586217 suql-1.1.5/src/
-drwx------   0 oval      (1000) users      (100)        0 2024-04-25 17:52:14.590216 suql-1.1.5/src/suql/
--rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/__init__.py
--rw-------   0 oval      (1000) users      (100)    17393 2024-04-25 17:52:02.000000 suql-1.1.5/src/suql/agent.py
--rw-------   0 oval      (1000) users      (100)    16980 2024-04-25 17:38:32.000000 suql-1.1.5/src/suql/faiss_embedding.py
--rw-------   0 oval      (1000) users      (100)     8792 2024-04-17 07:27:02.000000 suql-1.1.5/src/suql/free_text_fcns_server.py
--rw-------   0 oval      (1000) users      (100)     3563 2024-04-25 17:52:02.000000 suql-1.1.5/src/suql/postgresql_connection.py
--rw-------   0 oval      (1000) users      (100)     9612 2024-04-17 08:33:05.000000 suql-1.1.5/src/suql/prompt_continuation.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-25 17:52:14.590216 suql-1.1.5/src/suql/prompts/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.5/src/suql/prompts/__init__.py
--rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/prompts/answer_qa.prompt
--rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/prompts/field_classification.prompt
--rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/prompts/if_db_classification.prompt
--rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/prompts/opening_hours.prompt
--rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/prompts/parser_suql.prompt
--rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/prompts/verification.prompt
--rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/prompts/yelp_response_SQL.prompt
--rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/prompts/yelp_response_no_results.prompt
-drwx------   0 oval      (1000) users      (100)        0 2024-04-25 17:52:14.590216 suql-1.1.5/src/suql/sql_free_text_support/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.5/src/suql/sql_free_text_support/__init__.py
--rw-------   0 oval      (1000) users      (100)    66566 2024-04-25 17:52:02.000000 suql-1.1.5/src/suql/sql_free_text_support/execute_free_text_sql.py
--rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.5/src/suql/utils.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-25 17:52:14.590216 suql-1.1.5/src/suql.egg-info/
--rw-r--r--   0 oval      (1000) users      (100)     4882 2024-04-25 17:52:14.000000 suql-1.1.5/src/suql.egg-info/PKG-INFO
--rw-------   0 oval      (1000) users      (100)      824 2024-04-25 17:52:14.000000 suql-1.1.5/src/suql.egg-info/SOURCES.txt
--rw-------   0 oval      (1000) users      (100)        1 2024-04-25 17:52:14.000000 suql-1.1.5/src/suql.egg-info/dependency_links.txt
--rw-------   0 oval      (1000) users      (100)      186 2024-04-25 17:52:14.000000 suql-1.1.5/src/suql.egg-info/requires.txt
--rw-------   0 oval      (1000) users      (100)        5 2024-04-25 17:52:14.000000 suql-1.1.5/src/suql.egg-info/top_level.txt
+drwx------   0 oval      (1000) users      (100)        0 2024-04-30 04:29:06.602478 suql-1.1.6/
+-rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.6/LICENSE
+-rw-------   0 oval      (1000) users      (100)     5019 2024-04-30 04:29:06.602478 suql-1.1.6/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)     4415 2024-04-30 04:28:53.000000 suql-1.1.6/README.md
+-rw-------   0 oval      (1000) users      (100)       38 2024-04-30 04:29:06.602478 suql-1.1.6/setup.cfg
+-rw-------   0 oval      (1000) users      (100)     1539 2024-04-30 04:28:53.000000 suql-1.1.6/setup.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-30 04:29:06.598478 suql-1.1.6/src/
+drwx------   0 oval      (1000) users      (100)        0 2024-04-30 04:29:06.598478 suql-1.1.6/src/suql/
+-rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/__init__.py
+-rw-------   0 oval      (1000) users      (100)    17393 2024-04-25 17:52:02.000000 suql-1.1.6/src/suql/agent.py
+-rw-------   0 oval      (1000) users      (100)    20797 2024-04-30 04:28:53.000000 suql-1.1.6/src/suql/faiss_embedding.py
+-rw-------   0 oval      (1000) users      (100)     8792 2024-04-17 07:27:02.000000 suql-1.1.6/src/suql/free_text_fcns_server.py
+-rw-------   0 oval      (1000) users      (100)     3563 2024-04-25 17:52:02.000000 suql-1.1.6/src/suql/postgresql_connection.py
+-rw-------   0 oval      (1000) users      (100)     9612 2024-04-17 08:33:05.000000 suql-1.1.6/src/suql/prompt_continuation.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-30 04:29:06.602478 suql-1.1.6/src/suql/prompts/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.6/src/suql/prompts/__init__.py
+-rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/prompts/answer_qa.prompt
+-rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/prompts/field_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/prompts/if_db_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/prompts/opening_hours.prompt
+-rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/prompts/parser_suql.prompt
+-rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/prompts/verification.prompt
+-rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/prompts/yelp_response_SQL.prompt
+-rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/prompts/yelp_response_no_results.prompt
+drwx------   0 oval      (1000) users      (100)        0 2024-04-30 04:29:06.602478 suql-1.1.6/src/suql/sql_free_text_support/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.6/src/suql/sql_free_text_support/__init__.py
+-rw-------   0 oval      (1000) users      (100)    66566 2024-04-25 17:52:02.000000 suql-1.1.6/src/suql/sql_free_text_support/execute_free_text_sql.py
+-rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/utils.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-30 04:29:06.602478 suql-1.1.6/src/suql.egg-info/
+-rw-r--r--   0 oval      (1000) users      (100)     5019 2024-04-30 04:29:06.000000 suql-1.1.6/src/suql.egg-info/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)      824 2024-04-30 04:29:06.000000 suql-1.1.6/src/suql.egg-info/SOURCES.txt
+-rw-------   0 oval      (1000) users      (100)        1 2024-04-30 04:29:06.000000 suql-1.1.6/src/suql.egg-info/dependency_links.txt
+-rw-------   0 oval      (1000) users      (100)      206 2024-04-30 04:29:06.000000 suql-1.1.6/src/suql.egg-info/requires.txt
+-rw-------   0 oval      (1000) users      (100)        5 2024-04-30 04:29:06.000000 suql-1.1.6/src/suql.egg-info/top_level.txt
```

### Comparing `suql-1.1.5/LICENSE` & `suql-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `suql-1.1.5/PKG-INFO` & `suql-1.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.5
+Version: 1.1.6
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -76,14 +76,18 @@
 
 Ideal for using this repo to build a SUQL-powered conversational interface to your data out-of-the-box, like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See [install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/install_source.md) for details.
 
 ## Agent tutorial
 
 Check out [conv_agent.md](https://github.com/stanford-oval/suql/blob/main/docs/conv_agent.md) for more information on best practices for using SUQL to power your conversational agent.
 
+# Release notes
+
+Check [release_notes.md](https://github.com/stanford-oval/suql/blob/main/docs/release_notes.md) for new release notes.
+
 # Bugs / Contribution
 
 If you encounter a problem, first check [known_issues.md](https://github.com/stanford-oval/suql/blob/main/docs/known_issues.md). If it is not listed there, we welcome Issues and/or PRs!
 
 # Paper results
 
 To replicate our results on HybridQA and restaurants in our paper, see [paper_results.md](https://github.com/stanford-oval/suql/blob/main/docs/paper_results.md) for details.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.5 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.6 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
@@ -39,18 +39,20 @@
 install_pip.md) for details. ## Install from source Ideal for using this repo
 to build a SUQL-powered conversational interface to your data out-of-the-box,
 like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See
 [install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/
 install_source.md) for details. ## Agent tutorial Check out [conv_agent.md]
 (https://github.com/stanford-oval/suql/blob/main/docs/conv_agent.md) for more
 information on best practices for using SUQL to power your conversational
-agent. # Bugs / Contribution If you encounter a problem, first check
-[known_issues.md](https://github.com/stanford-oval/suql/blob/main/docs/
-known_issues.md). If it is not listed there, we welcome Issues and/or PRs! #
-Paper results To replicate our results on HybridQA and restaurants in our
-paper, see [paper_results.md](https://github.com/stanford-oval/suql/blob/main/
-docs/paper_results.md) for details. # Citation If you find this work useful to
-you, please consider citing us. ``` @inproceedings{liu2024suql, title={SUQL:
-Conversational Search over Structured and Unstructured Data with Large Language
-Models}, author={Shicheng Liu and Jialiang Xu and Wesley Tjangnaka and Sina J.
-Semnani and Chen Jie Yu and Monica S. Lam}, booktitle = {Findings of the
-Association for Computational Linguistics: NAACL 2024}, year={2024} } ```
+agent. # Release notes Check [release_notes.md](https://github.com/stanford-
+oval/suql/blob/main/docs/release_notes.md) for new release notes. # Bugs /
+Contribution If you encounter a problem, first check [known_issues.md](https://
+github.com/stanford-oval/suql/blob/main/docs/known_issues.md). If it is not
+listed there, we welcome Issues and/or PRs! # Paper results To replicate our
+results on HybridQA and restaurants in our paper, see [paper_results.md](https:
+//github.com/stanford-oval/suql/blob/main/docs/paper_results.md) for details. #
+Citation If you find this work useful to you, please consider citing us. ```
+@inproceedings{liu2024suql, title={SUQL: Conversational Search over Structured
+and Unstructured Data with Large Language Models}, author={Shicheng Liu and
+Jialiang Xu and Wesley Tjangnaka and Sina J. Semnani and Chen Jie Yu and Monica
+S. Lam}, booktitle = {Findings of the Association for Computational
+Linguistics: NAACL 2024}, year={2024} } ```
```

### Comparing `suql-1.1.5/README.md` & `suql-1.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,18 @@
 
 Ideal for using this repo to build a SUQL-powered conversational interface to your data out-of-the-box, like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See [install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/install_source.md) for details.
 
 ## Agent tutorial
 
 Check out [conv_agent.md](https://github.com/stanford-oval/suql/blob/main/docs/conv_agent.md) for more information on best practices for using SUQL to power your conversational agent.
 
+# Release notes
+
+Check [release_notes.md](https://github.com/stanford-oval/suql/blob/main/docs/release_notes.md) for new release notes.
+
 # Bugs / Contribution
 
 If you encounter a problem, first check [known_issues.md](https://github.com/stanford-oval/suql/blob/main/docs/known_issues.md). If it is not listed there, we welcome Issues and/or PRs!
 
 # Paper results
 
 To replicate our results on HybridQA and restaurants in our paper, see [paper_results.md](https://github.com/stanford-oval/suql/blob/main/docs/paper_results.md) for details.
```

#### html2text {}

```diff
@@ -31,18 +31,20 @@
 install_pip.md) for details. ## Install from source Ideal for using this repo
 to build a SUQL-powered conversational interface to your data out-of-the-box,
 like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See
 [install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/
 install_source.md) for details. ## Agent tutorial Check out [conv_agent.md]
 (https://github.com/stanford-oval/suql/blob/main/docs/conv_agent.md) for more
 information on best practices for using SUQL to power your conversational
-agent. # Bugs / Contribution If you encounter a problem, first check
-[known_issues.md](https://github.com/stanford-oval/suql/blob/main/docs/
-known_issues.md). If it is not listed there, we welcome Issues and/or PRs! #
-Paper results To replicate our results on HybridQA and restaurants in our
-paper, see [paper_results.md](https://github.com/stanford-oval/suql/blob/main/
-docs/paper_results.md) for details. # Citation If you find this work useful to
-you, please consider citing us. ``` @inproceedings{liu2024suql, title={SUQL:
-Conversational Search over Structured and Unstructured Data with Large Language
-Models}, author={Shicheng Liu and Jialiang Xu and Wesley Tjangnaka and Sina J.
-Semnani and Chen Jie Yu and Monica S. Lam}, booktitle = {Findings of the
-Association for Computational Linguistics: NAACL 2024}, year={2024} } ```
+agent. # Release notes Check [release_notes.md](https://github.com/stanford-
+oval/suql/blob/main/docs/release_notes.md) for new release notes. # Bugs /
+Contribution If you encounter a problem, first check [known_issues.md](https://
+github.com/stanford-oval/suql/blob/main/docs/known_issues.md). If it is not
+listed there, we welcome Issues and/or PRs! # Paper results To replicate our
+results on HybridQA and restaurants in our paper, see [paper_results.md](https:
+//github.com/stanford-oval/suql/blob/main/docs/paper_results.md) for details. #
+Citation If you find this work useful to you, please consider citing us. ```
+@inproceedings{liu2024suql, title={SUQL: Conversational Search over Structured
+and Unstructured Data with Large Language Models}, author={Shicheng Liu and
+Jialiang Xu and Wesley Tjangnaka and Sina J. Semnani and Chen Jie Yu and Monica
+S. Lam}, booktitle = {Findings of the Association for Computational
+Linguistics: NAACL 2024}, year={2024} } ```
```

### Comparing `suql-1.1.5/setup.py` & `suql-1.1.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 # Package metadata
 name = "suql"
-version = "1.1.5"
+version = "1.1.6"
 description = "Structured and Unstructured Query Language (SUQL) Python API"
 author = "Shicheng Liu"
 author_email = "shicheng@cs.stanford.edu"
 url = "https://github.com/stanford-oval/suql"
 
 # Specify the packages to include. You can use `find_packages` to automatically discover them.
 packages = find_packages(where="src")
@@ -19,15 +19,16 @@
     'Flask-RESTful==0.3.10',
     'requests==2.31.0',
     'spacy==3.6.0',
     'tiktoken==0.4.0',
     'psycopg2-binary==2.9.7',
     'pglast==5.3',
     'FlagEmbedding~=1.2.5',
-    'litellm==1.34.34'
+    'litellm==1.34.34',
+    'platformdirs>=4.0.0'
 ]
 
 # Additional package information
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
```

### Comparing `suql-1.1.5/src/suql/agent.py` & `suql-1.1.6/src/suql/agent.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.5/src/suql/faiss_embedding.py` & `suql-1.1.6/src/suql/faiss_embedding.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # stores a list of embeddings for reviews
 import hashlib
 from collections import OrderedDict
 
+import os
 import faiss
+import hashlib
+import pickle
 from FlagEmbedding import FlagModel
 from flask import Flask, request
 from tqdm import tqdm
+from platformdirs import user_cache_dir
 
 from suql.postgresql_connection import execute_sql
 from suql.utils import chunk_text
 
 # change this line for custom embedding model
 # embedding model output dimension
 EMBEDDING_DIMENSION = 1024
@@ -44,14 +48,21 @@
     return embeddings
 
 
 def compute_sha256(text):
     return hashlib.sha256(text.encode()).hexdigest()
 
 
+def consistent_tuple_hash(tuple_input):
+    # Serialize the tuple to bytes using pickle
+    tuple_bytes = pickle.dumps(tuple_input, protocol=pickle.HIGHEST_PROTOCOL)
+    # Return the SHA-256 hash of the serialized bytes
+    return hashlib.sha256(tuple_bytes).hexdigest()
+
+
 # A set that also preserves insertion order
 class OrderedSet:
     def __init__(self, iterable=None):
         self.items = OrderedDict()
         if iterable:
             self.add_all(iterable)
 
@@ -122,39 +133,50 @@
         table_name,
         primary_key_field_name,
         free_text_field_name,
         db_name="",
         user="select_user",
         password="select_user",
         chunking_param=0,
+        cache_embedding=True,
+        force_recompute=False
     ) -> None:
         # stores three lists:
         # 1. PSQL primary key for each row
         # 2. list of strings in this field
         # 3. matrix of embedding stored on GPU, each chunk is a row
         self.psql_row_ids = []
         self.all_free_text = []
         self.embeddings = None
+        
+        assert chunking_param >= 0
         self.chunking_param = chunking_param
         self.chunked_text = []
 
         # stores a table for bidirectional mapping (for each PSQL table and free text field) between
         # PSQL row ID <-> corresponding indexs for strings <-> corresponding embeddings stored on GPU
         self.document2embedding = {}
         self.embedding2document = {}
         self.id2document = {}
         self.document2id = {}
 
         # stores PSQL login credentails
         self.user = user
         self.password = password
+        
+        # store caching flag
+        assert type(cache_embedding) == bool
+        self.cache_embedding = cache_embedding
+        assert type(force_recompute) == bool
+        self.force_recompute = force_recompute
 
         self.initialize_from_sql(
             table_name, primary_key_field_name, free_text_field_name, db_name
         )
+        print(f"initializing embeddings for DB: {db_name}; TABLE: {table_name}; FREE_TEXT_FIELD: {free_text_field_name}")
         self.initialize_embedding()
 
     def initialize_from_sql(
         self, table_name, primary_key_field_name, free_text_field_name, db_name
     ):
         sql = "SELECT {}, {} FROM {}".format(
             primary_key_field_name, free_text_field_name, table_name
@@ -213,18 +235,44 @@
                         self.embedding2document[num] = document_counter
                     embedding_counter += document_embedding_len
                     document_counter += 1
 
             else:
                 raise ValueError("Expecting type Str")
 
+    def compute_hash(self):
+        # Convert lists to tuples for hashing
+        psql_row_ids_tuple = tuple(self.psql_row_ids)
+        all_free_text_tuple = tuple(self.all_free_text)
+        
+        # Create a combined tuple of all objects
+        combined_data = (psql_row_ids_tuple, all_free_text_tuple, self.chunking_param)
+        
+        # Compute and return the hash of the combined tuple
+        return consistent_tuple_hash(combined_data)
+
     def initialize_embedding(self):
-        print("initializing embeddings for all documents")
+        hash = self.compute_hash()
+        _user_cache_dir = user_cache_dir('suql')
+        faiss_cache_location = os.path.join(_user_cache_dir, f'{hash}.faiss_index')
+        if (os.path.exists(faiss_cache_location) and not self.force_recompute):
+            try:
+                print(f"initializing from existing faiss embedding index at {faiss_cache_location}")
+                self.embeddings = faiss.read_index(faiss_cache_location)
+                return
+            except Exception:
+                print(f"reading {faiss_cache_location} failed. Re-computing embeddings")
+        
         self.embeddings = faiss.IndexFlatIP(EMBEDDING_DIMENSION)
-        self.embeddings.add(embed_documents(self.chunked_text))
+        indexs = embed_documents(self.chunked_text)
+        self.embeddings.add(indexs)
+        
+        print(f"writing computed faiss embedding to {faiss_cache_location}")
+        os.makedirs(_user_cache_dir, exist_ok=True)
+        faiss.write_index(self.embeddings, faiss_cache_location)
 
     def dot_product(self, id_list, query, top, individual_id_list=[]):
         # given a list of id and a particular query, return the top ids and documents according to similarity score ranking
 
         if individual_id_list == []:
             document_indices = [
                 item
@@ -356,22 +404,58 @@
 class MultipleEmbeddingStore:
     def __init__(self) -> None:
         # table name -> free text field name -> EmbeddingStore
         self.mapping = {}
 
     def add(
         self,
-        table_name,
-        primary_key_field_name,
-        free_text_field_name,
-        db_name,
+        table_name: str,
+        primary_key_field_name: str,
+        free_text_field_name: str,
+        db_name: str,
         user="select_user",
         password="select_user",
         chunking_param=0,
+        cache_embedding=True,
+        force_recompute=False
     ):
+        """
+        Add a free text field to the SUQL embedding store to make it
+        available to the compiler.
+
+        # Parameters:
+
+        `table_name` (str): Table name of the free text field.
+        
+        `primary_key_field_name` (str): Primary key field name of the table `table_name`.
+        
+        `free_text_field_name` (str): Free text field name to be embedded.
+        
+        `db_name` (str): PostgreSQL database name of the table `table_name`.
+        
+        `user` (str, optional): User name with `SELECT` privilege on the table `table_name`.
+        Defaults to "select_user".
+        
+        `password` (str, optional): Password for the above user with `SELECT` privilege
+        on the table `table_name`. Defaults to "select_user".
+        
+        `chunking_param` (int, optional): Chunking parameter for embedding.
+        It denotes how many tokens (determined by `en_core_web_sm`) to chunk to for each
+        free text value. Defaults to 0, which denotes no chunking.
+        
+        `cache_embedding` (bool, optional): Whether to cache embeddings to disk. If cached,
+        this file computes a hash of the free text values. If the database values remains
+        unchanged, this file will directly use the cached embeddings. If there are changes
+        to the underlying values, this file will recompute the embeddings.
+        Defaults to True.
+        
+        `force_recompute` (bool, optional): Whether to force recomputing embeddings.
+        If set to True, this file will re-compute the embedding even if a cache exists
+        for the underlying values. Defaults to False.
+        """
         if (
             table_name in self.mapping
             and free_text_field_name in self.mapping[table_name]
         ):
             print(
                 "Table {} for free text field {} already in storage. Negelecting...".format(
                     table_name, free_text_field_name
@@ -384,14 +468,16 @@
             table_name,
             primary_key_field_name,
             free_text_field_name,
             db_name,
             user=user,
             password=password,
             chunking_param=chunking_param,
+            cache_embedding=cache_embedding,
+            force_recompute=force_recompute
         )
 
     def retrieve(self, table_name, free_text_field_name):
         return self.mapping[table_name][free_text_field_name]
 
     def _dot_product(self, id_list, field_query_list, top, single_table):
         # with joins, `field_query_list` stores the table and free text field as a tuple
```

### Comparing `suql-1.1.5/src/suql/free_text_fcns_server.py` & `suql-1.1.6/src/suql/free_text_fcns_server.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.5/src/suql/postgresql_connection.py` & `suql-1.1.6/src/suql/postgresql_connection.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.5/src/suql/prompt_continuation.py` & `suql-1.1.6/src/suql/prompt_continuation.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.5/src/suql/prompts/if_db_classification.prompt` & `suql-1.1.6/src/suql/prompts/if_db_classification.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.5/src/suql/prompts/opening_hours.prompt` & `suql-1.1.6/src/suql/prompts/opening_hours.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.5/src/suql/prompts/parser_suql.prompt` & `suql-1.1.6/src/suql/prompts/parser_suql.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.5/src/suql/prompts/yelp_response_SQL.prompt` & `suql-1.1.6/src/suql/prompts/yelp_response_SQL.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.5/src/suql/prompts/yelp_response_no_results.prompt` & `suql-1.1.6/src/suql/prompts/yelp_response_no_results.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.5/src/suql/sql_free_text_support/execute_free_text_sql.py` & `suql-1.1.6/src/suql/sql_free_text_support/execute_free_text_sql.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.5/src/suql/utils.py` & `suql-1.1.6/src/suql/utils.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.5/src/suql.egg-info/PKG-INFO` & `suql-1.1.6/src/suql.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.5
+Version: 1.1.6
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -76,14 +76,18 @@
 
 Ideal for using this repo to build a SUQL-powered conversational interface to your data out-of-the-box, like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See [install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/install_source.md) for details.
 
 ## Agent tutorial
 
 Check out [conv_agent.md](https://github.com/stanford-oval/suql/blob/main/docs/conv_agent.md) for more information on best practices for using SUQL to power your conversational agent.
 
+# Release notes
+
+Check [release_notes.md](https://github.com/stanford-oval/suql/blob/main/docs/release_notes.md) for new release notes.
+
 # Bugs / Contribution
 
 If you encounter a problem, first check [known_issues.md](https://github.com/stanford-oval/suql/blob/main/docs/known_issues.md). If it is not listed there, we welcome Issues and/or PRs!
 
 # Paper results
 
 To replicate our results on HybridQA and restaurants in our paper, see [paper_results.md](https://github.com/stanford-oval/suql/blob/main/docs/paper_results.md) for details.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.5 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.6 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
@@ -39,18 +39,20 @@
 install_pip.md) for details. ## Install from source Ideal for using this repo
 to build a SUQL-powered conversational interface to your data out-of-the-box,
 like the one for https://yelpbot.genie.stanford.edu discussed in the paper. See
 [install_source.md](https://github.com/stanford-oval/suql/blob/main/docs/
 install_source.md) for details. ## Agent tutorial Check out [conv_agent.md]
 (https://github.com/stanford-oval/suql/blob/main/docs/conv_agent.md) for more
 information on best practices for using SUQL to power your conversational
-agent. # Bugs / Contribution If you encounter a problem, first check
-[known_issues.md](https://github.com/stanford-oval/suql/blob/main/docs/
-known_issues.md). If it is not listed there, we welcome Issues and/or PRs! #
-Paper results To replicate our results on HybridQA and restaurants in our
-paper, see [paper_results.md](https://github.com/stanford-oval/suql/blob/main/
-docs/paper_results.md) for details. # Citation If you find this work useful to
-you, please consider citing us. ``` @inproceedings{liu2024suql, title={SUQL:
-Conversational Search over Structured and Unstructured Data with Large Language
-Models}, author={Shicheng Liu and Jialiang Xu and Wesley Tjangnaka and Sina J.
-Semnani and Chen Jie Yu and Monica S. Lam}, booktitle = {Findings of the
-Association for Computational Linguistics: NAACL 2024}, year={2024} } ```
+agent. # Release notes Check [release_notes.md](https://github.com/stanford-
+oval/suql/blob/main/docs/release_notes.md) for new release notes. # Bugs /
+Contribution If you encounter a problem, first check [known_issues.md](https://
+github.com/stanford-oval/suql/blob/main/docs/known_issues.md). If it is not
+listed there, we welcome Issues and/or PRs! # Paper results To replicate our
+results on HybridQA and restaurants in our paper, see [paper_results.md](https:
+//github.com/stanford-oval/suql/blob/main/docs/paper_results.md) for details. #
+Citation If you find this work useful to you, please consider citing us. ```
+@inproceedings{liu2024suql, title={SUQL: Conversational Search over Structured
+and Unstructured Data with Large Language Models}, author={Shicheng Liu and
+Jialiang Xu and Wesley Tjangnaka and Sina J. Semnani and Chen Jie Yu and Monica
+S. Lam}, booktitle = {Findings of the Association for Computational
+Linguistics: NAACL 2024}, year={2024} } ```
```

### Comparing `suql-1.1.5/src/suql.egg-info/SOURCES.txt` & `suql-1.1.6/src/suql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

