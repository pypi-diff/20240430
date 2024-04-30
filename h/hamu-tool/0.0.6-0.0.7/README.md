# Comparing `tmp/hamu-tool-0.0.6.tar.gz` & `tmp/hamu-tool-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hamu-tool-0.0.6.tar", last modified: Thu Mar 21 04:07:03 2024, max compression
+gzip compressed data, was "hamu-tool-0.0.7.tar", last modified: Tue Apr 30 09:32:24 2024, max compression
```

## Comparing `hamu-tool-0.0.6.tar` & `hamu-tool-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 04:07:29.766872 hamu-tool-0.0.6/
--rw-r--r--   0 root         (0) root         (0)      390 2024-03-21 04:07:29.682873 hamu-tool-0.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1325 2024-03-15 09:30:00.000000 hamu-tool-0.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 04:07:28.045888 hamu-tool-0.0.6/hamu_tool/
--rw-rw-r--   0 root         (0) root         (0)       21 2024-03-21 04:06:29.000000 hamu-tool-0.0.6/hamu_tool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 04:07:29.222877 hamu-tool-0.0.6/hamu_tool/dataset/
--rw-rw-r--   0 root         (0) root         (0)       37 2024-03-12 06:06:56.000000 hamu-tool-0.0.6/hamu_tool/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)      329 2024-03-11 04:16:12.000000 hamu-tool-0.0.6/hamu_tool/dataset/arguana_data_loader.py
--rw-rw-r--   0 root         (0) root         (0)     1992 2024-03-11 04:13:29.000000 hamu-tool-0.0.6/hamu_tool/dataset/data_loader.py
--rw-rw-r--   0 root         (0) root         (0)     7758 2024-03-13 02:48:32.000000 hamu-tool-0.0.6/hamu_tool/dataset/data_loader_base.py
--rw-rw-r--   0 root         (0) root         (0)      328 2024-03-11 04:16:19.000000 hamu-tool-0.0.6/hamu_tool/dataset/fiqa_data_loader.py
--rw-rw-r--   0 root         (0) root         (0)      344 2024-03-11 04:13:32.000000 hamu-tool-0.0.6/hamu_tool/dataset/nfcorpus_data_loader.py
--rw-r--r--   0 root         (0) root         (0)      321 2024-03-11 04:16:28.000000 hamu-tool-0.0.6/hamu_tool/dataset/quora_data_loader.py
--rw-r--r--   0 root         (0) root         (0)      333 2024-03-11 04:16:37.000000 hamu-tool-0.0.6/hamu_tool/dataset/robust04_data_loader.py
--rw-rw-r--   0 root         (0) root         (0)      340 2024-03-11 04:16:45.000000 hamu-tool-0.0.6/hamu_tool/dataset/scidocs_data_loader.py
--rw-rw-r--   0 root         (0) root         (0)      338 2024-03-11 04:16:58.000000 hamu-tool-0.0.6/hamu_tool/dataset/scifact_data_loader.py
--rw-r--r--   0 root         (0) root         (0)      338 2024-03-11 04:17:03.000000 hamu-tool-0.0.6/hamu_tool/dataset/trec_covid_data_loader.py
--rw-r--r--   0 root         (0) root         (0)      362 2024-03-11 04:17:09.000000 hamu-tool-0.0.6/hamu_tool/dataset/webis_touche_2020_data_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 04:07:29.418875 hamu-tool-0.0.6/hamu_tool/utils/
--rw-rw-r--   0 root         (0) root         (0)      108 2024-03-15 04:53:55.000000 hamu-tool-0.0.6/hamu_tool/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7220 2024-03-12 08:20:43.000000 hamu-tool-0.0.6/hamu_tool/utils/bib_extractor.py
--rw-rw-r--   0 root         (0) root         (0)     8629 2024-03-21 04:06:00.000000 hamu-tool-0.0.6/hamu_tool/utils/corpus_reader.py
--rw-r--r--   0 root         (0) root         (0)     4915 2024-03-16 04:32:45.000000 hamu-tool-0.0.6/hamu_tool/utils/pprint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 04:07:28.596883 hamu-tool-0.0.6/hamu_tool.egg-info/
--rw-r--r--   0 root         (0) root         (0)      390 2024-03-21 04:07:27.000000 hamu-tool-0.0.6/hamu_tool.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      836 2024-03-21 04:07:27.000000 hamu-tool-0.0.6/hamu_tool.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-21 04:07:27.000000 hamu-tool-0.0.6/hamu_tool.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-11 04:25:55.000000 hamu-tool-0.0.6/hamu_tool.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-21 04:07:27.000000 hamu-tool-0.0.6/hamu_tool.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-03-21 04:07:27.000000 hamu-tool-0.0.6/hamu_tool.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-21 04:07:29.768872 hamu-tool-0.0.6/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      593 2024-03-21 04:06:34.000000 hamu-tool-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:38:40.601727 hamu-tool-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)      390 2024-04-30 09:38:40.591727 hamu-tool-0.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1325 2024-03-15 09:30:00.000000 hamu-tool-0.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:38:40.231730 hamu-tool-0.0.7/hamu_tool/
+-rw-rw-r--   0 root         (0) root         (0)       21 2024-04-30 09:38:11.000000 hamu-tool-0.0.7/hamu_tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:38:40.551728 hamu-tool-0.0.7/hamu_tool/dataset/
+-rw-rw-r--   0 root         (0) root         (0)       37 2024-03-12 06:06:56.000000 hamu-tool-0.0.7/hamu_tool/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2024-04-30 06:08:48.000000 hamu-tool-0.0.7/hamu_tool/dataset/arguana_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2283 2024-04-30 06:09:22.000000 hamu-tool-0.0.7/hamu_tool/dataset/bioasq_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2024-04-30 06:09:25.000000 hamu-tool-0.0.7/hamu_tool/dataset/climate_fever_data_loader.py
+-rw-rw-r--   0 root         (0) root         (0)     2497 2024-04-30 08:19:11.000000 hamu-tool-0.0.7/hamu_tool/dataset/data_loader.py
+-rw-rw-r--   0 root         (0) root         (0)     5753 2024-04-29 23:54:14.000000 hamu-tool-0.0.7/hamu_tool/dataset/data_loader_base.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-04-30 06:09:31.000000 hamu-tool-0.0.7/hamu_tool/dataset/dbpedia_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2024-04-30 06:09:34.000000 hamu-tool-0.0.7/hamu_tool/dataset/fever_data_loader.py
+-rw-rw-r--   0 root         (0) root         (0)     1996 2024-04-30 06:09:36.000000 hamu-tool-0.0.7/hamu_tool/dataset/fiqa_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2024-04-30 06:09:38.000000 hamu-tool-0.0.7/hamu_tool/dataset/hotpotqa_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2024-04-30 06:09:41.000000 hamu-tool-0.0.7/hamu_tool/dataset/msmarco_data_loader.py
+-rw-rw-r--   0 root         (0) root         (0)     2227 2024-04-30 06:09:43.000000 hamu-tool-0.0.7/hamu_tool/dataset/nfcorpus_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2024-04-30 06:09:47.000000 hamu-tool-0.0.7/hamu_tool/dataset/nq_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1953 2024-04-30 06:09:50.000000 hamu-tool-0.0.7/hamu_tool/dataset/quora_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2024-04-30 06:09:55.000000 hamu-tool-0.0.7/hamu_tool/dataset/robust04_data_loader.py
+-rw-rw-r--   0 root         (0) root         (0)     2708 2024-04-30 09:21:46.000000 hamu-tool-0.0.7/hamu_tool/dataset/scidocs_data_loader.py
+-rw-rw-r--   0 root         (0) root         (0)     2110 2024-04-30 06:09:59.000000 hamu-tool-0.0.7/hamu_tool/dataset/scifact_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2024-04-30 06:10:02.000000 hamu-tool-0.0.7/hamu_tool/dataset/signal1m_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2024-04-30 08:18:43.000000 hamu-tool-0.0.7/hamu_tool/dataset/touche_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2024-04-30 08:18:55.000000 hamu-tool-0.0.7/hamu_tool/dataset/touche_v2_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2024-04-30 06:10:04.000000 hamu-tool-0.0.7/hamu_tool/dataset/trec_covid_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2387 2024-04-30 06:10:07.000000 hamu-tool-0.0.7/hamu_tool/dataset/trec_news_data_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:38:40.583727 hamu-tool-0.0.7/hamu_tool/utils/
+-rw-rw-r--   0 root         (0) root         (0)      108 2024-03-15 04:53:55.000000 hamu-tool-0.0.7/hamu_tool/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7220 2024-03-12 08:20:43.000000 hamu-tool-0.0.7/hamu_tool/utils/bib_extractor.py
+-rw-rw-r--   0 root         (0) root         (0)     8776 2024-04-25 06:49:16.000000 hamu-tool-0.0.7/hamu_tool/utils/corpus_reader.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2024-03-16 04:32:45.000000 hamu-tool-0.0.7/hamu_tool/utils/pprint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:38:40.371729 hamu-tool-0.0.7/hamu_tool.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      390 2024-04-30 09:38:39.000000 hamu-tool-0.0.7/hamu_tool.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1239 2024-04-30 09:38:40.000000 hamu-tool-0.0.7/hamu_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 09:38:39.000000 hamu-tool-0.0.7/hamu_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-11 04:25:55.000000 hamu-tool-0.0.7/hamu_tool.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-30 09:38:39.000000 hamu-tool-0.0.7/hamu_tool.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-30 09:38:39.000000 hamu-tool-0.0.7/hamu_tool.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 09:38:40.602727 hamu-tool-0.0.7/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      593 2024-04-30 09:38:32.000000 hamu-tool-0.0.7/setup.py
```

### Comparing `hamu-tool-0.0.6/README.md` & `hamu-tool-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `hamu-tool-0.0.6/hamu_tool/dataset/data_loader_base.py` & `hamu-tool-0.0.7/hamu_tool/dataset/data_loader_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ..utils.corpus_reader import CorpusReader
-from typing import Iterator
+from tqdm import tqdm
 import glob
 import os
 import requests
 import shutil
 import tempfile
 import urllib.parse
 
@@ -57,24 +57,29 @@
         Args:
             url (str): URL to download the dataset.
             data_dir (str): Directory to save the downloaded dataset.
 
         Raises:
             Exception: If failed to download the dataset.
         """
-        res = requests.get(url)
+        res = requests.get(url, stream=True)
         if res.status_code == 200:
             filename = res.headers.get('content-disposition').split('filename=')
             if len(filename) > 1:
                 filename = filename[1]
             else:
                 filename = res.headers.get('content-disposition').split('filename*=')[-1].split("''")[-1]
+            total = int(res.headers.get('content-length', 0))
+            pbar = tqdm(total=total, desc=filename, unit='B', unit_scale=True, unit_divisor=1024)
             data_path = os.path.join(data_dir, filename)
             with open(data_path, 'wb') as fp:
-                fp.write(res.content)
+                for data in res.iter_content(chunk_size=1024):
+                    pbar.update(len(data))
+                    fp.write(data)
+                # fp.write(res.content)
         else:
             raise Exception('Failed to download dataset')
 
 class DataLoaderQDRBase(DataLoaderBase):
     """Base class for DataLoaderQDR
     """
     def __init__(self, dataset_name : str, *args, **kwargs):
@@ -116,34 +121,14 @@
             idx (int): The index of the document.
 
         Returns:
             str: The fetched document ID.
         """
         return self.reader_doc.idx_list[idx]
 
-    def get_doc(self, did : str | int) -> str:
-        """Fetch a document by its ID.
-
-        Args:
-            did (str | int): The ID (str) or index (int) of the document.
-
-        Returns:
-            str: The fetched document.
-        """
-        return self.reader_doc[did]
-
-    def get_docs(self) -> Iterator[dict[str, str]]:
-        """Iterator for documents in the dataset.
-
-        Yields:
-            Iterator[dict[str, str]]: Iterator for documents in the dataset.
-        """
-        for it in self.reader_doc:
-            yield it
-
     def total_queries(self) -> int:
         """Total number of queries in the dataset.
 
         Returns:
             int: Total number of queries in the dataset.
         """
         return len(self.reader_query)
@@ -155,59 +140,17 @@
             idx (int): The index of the query.
 
         Returns:
             str: The fetched query ID.
         """
         return self.reader_query.idx_list[idx]
 
-    def get_query(self, qid : str | int) -> str:
-        """Fetch a query by its ID.
+    def total_qrels(self, mode : str) -> int:
+        """Total number of qrels in the dataset.
 
         Args:
-            qid (str | int): The ID (str) or index (int) of the query.
+            mode (str): Mode of the dataset.
 
         Returns:
-            str: The fetched query.
-        """
-        return self.reader_query[qid]
-
-    def get_queries(self) -> Iterator[dict[str, str]]:
-        """Iterator for queries in the dataset.
-
-        Yields:
-            Iterator[dict[str, str]]: Iterator for queries in the dataset.
-        """
-        for it in self.reader_query:
-            yield it
-
-    def get_qrel(self, qid : str, mode : str, with_score : bool = False) -> list[str] | list[tuple[str, int]]:
-        """Fetch the qrel for the given query ID.
-
-        Args:
-            qid (str): The ID of the query.
-            mode (str): The mode of the qrel such as 'train', 'dev', or 'test'. Check the document for each dataset.
-            with_score (bool, optional): Whether to include the score in the qrel. Defaults to False.
-
-        Raises:
-            Exception: If qrel for the given query ID is not found.
-
-        Returns:
-            list[str]: When with_score is False. List of relevant document IDs for the query.
-            list[tuple[str, int]]: When with_score is True. List of relevant document IDs and their scores for the query.
-        """
-        if qid not in self.qrel[mode]:
-            raise Exception(f'Qrel for query [{qid}] not found')
-        if with_score:
-            return self.qrel[mode][qid]
-        return [did for did, _ in self.qrel[mode][qid]]
-
-    def get_qrels(self, mode : str) -> Iterator[dict[str, any]]:
-        """Iterator for qrels in the dataset.
-
-        Args:
-            mode (str): The mode of the qrel such as 'train', 'dev', or 'test'. Check the document for each dataset.
-
-        Yields:
-            Iterator[dict[str, any]]: Iterator for qrels in the dataset.
+            int: Total number of qrels in the dataset.
         """
-        for qid, did, score in self.qrel_list[mode]:
-            yield {'qid': qid, 'did': did, 'score': score}
+        return len(self.qrel_list[mode])
```

