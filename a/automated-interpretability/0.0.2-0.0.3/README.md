# Comparing `tmp/automated_interpretability-0.0.2.tar.gz` & `tmp/automated_interpretability-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automated_interpretability-0.0.2.tar", max compression
+gzip compressed data, was "automated_interpretability-0.0.3.tar", max compression
```

## Comparing `automated_interpretability-0.0.2.tar` & `automated_interpretability-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0        0 2024-04-26 20:24:13.654582 automated_interpretability-0.0.2/neuron_explainer/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 20:24:13.654716 automated_interpretability-0.0.2/neuron_explainer/activations/__init__.py
--rw-r--r--   0        0        0     4751 2024-04-26 20:24:13.654851 automated_interpretability-0.0.2/neuron_explainer/activations/activation_records.py
--rw-r--r--   0        0        0    10808 2024-04-26 20:24:13.655025 automated_interpretability-0.0.2/neuron_explainer/activations/activations.py
--rw-r--r--   0        0        0     2179 2024-04-26 20:24:13.655130 automated_interpretability-0.0.2/neuron_explainer/activations/token_connections.py
--rw-r--r--   0        0        0     5498 2024-04-26 20:24:13.655251 automated_interpretability-0.0.2/neuron_explainer/api_client.py
--rw-r--r--   0        0        0      257 2024-04-26 20:24:13.655360 automated_interpretability-0.0.2/neuron_explainer/azure.py
--rw-r--r--   0        0        0        0 2024-04-26 20:24:13.655465 automated_interpretability-0.0.2/neuron_explainer/explanations/__init__.py
--rw-r--r--   0        0        0     7967 2024-04-26 20:24:13.655603 automated_interpretability-0.0.2/neuron_explainer/explanations/calibrated_simulator.py
--rw-r--r--   0        0        0    22179 2024-04-27 03:26:33.596456 automated_interpretability-0.0.2/neuron_explainer/explanations/explainer.py
--rw-r--r--   0        0        0     8867 2024-04-26 20:24:13.655965 automated_interpretability-0.0.2/neuron_explainer/explanations/explanations.py
--rw-r--r--   0        0        0    32989 2024-04-26 20:24:13.656149 automated_interpretability-0.0.2/neuron_explainer/explanations/few_shot_examples.py
--rw-r--r--   0        0        0     4698 2024-04-26 20:24:13.656293 automated_interpretability-0.0.2/neuron_explainer/explanations/prompt_builder.py
--rw-r--r--   0        0        0    52696 2024-04-26 20:24:13.656497 automated_interpretability-0.0.2/neuron_explainer/explanations/puzzles.json
--rw-r--r--   0        0        0     2178 2024-04-26 20:24:13.656717 automated_interpretability-0.0.2/neuron_explainer/explanations/puzzles.py
--rw-r--r--   0        0        0     5888 2024-04-26 20:24:13.656874 automated_interpretability-0.0.2/neuron_explainer/explanations/scoring.py
--rw-r--r--   0        0        0    45651 2024-04-27 05:42:47.856473 automated_interpretability-0.0.2/neuron_explainer/explanations/simulator.py
--rw-r--r--   0        0        0     6603 2024-04-26 20:24:13.657275 automated_interpretability-0.0.2/neuron_explainer/explanations/test_explainer.py
--rw-r--r--   0        0        0     7605 2024-04-26 20:24:13.657397 automated_interpretability-0.0.2/neuron_explainer/explanations/test_simulator.py
--rw-r--r--   0        0        0     4836 2024-04-26 20:24:13.657520 automated_interpretability-0.0.2/neuron_explainer/explanations/token_space_few_shot_examples.py
--rw-r--r--   0        0        0      147 2024-04-26 20:24:13.657701 automated_interpretability-0.0.2/neuron_explainer/fast_dataclasses/__init__.py
--rw-r--r--   0        0        0     3043 2024-04-26 20:24:13.657821 automated_interpretability-0.0.2/neuron_explainer/fast_dataclasses/fast_dataclasses.py
--rw-r--r--   0        0        0     2712 2024-04-26 20:24:13.657941 automated_interpretability-0.0.2/neuron_explainer/fast_dataclasses/test_fast_dataclasses.py
--rw-r--r--   0        0        0      467 2024-04-27 18:42:36.584815 automated_interpretability-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 automated_interpretability-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-26 20:24:13.654582 automated_interpretability-0.0.3/neuron_explainer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 20:24:13.654716 automated_interpretability-0.0.3/neuron_explainer/activations/__init__.py
+-rw-r--r--   0        0        0     4751 2024-04-26 20:24:13.654851 automated_interpretability-0.0.3/neuron_explainer/activations/activation_records.py
+-rw-r--r--   0        0        0    10808 2024-04-26 20:24:13.655025 automated_interpretability-0.0.3/neuron_explainer/activations/activations.py
+-rw-r--r--   0        0        0     2179 2024-04-26 20:24:13.655130 automated_interpretability-0.0.3/neuron_explainer/activations/token_connections.py
+-rw-r--r--   0        0        0     5455 2024-04-29 22:48:36.119355 automated_interpretability-0.0.3/neuron_explainer/api_client.py
+-rw-r--r--   0        0        0      257 2024-04-26 20:24:13.655360 automated_interpretability-0.0.3/neuron_explainer/azure.py
+-rw-r--r--   0        0        0        0 2024-04-26 20:24:13.655465 automated_interpretability-0.0.3/neuron_explainer/explanations/__init__.py
+-rw-r--r--   0        0        0     7967 2024-04-26 20:24:13.655603 automated_interpretability-0.0.3/neuron_explainer/explanations/calibrated_simulator.py
+-rw-r--r--   0        0        0    22224 2024-04-29 22:36:52.807527 automated_interpretability-0.0.3/neuron_explainer/explanations/explainer.py
+-rw-r--r--   0        0        0     8867 2024-04-26 20:24:13.655965 automated_interpretability-0.0.3/neuron_explainer/explanations/explanations.py
+-rw-r--r--   0        0        0    32989 2024-04-26 20:24:13.656149 automated_interpretability-0.0.3/neuron_explainer/explanations/few_shot_examples.py
+-rw-r--r--   0        0        0     4698 2024-04-26 20:24:13.656293 automated_interpretability-0.0.3/neuron_explainer/explanations/prompt_builder.py
+-rw-r--r--   0        0        0    52696 2024-04-26 20:24:13.656497 automated_interpretability-0.0.3/neuron_explainer/explanations/puzzles.json
+-rw-r--r--   0        0        0     2178 2024-04-26 20:24:13.656717 automated_interpretability-0.0.3/neuron_explainer/explanations/puzzles.py
+-rw-r--r--   0        0        0     5888 2024-04-26 20:24:13.656874 automated_interpretability-0.0.3/neuron_explainer/explanations/scoring.py
+-rw-r--r--   0        0        0    45651 2024-04-27 05:42:47.856473 automated_interpretability-0.0.3/neuron_explainer/explanations/simulator.py
+-rw-r--r--   0        0        0     6603 2024-04-26 20:24:13.657275 automated_interpretability-0.0.3/neuron_explainer/explanations/test_explainer.py
+-rw-r--r--   0        0        0     7605 2024-04-26 20:24:13.657397 automated_interpretability-0.0.3/neuron_explainer/explanations/test_simulator.py
+-rw-r--r--   0        0        0     4836 2024-04-26 20:24:13.657520 automated_interpretability-0.0.3/neuron_explainer/explanations/token_space_few_shot_examples.py
+-rw-r--r--   0        0        0      147 2024-04-26 20:24:13.657701 automated_interpretability-0.0.3/neuron_explainer/fast_dataclasses/__init__.py
+-rw-r--r--   0        0        0     3043 2024-04-26 20:24:13.657821 automated_interpretability-0.0.3/neuron_explainer/fast_dataclasses/fast_dataclasses.py
+-rw-r--r--   0        0        0     2712 2024-04-26 20:24:13.657941 automated_interpretability-0.0.3/neuron_explainer/fast_dataclasses/test_fast_dataclasses.py
+-rw-r--r--   0        0        0      467 2024-04-29 22:49:55.665812 automated_interpretability-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 automated_interpretability-0.0.3/PKG-INFO
```

### Comparing `automated_interpretability-0.0.2/neuron_explainer/activations/activation_records.py` & `automated_interpretability-0.0.3/neuron_explainer/activations/activation_records.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.2/neuron_explainer/activations/activations.py` & `automated_interpretability-0.0.3/neuron_explainer/activations/activations.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.2/neuron_explainer/activations/token_connections.py` & `automated_interpretability-0.0.3/neuron_explainer/activations/token_connections.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.2/neuron_explainer/api_client.py` & `automated_interpretability-0.0.3/neuron_explainer/api_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,26 +76,18 @@
                     delay_s = min(delay_s * backoff_multiplier, max_delay_s)
 
         return f_retry
 
     return decorate
 
 
