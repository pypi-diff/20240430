# Comparing `tmp/lango_cli_beta-0.0.1rc1.tar.gz` & `tmp/lango_cli_beta-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lango_cli_beta-0.0.1rc1.tar", max compression
+gzip compressed data, was "lango_cli_beta-0.0.1rc2.tar", max compression
```

## Comparing `lango_cli_beta-0.0.1rc1.tar` & `lango_cli_beta-0.0.1rc2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1072 2024-04-22 21:20:25.347250 lango_cli_beta-0.0.1rc1/LICENSE
--rw-r--r--   0        0        0    10886 2024-04-22 22:50:03.690083 lango_cli_beta-0.0.1rc1/README.md
--rw-r--r--   0        0        0        0 2024-04-22 22:50:03.690170 lango_cli_beta-0.0.1rc1/lango_cli_beta/__init__.py
--rw-r--r--   0        0        0    47973 2024-04-22 22:50:03.690392 lango_cli_beta-0.0.1rc1/lango_cli_beta/_sample_data/adversarial_attacks_on_llms.txt
--rw-r--r--   0        0        0    35074 2024-04-22 22:50:03.690898 lango_cli_beta-0.0.1rc1/lango_cli_beta/_sample_data/diffusion_models_for_video_generation.txt
--rw-r--r--   0        0        0    38804 2024-04-22 22:50:03.691112 lango_cli_beta-0.0.1rc1/lango_cli_beta/_sample_data/generalized_visual_language_models.txt
--rw-r--r--   0        0        0    38842 2024-04-22 22:50:03.691283 lango_cli_beta-0.0.1rc1/lango_cli_beta/_sample_data/learning_with_not_enough_data_p_1_semi_supervised_learning.txt
--rw-r--r--   0        0        0    31312 2024-04-22 22:50:03.692088 lango_cli_beta-0.0.1rc1/lango_cli_beta/_sample_data/learning_with_not_enough_data_p_2_active_earning.txt
--rw-r--r--   0        0        0    38894 2024-04-22 22:50:03.692415 lango_cli_beta-0.0.1rc1/lango_cli_beta/_sample_data/learning_with_not_enough_data_p_3_data_generation.txt
--rw-r--r--   0        0        0    46795 2024-04-22 22:50:03.692606 lango_cli_beta-0.0.1rc1/lango_cli_beta/_sample_data/llm_agents.txt
--rw-r--r--   0        0        0    30979 2024-04-22 22:50:03.692742 lango_cli_beta-0.0.1rc1/lango_cli_beta/_sample_data/prompt_eng.txt
--rw-r--r--   0        0        0    29209 2024-04-22 22:50:03.692902 lango_cli_beta-0.0.1rc1/lango_cli_beta/_sample_data/thinking_about_high_quality_human_data.txt
--rw-r--r--   0        0        0     3735 2024-04-22 22:51:33.041227 lango_cli_beta-0.0.1rc1/lango_cli_beta/cli.py
--rw-r--r--   0        0        0     2723 2024-04-22 22:50:03.693153 lango_cli_beta-0.0.1rc1/lango_cli_beta/constants.py
--rw-r--r--   0        0        0      587 2024-04-22 22:50:03.693626 lango_cli_beta-0.0.1rc1/lango_cli_beta/namespaces/chat.py
--rw-r--r--   0        0        0     8490 2024-04-22 23:04:40.154483 lango_cli_beta-0.0.1rc1/lango_cli_beta/namespaces/config.py
--rw-r--r--   0        0        0      337 2024-04-22 22:50:03.694327 lango_cli_beta-0.0.1rc1/lango_cli_beta/namespaces/export.py
--rw-r--r--   0        0        0     4583 2024-04-22 23:04:40.155115 lango_cli_beta-0.0.1rc1/lango_cli_beta/namespaces/ingest.py
--rw-r--r--   0        0        0     2110 2024-04-22 22:50:03.694680 lango_cli_beta-0.0.1rc1/lango_cli_beta/namespaces/init.py
--rw-r--r--   0        0        0     2725 2024-04-22 23:04:40.155535 lango_cli_beta-0.0.1rc1/lango_cli_beta/namespaces/start.py
--rw-r--r--   0        0        0     5854 2024-04-22 23:15:10.800827 lango_cli_beta-0.0.1rc1/lango_cli_beta/namespaces/utils.py
--rw-r--r--   0        0        0        0 2024-04-22 22:50:03.695229 lango_cli_beta-0.0.1rc1/lango_cli_beta/py.typed
--rw-r--r--   0        0        0     3739 2024-04-22 23:25:20.929240 lango_cli_beta-0.0.1rc1/lango_cli_beta/rag/basic_chat.py
--rw-r--r--   0        0        0     1127 2024-04-22 22:50:03.695732 lango_cli_beta-0.0.1rc1/lango_cli_beta/rag/chat.py
--rw-r--r--   0        0        0     4411 2024-04-22 22:50:03.695906 lango_cli_beta-0.0.1rc1/lango_cli_beta/rag/ingest.py
--rw-r--r--   0        0        0     1389 2024-04-22 23:04:40.156552 lango_cli_beta-0.0.1rc1/lango_cli_beta/rag/llm_chain.py
--rw-r--r--   0        0        0    10622 2024-04-22 23:25:20.929772 lango_cli_beta-0.0.1rc1/lango_cli_beta/rag/query_construction.py
--rw-r--r--   0        0        0      253 2024-04-22 22:50:03.696373 lango_cli_beta-0.0.1rc1/lango_cli_beta/rag/types.py
--rw-r--r--   0        0        0     1636 2024-04-22 23:04:40.156967 lango_cli_beta-0.0.1rc1/lango_cli_beta/rag/utils.py
--rw-r--r--   0        0        0     3951 2024-04-22 22:50:03.696592 lango_cli_beta-0.0.1rc1/lango_cli_beta/rag_config.py
--rw-r--r--   0        0        0      731 2024-04-22 22:50:03.696686 lango_cli_beta-0.0.1rc1/lango_cli_beta/utils.py
--rw-r--r--   0        0        0     2479 2024-04-22 23:26:29.589397 lango_cli_beta-0.0.1rc1/pyproject.toml
--rw-r--r--   0        0        0    12266 1970-01-01 00:00:00.000000 lango_cli_beta-0.0.1rc1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-26 00:38:25.039155 lango_cli_beta-0.0.1rc2/LICENSE
+-rw-r--r--   0        0        0    10886 2024-04-26 00:38:25.039545 lango_cli_beta-0.0.1rc2/README.md
+-rw-r--r--   0        0        0        0 2024-04-26 00:38:25.039609 lango_cli_beta-0.0.1rc2/lango_cli_beta/__init__.py
+-rw-r--r--   0        0        0    47973 2024-04-26 00:38:25.039851 lango_cli_beta-0.0.1rc2/lango_cli_beta/_sample_data/adversarial_attacks_on_llms.txt
+-rw-r--r--   0        0        0    35074 2024-04-26 00:38:25.040025 lango_cli_beta-0.0.1rc2/lango_cli_beta/_sample_data/diffusion_models_for_video_generation.txt
+-rw-r--r--   0        0        0    38804 2024-04-26 00:38:25.040184 lango_cli_beta-0.0.1rc2/lango_cli_beta/_sample_data/generalized_visual_language_models.txt
+-rw-r--r--   0        0        0    38842 2024-04-26 00:38:25.040341 lango_cli_beta-0.0.1rc2/lango_cli_beta/_sample_data/learning_with_not_enough_data_p_1_semi_supervised_learning.txt
+-rw-r--r--   0        0        0    31312 2024-04-26 00:38:25.040490 lango_cli_beta-0.0.1rc2/lango_cli_beta/_sample_data/learning_with_not_enough_data_p_2_active_earning.txt
+-rw-r--r--   0        0        0    38894 2024-04-26 00:38:25.040646 lango_cli_beta-0.0.1rc2/lango_cli_beta/_sample_data/learning_with_not_enough_data_p_3_data_generation.txt
+-rw-r--r--   0        0        0    46795 2024-04-26 00:38:25.040832 lango_cli_beta-0.0.1rc2/lango_cli_beta/_sample_data/llm_agents.txt
+-rw-r--r--   0        0        0    30979 2024-04-26 00:38:25.041005 lango_cli_beta-0.0.1rc2/lango_cli_beta/_sample_data/prompt_eng.txt
+-rw-r--r--   0        0        0    29209 2024-04-26 00:38:25.041155 lango_cli_beta-0.0.1rc2/lango_cli_beta/_sample_data/thinking_about_high_quality_human_data.txt
+-rw-r--r--   0        0        0     4117 2024-04-30 00:02:47.593471 lango_cli_beta-0.0.1rc2/lango_cli_beta/cli.py
+-rw-r--r--   0        0        0     2728 2024-04-26 00:38:25.041398 lango_cli_beta-0.0.1rc2/lango_cli_beta/constants.py
+-rw-r--r--   0        0        0      569 2024-04-26 00:38:25.041515 lango_cli_beta-0.0.1rc2/lango_cli_beta/namespaces/chat.py
+-rw-r--r--   0        0        0     8317 2024-04-26 00:38:25.041811 lango_cli_beta-0.0.1rc2/lango_cli_beta/namespaces/config.py
+-rw-r--r--   0        0        0      345 2024-04-26 00:38:25.041907 lango_cli_beta-0.0.1rc2/lango_cli_beta/namespaces/export.py
+-rw-r--r--   0        0        0     4446 2024-04-26 00:38:25.042043 lango_cli_beta-0.0.1rc2/lango_cli_beta/namespaces/ingest.py
+-rw-r--r--   0        0        0     2118 2024-04-26 00:38:25.042159 lango_cli_beta-0.0.1rc2/lango_cli_beta/namespaces/init.py
+-rw-r--r--   0        0        0     2763 2024-04-26 00:38:25.042267 lango_cli_beta-0.0.1rc2/lango_cli_beta/namespaces/start.py
+-rw-r--r--   0        0        0     5702 2024-04-26 00:38:25.042389 lango_cli_beta-0.0.1rc2/lango_cli_beta/namespaces/utils.py
+-rw-r--r--   0        0        0        0 2024-04-26 00:38:25.042415 lango_cli_beta-0.0.1rc2/lango_cli_beta/py.typed
+-rw-r--r--   0        0        0     3654 2024-04-26 00:38:25.042521 lango_cli_beta-0.0.1rc2/lango_cli_beta/rag/basic_chat.py
+-rw-r--r--   0        0        0      993 2024-04-26 00:38:25.042615 lango_cli_beta-0.0.1rc2/lango_cli_beta/rag/chat.py
+-rw-r--r--   0        0        0     3476 2024-04-30 00:02:47.593740 lango_cli_beta-0.0.1rc2/lango_cli_beta/rag/ingest.py
+-rw-r--r--   0        0        0     1405 2024-04-26 00:38:25.042828 lango_cli_beta-0.0.1rc2/lango_cli_beta/rag/llm_chain.py
+-rw-r--r--   0        0        0    10677 2024-04-26 00:38:25.043104 lango_cli_beta-0.0.1rc2/lango_cli_beta/rag/query_construction.py
+-rw-r--r--   0        0        0      253 2024-04-26 00:38:25.043168 lango_cli_beta-0.0.1rc2/lango_cli_beta/rag/types.py
+-rw-r--r--   0        0        0     1742 2024-04-30 00:02:47.594166 lango_cli_beta-0.0.1rc2/lango_cli_beta/rag/utils.py
+-rw-r--r--   0        0        0     3961 2024-04-26 00:38:25.043345 lango_cli_beta-0.0.1rc2/lango_cli_beta/rag_config.py
+-rw-r--r--   0        0        0     1064 2024-04-26 00:38:25.043436 lango_cli_beta-0.0.1rc2/lango_cli_beta/utils.py
+-rw-r--r--   0        0        0     2685 2024-04-30 00:03:23.224118 lango_cli_beta-0.0.1rc2/pyproject.toml
+-rw-r--r--   0        0        0    12316 1970-01-01 00:00:00.000000 lango_cli_beta-0.0.1rc2/PKG-INFO
```

### Comparing `lango_cli_beta-0.0.1rc1/LICENSE` & `lango_cli_beta-0.0.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `lango_cli_beta-0.0.1rc1/README.md` & `lango_cli_beta-0.0.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/_sample_data/adversarial_attacks_on_llms.txt` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/_sample_data/adversarial_attacks_on_llms.txt`

 * *Files identical despite different names*

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/_sample_data/diffusion_models_for_video_generation.txt` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/_sample_data/diffusion_models_for_video_generation.txt`

 * *Files identical despite different names*

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/_sample_data/generalized_visual_language_models.txt` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/_sample_data/generalized_visual_language_models.txt`

 * *Files identical despite different names*

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/_sample_data/learning_with_not_enough_data_p_1_semi_supervised_learning.txt` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/_sample_data/learning_with_not_enough_data_p_1_semi_supervised_learning.txt`

 * *Files identical despite different names*

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/_sample_data/learning_with_not_enough_data_p_2_active_earning.txt` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/_sample_data/learning_with_not_enough_data_p_2_active_earning.txt`

 * *Files identical despite different names*

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/_sample_data/learning_with_not_enough_data_p_3_data_generation.txt` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/_sample_data/learning_with_not_enough_data_p_3_data_generation.txt`

 * *Files identical despite different names*

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/_sample_data/llm_agents.txt` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/_sample_data/llm_agents.txt`

 * *Files identical despite different names*

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/_sample_data/prompt_eng.txt` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/_sample_data/prompt_eng.txt`

 * *Files identical despite different names*

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/_sample_data/thinking_about_high_quality_human_data.txt` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/_sample_data/thinking_about_high_quality_human_data.txt`

 * *Files identical despite different names*

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/cli.py` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # File containing logic for CLI
-from typing import Optional
+from typing import Literal, Optional, cast
 
 import typer
 from dotenv import load_dotenv
 
 from lango_cli_beta.constants import CLI_INVOKE_NAME
 from lango_cli_beta.namespaces.chat import chat_cli
 from lango_cli_beta.namespaces.config import _get_llm_prompt, config_cli
