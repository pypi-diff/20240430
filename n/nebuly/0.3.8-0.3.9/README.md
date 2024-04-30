# Comparing `tmp/nebuly-0.3.8.tar.gz` & `tmp/nebuly-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nebuly-0.3.8.tar", max compression
+gzip compressed data, was "nebuly-0.3.9.tar", max compression
```

## Comparing `nebuly-0.3.8.tar` & `nebuly-0.3.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     4399 2024-02-13 15:15:36.427893 nebuly-0.3.8/README.md
--rw-r--r--   0        0        0      106 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/__init__.py
--rw-r--r--   0        0        0       87 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/ab_testing/__init__.py
--rw-r--r--   0        0        0     2255 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/ab_testing/main.py
--rw-r--r--   0        0        0     3813 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/ab_testing/types.py
--rw-r--r--   0        0        0      290 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/api_key.py
--rw-r--r--   0        0        0     2819 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/config.py
--rw-r--r--   0        0        0      866 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/consumers.py
--rw-r--r--   0        0        0     6989 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/contextmanager.py
--rw-r--r--   0        0        0     4407 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/entities.py
--rw-r--r--   0        0        0     3393 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/events.py
--rw-r--r--   0        0        0     1590 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/exceptions.py
--rw-r--r--   0        0        0     1518 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/init.py
--rw-r--r--   0        0        0    27681 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/monkey_patching.py
--rw-r--r--   0        0        0      534 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/observers.py
--rw-r--r--   0        0        0        0 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/providers/__init__.py
--rw-r--r--   0        0        0     3235 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/providers/anthropic.py
--rw-r--r--   0        0        0     4789 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/providers/aws_bedrock.py
--rw-r--r--   0        0        0     2280 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/providers/base.py
--rw-r--r--   0        0        0     5350 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/providers/cohere.py
--rw-r--r--   0        0        0     1160 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/providers/common.py
--rw-r--r--   0        0        0     4574 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/providers/google.py
--rw-r--r--   0        0        0     4276 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/providers/huggingface.py
--rw-r--r--   0        0        0     4436 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/providers/huggingface_hub.py
--rw-r--r--   0        0        0    17441 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/providers/langchain.py
--rw-r--r--   0        0        0    14923 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/providers/llama_index.py
--rw-r--r--   0        0        0    10909 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/providers/openai.py
--rw-r--r--   0        0        0     5301 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/providers/openai_legacy.py
--rw-r--r--   0        0        0      433 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/providers/utils.py
--rw-r--r--   0        0        0     5713 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/providers/vertexai.py
--rw-r--r--   0        0        0     3782 2024-02-13 15:15:36.427893 nebuly-0.3.8/nebuly/requests.py
--rw-r--r--   0        0        0     1419 2024-02-13 15:15:36.431893 nebuly-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     4858 1970-01-01 00:00:00.000000 nebuly-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     4399 2024-02-14 16:32:46.834811 nebuly-0.3.9/README.md
+-rw-r--r--   0        0        0      106 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/__init__.py
+-rw-r--r--   0        0        0       87 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/ab_testing/__init__.py
+-rw-r--r--   0        0        0     2255 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/ab_testing/main.py
+-rw-r--r--   0        0        0     3813 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/ab_testing/types.py
+-rw-r--r--   0        0        0      290 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/api_key.py
+-rw-r--r--   0        0        0     2819 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/config.py
+-rw-r--r--   0        0        0      866 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/consumers.py
+-rw-r--r--   0        0        0     6989 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/contextmanager.py
+-rw-r--r--   0        0        0     4407 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/entities.py
+-rw-r--r--   0        0        0     3393 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/events.py
+-rw-r--r--   0        0        0     1590 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/exceptions.py
+-rw-r--r--   0        0        0     1518 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/init.py
+-rw-r--r--   0        0        0    27681 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/monkey_patching.py
+-rw-r--r--   0        0        0      534 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/observers.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/providers/__init__.py
+-rw-r--r--   0        0        0     3235 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/providers/anthropic.py
+-rw-r--r--   0        0        0     4789 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/providers/aws_bedrock.py
+-rw-r--r--   0        0        0     2280 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/providers/base.py
+-rw-r--r--   0        0        0     5350 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/providers/cohere.py
+-rw-r--r--   0        0        0     1160 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/providers/common.py
+-rw-r--r--   0        0        0     4574 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/providers/google.py
+-rw-r--r--   0        0        0     4276 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/providers/huggingface.py
+-rw-r--r--   0        0        0     4436 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/providers/huggingface_hub.py
+-rw-r--r--   0        0        0    17585 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/providers/langchain.py
+-rw-r--r--   0        0        0    14923 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/providers/llama_index.py
+-rw-r--r--   0        0        0    10909 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/providers/openai.py
+-rw-r--r--   0        0        0     5301 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/providers/openai_legacy.py
+-rw-r--r--   0        0        0      433 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/providers/utils.py
+-rw-r--r--   0        0        0     5713 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/providers/vertexai.py
+-rw-r--r--   0        0        0     3782 2024-02-14 16:32:46.834811 nebuly-0.3.9/nebuly/requests.py
+-rw-r--r--   0        0        0     1419 2024-02-14 16:32:46.838811 nebuly-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     4858 1970-01-01 00:00:00.000000 nebuly-0.3.9/PKG-INFO
```

### Comparing `nebuly-0.3.8/README.md` & `nebuly-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/ab_testing/main.py` & `nebuly-0.3.9/nebuly/ab_testing/main.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/ab_testing/types.py` & `nebuly-0.3.9/nebuly/ab_testing/types.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/config.py` & `nebuly-0.3.9/nebuly/config.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/consumers.py` & `nebuly-0.3.9/nebuly/consumers.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/contextmanager.py` & `nebuly-0.3.9/nebuly/contextmanager.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/entities.py` & `nebuly-0.3.9/nebuly/entities.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/events.py` & `nebuly-0.3.9/nebuly/events.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/exceptions.py` & `nebuly-0.3.9/nebuly/exceptions.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/init.py` & `nebuly-0.3.9/nebuly/init.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/monkey_patching.py` & `nebuly-0.3.9/nebuly/monkey_patching.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/observers.py` & `nebuly-0.3.9/nebuly/observers.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/providers/anthropic.py` & `nebuly-0.3.9/nebuly/providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/providers/aws_bedrock.py` & `nebuly-0.3.9/nebuly/providers/aws_bedrock.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/providers/base.py` & `nebuly-0.3.9/nebuly/providers/base.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/providers/cohere.py` & `nebuly-0.3.9/nebuly/providers/cohere.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/providers/common.py` & `nebuly-0.3.9/nebuly/providers/common.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/providers/google.py` & `nebuly-0.3.9/nebuly/providers/google.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/providers/huggingface.py` & `nebuly-0.3.9/nebuly/providers/huggingface.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/providers/huggingface_hub.py` & `nebuly-0.3.9/nebuly/providers/huggingface_hub.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/providers/langchain.py` & `nebuly-0.3.9/nebuly/providers/langchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,18 @@
     for key in chain.output_keys:
         output[key] = result[key]
     return _parse_output(output)
 
 
 def _parse_output(output: str | dict[str, Any] | AIMessage) -> str:
     if isinstance(output, dict):
