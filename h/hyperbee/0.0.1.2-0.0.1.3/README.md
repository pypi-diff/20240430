# Comparing `tmp/hyperbee-0.0.1.2.tar.gz` & `tmp/hyperbee-0.0.1.3.tar.gz`

## Comparing `hyperbee-0.0.1.2.tar` & `hyperbee-0.0.1.3.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 hyperbee-0.0.1.2/src/hyperbee/__init__.py
--rw-r--r--   0        0        0    16721 2020-02-02 00:00:00.000000 hyperbee-0.0.1.2/src/hyperbee/_client.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hyperbee-0.0.1.2/src/hyperbee/_version.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 hyperbee-0.0.1.2/src/hyperbee/version.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 hyperbee-0.0.1.2/src/hyperbee/resources/__init__.py
--rw-r--r--   0        0        0    29864 2020-02-02 00:00:00.000000 hyperbee-0.0.1.2/src/hyperbee/resources/completions.py
--rw-r--r--   0        0        0    10189 2020-02-02 00:00:00.000000 hyperbee-0.0.1.2/src/hyperbee/resources/models.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 hyperbee-0.0.1.2/src/hyperbee/resources/chat/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 hyperbee-0.0.1.2/src/hyperbee/resources/chat/chat.py
--rw-r--r--   0        0        0    33700 2020-02-02 00:00:00.000000 hyperbee-0.0.1.2/src/hyperbee/resources/chat/completions.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 hyperbee-0.0.1.2/.gitignore
--rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 hyperbee-0.0.1.2/README.md
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 hyperbee-0.0.1.2/pyproject.toml
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 hyperbee-0.0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/__init__.py
+-rw-r--r--   0        0        0    16770 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/_client.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/_version.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/version.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/resources/__init__.py
+-rw-r--r--   0        0        0    29864 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/resources/completions.py
+-rw-r--r--   0        0        0    10189 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/resources/models.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/resources/chat/__init__.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/resources/chat/chat.py
+-rw-r--r--   0        0        0    33700 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/resources/chat/completions.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/resources/pipeline/__init__.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/src/hyperbee/resources/pipeline/pipeline.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/.gitignore
+-rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/README.md
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 hyperbee-0.0.1.3/PKG-INFO
```

### Comparing `hyperbee-0.0.1.2/src/hyperbee/__init__.py` & `hyperbee-0.0.1.3/src/hyperbee/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.2/src/hyperbee/_client.py` & `hyperbee-0.0.1.3/src/hyperbee/_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,14 +117,15 @@
         self._default_stream_cls = Stream
 
         self.completions = resources.Completions(self)
         self.chat = resources.Chat(self)
         self.models = resources.Models(self)
         self.with_raw_response = HiveWithRawResponse(self)
         self.with_streaming_response = HiveWithStreamedResponse(self)
+        self.pipeline = resources.Pipeline(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
 
     @property
```

### Comparing `hyperbee-0.0.1.2/src/hyperbee/resources/__init__.py` & `hyperbee-0.0.1.3/src/hyperbee/resources/chat/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,22 +4,14 @@
     Chat,
     AsyncChat,
     ChatWithRawResponse,
     AsyncChatWithRawResponse,
     ChatWithStreamingResponse,
     AsyncChatWithStreamingResponse,
 )
-from .models import (
-    Models,
-    AsyncModels,
-    ModelsWithRawResponse,
-    AsyncModelsWithRawResponse,
-    ModelsWithStreamingResponse,
-    AsyncModelsWithStreamingResponse,
-)
 from .completions import (
     Completions,
     AsyncCompletions,
     CompletionsWithRawResponse,
     AsyncCompletionsWithRawResponse,
     CompletionsWithStreamingResponse,
     AsyncCompletionsWithStreamingResponse,
@@ -34,14 +26,8 @@
     "AsyncCompletionsWithStreamingResponse",
     "Chat",
     "AsyncChat",
     "ChatWithRawResponse",
     "AsyncChatWithRawResponse",
     "ChatWithStreamingResponse",
     "AsyncChatWithStreamingResponse",
-    "Models",
-    "AsyncModels",
-    "ModelsWithRawResponse",
-    "AsyncModelsWithRawResponse",
-    "ModelsWithStreamingResponse",
-    "AsyncModelsWithStreamingResponse"
 ]
```

### Comparing `hyperbee-0.0.1.2/src/hyperbee/resources/completions.py` & `hyperbee-0.0.1.3/src/hyperbee/resources/completions.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.2/src/hyperbee/resources/models.py` & `hyperbee-0.0.1.3/src/hyperbee/resources/models.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.2/src/hyperbee/resources/chat/__init__.py` & `hyperbee-0.0.1.3/src/hyperbee/resources/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,30 +4,48 @@
     Chat,
     AsyncChat,
     ChatWithRawResponse,
     AsyncChatWithRawResponse,
     ChatWithStreamingResponse,
     AsyncChatWithStreamingResponse,
 )
+from .models import (
+    Models,
+    AsyncModels,
+    ModelsWithRawResponse,
+    AsyncModelsWithRawResponse,
+    ModelsWithStreamingResponse,
+    AsyncModelsWithStreamingResponse,
+)
 from .completions import (
     Completions,
     AsyncCompletions,
     CompletionsWithRawResponse,
     AsyncCompletionsWithRawResponse,
     CompletionsWithStreamingResponse,
     AsyncCompletionsWithStreamingResponse,
 )
+from .pipeline import (
+    Pipeline,
+)
 
 __all__ = [
     "Completions",
     "AsyncCompletions",
     "CompletionsWithRawResponse",
     "AsyncCompletionsWithRawResponse",
     "CompletionsWithStreamingResponse",
     "AsyncCompletionsWithStreamingResponse",
     "Chat",
     "AsyncChat",
     "ChatWithRawResponse",
     "AsyncChatWithRawResponse",
     "ChatWithStreamingResponse",
     "AsyncChatWithStreamingResponse",
+    "Models",
+    "AsyncModels",
+    "ModelsWithRawResponse",
+    "AsyncModelsWithRawResponse",
+    "ModelsWithStreamingResponse",
+    "AsyncModelsWithStreamingResponse",
+    "Pipeline"
 ]
```

### Comparing `hyperbee-0.0.1.2/src/hyperbee/resources/chat/chat.py` & `hyperbee-0.0.1.3/src/hyperbee/resources/chat/chat.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.2/src/hyperbee/resources/chat/completions.py` & `hyperbee-0.0.1.3/src/hyperbee/resources/chat/completions.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.2/README.md` & `hyperbee-0.0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.1.2/pyproject.toml` & `hyperbee-0.0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hyperbee"
-version = "0.0.1.2"
+version = "0.0.1.3"
 description = "The official Python library for the hyperbee API"
 readme = "README.md"
 license = "Apache-2.0"
 authors = [
 { name = "Hive", email = "support@hyperbee.ai" },
 ]
 dependencies = [
```

### Comparing `hyperbee-0.0.1.2/PKG-INFO` & `hyperbee-0.0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hyperbee
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: The official Python library for the hyperbee API
 Project-URL: Homepage, https://github.com/HyperbeeAI/hive-python
 Project-URL: Repository, https://github.com/HyperbeeAI/hive-python
 Author-email: Hive <support@hyperbee.ai>
 License-Expression: Apache-2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