@@ -34,48 +34,61 @@
         False,
         "--version",
         "-v",
         help="Print the current CLI version.",
         callback=version_callback,
         is_eager=True,
     ),
-):
+) -> None:
     pass
 
 
 @app.command()
 def config(
     fast: Optional[bool] = typer.Option(
         False, help="Pass this flag to skip the interactive prompts."
     ),
     data_path: Optional[str] = typer.Option(
         None, help="The path to the data folder or file to ingest."
     ),
-    rag_type: Optional[str] = typer.Option(
+    rag_type: str = typer.Option(
         "basic",
         help="The type of RAG to create. Options: 'basic', 'query_construction'",
     ),
-    llm: Optional[str] = typer.Option(
-        "1", help=f"The LLM to use. Options: {_get_llm_prompt()}"
-    ),
+    llm: str = typer.Option("1", help=f"The LLM to use. Options: {_get_llm_prompt()}"),
     metadata: Optional[str] = typer.Option(
         None,
         help="The path to the metadata JSON file, or a JSON string.",
     ),
     json_schema: Optional[str] = typer.Option(
         None,
         help="Valid JSONSchema to be used in query construction. Either a path to a .json file, or a stringified version. All fields should be optional. Required if using 'query_construction' RAG.",
     ),
-    chunk_size: Optional[int] = typer.Option(
+    chunk_size: int = typer.Option(
         500, help="The size of the chunks to split the data into."
     ),
-    chunk_overlap: Optional[int] = typer.Option(75, help="The overlap between chunks."),
-):
+    chunk_overlap: int = typer.Option(75, help="The overlap between chunks."),
+) -> None:
+    if rag_type not in ["basic", "query_construction"]:
+        raise ValueError(
+            f"Invalid rag_type received: {rag_type}. Must be "
+            "'basic' or 'query_construction'."
+        )
+    _rag_type: Literal["basic", "query_construction"] = cast(
+        Literal["basic", "query_construction"], rag_type
+    )
     config_cli(
-        fast, data_path, rag_type, llm, metadata, json_schema, chunk_size, chunk_overlap
+        fast,
+        data_path,
+        _rag_type,
+        llm,
+        metadata,
+        json_schema,
+        chunk_size,
+        chunk_overlap,
     )
 
 
 @app.command()
 def upsert(
     fast: Optional[bool] = typer.Option(
         False, help="Pass this flag to skip the interactive prompts."
@@ -87,43 +100,43 @@
         None,
         help="The path to the metadata JSON file, or a JSON string.",
     ),
     json_schema: Optional[str] = typer.Option(
         None,
         help="Valid JSONSchema to be used in query construction. Either a path to a .json file, or a stringified version. All fields should be optional. Required if using 'query_construction' RAG.",
     ),
-    chunk_size: Optional[int] = typer.Option(
+    chunk_size: int = typer.Option(
         500, help="The size of the chunks to split the data into."
     ),
-    chunk_overlap: Optional[int] = typer.Option(75, help="The overlap between chunks."),
-):
+    chunk_overlap: int = typer.Option(75, help="The overlap between chunks."),
+) -> None:
     upsert_cli(fast, data_path, metadata, json_schema, chunk_size, chunk_overlap)
 
 
 @app.command()
-def chat():
+def chat() -> None:
     chat_cli()
 
 
 @app.command()
-def start():
+def start() -> None:
     start_cli()
 
 
 @app.command()
-def export():
+def export() -> None:
     export_cli()
 
 
 @app.command()
 def init(
     project_name: str = typer.Argument(..., help="Name of the project"),
     no_sample_data: Optional[bool] = typer.Option(
         None,
         help="Pass this flag to skip copying the sample data folder.",
     ),
-):
+) -> None:
     init_cli(project_name, no_sample_data)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/constants.py` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "json_schema": BASE_JSON_SCHEMA,
 }
 
 DEFAULT_CONFIG_FILE_NAME = "lango_cli.config.json"
 
 SAMPLE_DATA_FOLDER_NAME = "_sample_data"
 
-DEFAULT_CONFIG_PATH = Path.cwd() / DEFAULT_CONFIG_FILE_NAME
+DEFAULT_CONFIG_PATH = str(Path.cwd() / DEFAULT_CONFIG_FILE_NAME)
 
 JSON_SCHEMA_REQUIRED_MESSAGE = "JSONSchema is required for query construction. Please provide a valid JSON file path, or stringified JSON."
 
 # Script to get the container's IP address and start the lango-cli server.
 # This script is used in the Dockerfile for the `lango-cli export` command.
 GET_IP_AND_START_SCRIPT = """
 #!/bin/bash
```

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/namespaces/chat.py` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/namespaces/chat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """
 CLI commands
 """
 
-import typer
 from rich import print as rich_print
 
 from lango_cli_beta.constants import DEFAULT_CONFIG_PATH
 from lango_cli_beta.rag.chat import Chat
 from lango_cli_beta.rag_config import RagConfig
 
 
-def chat_cli():
+def chat_cli() -> None:
     rich_print(
         "[bold]Welcome to the [#d3e0e0]Lang[/#d3e0e0][#beb4fd]Chain[/#beb4fd] [#00ed64]MongoDB[/#00ed64] RAG CLI.[/bold]\n\n"
         + "[bold]Let's start [italic]chatting[/italic].[/bold]\n\n"
     )
     user_config = RagConfig(path_or_config=DEFAULT_CONFIG_PATH)
-    chat = Chat(config=user_config, typer=typer)
+    chat = Chat(config=user_config)
     chat.chat_loop()
```

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/namespaces/config.py` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/namespaces/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 CLI commands
 """
 
-from typing import Optional, Union
+from typing import Dict, List, Literal, Optional
 
 import typer
 from rich import print as rich_print
 from rich.prompt import Confirm as RichConfirm
 from rich.prompt import Prompt as RichPrompt
 
 from lango_cli_beta.constants import (
@@ -25,15 +25,15 @@
 
 DEFAULT_CONFIG = {
     "rag_type": "basic",
     "llm": "anthropic",
     "chunk_size": 500,
     "chunk_overlap": 75,
 }
-RAG_CANDIDATE_OPTIONS = [
+RAG_CANDIDATE_OPTIONS: List[Dict] = [
     {
         "name": "Basic RAG",
         "value": "basic",
     },
     {
         "name": "Query Construction RAG",
         "value": "query_construction",
@@ -63,19 +63,17 @@
     {
         "name": "Mixtral-8x7b",
         "value": "fireworks_mixtral_8x7b",
     },
 ]
 
 
-def get_llm(typer: typer) -> dict:
+def get_llm() -> dict:
     """Prompts the user for the LLM to use.
 
-    Args:
-        typer (typer): The typer instance to use for prompting.
     Returns:
         str: The LLM to use.
     """
 
     llm_options_prompt = "\n".join(
         f"  [bold][{i}]: {option['name']}[/bold]"
         for i, option in enumerate(LLM_OPTIONS, start=1)
@@ -86,27 +84,25 @@
     selected_llm = LLM_OPTIONS[int(llm_choice.strip()) - 1]
     rich_print(f"Selected LLM: [bold]{selected_llm['name']}[/bold]")
     typer.echo("\n")
     return selected_llm
 
 
 def process_fast_entry(
-    typer: typer,
-    rag_type: str = "",
-    llm: str = "",
-    ingest_data_path: Union[str, None] = None,
-    metadata: Union[str, None] = None,
-    chunk_size: int = 500,
-    chunk_overlap: int = 75,
-    json_schema: Optional[str] = None,
+    rag_type: Literal["basic", "query_construction"],
+    llm: str,
+    ingest_data_path: Optional[str],
+    metadata: Optional[str],
+    chunk_size: int,
+    chunk_overlap: int,
+    json_schema: Optional[str],
 ) -> None:
     """Processes the user's fast entry, skipping the interactive prompts.
 
     Args:
-        typer (typer): The typer instance to use for prompting.
         rag_type (str): The RAG type.
         llm (str): The LLM to use.
         ingest_data_path (str): The path to the data file, or folder with files to ingest.
         metadata (Union[str, None]): The path to the metadata JSON file, or a JSON string.
         chunk_size (int): The size of the chunks to split the data into.
         chunk_overlap (int): The overlap between chunks.
     Returns: None
@@ -139,28 +135,28 @@
     if json_schema is not None and _is_json_str_or_file(json_schema) is False:
         typer.echo(
             "Invalid metadata input. Please provide either a .json file, or a JSON string."
         )
         raise typer.Exit(1)
 
     # Parse the metadata/JSONSchema JSON string, or read the JSON file if provided
-    if metadata is not None:
-        metadata = _load_json(metadata)
-    if json_schema is not None:
-        json_schema = _load_json(json_schema)
+
+    metadata_dict = _load_json(metadata) if metadata is not None else None
+
+    json_schema_dict = _load_json(json_schema) if json_schema is not None else None
 
     user_config = RagConfig(
         path_or_config={
             "rag_type": rag_type,
             "llm": LLM_OPTIONS[int(llm)]["value"],
             "ingest_path": ingest_data_path,
-            "metadata": metadata,
+            "metadata": metadata_dict,
             "chunk_size": chunk_size,
             "chunk_overlap": chunk_overlap,
-            "json_schema": json_schema,
+            "json_schema": json_schema_dict,
         }
     )
     user_config.save_config(DEFAULT_CONFIG_PATH)
 
     # Ingest data from file/folder
     ingest = Ingester(user_config)
     ingest.ingest_data()
@@ -179,38 +175,35 @@
 def config_cli(
     fast: Optional[bool] = typer.Option(
         False, help="Pass this flag to skip the interactive prompts."
     ),
     data_path: Optional[str] = typer.Option(
         None, help="The path to the data folder or file to ingest."
     ),
-    rag_type: Optional[str] = typer.Option(
+    rag_type: Literal["basic", "query_construction"] = typer.Option(
         "basic",
         help="The type of RAG to create. Options: 'basic', 'query_construction'",
     ),
-    llm: Optional[str] = typer.Option(
-        "1", help=f"The LLM to use. Options: {_get_llm_prompt()}"
-    ),
+    llm: str = typer.Option("1", help=f"The LLM to use. Options: {_get_llm_prompt()}"),
     metadata: Optional[str] = typer.Option(
         None,
         help="The path to the metadata JSON file, or a JSON string.",
     ),
     json_schema: Optional[str] = typer.Option(
         None,
         help="Valid JSONSchema to be used in query construction. Either a path to a .json file, or a stringified version. All fields should be optional. Required if using 'query_construction' RAG.",
     ),
-    chunk_size: Optional[int] = typer.Option(
+    chunk_size: int = typer.Option(
         500, help="The size of the chunks to split the data into."
     ),
-    chunk_overlap: Optional[int] = typer.Option(75, help="The overlap between chunks."),
-):
+    chunk_overlap: int = typer.Option(75, help="The overlap between chunks."),
+) -> None:
     if fast:
         # Skip interactive prompt, use provided values
         process_fast_entry(
-            typer,
             ingest_data_path=data_path,
             rag_type=rag_type,
             llm=llm,
             metadata=metadata,
             chunk_size=chunk_size,
             chunk_overlap=chunk_overlap,
             json_schema=json_schema,
@@ -240,24 +233,24 @@
     # Print the user selection
     rich_print(
         f"Using: [bold]{RAG_CANDIDATE_OPTIONS[int_candidate_choice]['name']}[bold]"
     )
     typer.echo("\n")
 
     # Query Construction RAG selected, prompt for LLM
-    user_config.llm = get_llm(typer)["value"]
+    user_config.llm = get_llm()["value"]
 
     # Save config before ingesting data
     user_config.save_config(DEFAULT_CONFIG_PATH)
 
     # Ingest data now, or later
     ingest_now = RichConfirm.ask("Do you want to ingest the data now?")
     if ingest_now:
         typer.echo("\n")
-        user_config = ingest_data(typer, user_config)
+        user_config = ingest_data(user_config)
     else:
         rich_print(
             f"""Data can be ingested later via "[bold #00FF00]{CLI_INVOKE_NAME} upsert[/bold #00FF00]".\n"""
         )
     # Save the config file
     user_config.save_config(DEFAULT_CONFIG_PATH)
     rich_print(
```

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/namespaces/ingest.py` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/namespaces/ingest.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,26 +18,24 @@
     ingest_data,
 )
 from lango_cli_beta.rag.ingest import Ingester
 from lango_cli_beta.rag_config import RagConfig
 
 
 def process_fast_entry(
-    typer: typer,
-    ingest_data_path: Union[str, None] = None,
-    metadata: Union[str, None] = None,
-    chunk_size: int = 500,
-    chunk_overlap: int = 75,
-    user_config: RagConfig = None,
-    json_schema: Optional[str] = None,
+    ingest_data_path: Union[str, None],
+    metadata: Union[str, None],
+    chunk_size: int,
+    chunk_overlap: int,
+    user_config: RagConfig,
+    json_schema: Optional[str],
 ) -> None:
     """Processes the user's fast entry, skipping the interacive prompts.
 
     Args:
-        typer (typer): The typer instance to use for prompting.
         ingest_data_path (str): The path to the data file, or folder with files to ingest.
         metadata (Union[str, None]): The path to the metadata JSON file, or a JSON string.
         chunk_size (int): The size of the chunks to split the data into.
         chunk_overlap (int): The overlap between chunks.
     Returns: None
     """
 
@@ -63,24 +61,22 @@
     if json_schema is not None and _is_json_str_or_file(json_schema) is False:
         typer.echo(
             "Invalid JSONSchema input. Please provide a valid JSON file path, or stringified JSON."
         )
         raise typer.Exit(1)
 
     # Parse the metadata JSON string, or read the JSON file if provided
-    if metadata is not None:
-        metadata = _load_json(metadata)
-    if json_schema is not None:
-        json_schema = _load_json(json_schema)
+    metadata_dict = _load_json(metadata) if metadata is not None else None
+    json_schema_dict = _load_json(json_schema) if json_schema is not None else None
 
     user_config.ingest_path = ingest_data_path
-    user_config.metadata = metadata
+    user_config.metadata = metadata_dict
     user_config.chunk_size = int(chunk_size)
     user_config.chunk_overlap = int(chunk_overlap)
-    user_config.json_schema = json_schema
+    user_config.json_schema = json_schema_dict
 
     user_config.save_config(DEFAULT_CONFIG_PATH)
 
     rich_print("[bold #00FF00]Ingesting data now.[/bold #00FF00]")
     ingest = Ingester(user_config)
     ingest.ingest_data()
 
@@ -96,25 +92,24 @@
         None,
         help="The path to the metadata JSON file, or a JSON string.",
     ),
     json_schema: Optional[str] = typer.Option(
         None,
         help="Valid JSONSchema to be used in query construction. Either a path to a .json file, or a stringified version. All fields should be optional. Required if using 'query_construction' RAG.",
     ),
-    chunk_size: Optional[int] = typer.Option(
+    chunk_size: int = typer.Option(
         500, help="The size of the chunks to split the data into."
     ),
-    chunk_overlap: Optional[int] = typer.Option(75, help="The overlap between chunks."),
-):
+    chunk_overlap: int = typer.Option(75, help="The overlap between chunks."),
+) -> None:
     user_config = RagConfig(path_or_config=DEFAULT_CONFIG_PATH)
 
     if fast:
         # Skip interactive prompt, use provided values
         process_fast_entry(
-            typer,
             ingest_data_path=data_path,
             metadata=metadata,
             chunk_size=chunk_size,
             chunk_overlap=chunk_overlap,
             user_config=user_config,
             json_schema=json_schema,
         )
@@ -122,13 +117,13 @@
 
     rich_print(
         "[bold]Welcome to the [#d3e0e0]Lang[/#d3e0e0][#beb4fd]Chain[/#beb4fd] [#00ed64]MongoDB[/#00ed64] RAG CLI.[/bold]\n\n"
         + "[bold]Let's start [italic]indexing[/italic].[/bold]\n\n"
     )
 
     # Ingester data now, or later
-    user_config = ingest_data(typer, user_config)
+    user_config = ingest_data(user_config)
     # Save the config file
     user_config.save_config(DEFAULT_CONFIG_PATH)
     rich_print(
         f"[bold #0af2b0]Successfully created new RAG config.[/bold #0af2b0]\nSaved to [italic]{DEFAULT_CONFIG_PATH}[/italic]"
     )
```

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/namespaces/init.py` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/namespaces/init.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 def init_cli(
     project_name: str,
     no_sample_data: Optional[bool] = typer.Option(
         None,
         help="Pass this flag to skip copying the sample data folder.",
     ),
-):
+) -> None:
     # strip all non-alphanumeric characters from the project name, and make lowercase
     clean_project_name = "".join(e for e in project_name if e.isalnum()).lower()
     # Create a new directory with the project name
     project_dir = Path(clean_project_name)
     project_dir.mkdir(exist_ok=False)
 
     # write a new config file with the default RAG config
```

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/namespaces/start.py` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/namespaces/start.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 CLI commands
 """
 
 import uvicorn
-from fastapi import FastAPI
+from fastapi import FastAPI  # type: ignore
 from langchain_core.messages import HumanMessage
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.runnables import Runnable, RunnableLambda, RunnablePassthrough
 from langserve import add_routes
 
 from lango_cli_beta.constants import (
     DEFAULT_CONFIG_PATH,
@@ -21,16 +21,16 @@
     construct_query_construction_graph,
 )
 from lango_cli_beta.rag.types import ChatInputType
 from lango_cli_beta.rag.utils import _get_llm
 from lango_cli_beta.rag_config import RagConfig
 
 
-def construct_basic_rag_runnable(llm: str) -> Runnable[ChatInputType, str]:
-    llm = _get_llm(llm)
+def construct_basic_rag_runnable(llm_str: str) -> Runnable[ChatInputType, str]:
+    llm = _get_llm(llm_str)
     basic_retrieval_chain = simple_chat_retrieval()
     llm_chain = construct_llm_chain(llm, SYSTEM_MESSAGE)
     chat_chain = basic_retrieval_chain | llm_chain
     return chat_chain.with_types(input_type=ChatInputType)
 
 
 def construct_query_construction_runnable(
@@ -61,20 +61,20 @@
 
 
 def create_runnable(rag_config: RagConfig) -> Runnable[ChatInputType, str]:
     rag_type = rag_config.rag_type
     llm = rag_config.llm
     json_schema = rag_config.json_schema
     if rag_type == "query_construction":
-        return construct_query_construction_runnable(llm, json_schema)
+        return construct_query_construction_runnable(llm, json_schema or {})
     else:
         return construct_basic_rag_runnable(llm)
 
 
-def start_cli():
+def start_cli() -> None:
     user_config = RagConfig(path_or_config=DEFAULT_CONFIG_PATH)
     app = FastAPI(
         title="LangChain Server",
         version="1.0",
         description="A simple api server using Langchain's Runnable interfaces",
     )
```

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/namespaces/utils.py` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/namespaces/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import os
-from typing import Literal
+from typing import Any, Dict, Literal
 
 import typer
 from rich import print as rich_print
 from rich.prompt import Prompt as RichPrompt
 
 from lango_cli_beta.rag.ingest import Ingester
 from lango_cli_beta.rag_config import RagConfig
@@ -13,14 +13,15 @@
 def _is_only_txt_files(path: str) -> bool:
     """Whether or not a given file is .txt, or all files in a folder
     are .txt files."""
     if os.path.isfile(path):
         return path.endswith(".txt")
     elif os.path.isdir(path):
         return all(file.endswith(".txt") for file in os.listdir(path))
+    raise ValueError("Invalid path - must be a file or directory.")
 
 
 def _is_json_str_or_file(path: str) -> bool:
     """Whether or not a given file is a .json file, or a JSON string."""
     if path.endswith(".json"):
         return True
     try:
@@ -41,15 +42,15 @@
         with open(metadata_or_path, "r") as f:
             metadata = json.load(f)
     else:
         metadata = json.loads(metadata_or_path)
     return metadata
 
 
-def get_chunking_data(typer: typer) -> dict:
+def get_chunking_data() -> dict:
     chunk_size = RichPrompt.ask(
         "What chunk size do you want to use?\nPress enter to use the default [bold #d5b6f0][500][/bold #d5b6f0]",
         default=500,
     )
     rich_print(f"Selected chunk size: [bold]{chunk_size}[/bold]")
     typer.echo("\n")
     chunk_overlap = RichPrompt.ask(
@@ -61,37 +62,34 @@
     return {
         "chunk_size": int(chunk_size),
         "chunk_overlap": int(chunk_overlap),
     }
 
 
 def recursive_verify_or_prompt_json(
-    typer: typer, json_or_path: str, is_metadata: bool = None
-) -> str:
+    json_or_path: str, is_metadata: bool = False
+) -> Dict[str, Any]:
     prompt_str = "metadata" if is_metadata else "JSONSchema"
     is_valid = _is_json_str_or_file(json_or_path)
 
     if is_valid is False:
         json_or_path = typer.prompt(
             f"Invalid file type(s)/{prompt_str} string.\nPlease enter either the path to the .json file containing {prompt_str}, or valid stringified JSON with {prompt_str}",
             default=None,
         )
-        return recursive_verify_or_prompt_json(typer, json_or_path)
+        return recursive_verify_or_prompt_json(json_or_path)
     else:
         return _load_json(json_or_path)
 
 
-def get_ingest_path_and_json(
-    typer: typer, rag_type: Literal["basic", "query_construction"]
-) -> dict:
+def get_ingest_path_and_json(rag_type: Literal["basic", "query_construction"]) -> dict:
     """Prompts the user for the path to the data file they want to ingest,
     along with any metadata and JSONSchema, if required.
 
     Args:
-        typer (typer): The typer instance to use for prompting.
         rag_type (Literal["basic", "query_construction"]): The RAG type.
     Returns:
         dict: A dictionary containing the ingest path, metadata and JSONSchema.
     """
 
     ingest_data_path = typer.prompt(
         "Enter the path to the data file, or folder you want to ingest"
@@ -115,56 +113,53 @@
         "Enter either the path to the .json file containing metadata, or valid stringified JSON with metadata. (optional)",
         default="",
     )
     metadata_or_path = None if metadata_or_path == "" else metadata_or_path
     # Pre-instantiate metadata variable
     metadata = None
     if metadata_or_path is not None:
-        metadata = recursive_verify_or_prompt_json(
-            typer, metadata_or_path, is_metadata=True
-        )
+        metadata = recursive_verify_or_prompt_json(metadata_or_path, is_metadata=True)
 
     typer.echo("\n")
 
     # Pre-instantiate JSONSchema variable
     json_schema = None
     if rag_type == "query_construction" and metadata is not None:
         # Only request JSONSchema if metadata is provided, and RAG type is query_construction
         json_schema_or_path = typer.prompt(
             "Enter either the path to the .json file containing JSONSchema, or valid stringified JSON with JSONSchema. (required)",
         )
         json_schema = recursive_verify_or_prompt_json(
-            typer, json_schema_or_path, is_metadata=False
+            json_schema_or_path, is_metadata=False
         )
 
         typer.echo("\n")
 
     return {
         "ingest_data_path": ingest_data_path,
         "metadata": metadata,
         "json_schema": json_schema,
     }
 
 
-def ingest_data(typer: typer, user_config: RagConfig) -> RagConfig:
+def ingest_data(user_config: RagConfig) -> RagConfig:
     """Ingests data into the MongoDB vector store.
 
     Args:
-        typer (typer): The typer instance to use for prompting.
         user_config (dict): The user's configuration.
     Returns:
         dict: The updated user configuration.
     """
 
     # Optionally prompt for chunking data
-    chunking_data = get_chunking_data(typer)
+    chunking_data = get_chunking_data()
     user_config.chunk_size = int(chunking_data["chunk_size"])
     user_config.chunk_overlap = int(chunking_data["chunk_overlap"])
     # Prompt for the path to the data file
-    ingest_and_json = get_ingest_path_and_json(typer, user_config.rag_type)
+    ingest_and_json = get_ingest_path_and_json(user_config.rag_type)
     user_config.ingest_path = ingest_and_json["ingest_data_path"]
     user_config.metadata = ingest_and_json["metadata"]
     user_config.json_schema = ingest_and_json["json_schema"]
 
     rich_print("[bold #00FF00]Ingesting data now.[/bold #00FF00]")
     ingest = Ingester(user_config)
     ingest.ingest_data()
```

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/rag/basic_chat.py` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/rag/basic_chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Class containing logic for the chat interface"""
 
-from typing import List, Union
+from typing import Any, Dict, List, Union
 
-import typer as TyperType
+import typer
 from langchain_core.documents import Document
 from langchain_core.messages import AIMessage, HumanMessage, SystemMessage
 from langchain_core.runnables import (
     Runnable,
     RunnableLambda,
     RunnablePassthrough,
 )
@@ -39,71 +39,66 @@
 
 def documents_to_str(docs: List[Document]) -> str:
     """Convert a list of documents into a single string."""
 
     return "\n".join([doc.page_content for doc in docs])
 
 
-def clean_and_retrieve_docs(x):
+def clean_and_retrieve_docs(x: Dict[str, Any]) -> List[Document]:
     vectorstore = initialize_vectorstore()
     retriever = vectorstore.as_retriever(search_kwargs={"k": 6})
     input_human_message = x["input"][-1]
     return _clean_mongo_docs(retriever.invoke(input_human_message.content))
 
 
-def simple_chat_retrieval() -> Runnable[ChatInputType, str]:
+def simple_chat_retrieval() -> Runnable:
     chain = RunnablePassthrough.assign(
         documents=RunnableLambda(lambda x: clean_and_retrieve_docs(x)).with_config(
             config={"run_name": "retrieve_and_clean"}
         )
     ).with_config(config={"run_name": "assign_documents"}) | RunnablePassthrough.assign(
         context=RunnableLambda(lambda x: documents_to_str(x["documents"])).with_config(
             config={"run_name": "documents_to_str"}
         )
     ).with_config(config={"run_name": "assign_context_passthrough"})
     return chain
 
 
 class BasicChat:
-    typer: TyperType
-
     chat_chain: Runnable
 
     def __init__(
         self,
-        config: RagConfig = None,
-        typer: TyperType = None,
+        config: RagConfig,
     ) -> None:
-        self.typer = typer
-
         llm = _get_llm(config.llm)
         basic_retrieval_chain = simple_chat_retrieval()
         llm_chain = construct_llm_chain(llm, SYSTEM_MESSAGE)
 
         self.chat_chain = basic_retrieval_chain | llm_chain
 
-    def chat_loop(self):
+    def chat_loop(self) -> None:
         first_iter = True
         history: List[Union[HumanMessage, AIMessage, SystemMessage]] = []
 
         while True:
             prompt_message = (
                 "Start chatting here.\nType 'exit' to quit.\n[bold #fce8fc]Human[/bold #fce8fc]"
                 if first_iter
                 else "\n\n[bold]Human[/bold]"
             )
             if first_iter:
                 first_iter = False
 
             input = RichPrompt.ask(prompt_message)
-            self.typer.echo("\n")
+            typer.echo("\n")
 
             if input == "exit":
-                self.typer.echo("Aborting chat.")
-                raise self.typer.Exit(0)
+                typer.echo("Aborting chat.")
+                raise typer.Exit(0)
             history.append(HumanMessage(content=input))
 
             final_message = ""
             first_chunk = False
             for message in self.chat_chain.stream({"input": history}):
                 if first_chunk is False:
                     first_chunk = True
```

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/rag/chat.py` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/rag/chat.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 """Class containing logic for the chat interface"""
 
 from typing import Union
 
-import typer as TyperType
-
 from lango_cli_beta.rag.basic_chat import BasicChat
 from lango_cli_beta.rag.query_construction import QueryConstruction
 from lango_cli_beta.rag_config import RagConfig
 
 
 class Chat:
     config: RagConfig
 
-    typer: TyperType
-
     basic_chat_chain: Union[BasicChat, None] = None
 
     query_construction: Union[QueryConstruction, None] = None
 
     def __init__(
         self,
-        config: RagConfig = None,
-        typer: TyperType = None,
+        config: RagConfig,
     ) -> None:
         self.config = config
-        self.typer = typer
 
         if config.rag_type == "query_construction":
-            self.query_construction = QueryConstruction(config=config, typer=typer)
+            self.query_construction = QueryConstruction(config=config)
         else:
-            self.basic_chat_chain = BasicChat(config=config, typer=typer)
+            self.basic_chat_chain = BasicChat(config=config)
 
-    def chat_loop(self):
+    def chat_loop(self) -> None:
         if self.query_construction is not None:
             self.query_construction.chat_loop()
         elif self.basic_chat_chain is not None:
             self.basic_chat_chain.chat_loop()
         else:
             raise ValueError("No chat chain found.")
```

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/rag/llm_chain.py` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/rag/llm_chain.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,8 +35,8 @@
         RunnablePassthrough.assign(
             messages=lambda x: format_messages(x["input"], x["context"])
         )
         | prompt
         | llm
         | StrOutputParser()
     )
-    return chain.with_config(config={"run_name": "llm_chain"})
+    return chain.with_config(config={"run_name": "llm_chain"})  # type: ignore
```

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/rag/query_construction.py` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/rag/query_construction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Class containing logic for the chat interface"""
 
-from typing import List, Optional, Union
+from typing import Any, Dict, List, Union
 
-import typer as TyperType
+import typer
 from langchain_cohere import CohereRerank
 from langchain_core.documents import Document
 from langchain_core.language_models import BaseChatModel
 from langchain_core.messages import AIMessage, HumanMessage, SystemMessage
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.runnables import Runnable, RunnableConfig
@@ -21,15 +21,15 @@
 from lango_cli_beta.rag.llm_chain import construct_llm_chain
 from lango_cli_beta.rag.utils import _clean_mongo_docs, _get_llm
 from lango_cli_beta.rag_config import RagConfig
 from lango_cli_beta.utils import initialize_vectorstore
 
 
 class QueryConstructionState(TypedDict):
-    input: HumanMessage
+    input: str
     """The input from the user"""
     json_schema: dict
     # """The JSON schema for the structured output. Provided by the RagConfig"""
     llm: BaseChatModel
     # llm: str1
     """The language model to use"""
     documents: Union[list[Document], None]
@@ -38,30 +38,33 @@
     """Stringified documents"""
     filters: Union[dict, None]
     """Filters extracted from the input"""
     system_message: SystemMessage
     """The system message to use for the final generation"""
 
 
-def graph_documents_to_str(state: QueryConstructionState) -> str:
+def graph_documents_to_str(state: QueryConstructionState) -> Dict[str, str]:
     """Convert a list of documents into a single string."""
 
     docs = state["documents"]
-    context = "\n".join([doc.page_content for doc in docs])
+    context = "\n".join([doc.page_content for doc in docs]) if docs else ""
     return {"context": context}
 
 
-def rerank_docs(state: QueryConstructionState):
+def rerank_docs(state: QueryConstructionState) -> Dict[str, List[Document]]:
     """Rerank a list of documents using Cohere's 'rerank-english-v3.0'."""
     docs = state["documents"]
-    rephrased_query = state["input"]
-    reranker = CohereRerank(model="rerank-english-v3.0")
-
-    reranked_docs_output = reranker.rerank(docs, rephrased_query, top_n=10)
-    reranked_docs = [docs[doc["index"]] for doc in reranked_docs_output]
+    if docs:
+        rephrased_query = state["input"]
+        reranker = CohereRerank(model="rerank-english-v3.0")
+
+        reranked_docs_output = reranker.rerank(docs, rephrased_query, top_n=10)
+        reranked_docs = [docs[doc["index"]] for doc in reranked_docs_output]
+    else:
+        reranked_docs = []
 
     return {"documents": reranked_docs}
 
 
 def _convert_openai_filters_to_mongo(filters: Union[dict, None]) -> Union[dict, None]:
     """
     Converts filters returned from an OpenAI function call into filters MongoDB can accept.
@@ -79,16 +82,16 @@
     for key, value in filters.items():
         mongo_filters[key] = {"$eq": value}
 
     return mongo_filters
 
 
 def extract_filters_chain(
-    state: QueryConstructionState, config: Optional[RunnableConfig]
-):
+    state: QueryConstructionState, config: RunnableConfig
+) -> dict:
     llm: BaseChatModel = config["configurable"]["llm"]
     json_schema = state["json_schema"]
     model_with_tools = llm.with_structured_output(json_schema)
     prompt = ChatPromptTemplate.from_messages(
         [
             (
                 "system",
@@ -103,15 +106,15 @@
     extract_filters_chain = prompt | model_with_tools
     filters = extract_filters_chain.invoke({"input": state["input"]})
     return {
         "filters": filters,
     }
 
 
-def retrieve_docs(state: QueryConstructionState):
+def retrieve_docs(state: QueryConstructionState) -> dict:
     vectorstore = initialize_vectorstore()
     input = state["input"]
     filters = state["filters"]
 
     retriever = vectorstore.as_retriever(
         search_kwargs={
             "k": 30,
@@ -120,17 +123,15 @@
     )
     documents = retriever.invoke(input)
     # Remove the _id field inserted by MongoDB from the metadata
     cleaned_documents = _clean_mongo_docs(documents)
     return {"documents": cleaned_documents}
 
 
-def rephrase_query_chain(
-    state: QueryConstructionState, config: Optional[RunnableConfig]
-):
+def rephrase_query_chain(state: QueryConstructionState, config: RunnableConfig) -> dict:
     """Given an original query and any filters which are applied to the
     retrieval step, rephrase the query to not include any mention of the filters."""
     prompt = ChatPromptTemplate.from_messages(
         [
             (
                 "system",
                 "You are an advanced question asker.\n"
@@ -156,16 +157,16 @@
 
 def retrieve_or_rephrase_conditional(state: QueryConstructionState) -> str:
     if state["filters"] is not None:
         return "rephrase_query"
     return "retrieval"
 
 
-def construct_query_construction_graph():
-    workflow = StateGraph(QueryConstructionState)
+def construct_query_construction_graph() -> CompiledGraph:
+    workflow: Any = StateGraph(QueryConstructionState)
 
     workflow.add_node("extract_filters", extract_filters_chain)
     workflow.add_node("retrieval", retrieve_docs)
     workflow.add_node("rephrase_query", rephrase_query_chain)
 
     workflow.add_conditional_edges("extract_filters", retrieve_or_rephrase_conditional)
     workflow.add_edge("rephrase_query", "retrieval")
@@ -193,14 +194,15 @@
         docs_len = len(output["retrieval"]["documents"])
         return f"[bold]Step: [#ff6e5e]Retrieved Documents[/#ff6e5e][/bold]\n[bold #fcd63a]Num docs:[/bold #fcd63a] {docs_len}\n"
     if "rerank_docs" in output:
         docs_len = len(output["rerank_docs"]["documents"])
         return f"[bold]Step: [#ff6e5e]Reranked Documents[/#ff6e5e][/bold]\n[bold #fcd63a]Num docs:[/bold #fcd63a] {docs_len}\n"
     if "docs_to_str" in output:
         return "[bold]Step: [#ff6e5e]Convert Docs to String[/#ff6e5e][/bold]\n"
+    return ""
 
 
 def update_final_graph_output(output: dict, final_graph_output: dict) -> dict:
     if "rephrase_query" in output:
         final_graph_output["input"] = [
             HumanMessage(content=output["rephrase_query"]["input"])
         ]
@@ -208,56 +210,52 @@
         final_graph_output["context"] = output["docs_to_str"]["context"]
     return final_graph_output
 
 
 class QueryConstruction:
     config: RagConfig
 
-    typer: TyperType
-
     query_construction_graph: CompiledGraph
 
     llm_chain: Runnable
 
     llm: BaseChatModel
 
     vectorstore: MongoDBAtlasVectorSearch
 
     def __init__(
         self,
-        config: RagConfig = None,
-        typer: TyperType = None,
+        config: RagConfig,
     ) -> None:
         self.config = config
-        self.typer = typer
 
         self.vectorstore = initialize_vectorstore()
         self.llm = _get_llm(config.llm)
         self.query_construction_graph = construct_query_construction_graph()
         self.llm_chain = construct_llm_chain(self.llm, SYSTEM_MESSAGE)
 
-    def chat_loop(self):
+    def chat_loop(self) -> None:
         first_iter = True
         history: List[Union[HumanMessage, AIMessage, SystemMessage]] = []
 
         while True:
             prompt_message = (
                 "Start chatting here.\nType 'exit' to quit.\n[bold #fce8fc]Human[/bold #fce8fc]"
                 if first_iter
                 else "\n\n[bold]Human[/bold]"
             )
             if first_iter:
                 first_iter = False
 
             input = RichPrompt.ask(prompt_message)
-            self.typer.echo("\n")
+            typer.echo("\n")
 
             if input == "exit":
-                self.typer.echo("Aborting chat.")
-                raise self.typer.Exit(0)
+                typer.echo("Aborting chat.")
+                raise typer.Exit(0)
             input_human_message = HumanMessage(content=input)
 
             final_message = ""
             final_graph_output = {
                 "history": history,
                 "input": [input_human_message],
                 "context": "",
@@ -283,8 +281,8 @@
                 rich_print(stream_item, end="")
 
             # Update the message history
             new_messages = [
                 input_human_message,
                 AIMessage(content=final_message),
             ]
-            history.extend(new_messages)
+            history.extend(new_messages)  # type: ignore
```

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/rag/utils.py` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/rag/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from typing import List
 
 from langchain_core.documents import Document
+from langchain_core.language_models import BaseChatModel
 
 
-def _get_llm(llm: str):
+def _get_llm(llm: str) -> BaseChatModel:
     match llm:
         case "claude_3_opus":
             from langchain_anthropic.chat_models import ChatAnthropic
 
-            return ChatAnthropic(model_name="claude-3-opus-20240229", temperature=0)
+            return ChatAnthropic(model_name="claude-3-opus-20240229", temperature=0)  # type: ignore
         case "gpt_4_turbo":
             from langchain_openai.chat_models import ChatOpenAI
 
             return ChatOpenAI(model="gpt-4-turbo", temperature=0)
         case "command_r":
             from langchain_cohere.chat_models import ChatCohere
 
             return ChatCohere(model="command-r", temperature=0)
         case "mistral_large":
             from langchain_mistralai.chat_models import ChatMistralAI
 
-            return ChatMistralAI(model="mistral-large-latest", temperature=0)
+            return ChatMistralAI(model="mistral-large-latest", temperature=0)  # type: ignore
         case "gemini_pro":
             from langchain_google_vertexai.chat_models import ChatVertexAI
 
             return ChatVertexAI(model_name="gemini-pro", temperature=0)
         case "fireworks_mixtral_8x7b":
             from langchain_fireworks.chat_models import ChatFireworks
```

