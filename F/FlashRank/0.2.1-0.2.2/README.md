# Comparing `tmp/FlashRank-0.2.1.tar.gz` & `tmp/FlashRank-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlashRank-0.2.1.tar", last modified: Tue Apr 30 09:27:38 2024, max compression
+gzip compressed data, was "FlashRank-0.2.2.tar", last modified: Tue Apr 30 10:27:08 2024, max compression
```

## Comparing `FlashRank-0.2.1.tar` & `FlashRank-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-30 09:27:38.722456 FlashRank-0.2.1/
-drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-30 09:27:38.720617 FlashRank-0.2.1/FlashRank.egg-info/
--rw-r--r--   0 prithivida   (501) staff       (20)    10278 2024-04-30 09:27:38.000000 FlashRank-0.2.1/FlashRank.egg-info/PKG-INFO
--rw-r--r--   0 prithivida   (501) staff       (20)      294 2024-04-30 09:27:38.000000 FlashRank-0.2.1/FlashRank.egg-info/SOURCES.txt
--rw-r--r--   0 prithivida   (501) staff       (20)        1 2024-04-30 09:27:38.000000 FlashRank-0.2.1/FlashRank.egg-info/dependency_links.txt
--rw-r--r--   0 prithivida   (501) staff       (20)       43 2024-04-30 09:27:38.000000 FlashRank-0.2.1/FlashRank.egg-info/requires.txt
--rw-r--r--   0 prithivida   (501) staff       (20)       10 2024-04-30 09:27:38.000000 FlashRank-0.2.1/FlashRank.egg-info/top_level.txt
--rw-r--r--   0 prithivida   (501) staff       (20)    11357 2023-12-04 14:24:33.000000 FlashRank-0.2.1/LICENSE
--rw-r--r--   0 prithivida   (501) staff       (20)    10278 2024-04-30 09:27:38.722277 FlashRank-0.2.1/PKG-INFO
--rw-r--r--   0 prithivida   (501) staff       (20)     9757 2024-03-19 01:23:34.000000 FlashRank-0.2.1/README.md
-drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-30 09:27:38.721979 FlashRank-0.2.1/flashrank/
--rw-r--r--   0 prithivida   (501) staff       (20)      608 2024-03-19 00:50:27.000000 FlashRank-0.2.1/flashrank/Config.py
--rw-r--r--   0 prithivida   (501) staff       (20)     7193 2024-04-30 09:24:47.000000 FlashRank-0.2.1/flashrank/Ranker.py
--rw-r--r--   0 prithivida   (501) staff       (20)    10457 2023-12-13 12:36:57.000000 FlashRank-0.2.1/flashrank/Rankerb.py
--rw-r--r--   0 prithivida   (501) staff       (20)     6093 2024-01-29 14:51:57.000000 FlashRank-0.2.1/flashrank/Rankerc.py
--rw-r--r--   0 prithivida   (501) staff       (20)       41 2024-04-30 09:25:26.000000 FlashRank-0.2.1/flashrank/__init__.py
--rw-r--r--   0 prithivida   (501) staff       (20)       38 2024-04-30 09:27:38.722492 FlashRank-0.2.1/setup.cfg
--rw-r--r--   0 prithivida   (501) staff       (20)      819 2024-04-30 09:26:14.000000 FlashRank-0.2.1/setup.py
+drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-30 10:27:08.467244 FlashRank-0.2.2/
+drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-30 10:27:08.465731 FlashRank-0.2.2/FlashRank.egg-info/
+-rw-r--r--   0 prithivida   (501) staff       (20)    10278 2024-04-30 10:27:08.000000 FlashRank-0.2.2/FlashRank.egg-info/PKG-INFO
+-rw-r--r--   0 prithivida   (501) staff       (20)      294 2024-04-30 10:27:08.000000 FlashRank-0.2.2/FlashRank.egg-info/SOURCES.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)        1 2024-04-30 10:27:08.000000 FlashRank-0.2.2/FlashRank.egg-info/dependency_links.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)       68 2024-04-30 10:27:08.000000 FlashRank-0.2.2/FlashRank.egg-info/requires.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)       10 2024-04-30 10:27:08.000000 FlashRank-0.2.2/FlashRank.egg-info/top_level.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)    11357 2023-12-04 14:24:33.000000 FlashRank-0.2.2/LICENSE
+-rw-r--r--   0 prithivida   (501) staff       (20)    10278 2024-04-30 10:27:08.467045 FlashRank-0.2.2/PKG-INFO
+-rw-r--r--   0 prithivida   (501) staff       (20)     9757 2024-03-19 01:23:34.000000 FlashRank-0.2.2/README.md
+drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-30 10:27:08.466722 FlashRank-0.2.2/flashrank/
+-rw-r--r--   0 prithivida   (501) staff       (20)      724 2024-04-30 10:04:33.000000 FlashRank-0.2.2/flashrank/Config.py
+-rw-r--r--   0 prithivida   (501) staff       (20)     9893 2024-04-30 10:26:09.000000 FlashRank-0.2.2/flashrank/Ranker.py
+-rw-r--r--   0 prithivida   (501) staff       (20)    10457 2023-12-13 12:36:57.000000 FlashRank-0.2.2/flashrank/Rankerb.py
+-rw-r--r--   0 prithivida   (501) staff       (20)     6093 2024-01-29 14:51:57.000000 FlashRank-0.2.2/flashrank/Rankerc.py
+-rw-r--r--   0 prithivida   (501) staff       (20)       41 2024-04-30 09:25:26.000000 FlashRank-0.2.2/flashrank/__init__.py
+-rw-r--r--   0 prithivida   (501) staff       (20)       38 2024-04-30 10:27:08.467286 FlashRank-0.2.2/setup.cfg
+-rw-r--r--   0 prithivida   (501) staff       (20)      855 2024-04-30 10:22:38.000000 FlashRank-0.2.2/setup.py
```

### Comparing `FlashRank-0.2.1/FlashRank.egg-info/PKG-INFO` & `FlashRank-0.2.2/FlashRank.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlashRank
-Version: 0.2.1
+Version: 0.2.2
 Summary: Ultra lite & Super fast SoTA cross-encoder based re-ranking for your search & retrieval pipelines.
 Home-page: https://github.com/PrithivirajDamodaran/FlashRank
 Author: Prithivi Da
 Author-email: 
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `FlashRank-0.2.1/LICENSE` & `FlashRank-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FlashRank-0.2.1/PKG-INFO` & `FlashRank-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlashRank
-Version: 0.2.1
+Version: 0.2.2
 Summary: Ultra lite & Super fast SoTA cross-encoder based re-ranking for your search & retrieval pipelines.
 Home-page: https://github.com/PrithivirajDamodaran/FlashRank
 Author: Prithivi Da
 Author-email: 
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `FlashRank-0.2.1/README.md` & `FlashRank-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `FlashRank-0.2.1/flashrank/Config.py` & `FlashRank-0.2.2/flashrank/Config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # Moved to HF - My cloud bucket and $ wont be abused anymore :-)
 # THE HF Repo is UNDER CC-BY-SA LICENSE. USE APPROPRIATELY.
 model_url = 'https://huggingface.co/prithivida/flashrank/resolve/main/{}.zip'
+listwise_rankers = {'rank_zephyr_7b_v1_full'}
 
 default_cache_dir = "/tmp"
 default_model = "ms-marco-TinyBERT-L-2-v2"
 model_file_map = {
     "ms-marco-TinyBERT-L-2-v2": "flashrank-TinyBERT-L-2-v2.onnx",
     "ms-marco-MiniLM-L-12-v2": "flashrank-MiniLM-L-12-v2_Q.onnx",
     "ms-marco-MultiBERT-L-12": "flashrank-MultiBERT-L12_Q.onnx",
     "rank-T5-flan": "flashrank-rankt5_Q.onnx",
-    "ce-esci-MiniLM-L12-v2": "flashrank-ce-esci-MiniLM-L12-v2_Q.onnx"
-}
+    "ce-esci-MiniLM-L12-v2": "flashrank-ce-esci-MiniLM-L12-v2_Q.onnx",
+    "rank_zephyr_7b_v1_full": "rank_zephyr_7b_v1_full.Q4_K_M.gguf"
+}
+
```

