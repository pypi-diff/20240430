# Comparing `tmp/llmsmith-0.2.0.tar.gz` & `tmp/llmsmith-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmsmith-0.2.0.tar", max compression
+gzip compressed data, was "llmsmith-0.3.0.tar", max compression
```

## Comparing `llmsmith-0.2.0.tar` & `llmsmith-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,38 @@
--rw-r--r--   0        0        0     1101 2024-04-03 09:01:34.959168 llmsmith-0.2.0/LICENSE
--rw-r--r--   0        0        0     1492 2024-04-15 06:09:18.276703 llmsmith-0.2.0/README.md
--rw-r--r--   0        0        0       78 2024-03-15 04:21:07.861053 llmsmith-0.2.0/llmsmith/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 11:47:53.187559 llmsmith-0.2.0/llmsmith/job/__init__.py
--rw-r--r--   0        0        0     7428 2024-04-02 12:37:57.531013 llmsmith-0.2.0/llmsmith/job/base.py
--rw-r--r--   0        0        0     8550 2024-04-03 05:58:40.426172 llmsmith-0.2.0/llmsmith/job/job.py
--rw-r--r--   0        0        0        0 2024-03-14 11:03:16.994184 llmsmith-0.2.0/llmsmith/task/__init__.py
--rw-r--r--   0        0        0     1329 2024-04-02 12:23:38.410395 llmsmith-0.2.0/llmsmith/task/base.py
--rw-r--r--   0        0        0      229 2024-03-19 10:00:36.806582 llmsmith-0.2.0/llmsmith/task/models.py
--rw-r--r--   0        0        0        0 2024-03-15 07:53:27.486482 llmsmith-0.2.0/llmsmith/task/retrieval/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 07:44:57.026421 llmsmith-0.2.0/llmsmith/task/retrieval/vector/__init__.py
--rw-r--r--   0        0        0      147 2024-04-09 10:26:53.708807 llmsmith-0.2.0/llmsmith/task/retrieval/vector/base.py
--rw-r--r--   0        0        0     3667 2024-04-10 05:44:39.948855 llmsmith-0.2.0/llmsmith/task/retrieval/vector/chromadb.py
--rw-r--r--   0        0        0        0 2024-04-09 12:03:40.797998 llmsmith-0.2.0/llmsmith/task/retrieval/vector/options/__init__.py
--rw-r--r--   0        0        0      906 2024-04-10 13:01:55.980002 llmsmith-0.2.0/llmsmith/task/retrieval/vector/options/chromadb.py
--rw-r--r--   0        0        0     1325 2024-04-10 05:42:08.573365 llmsmith-0.2.0/llmsmith/task/retrieval/vector/options/qdrant.py
--rw-r--r--   0        0        0     4316 2024-04-11 04:01:18.457684 llmsmith-0.2.0/llmsmith/task/retrieval/vector/qdrant.py
--rw-r--r--   0        0        0        0 2024-03-15 11:22:26.459597 llmsmith-0.2.0/llmsmith/task/textgen/__init__.py
--rw-r--r--   0        0        0     3042 2024-04-04 09:07:05.709627 llmsmith-0.2.0/llmsmith/task/textgen/claude.py
--rw-r--r--   0        0        0      649 2024-04-04 09:30:06.752488 llmsmith-0.2.0/llmsmith/task/textgen/errors.py
--rw-r--r--   0        0        0     4460 2024-04-13 10:05:58.713381 llmsmith-0.2.0/llmsmith/task/textgen/gemini.py
--rw-r--r--   0        0        0     3185 2024-04-03 10:54:14.137132 llmsmith-0.2.0/llmsmith/task/textgen/openai.py
--rw-r--r--   0        0        0        0 2024-03-19 08:37:09.919088 llmsmith-0.2.0/llmsmith/task/textgen/options/__init__.py
--rw-r--r--   0        0        0     1498 2024-04-04 09:30:06.753059 llmsmith-0.2.0/llmsmith/task/textgen/options/claude.py
--rw-r--r--   0        0        0     1466 2024-04-03 10:54:40.771025 llmsmith-0.2.0/llmsmith/task/textgen/options/gemini.py
--rw-r--r--   0        0        0     2108 2024-04-03 10:54:48.638547 llmsmith-0.2.0/llmsmith/task/textgen/options/openai.py
--rw-r--r--   0        0        0     1845 2024-04-15 05:39:00.550872 llmsmith-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3191 1970-01-01 00:00:00.000000 llmsmith-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-03 09:01:34.959168 llmsmith-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1506 2024-04-30 06:58:37.514663 llmsmith-0.3.0/README.md
+-rw-r--r--   0        0        0       78 2024-03-15 04:21:07.861053 llmsmith-0.3.0/llmsmith/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:18:59.343170 llmsmith-0.3.0/llmsmith/agent/__init__.py
+-rw-r--r--   0        0        0      209 2024-04-18 09:12:45.143269 llmsmith-0.3.0/llmsmith/agent/errors.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:19:30.041692 llmsmith-0.3.0/llmsmith/agent/function/__init__.py
+-rw-r--r--   0        0        0     5934 2024-04-29 11:21:40.340274 llmsmith-0.3.0/llmsmith/agent/function/gemini.py
+-rw-r--r--   0        0        0     8897 2024-04-30 06:33:06.377475 llmsmith-0.3.0/llmsmith/agent/function/openai.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:43:58.075908 llmsmith-0.3.0/llmsmith/agent/function/options/__init__.py
+-rw-r--r--   0        0        0     1996 2024-04-30 04:53:53.672366 llmsmith-0.3.0/llmsmith/agent/function/options/openai.py
+-rw-r--r--   0        0        0        0 2024-04-18 05:26:07.193675 llmsmith-0.3.0/llmsmith/agent/tool/__init__.py
+-rw-r--r--   0        0        0     1013 2024-04-18 12:17:09.379744 llmsmith-0.3.0/llmsmith/agent/tool/gemini.py
+-rw-r--r--   0        0        0     2001 2024-04-29 11:21:40.340139 llmsmith-0.3.0/llmsmith/agent/tool/openai.py
+-rw-r--r--   0        0        0        0 2024-03-14 11:47:53.187559 llmsmith-0.3.0/llmsmith/job/__init__.py
+-rw-r--r--   0        0        0     7428 2024-04-02 12:37:57.531013 llmsmith-0.3.0/llmsmith/job/base.py
+-rw-r--r--   0        0        0     8550 2024-04-03 05:58:40.426172 llmsmith-0.3.0/llmsmith/job/job.py
+-rw-r--r--   0        0        0        0 2024-03-14 11:03:16.994184 llmsmith-0.3.0/llmsmith/task/__init__.py
+-rw-r--r--   0        0        0     1329 2024-04-02 12:23:38.410395 llmsmith-0.3.0/llmsmith/task/base.py
+-rw-r--r--   0        0        0      437 2024-04-22 10:15:31.395712 llmsmith-0.3.0/llmsmith/task/models.py
+-rw-r--r--   0        0        0        0 2024-03-15 07:53:27.486482 llmsmith-0.3.0/llmsmith/task/retrieval/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 07:44:57.026421 llmsmith-0.3.0/llmsmith/task/retrieval/vector/__init__.py
+-rw-r--r--   0        0        0      147 2024-04-09 10:26:53.708807 llmsmith-0.3.0/llmsmith/task/retrieval/vector/base.py
+-rw-r--r--   0        0        0     3667 2024-04-10 05:44:39.948855 llmsmith-0.3.0/llmsmith/task/retrieval/vector/chromadb.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:03:40.797998 llmsmith-0.3.0/llmsmith/task/retrieval/vector/options/__init__.py
+-rw-r--r--   0        0        0      906 2024-04-10 13:01:55.980002 llmsmith-0.3.0/llmsmith/task/retrieval/vector/options/chromadb.py
+-rw-r--r--   0        0        0     1325 2024-04-10 05:42:08.573365 llmsmith-0.3.0/llmsmith/task/retrieval/vector/options/qdrant.py
+-rw-r--r--   0        0        0     4316 2024-04-11 04:01:18.457684 llmsmith-0.3.0/llmsmith/task/retrieval/vector/qdrant.py
+-rw-r--r--   0        0        0        0 2024-03-15 11:22:26.459597 llmsmith-0.3.0/llmsmith/task/textgen/__init__.py
+-rw-r--r--   0        0        0     3042 2024-04-04 09:07:05.709627 llmsmith-0.3.0/llmsmith/task/textgen/claude.py
+-rw-r--r--   0        0        0      681 2024-04-18 12:18:54.653626 llmsmith-0.3.0/llmsmith/task/textgen/errors.py
+-rw-r--r--   0        0        0     7108 2024-04-29 11:21:40.339852 llmsmith-0.3.0/llmsmith/task/textgen/gemini.py
+-rw-r--r--   0        0        0     6447 2024-04-29 11:21:40.339843 llmsmith-0.3.0/llmsmith/task/textgen/openai.py
+-rw-r--r--   0        0        0        0 2024-03-19 08:37:09.919088 llmsmith-0.3.0/llmsmith/task/textgen/options/__init__.py
+-rw-r--r--   0        0        0     1498 2024-04-04 09:30:06.753059 llmsmith-0.3.0/llmsmith/task/textgen/options/claude.py
+-rw-r--r--   0        0        0     1346 2024-04-18 07:13:19.756541 llmsmith-0.3.0/llmsmith/task/textgen/options/gemini.py
+-rw-r--r--   0        0        0     1890 2024-04-22 08:24:34.750821 llmsmith-0.3.0/llmsmith/task/textgen/options/openai.py
+-rw-r--r--   0        0        0     1845 2024-04-30 10:42:49.875910 llmsmith-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3205 1970-01-01 00:00:00.000000 llmsmith-0.3.0/PKG-INFO
```

### Comparing `llmsmith-0.2.0/LICENSE` & `llmsmith-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmsmith-0.2.0/README.md` & `llmsmith-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -22,12 +22,12 @@
 - `gemini`
 - `chromadb`
 - `qdrant`
 - `all` (downloads all extra dependencies)
 
 ## Example
 
