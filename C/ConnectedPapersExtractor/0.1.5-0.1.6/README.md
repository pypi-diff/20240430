# Comparing `tmp/connectedpapersextractor-0.1.5.tar.gz` & `tmp/connectedpapersextractor-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectedpapersextractor-0.1.5.tar", max compression
+gzip compressed data, was "connectedpapersextractor-0.1.6.tar", max compression
```

## Comparing `connectedpapersextractor-0.1.5.tar` & `connectedpapersextractor-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1070 2024-04-23 21:01:05.479303 connectedpapersextractor-0.1.5/LICENSE
--rw-r--r--   0        0        0      616 2024-04-29 14:52:18.951047 connectedpapersextractor-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      198 2024-04-27 22:23:56.499918 connectedpapersextractor-0.1.5/src/connectedpapersextractor/ArticleFilter.py
--rw-r--r--   0        0        0      183 2024-04-28 11:36:25.108943 connectedpapersextractor-0.1.5/src/connectedpapersextractor/Config.py
--rw-r--r--   0        0        0      374 2024-04-28 13:45:00.686988 connectedpapersextractor-0.1.5/src/connectedpapersextractor/MainPartsExtractor.py
--rw-r--r--   0        0        0     2157 2024-04-29 13:12:12.624547 connectedpapersextractor-0.1.5/src/connectedpapersextractor/PdfSummary.py
--rw-r--r--   0        0        0     2486 2024-04-28 13:45:00.750987 connectedpapersextractor-0.1.5/src/connectedpapersextractor/_AIExtractor.py
--rw-r--r--   0        0        0      344 2024-04-28 13:39:32.895971 connectedpapersextractor-0.1.5/src/connectedpapersextractor/__init__.py
--rw-r--r--   0        0        0      704 2024-04-29 13:14:31.644921 connectedpapersextractor-0.1.5/src/connectedpapersextractor/_add_docs.py
--rw-r--r--   0        0        0      872 2024-04-28 11:53:43.189003 connectedpapersextractor-0.1.5/src/connectedpapersextractor/_combine_summaries.py
--rw-r--r--   0        0        0     2668 2024-04-28 15:05:13.301962 connectedpapersextractor-0.1.5/src/connectedpapersextractor/_get_pdf_summaries.py
--rw-r--r--   0        0        0     1170 2024-04-28 16:50:24.953804 connectedpapersextractor-0.1.5/src/connectedpapersextractor/_refine_documents.py
--rw-r--r--   0        0        0      768 2024-04-28 17:10:03.753179 connectedpapersextractor-0.1.5/src/connectedpapersextractor/_stuff_documents.py
--rw-r--r--   0        0        0     1451 2024-04-29 14:51:28.995045 connectedpapersextractor-0.1.5/src/connectedpapersextractor/_summarize_documents.py
--rw-r--r--   0        0        0     1538 2024-04-29 13:22:39.662122 connectedpapersextractor-0.1.5/src/connectedpapersextractor/create_related_work.py
--rw-r--r--   0        0        0     1450 2024-04-28 13:47:45.376986 connectedpapersextractor-0.1.5/src/connectedpapersextractor/get_summaries.py
--rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 connectedpapersextractor-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-23 21:01:05.479303 connectedpapersextractor-0.1.6/LICENSE
+-rw-r--r--   0        0        0      616 2024-04-29 20:45:47.536839 connectedpapersextractor-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-27 22:23:56.499918 connectedpapersextractor-0.1.6/src/connectedpapersextractor/ArticleFilter.py
+-rw-r--r--   0        0        0      183 2024-04-28 11:36:25.108943 connectedpapersextractor-0.1.6/src/connectedpapersextractor/Config.py
+-rw-r--r--   0        0        0      374 2024-04-28 13:45:00.686988 connectedpapersextractor-0.1.6/src/connectedpapersextractor/MainPartsExtractor.py
+-rw-r--r--   0        0        0     2157 2024-04-29 13:12:12.624547 connectedpapersextractor-0.1.6/src/connectedpapersextractor/PdfSummary.py
+-rw-r--r--   0        0        0     2486 2024-04-28 13:45:00.750987 connectedpapersextractor-0.1.6/src/connectedpapersextractor/_AIExtractor.py
+-rw-r--r--   0        0        0      344 2024-04-28 13:39:32.895971 connectedpapersextractor-0.1.6/src/connectedpapersextractor/__init__.py
+-rw-r--r--   0        0        0      531 2024-04-29 20:28:54.583294 connectedpapersextractor-0.1.6/src/connectedpapersextractor/_add_docs.py
+-rw-r--r--   0        0        0      872 2024-04-28 11:53:43.189003 connectedpapersextractor-0.1.6/src/connectedpapersextractor/_combine_summaries.py
+-rw-r--r--   0        0        0     2668 2024-04-28 15:05:13.301962 connectedpapersextractor-0.1.6/src/connectedpapersextractor/_get_pdf_summaries.py
+-rw-r--r--   0        0        0     1170 2024-04-28 16:50:24.953804 connectedpapersextractor-0.1.6/src/connectedpapersextractor/_refine_documents.py
+-rw-r--r--   0        0        0      768 2024-04-28 17:10:03.753179 connectedpapersextractor-0.1.6/src/connectedpapersextractor/_stuff_documents.py
+-rw-r--r--   0        0        0     1461 2024-04-29 20:28:54.591294 connectedpapersextractor-0.1.6/src/connectedpapersextractor/_summarize_documents.py
+-rw-r--r--   0        0        0     1516 2024-04-29 20:28:54.595295 connectedpapersextractor-0.1.6/src/connectedpapersextractor/create_related_work.py
+-rw-r--r--   0        0        0     1450 2024-04-28 13:47:45.376986 connectedpapersextractor-0.1.6/src/connectedpapersextractor/get_summaries.py
+-rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 connectedpapersextractor-0.1.6/PKG-INFO
```

### Comparing `connectedpapersextractor-0.1.5/LICENSE` & `connectedpapersextractor-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.5/pyproject.toml` & `connectedpapersextractor-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ConnectedPapersExtractor"
-version = "0.1.5"
+version = "0.1.6"
 description = "A package for creating summaries based on https://www.connectedpapers.com/."
 authors = ["Tesla2000 <fratajczak124@gmail.com>"]
 license = "MIT License"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 langchain = "^0.1.16"