### Comparing `hamu-tool-0.0.6/hamu_tool/utils/bib_extractor.py` & `hamu-tool-0.0.7/hamu_tool/utils/bib_extractor.py`

 * *Files identical despite different names*

### Comparing `hamu-tool-0.0.6/hamu_tool/utils/corpus_reader.py` & `hamu-tool-0.0.7/hamu_tool/utils/corpus_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 - Build an index file for a given data file.
 """
 
 import datetime
 import json
 import mmap
 import os
-import unidecode
+# import unidecode
 
 class CorpusReader:
     """A reader for efficiently accessing documents in a corpus using an index.
     """
     def __init__(self, index_path : str):
         """Initialize the corpus reader using an pre-built index file.
 
@@ -33,15 +33,15 @@
         self.data_offset = 0
         self.index_path = index_path
         if not os.path.exists(self.index_path):
             raise FileNotFoundError(f'Index file not found: [{self.index_path}]')
         self.index_file_size = os.path.getsize(self.index_path)
         with open(f'{self.index_path}', 'r', encoding='utf-8') as fp:
             for line in fp:
-                self.data_offset += len(line)
+                self.data_offset += len(line.encode())
                 idx, start_idx, end_idx = line.strip().split('\t')
                 if (idx, start_idx, end_idx) == ('0', '0', '0'):
                     break
                 self.index[idx] = {'start': int(start_idx), 'end': int(end_idx)}
                 self.idx_list.append(idx)
                 self.idx_set.add(idx)
         self.fp = open(f'{self.index_path}', 'r+b')
