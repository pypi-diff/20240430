# Comparing `tmp/llama_index_llms_nvidia_triton-0.1.4.tar.gz` & `tmp/llama_index_llms_nvidia_triton-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_nvidia_triton-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_llms_nvidia_triton-0.1.5.tar", max compression
```

## Comparing `llama_index_llms_nvidia_triton-0.1.4.tar` & `llama_index_llms_nvidia_triton-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       45 2024-04-23 19:40:20.068774 llama_index_llms_nvidia_triton-0.1.4/README.md
--rw-r--r--   0        0        0     1637 2024-04-23 19:40:20.068774 llama_index_llms_nvidia_triton-0.1.4/llama_index/llms/nvidia_triton/__init__.py
--rw-r--r--   0        0        0    10865 2024-04-23 19:40:20.068774 llama_index_llms_nvidia_triton-0.1.4/llama_index/llms/nvidia_triton/base.py
--rw-r--r--   0        0        0    13918 2024-04-23 19:40:20.068774 llama_index_llms_nvidia_triton-0.1.4/llama_index/llms/nvidia_triton/utils.py
--rw-r--r--   0        0        0     1526 2024-04-23 19:40:20.068774 llama_index_llms_nvidia_triton-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 llama_index_llms_nvidia_triton-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       45 2024-04-30 16:12:14.683907 llama_index_llms_nvidia_triton-0.1.5/README.md
+-rw-r--r--   0        0        0     1637 2024-04-30 16:12:14.683907 llama_index_llms_nvidia_triton-0.1.5/llama_index/llms/nvidia_triton/__init__.py
+-rw-r--r--   0        0        0    12016 2024-04-30 16:12:14.683907 llama_index_llms_nvidia_triton-0.1.5/llama_index/llms/nvidia_triton/base.py
+-rw-r--r--   0        0        0    13918 2024-04-30 16:12:14.683907 llama_index_llms_nvidia_triton-0.1.5/llama_index/llms/nvidia_triton/utils.py
+-rw-r--r--   0        0        0     1542 2024-04-30 16:12:14.683907 llama_index_llms_nvidia_triton-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 llama_index_llms_nvidia_triton-0.1.5/PKG-INFO
```

### Comparing `llama_index_llms_nvidia_triton-0.1.4/llama_index/llms/nvidia_triton/__init__.py` & `llama_index_llms_nvidia_triton-0.1.5/llama_index/llms/nvidia_triton/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_nvidia_triton-0.1.4/llama_index/llms/nvidia_triton/base.py` & `llama_index_llms_nvidia_triton-0.1.5/llama_index/llms/nvidia_triton/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     CompletionResponseAsyncGen,
     CompletionResponseGen,
     LLMMetadata,
 )
 from llama_index.core.llms.callbacks import llm_chat_callback
 from llama_index.core.base.llms.generic_utils import (
     completion_to_chat_decorator,
+    stream_completion_to_chat_decorator,
 )
 from llama_index.core.llms.llm import LLM
 from llama_index.llms.nvidia_triton.utils import GrpcTritonClient
 
 DEFAULT_SERVER_URL = "localhost:8001"
 DEFAULT_MAX_RETRIES = 3
 DEFAULT_TIMEOUT = 60.0
@@ -232,18 +233,20 @@
         )
 
     @llm_chat_callback()
     def chat(self, messages: Sequence[ChatMessage], **kwargs: Any) -> ChatResponse:
         chat_fn = completion_to_chat_decorator(self.complete)
         return chat_fn(messages, **kwargs)
 
+    @llm_chat_callback()
     def stream_chat(
         self, messages: Sequence[ChatMessage], **kwargs: Any
     ) -> ChatResponseGen:
-        raise NotImplementedError
+        chat_stream_fn = stream_completion_to_chat_decorator(self.stream_complete)
+        return chat_stream_fn(messages, **kwargs)
 
     def complete(
         self, prompt: str, formatted: bool = False, **kwargs: Any
     ) -> CompletionResponse:
         from tritonclient.utils import InferenceServerException
 
         client = self._get_client()
@@ -262,24 +265,51 @@
             model_params["model_name"], request_id, **invocation_params
         )
         response = ""
         for token in result_queue:
             if isinstance(token, InferenceServerException):
                 client.stop_stream(model_params["model_name"], request_id)
                 raise token
-            response = response + token
+            response += token
 
         return CompletionResponse(
             text=response,
         )
 
     def stream_complete(
         self, prompt: str, formatted: bool = False, **kwargs: Any
     ) -> CompletionResponseGen:
-        raise NotImplementedError
+        from tritonclient.utils import InferenceServerException
+
+        client = self._get_client()
+
+        invocation_params = self._get_model_default_parameters
+        invocation_params.update(kwargs)
+        invocation_params["prompt"] = [[prompt]]
+        model_params = self._identifying_params
+        model_params.update(kwargs)
+        request_id = str(random.randint(1, 9999999))  # nosec
+
+        if self.triton_load_model_call:
+            client.load_model(model_params["model_name"])
+
+        result_queue = client.request_streaming(
+            model_params["model_name"], request_id, **invocation_params
+        )
+
+        def gen() -> CompletionResponseGen:
+            text = ""
+            for token in result_queue:
+                if isinstance(token, InferenceServerException):
+                    client.stop_stream(model_params["model_name"], request_id)
+                    raise token
+                text += token
+                yield CompletionResponse(text=text, delta=token)
+
+        return gen()
 
     async def achat(
         self, messages: Sequence[ChatMessage], **kwargs: Any
     ) -> ChatResponse:
         raise NotImplementedError
 
     async def acomplete(
```

### Comparing `llama_index_llms_nvidia_triton-0.1.4/llama_index/llms/nvidia_triton/utils.py` & `llama_index_llms_nvidia_triton-0.1.5/llama_index/llms/nvidia_triton/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_nvidia_triton-0.1.4/pyproject.toml` & `llama_index_llms_nvidia_triton-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 [tool.mypy]
 disallow_untyped_defs = true
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
-authors = ["Your Name <you@example.com>"]
+authors = ["Rohith Ramakrishnan <rrohith2001@gmail.com>"]
 description = "llama-index llms nvidia triton integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-nvidia-triton"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.dependencies.tritonclient]
 extras = ["all"]
```

### Comparing `llama_index_llms_nvidia_triton-0.1.4/PKG-INFO` & `llama_index_llms_nvidia_triton-0.1.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-nvidia-triton
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index llms nvidia triton integration
 License: MIT
-Author: Your Name
-Author-email: you@example.com
+Author: Rohith Ramakrishnan
+Author-email: rrohith2001@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
```