### Comparing `FlashRank-0.2.1/flashrank/Ranker.py` & `FlashRank-0.2.2/flashrank/Ranker.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 from tokenizers import AddedToken, Tokenizer
 import onnxruntime as ort
 import numpy as np
 import os
 import zipfile
 import requests
 from tqdm import tqdm
-from flashrank.Config import default_model, default_cache_dir, model_url, model_file_map
+from flashrank.Config import default_model, default_cache_dir, model_url, model_file_map, listwise_rankers
 import collections
 from typing import Optional, List, Dict, Any
+from llama_cpp import Llama
 
 class RerankRequest:
     """ Represents a reranking request with a query and a list of passages. 
     
     Attributes:
         query (Optional[str]): The query for which the passages need to be reranked.
         passages (List[Dict[str, Any]]): The list of passages to be reranked.
@@ -41,16 +42,24 @@
             cache_dir (str): The directory where models are cached.
             max_length (int): The maximum length of the tokens.
         """
         self.cache_dir: Path = Path(cache_dir)
         self.model_dir: Path = self.cache_dir / model_name
         self._prepare_model_dir(model_name)
         model_file = model_file_map[model_name]
-        self.session = ort.InferenceSession(str(self.model_dir / model_file))
-        self.tokenizer: Tokenizer = self._get_tokenizer(max_length)
+
+        if model_name in listwise_rankers:
+            self.llm_model = Llama(
+              model_path=str(self.model_dir / model_file),
+              n_ctx=max_length,  
+              n_threads=8,          
+            ) 
+        else:
+            self.session = ort.InferenceSession(str(self.model_dir / model_file))
+            self.tokenizer: Tokenizer = self._get_tokenizer(max_length)
 
     def _prepare_model_dir(self, model_name: str):
         """ Ensures the model directory is prepared by downloading and extracting the model if not present.
 
         Args:
             model_name (str): The name of the model to be prepared.
         """