-Refer [this](https://llmsmith.readthedocs.io/en/latest/examples.html) page from the documentation to see how a naive RAG functionality can be created using LLMSmith.
+Refer [this](https://llmsmith.readthedocs.io/en/latest/examples.html) page from the documentation to see examples on how LLMSmith can be used to build LLM powered functionalities.
 
 ## Documentation
 
 An extensive documentation for LLMSmith is hosted in Read the Docs here - [https://llmsmith.readthedocs.io/en/latest](https://llmsmith.readthedocs.io/en/latest)
```

### Comparing `llmsmith-0.2.0/llmsmith/job/base.py` & `llmsmith-0.3.0/llmsmith/job/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.2.0/llmsmith/job/job.py` & `llmsmith-0.3.0/llmsmith/job/job.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.2.0/llmsmith/task/base.py` & `llmsmith-0.3.0/llmsmith/task/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.2.0/llmsmith/task/retrieval/vector/chromadb.py` & `llmsmith-0.3.0/llmsmith/task/retrieval/vector/chromadb.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.2.0/llmsmith/task/retrieval/vector/options/chromadb.py` & `llmsmith-0.3.0/llmsmith/task/retrieval/vector/options/chromadb.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.2.0/llmsmith/task/retrieval/vector/options/qdrant.py` & `llmsmith-0.3.0/llmsmith/task/retrieval/vector/options/qdrant.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.2.0/llmsmith/task/retrieval/vector/qdrant.py` & `llmsmith-0.3.0/llmsmith/task/retrieval/vector/qdrant.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.2.0/llmsmith/task/textgen/claude.py` & `llmsmith-0.3.0/llmsmith/task/textgen/claude.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.2.0/llmsmith/task/textgen/errors.py` & `llmsmith-0.3.0/llmsmith/task/textgen/errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-class TextGenError(Exception):
-    """Base error for all text generation errors"""
+class TextGenException(Exception):
+    """Base exception for all text generation related errors"""
 
 
-class TextGenFailedError(TextGenError):
+class TextGenFailedException(TextGenException):
     """Raised when the AI fails to generate text for some reason (like unsafe prompt, exceeded token count etc.)"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args)
         self.failure_reason = kwargs.get("failure_reason")
 
 
-class PromptBlockedError(TextGenError):
+class PromptBlockedException(TextGenException):
     """Raised when the prompt is blocked by the AI for some reason (like blocked prompt for example)"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args)
         self.block_reason = kwargs.get("block_reason")
```

### Comparing `llmsmith-0.2.0/llmsmith/task/textgen/options/claude.py` & `llmsmith-0.3.0/llmsmith/task/textgen/options/claude.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.2.0/llmsmith/task/textgen/options/gemini.py` & `llmsmith-0.3.0/llmsmith/task/textgen/options/gemini.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Any, TypedDict, Union
 
 try:
     from google.generativeai.types.generation_types import GenerationConfigType
     from google.generativeai.types.safety_types import SafetySettingOptions
-    from google.generativeai.types.content_types import FunctionLibraryType
 except ImportError:
     raise ImportError(
         "The 'google.generativeai' library is required to use GeminiTextGenOptions. You can install it with `pip install \"llmsmith[gemini]\"`"
     )
 
 
 class GeminiTextGenOptions(TypedDict):
@@ -20,13 +19,12 @@
     * https://github.com/google/generative-ai-python/blob/v0.4.0/google/generativeai/types/safety_types.py
     * https://github.com/google/generative-ai-python/blob/v0.4.0/google/generativeai/types/content_types.py
     * https://ai.google.dev/tutorials/python_quickstart
     """
 
     generation_config: Union[GenerationConfigType, None]
     safety_settings: Union[SafetySettingOptions, None]
-    tools: Union[FunctionLibraryType, None]
     request_options: Union[dict[str, Any], None]
 
 
 def _completion_create_options_dict(options: GeminiTextGenOptions) -> dict:
     return {attr: options.get(attr) for attr in GeminiTextGenOptions.__annotations__}
```

### Comparing `llmsmith-0.2.0/pyproject.toml` & `llmsmith-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "LLMSmith"
-version = "0.2.0"
+version = "0.3.0"
 description = "Lightweight Python library designed for developing functionalities powered by Large Language Models (LLMs)"
 authors = ["Dheeraj Gopinath <dheeraj.gopinath@gmail.com>"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
-openai = {version = "^1.13.3", optional = true}
+openai = {version = "^1.23.2", optional = true}
 anthropic = {version = "^0.19.2", optional = true}
 google-generativeai = {version = "^0.4.0", optional = true}
 chromadb-client = {version = "^0.4.25.dev0", optional = true}
 onnxruntime = {version = "^1.17.1", optional = true}
 protobuf = {version = "3.20.3", optional = true}
 tokenizers = {version = "^0.15.2", optional = true}
 python-dotenv = "^1.0.1"
```

### Comparing `llmsmith-0.2.0/PKG-INFO` & `llmsmith-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLMSmith
-Version: 0.2.0
+Version: 0.3.0
 Summary: Lightweight Python library designed for developing functionalities powered by Large Language Models (LLMs)
 Author: Dheeraj Gopinath
 Author-email: dheeraj.gopinath@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,15 @@
 Provides-Extra: gemini
 Provides-Extra: openai
 Provides-Extra: qdrant
 Requires-Dist: anthropic (>=0.19.2,<0.20.0) ; extra == "claude" or extra == "all"
 Requires-Dist: chromadb-client (>=0.4.25.dev0,<0.5.0) ; extra == "chromadb" or extra == "all"
 Requires-Dist: google-generativeai (>=0.4.0,<0.5.0) ; extra == "gemini" or extra == "all"
 Requires-Dist: onnxruntime (>=1.17.1,<2.0.0) ; extra == "chromadb" or extra == "all"
-Requires-Dist: openai (>=1.13.3,<2.0.0) ; extra == "openai" or extra == "all"
+Requires-Dist: openai (>=1.23.2,<2.0.0) ; extra == "openai" or extra == "all"
 Requires-Dist: protobuf (==3.20.3) ; extra == "chromadb" or extra == "all"
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: qdrant-client (>=1.8.2,<2.0.0) ; extra == "qdrant" or extra == "all"
 Requires-Dist: tokenizers (>=0.15.2,<0.16.0) ; extra == "chromadb" or extra == "all"
 Description-Content-Type: text/markdown
 
 # 🧰 LLMSmith
@@ -56,13 +56,13 @@
 - `gemini`
 - `chromadb`
 - `qdrant`
 - `all` (downloads all extra dependencies)
 
 ## Example
 
-Refer [this](https://llmsmith.readthedocs.io/en/latest/examples.html) page from the documentation to see how a naive RAG functionality can be created using LLMSmith.
+Refer [this](https://llmsmith.readthedocs.io/en/latest/examples.html) page from the documentation to see examples on how LLMSmith can be used to build LLM powered functionalities.
 
 ## Documentation
 
 An extensive documentation for LLMSmith is hosted in Read the Docs here - [https://llmsmith.readthedocs.io/en/latest](https://llmsmith.readthedocs.io/en/latest)
```