### Comparing `lango_cli_beta-0.0.1rc1/lango_cli_beta/rag_config.py` & `lango_cli_beta-0.0.1rc2/lango_cli_beta/rag_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         "mistral_large",
         "gemini_pro",
         "fireworks_mixtral_8x7b",
     ]
 
     rag_type: Literal["basic", "query_construction"]
 
-    ingest_path: str = None
+    ingest_path: Optional[str] = None
 
     metadata: Union[dict, None] = None
     """Metadata to be applied to all documents in the vector store."""
 
     json_schema: Union[dict, None] = None
     """JSONSchema used for query construction. Required for query_construction rag_type."""
```

### Comparing `lango_cli_beta-0.0.1rc1/pyproject.toml` & `lango_cli_beta-0.0.1rc2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "lango-cli-beta"
-version = "0.0.1rc1"
+version = "0.0.1rc2"
 description = ""
 authors = []
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.scripts]
 lango-cli = "lango_cli_beta.cli:app"
 
 [tool.poetry.dependencies]
-python = "<4.0,>=3.9.0"
+python = "<3.12,>=3.9.0"
 langchain-core = "^0.1.43"
 typer = ">=0.9.0,<0.10.0"
 langchain = "^0.1.16"
 langchain-openai = "^0.1.3"
 pymongo = "^4.6.3"
 langchain-text-splitters = "^0.0.1"
 python-dotenv = "^1.0.1"
