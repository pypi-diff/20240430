# Comparing `tmp/scrapegraphai-0.4.1.tar.gz` & `tmp/scrapegraphai-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.4.1.tar", max compression
+gzip compressed data, was "scrapegraphai-0.4.2.tar", max compression
```

## Comparing `scrapegraphai-0.4.1.tar` & `scrapegraphai-0.4.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1065 2024-04-28 18:30:16.316592 scrapegraphai-0.4.1/LICENSE
--rw-r--r--   0        0        0     7907 2024-04-28 18:30:16.316592 scrapegraphai-0.4.1/README.md
--rw-r--r--   0        0        0     1660 2024-04-28 18:30:35.296634 scrapegraphai-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6670 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      258 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     3817 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5128 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2493 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     2192 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     2378 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3120 2024-04-28 18:30:16.344592 scrapegraphai-0.4.1/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0      202 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0      829 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      290 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      601 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      651 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      839 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      590 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      575 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1721 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1657 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      584 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7544 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3647 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     6860 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     7236 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     4097 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1592 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3337 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     5136 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     6555 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     4507 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     6118 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     1635 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      286 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     1742 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1443 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     3630 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      513 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0      731 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     1070 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1118 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      631 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0      990 2024-04-28 18:30:16.348592 scrapegraphai-0.4.1/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0     9619 1970-01-01 00:00:00.000000 scrapegraphai-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-03-03 14:00:51.183606 scrapegraphai-0.4.2/LICENSE
+-rw-r--r--   0        0        0     7907 2024-04-25 10:10:10.131040 scrapegraphai-0.4.2/README.md
+-rw-r--r--   0        0        0     1662 2024-04-29 12:48:39.748002 scrapegraphai-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-27 15:26:34.905630 scrapegraphai-0.4.2/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-03-03 14:00:51.196546 scrapegraphai-0.4.2/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6670 2024-03-24 19:34:24.965713 scrapegraphai-0.4.2/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      258 2024-04-20 20:58:42.218942 scrapegraphai-0.4.2/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0     4003 2024-04-29 12:44:54.713204 scrapegraphai-0.4.2/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     5128 2024-04-29 08:23:25.393540 scrapegraphai-0.4.2/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2493 2024-04-26 19:55:52.053207 scrapegraphai-0.4.2/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     2192 2024-04-26 19:55:52.053536 scrapegraphai-0.4.2/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     2378 2024-04-26 19:55:52.053681 scrapegraphai-0.4.2/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3120 2024-04-26 19:55:52.053819 scrapegraphai-0.4.2/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0      202 2024-04-25 10:11:59.646772 scrapegraphai-0.4.2/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0      874 2024-04-29 12:44:54.713452 scrapegraphai-0.4.2/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-04-09 11:20:43.626222 scrapegraphai-0.4.2/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2024-04-25 10:11:59.647049 scrapegraphai-0.4.2/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2024-04-08 20:25:15.266957 scrapegraphai-0.4.2/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      290 2024-04-12 10:59:59.485515 scrapegraphai-0.4.2/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      601 2024-04-09 11:20:43.626608 scrapegraphai-0.4.2/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      651 2024-04-08 20:25:27.931161 scrapegraphai-0.4.2/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      839 2024-04-12 10:59:59.485625 scrapegraphai-0.4.2/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      590 2024-04-08 20:25:35.475199 scrapegraphai-0.4.2/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      575 2024-04-08 20:25:42.545477 scrapegraphai-0.4.2/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1721 2024-04-08 20:25:31.195250 scrapegraphai-0.4.2/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1657 2024-04-08 20:25:37.349894 scrapegraphai-0.4.2/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      584 2024-04-26 17:27:54.828992 scrapegraphai-0.4.2/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7544 2024-04-08 20:25:53.786578 scrapegraphai-0.4.2/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-04-20 20:58:42.219990 scrapegraphai-0.4.2/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3647 2024-04-29 08:23:25.393880 scrapegraphai-0.4.2/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     6860 2024-04-26 17:27:54.829836 scrapegraphai-0.4.2/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     7236 2024-04-25 10:10:10.155594 scrapegraphai-0.4.2/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     4097 2024-04-20 20:58:42.221320 scrapegraphai-0.4.2/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1592 2024-04-20 20:58:42.221535 scrapegraphai-0.4.2/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3337 2024-04-20 20:58:42.221690 scrapegraphai-0.4.2/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     5136 2024-04-29 08:23:25.394564 scrapegraphai-0.4.2/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     6555 2024-04-29 08:23:25.395239 scrapegraphai-0.4.2/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     4507 2024-04-25 10:10:10.156452 scrapegraphai-0.4.2/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     6118 2024-04-26 17:27:54.830083 scrapegraphai-0.4.2/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     1635 2024-04-22 19:30:38.104934 scrapegraphai-0.4.2/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      286 2024-04-29 08:23:25.395683 scrapegraphai-0.4.2/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     1742 2024-04-25 10:10:10.156867 scrapegraphai-0.4.2/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1443 2024-04-25 10:10:10.157249 scrapegraphai-0.4.2/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3630 2024-04-06 12:43:33.712449 scrapegraphai-0.4.2/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      513 2024-04-29 08:23:25.396014 scrapegraphai-0.4.2/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0      731 2024-04-29 08:23:25.396243 scrapegraphai-0.4.2/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     1070 2024-04-25 10:10:10.157483 scrapegraphai-0.4.2/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1118 2024-04-06 12:46:22.008255 scrapegraphai-0.4.2/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      631 2024-04-06 12:44:50.349656 scrapegraphai-0.4.2/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0      990 2024-03-18 13:23:59.117686 scrapegraphai-0.4.2/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0     9619 1970-01-01 00:00:00.000000 scrapegraphai-0.4.2/PKG-INFO
```

### Comparing `scrapegraphai-0.4.1/LICENSE` & `scrapegraphai-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/README.md` & `scrapegraphai-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/pyproject.toml` & `scrapegraphai-0.4.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 [tool.poetry]
 name = "scrapegraphai"