-API_KEY = os.getenv("OPENAI_API_KEY")
-assert API_KEY, "Please set the OPENAI_API_KEY environment variable"
-API_HTTP_HEADERS = {
-    "Content-Type": "application/json",
-    "Authorization": "Bearer " + API_KEY,
-}
-BASE_API_URL = "https://api.openai.com/v1"
-
-
 class ApiClient:
     """Performs inference using the OpenAI API. Supports response caching and concurrency limits."""
 
+    BASE_API_URL = "https://api.openai.com/v1"
     def __init__(
         self,
         model_name: str,
         # If set, no more than this number of HTTP requests will be made concurrently.
         max_concurrent: Optional[int] = None,
         # Whether to cache request/response pairs in memory to avoid duplicating requests.
         cache: bool = False,
@@ -112,31 +104,35 @@
         else:
             self._cache = None
 
     @exponential_backoff(retry_on=is_api_error)
     async def make_request(
         self, timeout_seconds: Optional[int] = None, json_mode: Optional[bool] = False, **kwargs: Any
     ) -> dict[str, Any]:
+        api_http_headers = {
+            "Content-Type": "application/json",
+            "Authorization": "Bearer " + os.getenv("OPENAI_API_KEY"),
+        }
         if self._cache is not None:
             key = orjson.dumps(kwargs)
             if key in self._cache:
                 return self._cache[key]
         async with contextlib.AsyncExitStack() as stack:
             if self._concurrency_check is not None:
                 await stack.enter_async_context(self._concurrency_check)
             http_client = await stack.enter_async_context(
                 httpx.AsyncClient(timeout=timeout_seconds)
             )
             # If the request has a "messages" key, it should be sent to the /chat/completions
             # endpoint. Otherwise, it should be sent to the /completions endpoint.
-            url = BASE_API_URL + ("/chat/completions" if "messages" in kwargs else "/completions")
+            url = ApiClient.BASE_API_URL + ("/chat/completions" if "messages" in kwargs else "/completions")
             kwargs["model"] = self.model_name
             if json_mode:
                 kwargs["response_format"] = {"type": "json_object"}
-            response = await http_client.post(url, headers=API_HTTP_HEADERS, json=kwargs)
+            response = await http_client.post(url, headers=api_http_headers, json=kwargs)
         # The response json has useful information but the exception doesn't include it, so print it
         # out then reraise.
         try:
             response.raise_for_status()
         except Exception as e:
             print(response.json())
             raise e
```

### Comparing `automated_interpretability-0.0.2/neuron_explainer/explanations/calibrated_simulator.py` & `automated_interpretability-0.0.3/neuron_explainer/explanations/calibrated_simulator.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.2/neuron_explainer/explanations/explainer.py` & `automated_interpretability-0.0.3/neuron_explainer/explanations/explainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,20 @@
     def from_int(cls, i: int) -> ContextSize:
         for context_size in cls:
             if context_size.value == i:
                 return context_size
         raise ValueError(f"{i} is not a valid ContextSize")
 
 
-HARMONY_V4_MODELS = ["gpt-3.5-turbo", "gpt-4", "gpt-4-1106-preview"]
+HARMONY_V4_MODELS = [
+    "gpt-3.5-turbo",
+    "gpt-4",
+    "gpt-4-1106-preview",
+    "gpt-4-turbo-2024-04-09",
+]
 
 
 class NeuronExplainer(ABC):
     """
     Abstract base class for Explainer classes that generate explanations from subclass-specific
     input data.
     """
```

### Comparing `automated_interpretability-0.0.2/neuron_explainer/explanations/explanations.py` & `automated_interpretability-0.0.3/neuron_explainer/explanations/explanations.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.2/neuron_explainer/explanations/few_shot_examples.py` & `automated_interpretability-0.0.3/neuron_explainer/explanations/few_shot_examples.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.2/neuron_explainer/explanations/prompt_builder.py` & `automated_interpretability-0.0.3/neuron_explainer/explanations/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.2/neuron_explainer/explanations/puzzles.json` & `automated_interpretability-0.0.3/neuron_explainer/explanations/puzzles.json`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.2/neuron_explainer/explanations/puzzles.py` & `automated_interpretability-0.0.3/neuron_explainer/explanations/puzzles.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.2/neuron_explainer/explanations/scoring.py` & `automated_interpretability-0.0.3/neuron_explainer/explanations/scoring.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.2/neuron_explainer/explanations/simulator.py` & `automated_interpretability-0.0.3/neuron_explainer/explanations/simulator.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.2/neuron_explainer/explanations/test_explainer.py` & `automated_interpretability-0.0.3/neuron_explainer/explanations/test_explainer.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.2/neuron_explainer/explanations/test_simulator.py` & `automated_interpretability-0.0.3/neuron_explainer/explanations/test_simulator.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.2/neuron_explainer/explanations/token_space_few_shot_examples.py` & `automated_interpretability-0.0.3/neuron_explainer/explanations/token_space_few_shot_examples.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.2/neuron_explainer/fast_dataclasses/fast_dataclasses.py` & `automated_interpretability-0.0.3/neuron_explainer/fast_dataclasses/fast_dataclasses.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.2/neuron_explainer/fast_dataclasses/test_fast_dataclasses.py` & `automated_interpretability-0.0.3/neuron_explainer/fast_dataclasses/test_fast_dataclasses.py`

 * *Files identical despite different names*

### Comparing `automated_interpretability-0.0.2/PKG-INFO` & `automated_interpretability-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automated-interpretability
-Version: 0.0.2
+Version: 0.0.3
 Summary: OpenAI's implementation of automated-interpretability, with some updates. Not officially affiliated with OpenAI.
 Author: OpenAI
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

