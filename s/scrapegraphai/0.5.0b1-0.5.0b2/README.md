# Comparing `tmp/scrapegraphai-0.5.0b1.tar.gz` & `tmp/scrapegraphai-0.5.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.5.0b1.tar", max compression
+gzip compressed data, was "scrapegraphai-0.5.0b2.tar", max compression
```

## Comparing `scrapegraphai-0.5.0b1.tar` & `scrapegraphai-0.5.0b2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1065 2024-04-30 01:00:25.464008 scrapegraphai-0.5.0b1/LICENSE
--rw-r--r--   0        0        0     7908 2024-04-30 01:00:25.464008 scrapegraphai-0.5.0b1/README.md
--rw-r--r--   0        0        0     1689 2024-04-30 01:00:43.868112 scrapegraphai-0.5.0b1/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6670 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      258 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     4359 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5128 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2493 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     2192 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     2378 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3120 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0      202 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0      987 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      313 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      601 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      651 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      611 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      839 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      590 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      575 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1721 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1657 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      584 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7544 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3647 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     6860 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     7236 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     4097 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1592 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3337 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     5136 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     6555 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     4507 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     6729 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     1635 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      286 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     1742 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1443 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     3630 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      513 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0      731 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     1070 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1118 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      631 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0      990 2024-04-30 01:00:25.492008 scrapegraphai-0.5.0b1/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0     9662 1970-01-01 00:00:00.000000 scrapegraphai-0.5.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-30 05:57:08.511579 scrapegraphai-0.5.0b2/LICENSE
+-rw-r--r--   0        0        0     8011 2024-04-30 05:57:08.511579 scrapegraphai-0.5.0b2/README.md
+-rw-r--r--   0        0        0     1712 2024-04-30 05:57:33.199783 scrapegraphai-0.5.0b2/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6670 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      258 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0     4359 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     5128 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2493 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     2297 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     2484 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3225 2024-04-30 05:57:08.539579 scrapegraphai-0.5.0b2/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0      202 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0      987 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      313 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      601 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      651 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      611 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      839 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      590 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      575 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1721 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1657 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      584 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7544 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3992 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     6860 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     7236 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     4097 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1592 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3337 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     5136 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     6555 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     4507 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     6729 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     1635 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      286 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     1742 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1443 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3630 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      513 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0      731 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     1070 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1118 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      631 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0      990 2024-04-30 05:57:08.543579 scrapegraphai-0.5.0b2/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0     9809 1970-01-01 00:00:00.000000 scrapegraphai-0.5.0b2/PKG-INFO
```

### Comparing `scrapegraphai-0.5.0b1/LICENSE` & `scrapegraphai-0.5.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/README.md` & `scrapegraphai-0.5.0b2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 ## 🚀 Quick install
 
 The reference page for Scrapegraph-ai is available on the official page of pypy: [pypi](https://pypi.org/project/scrapegraphai/).
 
 ```bash
 pip install scrapegraphai
 ```
+you will also need to install Playwright for javascript-based scraping:
+```bash
+playwright install
+```
 ## 🔍 Demo
 Official streamlit demo:
 
 [![My Skills](https://skillicons.dev/icons?i=react)](https://scrapegraph-ai-demo.streamlit.app/)
 
 Try it directly on the web using Google Colab:
```

### Comparing `scrapegraphai-0.5.0b1/pyproject.toml` & `scrapegraphai-0.5.0b2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "scrapegraphai"
 
-version = "0.5.0b1"
+version = "0.5.0b2"
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
@@ -35,14 +35,15 @@
 tiktoken = {version = ">=0.5.2,<0.6.0"}
 tqdm = "4.66.1"
 graphviz = "0.20.1"
 google = "3.0.0"
 minify-html = "0.15.0"
 free-proxy = "1.1.1"
 langchain-groq = "0.1.3"
+playwright = "^1.43.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "8.0.0"
 
 [tool.poetry.group.docs]
 optional = true
```

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.5.0b2/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.5.0b2/scrapegraphai/graphs/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.5.0b2/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.5.0b2/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.5.0b2/scrapegraphai/graphs/search_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
             input="user_prompt",
             output=["url"],
             node_config={"llm": self.llm_model}
         )
         fetch_node = FetchNode(
             input="url | local_dir",
             output=["doc"],
+            node_config={"headless": True if self.config is None else self.config.get("headless", True)}
         )
         parse_node = ParseNode(
             input="doc",
             output=["parsed_doc"],
             node_config={"chunk_size": self.model_token}
         )
         rag_node = RAGNode(
```

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.5.0b2/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,21 +21,23 @@
         """
         Initializes the SmartScraperGraph with a prompt, source, and configuration.
         """
         super().__init__(prompt, config, source)
 
         self.input_key = "url" if source.startswith("http") else "local_dir"
 
+
     def _create_graph(self):
         """
         Creates the graph of nodes representing the workflow for web scraping.
         """
         fetch_node = FetchNode(
             input="url | local_dir",
             output=["doc"],
+            node_config={"headless": True if self.config is None else self.config.get("headless", True)}
         )
         parse_node = ParseNode(
             input="doc",
             output=["parsed_doc"],
             node_config={"chunk_size": self.model_token}
         )
         rag_node = RAGNode(
```

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.5.0b2/scrapegraphai/graphs/speech_graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     def _create_graph(self):
         """
         Creates the graph of nodes representing the workflow for web scraping and summarization.
         """
         fetch_node = FetchNode(
             input="url | local_dir",
             output=["doc"],
+            node_config={"headless": True if self.config is None else self.config.get("headless", True)}
         )
         parse_node = ParseNode(
             input="doc",
             output=["parsed_doc"],
             node_config={"chunk_size": self.model_token}
         )
         rag_node = RAGNode(
```

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.5.0b2/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.5.0b2/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.5.0b2/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/models/azure_openai.py` & `scrapegraphai-0.5.0b2/scrapegraphai/models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/models/gemini.py` & `scrapegraphai-0.5.0b2/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/models/groq.py` & `scrapegraphai-0.5.0b2/scrapegraphai/models/groq.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/models/hugging_face.py` & `scrapegraphai-0.5.0b2/scrapegraphai/models/hugging_face.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/models/ollama.py` & `scrapegraphai-0.5.0b2/scrapegraphai/models/ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/models/openai.py` & `scrapegraphai-0.5.0b2/scrapegraphai/models/openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.5.0b2/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.5.0b2/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/nodes/__init__.py` & `scrapegraphai-0.5.0b2/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.5.0b2/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.5.0b2/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.5.0b2/scrapegraphai/nodes/fetch_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ 
 Module for fetching the HTML node
 """
 
-from typing import List
-from langchain_community.document_loaders import AsyncHtmlLoader
+from typing import List, Optional
+from langchain_community.document_loaders import AsyncChromiumLoader
 from langchain_core.documents import Document
 from .base_node import BaseNode
 from ..utils.remover import remover
 
 
 class FetchNode(BaseNode):
     """
@@ -33,23 +33,25 @@
     Methods:
         execute(state): Fetches the HTML content for the URL specified in the state and
                         updates the state with this content under the 'document' key.
                         The 'url' key must be present in the state for the operation
                         to succeed.
     """
 
-    def __init__(self, input: str, output: List[str], node_name: str = "Fetch"):
+    def __init__(self, input: str, output: List[str], node_config: Optional[dict], node_name: str = "Fetch"):
         """
         Initializes the FetchHTMLNode with a node name and node type.
         Arguments:
             node_name (str): name of the node
             prox_rotation (bool): if you wamt to rotate proxies
         """
         super().__init__(node_name, "node", input, output, 1)
 
+        self.headless = True if node_config is None else node_config.get("headless", True)
+
     def execute(self, state):
         """
         Executes the node's logic to fetch HTML content from a specified URL and
         update the state with this content.
 
         Args:
             state (dict): The current state of the graph, expected to contain a 'url' key.
@@ -75,18 +77,25 @@
         if not source.startswith("http"):
             compressed_document = [Document(page_content=remover(source), metadata={
                 "source": "local_dir"
             })]
 
         else:
             if self.node_config is not None and self.node_config.get("endpoint") is not None:
-                loader = AsyncHtmlLoader(
-                    source, proxies={"http": self.node_config["endpoint"]})
+                
+                loader = AsyncChromiumLoader(
+                    [source],
+                    proxies={"http": self.node_config["endpoint"]},
+                    headless=self.headless,
+                )
             else:
-                loader = AsyncHtmlLoader(source)
+                loader = AsyncChromiumLoader(
+                    [source],
+                    headless=self.headless,
+                )
 
             document = loader.load()
             compressed_document = [
-                Document(page_content=remover(str(document)))]
+                Document(page_content=remover(str(document[0].page_content)))]
 
         state.update({self.output[0]: compressed_document})
         return state
```

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.5.0b2/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.5.0b2/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.5.0b2/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.5.0b2/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.5.0b2/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.5.0b2/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-0.5.0b2/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.5.0b2/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-0.5.0b2/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.5.0b2/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.5.0b2/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.5.0b2/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.5.0b2/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.5.0b2/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-0.5.0b2/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/utils/remover.py` & `scrapegraphai-0.5.0b2/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.5.0b2/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.5.0b2/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.5.0b2/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b1/PKG-INFO` & `scrapegraphai-0.5.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.5.0b1
+Version: 0.5.0b2
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -25,14 +25,15 @@
 Requires-Dist: html2text (==2020.1.16)
 Requires-Dist: langchain (==0.1.14)
 Requires-Dist: langchain-google-genai (==1.0.1)
 Requires-Dist: langchain-groq (==0.1.3)
 Requires-Dist: langchain-openai (==0.1.1)
 Requires-Dist: minify-html (==0.15.0)
 Requires-Dist: pandas (==2.0.3)
+Requires-Dist: playwright (>=1.43.0,<2.0.0)
 Requires-Dist: python-dotenv (==1.0.1)
 Requires-Dist: tiktoken (>=0.5.2,<0.6.0)
 Requires-Dist: tqdm (==4.66.1)
 Project-URL: Documentation, https://scrapegraph-doc.onrender.com/
 Project-URL: Repository, https://github.com/VinciGit00/Scrapegraph-ai
 Description-Content-Type: text/markdown
 
@@ -57,14 +58,18 @@
 ## 🚀 Quick install
 
 The reference page for Scrapegraph-ai is available on the official page of pypy: [pypi](https://pypi.org/project/scrapegraphai/).
 
 ```bash
 pip install scrapegraphai
 ```
+you will also need to install Playwright for javascript-based scraping:
+```bash
+playwright install
+```
 ## 🔍 Demo
 Official streamlit demo:
 
 [![My Skills](https://skillicons.dev/icons?i=react)](https://scrapegraph-ai-demo.streamlit.app/)
 
 Try it directly on the web using Google Colab:
```