+        if "answer" in output:
+            return str(output["answer"])
+        if "output" in output:
+            return str(output["output"])
         return "\n".join([f"{key}: {value}" for key, value in output.items()])
     if isinstance(output, AIMessage):
         return str(output.content)
     return output
 
 
 def _parse_langchain_data(data: Any) -> str:
```

### Comparing `nebuly-0.3.8/nebuly/providers/llama_index.py` & `nebuly-0.3.9/nebuly/providers/llama_index.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/providers/openai.py` & `nebuly-0.3.9/nebuly/providers/openai.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/providers/openai_legacy.py` & `nebuly-0.3.9/nebuly/providers/openai_legacy.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/providers/vertexai.py` & `nebuly-0.3.9/nebuly/providers/vertexai.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/nebuly/requests.py` & `nebuly-0.3.9/nebuly/requests.py`

 * *Files identical despite different names*

### Comparing `nebuly-0.3.8/pyproject.toml` & `nebuly-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nebuly"
-version = "0.3.8"
+version = "0.3.9"
 description = "The SDK for instrumenting applications for tracking AI costs."
 authors = ["Nebuly"]
 readme = "README.md"
 packages = [{ include = "nebuly" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
```

### Comparing `nebuly-0.3.8/PKG-INFO` & `nebuly-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nebuly
-Version: 0.3.8
+Version: 0.3.9
 Summary: The SDK for instrumenting applications for tracking AI costs.
 Author: Nebuly
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