-version = "0.4.1"
+
+version = "0.4.2"
+
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `scrapegraphai-0.4.1/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.4.2/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.4.2/scrapegraphai/graphs/abstract_graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,21 +60,26 @@
                 raise KeyError("Model not supported")
             return Gemini(llm_params)
 
         elif "ollama" in llm_params["model"]:
             llm_params["model"] = llm_params["model"].split("/")[-1]
 
             # allow user to set model_tokens in config
-            if "model_tokens" in llm_params:
-                self.model_token = llm_params["model_tokens"]
-            elif llm_params["model"] in models_tokens["ollama"]:
-                try:
-                    self.model_token = models_tokens["ollama"][llm_params["model"]]
-                except KeyError:
-                    raise KeyError("Model not supported")
+            try:
+                if "model_tokens" in llm_params:
+                    self.model_token = llm_params["model_tokens"]
+                elif llm_params["model"] in models_tokens["ollama"]:
+                    try:
+                        self.model_token = models_tokens["ollama"][llm_params["model"]]
+                    except KeyError:
+                        raise KeyError("Model not supported")
+                else:
+                    self.model_token = 8192
+            except AttributeError:
+                self.model_token = 8192
 
             return Ollama(llm_params)
         elif "hugging_face" in llm_params["model"]:
             try:
                 self.model_token = models_tokens["hugging_face"][llm_params["model"]]
             except KeyError:
                 raise KeyError("Model not supported")
```

### Comparing `scrapegraphai-0.4.1/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.4.2/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.4.2/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.4.2/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.4.2/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.4.2/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.4.2/scrapegraphai/helpers/models_tokens.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,9 +27,12 @@
         "llama2": 4096,
         "llama3": 8192,
         "mistral": 8192,
         "codellama": 16000,
         "dolphin-mixtral": 32000,
         "mistral-openorca": 32000,
         "stablelm-zephyr": 8192
+    },
+    "gemma": {
+        "gemma": 8192,
     }
 }
```

### Comparing `scrapegraphai-0.4.1/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.4.2/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.4.2/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/models/azure_openai.py` & `scrapegraphai-0.4.2/scrapegraphai/models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/models/gemini.py` & `scrapegraphai-0.4.2/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/models/hugging_face.py` & `scrapegraphai-0.4.2/scrapegraphai/models/hugging_face.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/models/ollama.py` & `scrapegraphai-0.4.2/scrapegraphai/models/ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/models/openai.py` & `scrapegraphai-0.4.2/scrapegraphai/models/openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.4.2/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.4.2/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/nodes/__init__.py` & `scrapegraphai-0.4.2/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.4.2/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.4.2/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.4.2/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.4.2/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.4.2/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.4.2/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.4.2/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.4.2/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.4.2/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-0.4.2/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.4.2/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-0.4.2/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.4.2/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.4.2/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.4.2/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.4.2/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.4.2/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-0.4.2/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/utils/remover.py` & `scrapegraphai-0.4.2/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.4.2/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.4.2/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.4.2/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.4.1/PKG-INFO` & `scrapegraphai-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.4.1
+Version: 0.4.2
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >=3.9,<4.0
```

