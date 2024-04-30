# Comparing `tmp/scrapegraphai-0.5.0b4.tar.gz` & `tmp/scrapegraphai-0.5.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.5.0b4.tar", max compression
+gzip compressed data, was "scrapegraphai-0.5.0b5.tar", max compression
```

## Comparing `scrapegraphai-0.5.0b4.tar` & `scrapegraphai-0.5.0b5.tar`

### file list

```diff
@@ -1,52 +1,54 @@
--rw-r--r--   0        0        0     1065 2024-04-30 09:52:09.572776 scrapegraphai-0.5.0b4/LICENSE
--rw-r--r--   0        0        0     8011 2024-04-30 09:52:09.572776 scrapegraphai-0.5.0b4/README.md
--rw-r--r--   0        0        0     1712 2024-04-30 09:52:29.881000 scrapegraphai-0.5.0b4/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6670 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      258 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     4359 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5128 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2615 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     2297 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     2484 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3225 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0      202 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0     1118 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      313 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      601 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      651 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      611 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      839 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      590 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      575 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1721 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1657 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      584 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7544 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3992 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     6860 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     7236 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     4097 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1592 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3337 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     5136 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     6555 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     4507 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     6729 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     1635 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      286 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     1742 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1443 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     3630 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      513 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0      731 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     1070 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1118 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      631 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0      990 2024-04-30 09:52:09.600776 scrapegraphai-0.5.0b4/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0     9809 1970-01-01 00:00:00.000000 scrapegraphai-0.5.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-30 12:30:57.894987 scrapegraphai-0.5.0b5/LICENSE
+-rw-r--r--   0        0        0     8753 2024-04-30 12:30:57.894987 scrapegraphai-0.5.0b5/README.md
+-rw-r--r--   0        0        0     1712 2024-04-30 12:31:20.718867 scrapegraphai-0.5.0b5/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6670 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      354 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0     4359 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     5128 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2367 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/graphs/json_scraper_graph.py
+-rw-r--r--   0        0        0     2615 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     2297 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     2484 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3225 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0     2361 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/graphs/xml_scraper_graph.py
+-rw-r--r--   0        0        0      202 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     1118 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      313 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      601 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      651 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      611 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      839 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      590 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      575 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1721 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1657 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      584 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7544 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     4187 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     6860 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     7236 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     4097 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1592 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3337 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     5136 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     6555 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     4507 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     6729 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     1635 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      286 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     1742 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1443 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3630 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      513 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0      731 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     1070 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1118 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      631 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0      990 2024-04-30 12:30:57.922987 scrapegraphai-0.5.0b5/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0    10551 1970-01-01 00:00:00.000000 scrapegraphai-0.5.0b5/PKG-INFO
```

### Comparing `scrapegraphai-0.5.0b4/LICENSE` & `scrapegraphai-0.5.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/README.md` & `scrapegraphai-0.5.0b5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -130,15 +130,46 @@
     config=graph_config
 )
 
 result = smart_scraper_graph.run()
 print(result)
 ```
 
-### Case 4: Extracting information using Gemini 
+### Case 4: Extracting information using Groq
+```python
+from scrapegraphai.graphs import SmartScraperGraph
+from scrapegraphai.utils import prettify_exec_info
+
+groq_key = os.getenv("GROQ_APIKEY")
+
+graph_config = {
+    "llm": {
+        "model": "groq/gemma-7b-it",
+        "api_key": groq_key,
+        "temperature": 0
+    },
+    "embeddings": {
+        "model": "ollama/nomic-embed-text",
+        "temperature": 0,
+        "base_url": "http://localhost:11434", 
+    },
+    "headless": False
+}
+
+smart_scraper_graph = SmartScraperGraph(
+    prompt="List me all the projects with their description and the author.",
+    source="https://perinim.github.io/projects",
+    config=graph_config
+)
+
+result = smart_scraper_graph.run()
+print(result)
+```
+
+### Case 5: Extracting information using Gemini 
 ```python
 from scrapegraphai.graphs import SmartScraperGraph
 GOOGLE_APIKEY = "YOUR_API_KEY"
 
 # Define the configuration for the graph
 graph_config = {
     "llm": {
```

### Comparing `scrapegraphai-0.5.0b4/pyproject.toml` & `scrapegraphai-0.5.0b5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "scrapegraphai"
 
-version = "0.5.0b4"
+version = "0.5.0b5"
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
```

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.5.0b5/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.5.0b5/scrapegraphai/graphs/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.5.0b5/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.5.0b5/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.5.0b5/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.5.0b5/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.5.0b5/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.5.0b5/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.5.0b5/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.5.0b5/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/models/azure_openai.py` & `scrapegraphai-0.5.0b5/scrapegraphai/models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/models/gemini.py` & `scrapegraphai-0.5.0b5/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/models/groq.py` & `scrapegraphai-0.5.0b5/scrapegraphai/models/groq.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/models/hugging_face.py` & `scrapegraphai-0.5.0b5/scrapegraphai/models/hugging_face.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/models/ollama.py` & `scrapegraphai-0.5.0b5/scrapegraphai/models/ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/models/openai.py` & `scrapegraphai-0.5.0b5/scrapegraphai/models/openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.5.0b5/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.5.0b5/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/nodes/__init__.py` & `scrapegraphai-0.5.0b5/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.5.0b5/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.5.0b5/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.5.0b5/scrapegraphai/nodes/fetch_node.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,17 +68,20 @@
         # Interpret input keys based on the provided input expression
         input_keys = self.get_input_keys(state)
 
         # Fetching data from the state based on the input keys
         input_data = [state[key] for key in input_keys]
 
         source = input_data[0]
-
+        if self.input == "json_dir" or self.input == "xml_dir":
+            compressed_document = [Document(page_content=source, metadata={
+                "source": "local_dir"
+            })]
         # if it is a local directory
-        if not source.startswith("http"):
+        elif not source.startswith("http"):
             compressed_document = [Document(page_content=remover(source), metadata={
                 "source": "local_dir"
             })]
 
         else:
             if self.node_config is not None and self.node_config.get("endpoint") is not None:
```

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.5.0b5/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.5.0b5/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.5.0b5/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.5.0b5/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.5.0b5/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.5.0b5/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-0.5.0b5/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.5.0b5/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-0.5.0b5/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.5.0b5/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.5.0b5/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.5.0b5/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.5.0b5/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.5.0b5/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-0.5.0b5/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/utils/remover.py` & `scrapegraphai-0.5.0b5/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.5.0b5/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.5.0b5/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.5.0b5/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b4/PKG-INFO` & `scrapegraphai-0.5.0b5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.5.0b4
+Version: 0.5.0b5
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -169,15 +169,46 @@
     config=graph_config
 )
 
 result = smart_scraper_graph.run()
 print(result)
 ```
 
-### Case 4: Extracting information using Gemini 
+### Case 4: Extracting information using Groq
+```python
+from scrapegraphai.graphs import SmartScraperGraph
+from scrapegraphai.utils import prettify_exec_info
+
+groq_key = os.getenv("GROQ_APIKEY")
+
+graph_config = {
+    "llm": {
+        "model": "groq/gemma-7b-it",
+        "api_key": groq_key,
+        "temperature": 0
+    },
+    "embeddings": {
+        "model": "ollama/nomic-embed-text",
+        "temperature": 0,
+        "base_url": "http://localhost:11434", 
+    },
+    "headless": False
+}
+
+smart_scraper_graph = SmartScraperGraph(
+    prompt="List me all the projects with their description and the author.",
+    source="https://perinim.github.io/projects",
+    config=graph_config
+)
+
+result = smart_scraper_graph.run()
+print(result)
+```
+
+### Case 5: Extracting information using Gemini 
 ```python
 from scrapegraphai.graphs import SmartScraperGraph
 GOOGLE_APIKEY = "YOUR_API_KEY"
 
 # Define the configuration for the graph
 graph_config = {
     "llm": {
```

