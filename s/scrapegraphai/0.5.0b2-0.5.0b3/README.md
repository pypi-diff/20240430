# Comparing `tmp/scrapegraphai-0.5.0b2.tar.gz` & `tmp/scrapegraphai-0.5.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.5.0b2.tar", max compression
+gzip compressed data, was "scrapegraphai-0.5.0b3.tar", max compression
```

## Comparing `scrapegraphai-0.5.0b2.tar` & `scrapegraphai-0.5.0b3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1065 2024-04-30 05:57:08.511579 scrapegraphai-0.5.0b2/LICENSE
--rw-r--r--   0        0        0     8011 2024-04-30 05:57:08.511579 scrapegraphai-0.5.0b2/README.md
--rw-r--r--   0        0        0     1712 2024-04-30 05:57:33.199783 scrapegraphai-0.5.0b2/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6670 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      258 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     4359 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5128 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2493 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     2297 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     2484 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3225 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0      202 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0      987 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      313 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      601 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      651 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      611 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      839 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      590 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      575 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1721 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1657 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      584 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7544 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3992 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     6860 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     7236 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     4097 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1592 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3337 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     5136 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     6555 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     4507 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     6729 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     1635 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      286 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     1742 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1443 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     3630 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      513 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0      731 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     1070 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1118 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      631 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0      990 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0     9809 1970-01-01 00:00:00.000000 scrapegraphai-0.5.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-30 08:13:26.927114 scrapegraphai-0.5.0b3/LICENSE
+-rw-r--r--   0        0        0     8011 2024-04-30 08:13:26.927114 scrapegraphai-0.5.0b3/README.md
+-rw-r--r--   0        0        0     1712 2024-04-30 08:13:53.867178 scrapegraphai-0.5.0b3/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6670 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      258 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0     4359 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     5128 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2493 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     2297 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     2484 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3225 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0      202 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     1118 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      313 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      601 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      651 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      611 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      839 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      590 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      575 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1721 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1657 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      584 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7544 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3992 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     6860 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     7236 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     4097 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1592 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3337 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     5136 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     6555 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     4507 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     6729 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     1635 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      286 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     1742 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1443 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3630 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      513 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0      731 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     1070 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1118 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      631 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0      990 2024-04-30 08:13:26.955114 scrapegraphai-0.5.0b3/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0     9809 1970-01-01 00:00:00.000000 scrapegraphai-0.5.0b3/PKG-INFO
```

### Comparing `scrapegraphai-0.5.0b2/LICENSE` & `scrapegraphai-0.5.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/README.md` & `scrapegraphai-0.5.0b3/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/pyproject.toml` & `scrapegraphai-0.5.0b3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "scrapegraphai"
 
-version = "0.5.0b2"
+version = "0.5.0b3"
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
```

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.5.0b3/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.5.0b3/scrapegraphai/graphs/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.5.0b3/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.5.0b3/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.5.0b3/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.5.0b3/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.5.0b3/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.5.0b3/scrapegraphai/helpers/models_tokens.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,15 +28,20 @@
         "llama3": 8192,
         "mistral": 8192,
         "codellama": 16000,
         "dolphin-mixtral": 32000,
         "mistral-openorca": 32000,
         "stablelm-zephyr": 8192
     },
-    
     "groq": {
         "llama3-8b-8192": 8192,
         "llama3-70b-8192": 8192,
         "mixtral-8x7b-32768": 32768,
         "gemma-7b-it": 8192,
     },
+    "claude": {
+        "claude_instant": 100000,
+        "claude2": 9000,
+        "claude2.1": 200000,
+        "claude3": 200000
+    }
 }
```

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.5.0b3/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.5.0b3/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/models/azure_openai.py` & `scrapegraphai-0.5.0b3/scrapegraphai/models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/models/gemini.py` & `scrapegraphai-0.5.0b3/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/models/groq.py` & `scrapegraphai-0.5.0b3/scrapegraphai/models/groq.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/models/hugging_face.py` & `scrapegraphai-0.5.0b3/scrapegraphai/models/hugging_face.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/models/ollama.py` & `scrapegraphai-0.5.0b3/scrapegraphai/models/ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/models/openai.py` & `scrapegraphai-0.5.0b3/scrapegraphai/models/openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.5.0b3/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.5.0b3/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/nodes/__init__.py` & `scrapegraphai-0.5.0b3/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.5.0b3/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.5.0b3/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.5.0b3/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.5.0b3/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.5.0b3/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.5.0b3/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.5.0b3/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.5.0b3/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.5.0b3/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-0.5.0b3/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.5.0b3/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-0.5.0b3/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.5.0b3/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.5.0b3/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.5.0b3/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.5.0b3/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.5.0b3/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-0.5.0b3/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/utils/remover.py` & `scrapegraphai-0.5.0b3/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.5.0b3/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.5.0b3/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.5.0b3/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b2/PKG-INFO` & `scrapegraphai-0.5.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.5.0b2
+Version: 0.5.0b3
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >=3.9,<4.0
```