@@ -124,42 +133,96 @@
         vocab = collections.OrderedDict()
         with open(vocab_file, "r", encoding="utf-8") as reader:
             tokens = reader.readlines()
         for index, token in enumerate(tokens):
             token = token.rstrip("\n")
             vocab[token] = index
         return vocab
+    
+    def _get_prefix_prompt(self, query, num):
+        return [
+            {
+                "role": "system",
+                "content": "You are RankGPT, an intelligent assistant that can rank passages based on their relevancy to the query.",
+            },
+            {
+                "role": "user",
+                "content": f"I will provide you with {num} passages, each indicated by number identifier []. \nRank the passages based on their relevance to query: {query}.",
+            },
+            {"role": "assistant", "content": "Okay, please provide the passages."},
+        ]
+
+    def _get_postfix_prompt(self, query, num):
+        example_ordering = "[2] > [1]"
+        return {
+            "role": "user",
+            "content": f"Search Query: {query}.\nRank the {num} passages above based on their relevance to the search query. All the passages should be included and listed using identifiers, in descending order of relevance. The output format should be [] > [], e.g., {example_ordering}, Only respond with the ranking results, do not say any word or explain.",
+        }
+
+
 
     def rerank(self, request: RerankRequest) -> List[Dict[str, Any]]:
         """ Reranks a list of passages based on a query using a pre-trained model.
 
         Args:
             request (RerankRequest): The request containing the query and passages to rerank.
 
         Returns:
             List[Dict[str, Any]]: The reranked list of passages with added scores.
         """
         query = request.query
         passages = request.passages