```

### Comparing `connectedpapersextractor-0.1.5/src/connectedpapersextractor/PdfSummary.py` & `connectedpapersextractor-0.1.6/src/connectedpapersextractor/PdfSummary.py`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.5/src/connectedpapersextractor/_AIExtractor.py` & `connectedpapersextractor-0.1.6/src/connectedpapersextractor/_AIExtractor.py`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.5/src/connectedpapersextractor/_combine_summaries.py` & `connectedpapersextractor-0.1.6/src/connectedpapersextractor/_combine_summaries.py`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.5/src/connectedpapersextractor/_get_pdf_summaries.py` & `connectedpapersextractor-0.1.6/src/connectedpapersextractor/_get_pdf_summaries.py`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.5/src/connectedpapersextractor/_refine_documents.py` & `connectedpapersextractor-0.1.6/src/connectedpapersextractor/_refine_documents.py`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.5/src/connectedpapersextractor/_stuff_documents.py` & `connectedpapersextractor-0.1.6/src/connectedpapersextractor/_stuff_documents.py`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.5/src/connectedpapersextractor/_summarize_documents.py` & `connectedpapersextractor-0.1.6/src/connectedpapersextractor/_summarize_documents.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import json
 import warnings
 from dataclasses import asdict
 from typing import Optional
 
-from langchain_core.embeddings import Embeddings
+
 from langchain_core.language_models import BaseLanguageModel
+from langchain_text_splitters import TextSplitter
 
 from . import Config
 from .MainPartsExtractor import MainPartsExtractor
 from .PdfSummary import PdfSummaries
 from ._add_docs import _add_docs
 from ._refine_documents import _refine_documents
 from ._stuff_documents import _stuff_documents
 
 
 def _summarize_documents(
     summaries: PdfSummaries,
     main_parts_extractor: MainPartsExtractor,
     llm: Optional[BaseLanguageModel] = None,
-    embeddings: Optional[Embeddings] = None,
+    text_splitter: Optional[TextSplitter] = None,
 ) -> PdfSummaries:
     metadata_path = summaries[0].file_path.parent.joinpath(Config.metadate_file_name)
     for summary in summaries:
         if summary.text_summary is not None:
             continue
-        _add_docs(summary, embeddings)
+        _add_docs(summary, text_splitter)
         docs = main_parts_extractor.extract(summary)
         try:
             text_summary = _stuff_documents(llm, docs)
         except Exception as e:
             warnings.warn(str(e))
             text_summary = _refine_documents(llm, docs)
         summary.text_summary = text_summary
```

### Comparing `connectedpapersextractor-0.1.5/src/connectedpapersextractor/create_related_work.py` & `connectedpapersextractor-0.1.6/src/connectedpapersextractor/create_related_work.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 from operator import attrgetter
 from typing import Union, Optional
 
-from langchain_core.embeddings import Embeddings
 from langchain_core.language_models import LanguageModelInput
 from langchain_core.messages import BaseMessage
 from langchain_core.runnables import Runnable
+from langchain_text_splitters import TextSplitter
 
 from . import MainPartsExtractor
 from .MainPartsExtractor import _DefaultExtractor
 from .PdfSummary import PdfSummaries
 from ._combine_summaries import _combine_summaries
 from ._summarize_documents import _summarize_documents
 
 
 def create_related_work(
     summaries: PdfSummaries,
     llm: Union[
         Runnable[LanguageModelInput, str],
         Optional[Runnable[LanguageModelInput, BaseMessage]],
     ] = None,
-    embeddings: Optional[Embeddings] = None,
+    text_splitter: Optional[TextSplitter] = None,
     main_parts_extractor: Optional[MainPartsExtractor] = None,
     refine: bool = True,
 ) -> str:
     if not summaries:
         raise ValueError("Summaries must be provided")
     if main_parts_extractor is None:
         main_parts_extractor = _DefaultExtractor()
     if llm is None:
         from langchain_openai import ChatOpenAI
         llm = ChatOpenAI(temperature=0, model_name="gpt-3.5-turbo-16k")
-        llm.max_tokens = 16385
     summaries_with_text = _summarize_documents(
-        summaries, main_parts_extractor, llm, embeddings
+        summaries, main_parts_extractor, llm, text_splitter
     )
     combined_summaries = "\n\n".join(
         map(": ".join, map(attrgetter("title", "text_summary"), summaries_with_text))
     )
     if refine and len(summaries) != 1:
         return _combine_summaries(combined_summaries, llm)
     return combined_summaries
```

### Comparing `connectedpapersextractor-0.1.5/src/connectedpapersextractor/get_summaries.py` & `connectedpapersextractor-0.1.6/src/connectedpapersextractor/get_summaries.py`

 * *Files identical despite different names*

### Comparing `connectedpapersextractor-0.1.5/PKG-INFO` & `connectedpapersextractor-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConnectedPapersExtractor
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for creating summaries based on https://www.connectedpapers.com/.
 License: MIT
 Author: Tesla2000
 Author-email: fratajczak124@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