@@ -170,26 +170,29 @@
         with open(f'{index_path}', 'w', encoding='utf-8', newline='\n') as fp_idx, \
             open(f'{index_path}.data', 'w', encoding='utf-8', newline='\n') as fp_data, \
             open(data_path, 'r', encoding='utf-8') as fp:
             file_name = data_path.split('/')[-1]
             cnt = 0
             cnt_doc = 0
             for line in fp:
-                data_pre = json.loads(line)
-                data = {}
-                for key_pre in data_pre:
-                    key = unidecode.unidecode(key_pre)
-                    value = unidecode.unidecode(data_pre[key_pre])
-                    data[key] = value
-                idx_field = unidecode.unidecode(idx_field)
+                # data_pre = json.loads(line)
+                # data = {}
+                # for key_pre in data_pre:
+                #     key = unidecode.unidecode(key_pre)
+                #     value = unidecode.unidecode(data_pre[key_pre])
+                #     data[key] = value
+                # idx_field = unidecode.unidecode(idx_field)
+                data = json.loads(line) # new
                 idx = data[idx_field]
                 content = json.dumps(data, ensure_ascii=False, separators=(',', ':'))
                 fp_data.write(content)
-                fp_idx.write(f'{idx}\t{cnt}\t{cnt + len(content)}\n')
-                cnt += len(content)
+                # size = len(content)
+                size = len(content.encode()) # new
+                fp_idx.write(f'{idx}\t{cnt}\t{cnt + size}\n')
+                cnt += size
                 cnt_doc += 1
                 if verbose and cnt_doc % 1000 == 0:
                     now = datetime.datetime.now().strftime('%H:%M:%S')
                     print(f'[ {now} ] Corpus Reader | file: {file_name} | reading documents | doc: {cnt_doc:,} |', end='\r', flush=True)
             if verbose:
                 now = datetime.datetime.now().strftime('%H:%M:%S')
                 print(f'[ {now} ] Corpus Reader | file: {file_name} | reading documents | doc: {cnt_doc:,} |', flush=True)
```

### Comparing `hamu-tool-0.0.6/hamu_tool/utils/pprint.py` & `hamu-tool-0.0.7/hamu_tool/utils/pprint.py`

 * *Files identical despite different names*

### Comparing `hamu-tool-0.0.6/setup.py` & `hamu-tool-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hamu-tool',
-    version='0.0.6',
+    version='0.0.7',
     description='Many useful tools for computer scientists!',
     license='MIT',
     author='DoHyeon Lee',
     author_email='waylight3@snu.ac.kr',
     url='https://github.com/waylight3/hamu-tool',
     keywords=['hamu', 'tool', 'computer', 'science', 'useful', 'toolkit', 'library', 'python', 'package', 'module', 'utility', 'function', 'class', 'method'],
     install_requires=['unidecode >= 1.2.0'],
```