-        query_passage_pairs = [[query, passage["text"]] for passage in passages]
-
-        input_text = self.tokenizer.encode_batch(query_passage_pairs)
-        input_ids = np.array([e.ids for e in input_text])
-        token_type_ids = np.array([e.type_ids for e in input_text])
-        attention_mask = np.array([e.attention_mask for e in input_text])
-
-        use_token_type_ids = token_type_ids is not None and not np.all(token_type_ids == 0)
-
-        onnx_input = {"input_ids": input_ids.astype(np.int64), "attention_mask": attention_mask.astype(np.int64)}
-        if use_token_type_ids:
-            onnx_input["token_type_ids"] = token_type_ids.astype(np.int64)
 
-        outputs = self.session.run(None, onnx_input)
+        # self.llm_model will be instantiated for GGUF based Listwise LLM models
+        if self.llm_model:
+            num_of_passages = len(passages)
+            messages = self._get_prefix_prompt(query, num_of_passages)
+
+            result_map = {}
+            for rank, passage in enumerate(passages):
+                messages.append(
+                    {
+                        "role": "user",
+                        "content": f"[{rank + 1}] {passage['text']}",
+                    }
+                )
+                messages.append(
+                        {
+                            "role": "assistant", 
+                            "content": f"Received passage [{rank + 1}]."
+                        }
+                )
+                
+                result_map[rank + 1] = passage
+
+            messages.append(self._get_postfix_prompt(query, num_of_passages))
+            raw_ranks = self.llm_model.create_chat_completion(messages)
+            results = []
+            for rank in raw_ranks["choices"][0]["message"]["content"].split(" > "):
+                results.append(result_map[int(rank[1])])
+            return results    
+
+        # self.session will be instantiated for ONNX based pairwise CE models
+        else:
+            query_passage_pairs = [[query, passage["text"]] for passage in passages]
+
+            input_text = self.tokenizer.encode_batch(query_passage_pairs)
+            input_ids = np.array([e.ids for e in input_text])
+            token_type_ids = np.array([e.type_ids for e in input_text])
+            attention_mask = np.array([e.attention_mask for e in input_text])
+
+            use_token_type_ids = token_type_ids is not None and not np.all(token_type_ids == 0)
+
+            onnx_input = {"input_ids": input_ids.astype(np.int64), "attention_mask": attention_mask.astype(np.int64)}
+            if use_token_type_ids:
+                onnx_input["token_type_ids"] = token_type_ids.astype(np.int64)
+
+            outputs = self.session.run(None, onnx_input)
 
-        scores = np.exp(outputs[0]) / (1 + np.exp(outputs[0])) if outputs[0].shape[1] > 1 else np.exp(outputs[0].flatten()) / (1 + np.exp(outputs[0].flatten()))
-        scores = scores.tolist()
+            scores = np.exp(outputs[0]) / (1 + np.exp(outputs[0])) if outputs[0].shape[1] > 1 else np.exp(outputs[0].flatten()) / (1 + np.exp(outputs[0].flatten()))
+            scores = scores.tolist()
 
-        for score, passage in zip(scores, passages):
-            passage["score"] = score
+            for score, passage in zip(scores, passages):
+                passage["score"] = score
 
-        passages.sort(key=lambda x: x["score"], reverse=True)
-        return passages
+            passages.sort(key=lambda x: x["score"], reverse=True)
+            return passages
```

### Comparing `FlashRank-0.2.1/flashrank/Rankerb.py` & `FlashRank-0.2.2/flashrank/Rankerb.py`

 * *Files identical despite different names*

### Comparing `FlashRank-0.2.1/flashrank/Rankerc.py` & `FlashRank-0.2.2/flashrank/Rankerc.py`

 * *Files identical despite different names*

### Comparing `FlashRank-0.2.1/setup.py` & `FlashRank-0.2.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FlashRank', 
-    version='0.2.1', 
+    version='0.2.2', 
     packages=find_packages(),
     install_requires=[
         'tokenizers',
         'onnxruntime',
         'numpy',
         'requests',
-        'tqdm'
+        'tqdm',
+        'llama-cpp-python==0.2.67'
     ],  
     author='Prithivi Da',
     author_email='',
     description='Ultra lite & Super fast SoTA cross-encoder based re-ranking for your search & retrieval pipelines.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/PrithivirajDamodaran/FlashRank',
```