@@ -23,18 +23,20 @@
 langchain-anthropic = "^0.1.9"
 langchain-cohere = "^0.1.2"
 langchain-mistralai = "^0.1.2"
 langchain-google-vertexai = "^1.0.1"
 langchain-fireworks = "^0.1.2"
 langgraph = ">=0.0.38,<0.1"
 langserve = { version = "^0.1.0", extras = ["all"] }
-fastapi = "^0.110.2"
+fastapi = ">=0.110.2,<1"
 uvicorn = ">=0.23.2,<0.24.0"
-pydantic = "1.10.13"
+pydantic = ">=1.10.13,<2"
 rich = "^13.7.1"
+langchain-community = ">=0.0.34"
+unstructured = { extras = ["all-docs"], version = "^0.13.4" }
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
@@ -52,15 +54,20 @@
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 
 [tool.poetry.group.typing.dependencies]
-mypy = "^0.991"
+mypy = "^1"
+
+[tool.poetry.group.test_integration]
+optional = true
+
+[tool.poetry.group.test_integration.dependencies]
 
 [tool.ruff]
 select = [
   "E", # pycodestyle
   "F", # pyflakes
   "I", # isort
 ]
```

### Comparing `lango_cli_beta-0.0.1rc1/PKG-INFO` & `lango_cli_beta-0.0.1rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: lango-cli-beta
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: 
 License: MIT
-Requires-Python: >=3.9.0,<4.0
+Requires-Python: >=3.9.0,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: fastapi (>=0.110.2,<0.111.0)
+Requires-Dist: fastapi (>=0.110.2,<1)
 Requires-Dist: langchain (>=0.1.16,<0.2.0)
 Requires-Dist: langchain-anthropic (>=0.1.9,<0.2.0)
 Requires-Dist: langchain-cohere (>=0.1.2,<0.2.0)
+Requires-Dist: langchain-community (>=0.0.34)
 Requires-Dist: langchain-core (>=0.1.43,<0.2.0)
 Requires-Dist: langchain-fireworks (>=0.1.2,<0.2.0)
 Requires-Dist: langchain-google-vertexai (>=1.0.1,<2.0.0)
 Requires-Dist: langchain-mistralai (>=0.1.2,<0.2.0)
 Requires-Dist: langchain-mongodb (>=0.1.3,<0.2.0)
 Requires-Dist: langchain-openai (>=0.1.3,<0.2.0)
 Requires-Dist: langchain-text-splitters (>=0.0.1,<0.0.2)
 Requires-Dist: langgraph (>=0.0.38,<0.1)
 Requires-Dist: langserve[all] (>=0.1.0,<0.2.0)
 Requires-Dist: motor (>=3.4.0,<4.0.0)
-Requires-Dist: pydantic (==1.10.13)
+Requires-Dist: pydantic (>=1.10.13,<2)
 Requires-Dist: pymongo (>=4.6.3,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: unstructured[all-docs] (>=0.13.4,<0.14.0)
 Requires-Dist: uvicorn (>=0.23.2,<0.24.0)
 Description-Content-Type: text/markdown
 
 # lango-cli-beta
 
 ## Installation
```

