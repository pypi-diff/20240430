# Comparing `tmp/substrate-120240418.0.10.tar.gz` & `tmp/substrate-120240430.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrate-120240418.0.10.tar", max compression
+gzip compressed data, was "substrate-120240430.0.0.tar", max compression
```

## Comparing `substrate-120240418.0.10.tar` & `substrate-120240430.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240418.0.10/LICENSE
--rw-r--r--   0        0        0     2479 2024-04-30 15:07:37.029522 substrate-120240418.0.10/README.md
--rw-r--r--   0        0        0     2066 2024-04-30 16:05:26.952395 substrate-120240418.0.10/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 19:17:25.000000 substrate-120240418.0.10/substrate/.keep
--rw-r--r--   0        0        0       17 2024-04-30 15:27:43.000000 substrate-120240418.0.10/substrate/GEN_VERSION
--rw-r--r--   0        0        0     2280 2024-04-30 15:27:45.000000 substrate-120240418.0.10/substrate/__init__.py
--rw-r--r--   0        0        0     6443 2024-04-19 14:16:03.281048 substrate-120240418.0.10/substrate/_client.py
--rw-r--r--   0        0        0       30 2024-03-13 14:46:31.829473 substrate-120240418.0.10/substrate/_version.py
--rw-r--r--   0        0        0        1 2024-04-30 15:34:56.208304 substrate-120240418.0.10/substrate/core/__init__.py
--rw-r--r--   0        0        0       27 2024-04-30 15:34:56.207625 substrate-120240418.0.10/substrate/core/_version.py
--rw-r--r--   0        0        0     1535 2024-04-30 15:34:56.210898 substrate-120240418.0.10/substrate/core/base_future.py
--rw-r--r--   0        0        0        0 2024-04-30 15:34:56.215661 substrate-120240418.0.10/substrate/core/client/__init__.py
--rw-r--r--   0        0        0     1750 2024-04-30 15:34:56.215875 substrate-120240418.0.10/substrate/core/client/find_futures_client.py
--rw-r--r--   0        0        0     2697 2024-04-30 15:34:56.216120 substrate-120240418.0.10/substrate/core/client/future.py
--rw-r--r--   0        0        0     1212 2024-04-30 15:34:56.215460 substrate-120240418.0.10/substrate/core/client/graph.py
--rw-r--r--   0        0        0     1149 2024-04-30 15:34:56.209209 substrate-120240418.0.10/substrate/core/coregraph.py
--rw-r--r--   0        0        0     2212 2024-04-30 15:34:56.206329 substrate-120240418.0.10/substrate/core/corenode.py
--rw-r--r--   0        0        0     1227 2024-04-30 15:34:56.211147 substrate-120240418.0.10/substrate/core/future_directive.py
--rw-r--r--   0        0        0      894 2024-04-30 15:34:56.206094 substrate-120240418.0.10/substrate/core/id_generator.py
--rw-r--r--   0        0        0    43544 2024-04-30 15:34:56.206734 substrate-120240418.0.10/substrate/core/models.py
--rw-r--r--   0        0        0     2332 2024-04-30 15:34:56.205783 substrate-120240418.0.10/substrate/core/sb.py
--rw-r--r--   0        0        0    32553 2024-04-19 00:53:25.000000 substrate-120240418.0.10/substrate/dataclass_models.py
--rw-r--r--   0        0        0    49125 2024-04-29 23:13:38.000000 substrate-120240418.0.10/substrate/future_dataclass_models.py
--rw-r--r--   0        0        0    45754 2024-04-30 15:27:44.000000 substrate-120240418.0.10/substrate/nodes.py
--rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240418.0.10/substrate/py.typed
--rw-r--r--   0        0        0     2132 2024-04-30 15:31:40.067652 substrate-120240418.0.10/substrate/substrate.py
--rw-r--r--   0        0        0     1015 2024-04-30 15:26:11.836346 substrate-120240418.0.10/substrate/substrate_response.py
--rw-r--r--   0        0        0    38598 2024-04-29 23:13:36.000000 substrate-120240418.0.10/substrate/typeddict_models.py
--rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 substrate-120240418.0.10/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240430.0.0/LICENSE
+-rw-r--r--   0        0        0     2675 2024-04-30 17:24:23.830575 substrate-120240430.0.0/README.md
+-rw-r--r--   0        0        0     2079 2024-04-30 18:53:09.761612 substrate-120240430.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 19:17:25.000000 substrate-120240430.0.0/substrate/.keep
+-rw-r--r--   0        0        0       17 2024-04-30 18:29:59.000000 substrate-120240430.0.0/substrate/GEN_VERSION
+-rw-r--r--   0        0        0     2280 2024-04-30 18:30:00.000000 substrate-120240430.0.0/substrate/__init__.py
+-rw-r--r--   0        0        0     5758 2024-04-30 17:48:32.046681 substrate-120240430.0.0/substrate/_client.py
+-rw-r--r--   0        0        0       30 2024-03-13 14:46:31.829473 substrate-120240430.0.0/substrate/_version.py
+-rw-r--r--   0        0        0        1 2024-04-30 18:52:14.905317 substrate-120240430.0.0/substrate/core/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-30 18:52:14.901427 substrate-120240430.0.0/substrate/core/_version.py
+-rw-r--r--   0        0        0     1535 2024-04-30 18:52:14.905804 substrate-120240430.0.0/substrate/core/base_future.py
+-rw-r--r--   0        0        0        0 2024-04-30 18:52:14.906396 substrate-120240430.0.0/substrate/core/client/__init__.py
+-rw-r--r--   0        0        0     1750 2024-04-30 18:52:14.906557 substrate-120240430.0.0/substrate/core/client/find_futures_client.py
+-rw-r--r--   0        0        0     2697 2024-04-30 18:52:14.906807 substrate-120240430.0.0/substrate/core/client/future.py
+-rw-r--r--   0        0        0     1212 2024-04-30 18:52:14.906269 substrate-120240430.0.0/substrate/core/client/graph.py
+-rw-r--r--   0        0        0     1149 2024-04-30 18:52:14.905579 substrate-120240430.0.0/substrate/core/coregraph.py
+-rw-r--r--   0        0        0     2212 2024-04-30 18:52:14.900064 substrate-120240430.0.0/substrate/core/corenode.py
+-rw-r--r--   0        0        0     1227 2024-04-30 18:52:14.905968 substrate-120240430.0.0/substrate/core/future_directive.py
+-rw-r--r--   0        0        0      894 2024-04-30 18:52:14.899784 substrate-120240430.0.0/substrate/core/id_generator.py
+-rw-r--r--   0        0        0    38367 2024-04-30 18:52:14.900402 substrate-120240430.0.0/substrate/core/models.py
+-rw-r--r--   0        0        0     2332 2024-04-30 18:52:14.899567 substrate-120240430.0.0/substrate/core/sb.py
+-rw-r--r--   0        0        0    32553 2024-04-19 00:53:25.000000 substrate-120240430.0.0/substrate/dataclass_models.py
+-rw-r--r--   0        0        0    49125 2024-04-30 18:29:58.000000 substrate-120240430.0.0/substrate/future_dataclass_models.py
+-rw-r--r--   0        0        0    45754 2024-04-30 18:30:00.000000 substrate-120240430.0.0/substrate/nodes.py
+-rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240430.0.0/substrate/py.typed
+-rw-r--r--   0        0        0     2132 2024-04-30 17:24:23.841883 substrate-120240430.0.0/substrate/substrate.py
+-rw-r--r--   0        0        0     1015 2024-04-30 17:24:23.842724 substrate-120240430.0.0/substrate/substrate_response.py
+-rw-r--r--   0        0        0    38598 2024-04-30 18:29:55.000000 substrate-120240430.0.0/substrate/typeddict_models.py
+-rw-r--r--   0        0        0     3312 1970-01-01 00:00:00.000000 substrate-120240430.0.0/PKG-INFO
```

### Comparing `substrate-120240418.0.10/LICENSE` & `substrate-120240430.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `substrate-120240418.0.10/README.md` & `substrate-120240430.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -54,11 +54,20 @@
 ```python
 response = await substrate.async_run(story, summary)
 ```
 
 Get the output of the summary node by passing it to `response.get`.
 
 ```python
-summary_out = response.get(story)
-print(summary_out.text);
+summary_out = response.get(summary)
+print(summary_out.text)
 // Princess Lily, a kind-hearted young princess, discovers a book of spells and uses it to grant her family and kingdom happiness.
 ```
+
+## Examples
+
+To run the above example as a notebook, navigate to the `examples/notebooks` directory and run:
+
+```sh
+make ensure     # install dependencies
+make basic      # run the notebook
+```
```

### Comparing `substrate-120240418.0.10/pyproject.toml` & `substrate-120240430.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "substrate"
-version = "120240418.0.10"
+version = "120240430.0.0"
 description = "Substrate Python SDK"
 readme = "README.md"
 authors = [ "vprtwn <ben@substrate.run>", "liamgriffiths <liam@substrate.run>",]
 [[tool.poetry.packages]]
 include = "substrate"
 
 [tool.pyright]
 typeCheckingMode = "basic"
 pythonVersion = "3.7"
 exclude = [ ".venv",]
 
-[tool.ruff]
-line-length = 120
-output-format = "grouped"
-target-version = "py310"
-
 [tool.mypy]
 pretty = true
 show_error_codes = true
 strict_equality = true
 implicit_reexport = true
 check_untyped_defs = true
 no_implicit_optional = true
@@ -37,21 +32,26 @@
 disallow_subclassing_any = true
 disallow_incomplete_defs = true
 disallow_untyped_decorators = true
 cache_fine_grained = true
 warn_unused_ignores = false
 warn_redundant_casts = false
 
+[tool.ruff]
+line-length = 120
+output-format = "grouped"
+target-version = "py310"
+exclude = [ "examples/notebooks",]
+
 [tool.poetry.dependencies]
 python = ">=3.9"
 networkx = ">=3.2.1"
 httpx = ">=0.26.0"
 distro = ">=1.8.0"
 typing-extensions = "^4.10.0"
-requests = "^2.31.0"
 pydantic = ">=1.0.0"
 
 [tool.ruff.lint]
 ignore-init-module-imports = true
 ignore = [ "B006", "T201", "T203", "ARG002", "ARG001",]
 unfixable = [ "T201", "T203",]
 select = [ "I", "B", "F401", "E722", "ARG", "TCH004",]
```

### Comparing `substrate-120240418.0.10/substrate/__init__.py` & `substrate-120240430.0.0/substrate/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 ꩜ Substrate Python SDK
 
-20240418.20240429
+20240430.20240430
 """
 
 from .nodes import (
     CLIP,
     XTTSV2,
     JinaV2,
     BigLaMa,
```

### Comparing `substrate-120240418.0.10/substrate/_client.py` & `substrate-120240430.0.0/substrate/_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -203,26 +203,7 @@
         res = APIResponse(
             status_code=http_response.status_code,
             json=_json,
             headers=http_response.headers,
             request=body,
         )
         return res
-
-    def post_compose_requests(self, dag: Dict[str, Any]) -> APIResponse:
-        import requests  # Ensure to import requests
-
-        url = f"{self._base_url}/compose"
-        body = {"dag": dag}
-        http_response = requests.post(url, headers=self.default_headers, json=body)
-        _json = None
-        try:
-            _json = http_response.json()
-        except Exception as exc:
-            log.debug("Could not read JSON from response data due to %s - %s", type(exc), exc)
-        res = APIResponse(
-            status_code=http_response.status_code,
-            json=_json,
-            headers=http_response.headers,
-            request=body,
-        )
-        return res
```

### Comparing `substrate-120240418.0.10/substrate/core/base_future.py` & `substrate-120240430.0.0/substrate/core/base_future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240418.0.10/substrate/core/client/find_futures_client.py` & `substrate-120240430.0.0/substrate/core/client/find_futures_client.py`

 * *Files identical despite different names*

### Comparing `substrate-120240418.0.10/substrate/core/client/future.py` & `substrate-120240430.0.0/substrate/core/client/future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240418.0.10/substrate/core/client/graph.py` & `substrate-120240430.0.0/substrate/core/client/graph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240418.0.10/substrate/core/coregraph.py` & `substrate-120240430.0.0/substrate/core/coregraph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240418.0.10/substrate/core/corenode.py` & `substrate-120240430.0.0/substrate/core/corenode.py`

 * *Files identical despite different names*

### Comparing `substrate-120240418.0.10/substrate/core/future_directive.py` & `substrate-120240430.0.0/substrate/core/future_directive.py`

 * *Files identical despite different names*

### Comparing `substrate-120240418.0.10/substrate/core/id_generator.py` & `substrate-120240430.0.0/substrate/core/id_generator.py`

 * *Files identical despite different names*

### Comparing `substrate-120240418.0.10/substrate/core/models.py` & `substrate-120240430.0.0/substrate/core/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,21 +6,18 @@
 
 
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional
 from typing_extensions import Literal, Annotated
 
-from pydantic import Extra, Field, BaseModel
+from pydantic import Field, BaseModel
 
 
 class ErrorOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     type: Literal["api_error", "invalid_request_error"]
     """
     The type of error returned.
     """
     message: str
     """
     A message providing more details about the error.
@@ -28,17 +25,14 @@
     request_id: Optional[str] = None
     """
     A unique identifier for the request.
     """
 
 
 class RunCodeIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     code: str
     """
     Code to execute.
     """
     args: Optional[List[str]] = None
     """
     List of command line arguments.
@@ -46,17 +40,14 @@
     language: Literal["python", "typescript", "javascript"] = "python"
     """
     Interpreter to use.
     """
 
 
 class RunCodeOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     output: Optional[str] = None
     """
     Contents of `stdout` after executing the code.
     """
     json_output: Dict[str, Any]
     """
     `output` as parsed JSON. Print serialized json to `stdout` to receive JSON.
@@ -64,17 +55,14 @@
     error: Optional[str] = None
     """
     Contents of `stderr` after executing the code.
     """
 
 
 class GenerateTextIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     prompt: str
     """
     Input prompt.
     """
     temperature: Annotated[float, Field(ge=0.0, le=1.0)] = 0.4
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
@@ -91,27 +79,21 @@
     ] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 class GenerateTextOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     text: str
     """
     Text response.
     """
 
 
 class GenerateJSONIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     prompt: str
     """
     Input prompt.
     """
     json_schema: Dict[str, Any]
     """
     JSON schema to guide `json_object` response.
@@ -127,27 +109,21 @@
     node: Literal["Mistral7BInstruct", "Mixtral8x7BInstruct"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 class GenerateJSONOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     json_object: Dict[str, Any]
     """
     JSON response.
     """
 
 
 class MultiGenerateTextIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     prompt: str
     """
     Input prompt.
     """
     num_choices: Annotated[int, Field(ge=1, le=8)]
     """
     Number of choices to generate.
@@ -168,27 +144,21 @@
     ] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 class MultiGenerateTextOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     choices: List[GenerateTextOut]
     """
     Response choices.
     """
 
 
 class BatchGenerateTextIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     prompts: List[str]
     """
     Batch input prompts.
     """
     temperature: Annotated[float, Field(ge=0.0, le=1.0)] = 0.4
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
@@ -200,27 +170,21 @@
     node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 class BatchGenerateTextOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     outputs: List[GenerateTextOut]
     """
     Batch outputs.
     """
 
 
 class MultiGenerateJSONIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     prompt: str
     """
     Input prompt.
     """
     json_schema: Dict[str, Any]
     """
     JSON schema to guide `json_object` response.
@@ -240,27 +204,21 @@
     node: Literal["Mistral7BInstruct", "Mixtral8x7BInstruct"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 class MultiGenerateJSONOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     choices: List[GenerateJSONOut]
     """
     Response choices.
     """
 
 
 class BatchGenerateJSONIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     prompts: List[str]
     """
     Batch input prompts.
     """
     json_schema: Dict[str, Any]
     """
     JSON schema to guide `json_object` response.
@@ -276,27 +234,21 @@
     node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 class BatchGenerateJSONOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     outputs: List[GenerateJSONOut]
     """
     Batch outputs.
     """
 
 
 class Mistral7BInstructIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     prompt: str
     """
     Input prompt.
     """
     num_choices: Annotated[int, Field(ge=1, le=8)] = 1
     """
     Number of choices to generate.
@@ -312,41 +264,32 @@
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
 
 
 class Mistral7BInstructChoice(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     text: Optional[str] = None
     """
     Text response, if `json_schema` was not provided.
     """
     json_object: Optional[Dict[str, Any]] = None
     """
     JSON response, if `json_schema` was provided.
     """
 
 
 class Mistral7BInstructOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     choices: List[Mistral7BInstructChoice]
     """
     Response choices.
     """
 
 
 class Mixtral8x7BInstructIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     prompt: str
     """
     Input prompt.
     """
     num_choices: Annotated[int, Field(ge=1, le=8)] = 1
     """
     Number of choices to generate.
@@ -362,41 +305,32 @@
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
 
 
 class Mixtral8x7BChoice(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     text: Optional[str] = None
     """
     Text response, if `json_schema` was not provided.
     """
     json_object: Optional[Dict[str, Any]] = None
     """
     JSON response, if `json_schema` was provided.
     """
 
 
 class Mixtral8x7BInstructOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     choices: List[Mixtral8x7BChoice]
     """
     Response choices.
     """
 
 
 class Llama3Instruct8BIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     prompt: str
     """
     Input prompt.
     """
     num_choices: Annotated[int, Field(ge=1, le=8)] = 1
     """
     Number of choices to generate.
@@ -408,37 +342,28 @@
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
 
 
 class Llama3Instruct8BChoice(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     text: Optional[str] = None
     """
     Text response.
     """
 
 
 class Llama3Instruct8BOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     choices: List[Llama3Instruct8BChoice]
     """
     Response choices.
     """
 
 
 class Llama3Instruct70BIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     prompt: str
     """
     Input prompt.
     """
     num_choices: Annotated[int, Field(ge=1, le=8)] = 1
     """
     Number of choices to generate.
@@ -450,37 +375,28 @@
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
 
 
 class Llama3Instruct70BChoice(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     text: Optional[str] = None
     """
     Text response.
     """
 
 
 class Llama3Instruct70BOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     choices: List[Llama3Instruct70BChoice]
     """
     Response choices.
     """
 
 
 class GenerateTextVisionIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     prompt: str
     """
     Text prompt.
     """
     image_uris: List[str]
     """
     Image prompts.
@@ -492,27 +408,21 @@
     node: Literal["Firellava13B"] = "Firellava13B"
     """
     Selected node.
     """
 
 
 class GenerateTextVisionOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     text: str
     """
     Text response.
     """
 
 
 class Firellava13BIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     prompt: str
     """
     Text prompt.
     """
     image_uris: List[str]
     """
     Image prompts.
@@ -520,27 +430,21 @@
     max_tokens: int = 800
     """
     Maximum number of tokens to generate.
     """
 
 
 class Firellava13BOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     text: str
     """
     Text response.
     """
 
 
 class GenerateImageIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     prompt: str
     """
     Text prompt.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
@@ -548,27 +452,21 @@
     node: Literal["StableDiffusionXL"] = "StableDiffusionXL"
     """
     Selected node.
     """
 
 
 class GenerateImageOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 class MultiGenerateImageIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     prompt: str
     """
     Text prompt.
     """
     num_images: Annotated[int, Field(ge=1, le=8)]
     """
     Number of images to generate.
@@ -580,27 +478,21 @@
     node: Literal["StableDiffusionXL"] = "StableDiffusionXL"
     """
     Selected node.
     """
 
 
 class MultiGenerateImageOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     outputs: List[GenerateImageOut]
     """
     Generated images.
     """
 
 
 class StableDiffusionXLIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     prompt: str
     """
     Text prompt.
     """
     negative_prompt: Optional[str] = None
     """
     Negative input prompt.
@@ -632,41 +524,32 @@
     guidance_scale: Annotated[float, Field(ge=0.0, le=30.0)] = 7
     """
     Higher values adhere to the text prompt more strongly, typically at the expense of image quality.
     """
 
 
 class StableDiffusionImage(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
     seed: int
     """
     The random noise seed used for generation.
     """
 
 
 class StableDiffusionXLOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     outputs: List[StableDiffusionImage]
     """
     Generated images.
     """
 
 
 class StableDiffusionXLLightningIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     prompt: str
     """
     Text prompt.
     """
     negative_prompt: Optional[str] = None
     """
     Negative input prompt.
@@ -690,27 +573,21 @@
     seeds: Optional[List[int]] = None
     """
     Seeds for deterministic generation. Default is a random seed.
     """
 
 
 class StableDiffusionXLLightningOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     outputs: List[StableDiffusionImage]
     """
     Generated images.
     """
 
 
 class StableDiffusionXLIPAdapterIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     prompt: str
     """
     Text prompt.
     """
     image_prompt_uri: Optional[str] = None
     """
     Image prompt.
@@ -742,27 +619,21 @@
     seeds: Optional[List[int]] = None
     """
     Random noise seeds. Default is random seeds for each generation.
     """
 
 
 class StableDiffusionXLIPAdapterOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     outputs: List[StableDiffusionImage]
     """
     Generated images.
     """
 
 
 class StableDiffusionXLControlNetIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Input image.
     """
     control_method: Literal["edge", "depth", "illusion"]
     """
     Strategy to control generation using the input image.
@@ -794,27 +665,21 @@
     seeds: Optional[List[int]] = None
     """
     Random noise seeds. Default is random seeds for each generation.
     """
 
 
 class StableDiffusionXLControlNetOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     outputs: List[StableDiffusionImage]
     """
     Generated images.
     """
 
 
 class GenerativeEditImageIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Original image.
     """
     prompt: str
     """
     Text prompt.
@@ -830,27 +695,21 @@
     node: Literal["StableDiffusionXLInpaint"] = "StableDiffusionXLInpaint"
     """
     Selected node.
     """
 
 
 class GenerativeEditImageOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 class MultiGenerativeEditImageIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Original image.
     """
     prompt: str
     """
     Text prompt.
@@ -870,27 +729,21 @@
     node: Literal["StableDiffusionXLInpaint"] = "StableDiffusionXLInpaint"
     """
     Selected node.
     """
 
 
 class MultiGenerativeEditImageOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     outputs: List[GenerativeEditImageOut]
     """
     Generated images.
     """
 
 
 class StableDiffusionXLInpaintIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Original image.
     """
     prompt: str
     """
     Text prompt.
@@ -922,27 +775,21 @@
     seeds: Optional[List[int]] = None
     """
     Random noise seeds. Default is random seeds for each generation.
     """
 
 
 class StableDiffusionXLInpaintOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     outputs: List[StableDiffusionImage]
     """
     Generated images.
     """
 
 
 class BoundingBox(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     x1: float
     """
     Top left corner x.
     """
     y1: float
     """
     Top left corner y.
@@ -954,31 +801,25 @@
     y2: float
     """
     Bottom right corner y.
     """
 
 
 class Point(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     x: int
     """
     X position.
     """
     y: int
     """
     Y position.
     """
 
 
 class FillMaskIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Input image.
     """
     mask_image_uri: str
     """
     Mask image that controls which pixels are inpainted.
@@ -990,27 +831,21 @@
     node: Literal["BigLaMa"] = "BigLaMa"
     """
     Selected node.
     """
 
 
 class FillMaskOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 class BigLaMaIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Input image.
     """
     mask_image_uri: str
     """
     Mask image that controls which pixels are inpainted.
@@ -1018,27 +853,21 @@
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 class BigLaMaOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 class RemoveBackgroundIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Input image.
     """
     return_mask: bool = False
     """
     Return a mask image instead of the original content.
@@ -1054,51 +883,39 @@
     node: Literal["DISISNet"] = "DISISNet"
     """
     Selected node.
     """
 
 
 class RemoveBackgroundOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 class DISISNetIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Input image.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 class DISISNetOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 class UpscaleImageIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Input image.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
@@ -1106,51 +923,39 @@
     node: Literal["RealESRGAN"] = "RealESRGAN"
     """
     Selected node.
     """
 
 
 class UpscaleImageOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 class RealESRGANIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Input image.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 class RealESRGANOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 class SegmentUnderPointIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Input image.
     """
     point: Point
     """
     Point prompt.
@@ -1162,27 +967,21 @@
     node: Literal["SegmentAnything"] = "SegmentAnything"
     """
     Selected node.
     """
 
 
 class SegmentUnderPointOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     mask_image_uri: str
     """
     Detected segments in 'mask image' format. Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 class SegmentAnythingIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Input image.
     """
     point_prompts: Optional[List[Point]] = None
     """
     Point prompts, to detect a segment under the point. One of `point_prompts` or `box_prompts` must be set.
@@ -1194,27 +993,21 @@
     store: Optional[str] = None
     """
     Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 class SegmentAnythingOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     mask_image_uri: str
     """
     Detected segments in 'mask image' format. Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
     """
 
 
 class TranscribeMediaIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     audio_uri: str
     """
     Input audio.
     """
     prompt: Optional[str] = None
     """
     Prompt to guide model on the content and context of input audio.
@@ -1238,17 +1031,14 @@
     suggest_chapters: bool = False
     """
     Suggest automatic chapter markers.
     """
 
 
 class TranscribedWord(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     word: str
     """
     Text of word.
     """
     start: Optional[float] = None
     """
     Start time of word, in seconds.
@@ -1260,17 +1050,14 @@
     speaker: Optional[str] = None
     """
     ID of speaker, if `diarize` is enabled.
     """
 
 
 class TranscribedSegment(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     text: str
     """
     Text of segment.
     """
     start: float
     """
     Start time of segment, in seconds.
@@ -1286,31 +1073,25 @@
     words: Optional[List[TranscribedWord]] = None
     """
     Aligned words, if `align` is enabled.
     """
 
 
 class ChapterMarker(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     title: str
     """
     Chapter title.
     """
     start: float
     """
     Start time of chapter, in seconds.
     """
 
 
 class TranscribeMediaOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     text: str
     """
     Transcribed text.
     """
     segments: Optional[List[TranscribedSegment]] = None
     """
     Transcribed segments, if `segment` is enabled.
@@ -1318,17 +1099,14 @@
     chapters: Optional[List[ChapterMarker]] = None
     """
     Chapter markers, if `suggest_chapters` is enabled.
     """
 
 
 class GenerateSpeechIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     text: str
     """
     Input text.
     """
     store: Optional[str] = None
     """
     Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the audio data will be returned as a base64-encoded string.
@@ -1336,27 +1114,21 @@
     node: Literal["XTTSV2"] = "XTTSV2"
     """
     Selected node.
     """
 
 
 class GenerateSpeechOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     audio_uri: str
     """
     Base 64-encoded WAV audio bytes, or a hosted audio url if `store` is provided.
     """
 
 
 class XTTSV2In(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     text: str
     """
     Input text.
     """
     audio_uri: Optional[str] = None
     """
     Reference audio used to synthesize the speaker. If unset, a default speaker voice will be used.
@@ -1368,27 +1140,21 @@
     store: Optional[str] = None
     """
     Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the audio data will be returned as a base64-encoded string.
     """
 
 
 class XTTSV2Out(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     audio_uri: str
     """
     Base 64-encoded WAV audio bytes, or a hosted audio url if `store` is provided.
     """
 
 
 class Embedding(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     vector: List[float]
     """
     Embedding vector.
     """
     doc_id: Optional[str] = None
     """
     Vector store document ID.
@@ -1396,17 +1162,14 @@
     metadata: Optional[Dict[str, Any]] = None
     """
     Vector store document metadata.
     """
 
 
 class EmbedTextIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     text: str
     """
     Text to embed.
     """
     collection_name: Optional[str] = None
     """
     Vector store name.
@@ -1426,27 +1189,21 @@
     model: Literal["jina-v2", "clip"] = "jina-v2"
     """
     Selected embedding model.
     """
 
 
 class EmbedTextOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     embedding: Embedding
     """
     Generated embedding.
     """
 
 
 class EmbedTextItem(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     text: str
     """
     Text to embed.
     """
     metadata: Optional[Dict[str, Any]] = None
     """
     Metadata that can be used to query the vector store. Ignored if `store` is unset.
@@ -1454,17 +1211,14 @@
     doc_id: Optional[str] = None
     """
     Vector store document ID. Ignored if `store` is unset.
     """
 
 
 class MultiEmbedTextIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     items: List[EmbedTextItem]
     """
     Items to embed.
     """
     collection_name: Optional[str] = None
     """
     Vector store name.
@@ -1476,27 +1230,21 @@
     model: Literal["jina-v2", "clip"] = "jina-v2"
     """
     Selected embedding model.
     """
 
 
 class MultiEmbedTextOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     embeddings: List[Embedding]
     """
     Generated embeddings.
     """
 
 
 class JinaV2In(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     items: List[EmbedTextItem]
     """
     Items to embed.
     """
     collection_name: Optional[str] = None
     """
     Vector store name.
@@ -1504,27 +1252,21 @@
     embedded_metadata_keys: Optional[List[str]] = None
     """
     Choose keys from `metadata` to embed with text.
     """
 
 
 class JinaV2Out(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     embeddings: List[Embedding]
     """
     Generated embeddings.
     """
 
 
 class EmbedImageIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Image to embed.
     """
     collection_name: Optional[str] = None
     """
     Vector store name.
@@ -1536,41 +1278,32 @@
     model: Literal["clip"] = "clip"
     """
     Selected embedding model.
     """
 
 
 class EmbedImageOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     embedding: Embedding
     """
     Generated embedding.
     """
 
 
 class EmbedImageItem(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: str
     """
     Image to embed.
     """
     doc_id: Optional[str] = None
     """
     Vector store document ID. Ignored if `store` is unset.
     """
 
 
 class EmbedTextOrImageItem(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     image_uri: Optional[str] = None
     """
     Image to embed.
     """
     text: Optional[str] = None
     """
     Text to embed.
@@ -1582,17 +1315,14 @@
     doc_id: Optional[str] = None
     """
     Vector store document ID. Ignored if `store` is unset.
     """
 
 
 class MultiEmbedImageIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     items: List[EmbedImageItem]
     """
     Items to embed.
     """
     collection_name: Optional[str] = None
     """
     Vector store name.
@@ -1600,27 +1330,21 @@
     model: Literal["clip"] = "clip"
     """
     Selected embedding model.
     """
 
 
 class MultiEmbedImageOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     embeddings: List[Embedding]
     """
     Generated embeddings.
     """
 
 
 class CLIPIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     items: List[EmbedTextOrImageItem]
     """
     Items to embed.
     """
     collection_name: Optional[str] = None
     """
     Vector store name.
@@ -1628,27 +1352,21 @@
     embedded_metadata_keys: Optional[List[str]] = None
     """
     Choose keys from `metadata` to embed with text. Only applies to text items.
     """
 
 
 class CLIPOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     embeddings: List[Embedding]
     """
     Generated embeddings.
     """
 
 
 class CreateVectorStoreIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     collection_name: Annotated[str, Field(max_length=63, min_length=1)]
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model.
@@ -1664,17 +1382,14 @@
     metric: Literal["cosine", "l2", "inner"] = "inner"
     """
     The distance metric to construct the index with.
     """
 
 
 class CreateVectorStoreOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     collection_name: Annotated[str, Field(max_length=63, min_length=1)]
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model.
@@ -1692,46 +1407,34 @@
     The distance metric to construct the index with.
     """
 
 
 class ListVectorStoresIn(BaseModel):
     pass
 
-    class Config:
-        extra = Extra.allow
-
 
 class ListVectorStoresOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     items: Optional[List[CreateVectorStoreOut]] = None
     """
     List of vector stores.
     """
 
 
 class DeleteVectorStoreIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     collection_name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model.
     """
 
 
 class DeleteVectorStoreOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     collection_name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model.
@@ -1739,17 +1442,14 @@
 
 
 class Vector(BaseModel):
     """
     Canonical representation of document with embedding vector.
     """
 
-    class Config:
-        extra = Extra.allow
-
     id: str
     """
     Document ID.
     """
     vector: List[float]
     """
     Embedding vector.
@@ -1757,17 +1457,14 @@
     metadata: Dict[str, Any]
     """
     Document metadata.
     """
 
 
 class FetchVectorsIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     collection_name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model.
@@ -1775,47 +1472,35 @@
     ids: Annotated[List[str], Field(max_items=100)]
     """
     Document IDs to retrieve.
     """
 
 
 class FetchVectorsOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     vectors: List[Vector]
     """
     Retrieved vectors.
     """
 
 
 class UpdateVectorsOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     count: int
     """
     Number of vectors modified.
     """
 
 
 class DeleteVectorsOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     count: int
     """
     Number of vectors modified.
     """
 
 
 class UpdateVectorParams(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     id: str
     """
     Document ID.
     """
     vector: Optional[List[float]] = None
     """
     Embedding vector.
@@ -1823,17 +1508,14 @@
     metadata: Optional[Dict[str, Any]] = None
     """
     Document metadata.
     """
 
 
 class UpdateVectorsIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     collection_name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model.
@@ -1841,17 +1523,14 @@
     vectors: Annotated[List[UpdateVectorParams], Field(max_items=100)]
     """
     Vectors to upsert.
     """
 
 
 class DeleteVectorsIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     collection_name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model.
@@ -1859,17 +1538,14 @@
     ids: Annotated[List[str], Field(max_items=100)]
     """
     Document IDs to delete.
     """
 
 
 class QueryVectorStoreIn(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     collection_name: str
     """
     Vector store to query against.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model.
@@ -1909,17 +1585,14 @@
     filters: Optional[Dict[str, Any]] = None
     """
     Filter metadata by key-value pairs.
     """
 
 
 class VectorStoreQueryResult(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     id: str
     """
     Document ID.
     """
     distance: float
     """
     Similarity score.
@@ -1931,17 +1604,14 @@
     metadata: Optional[Dict[str, Any]] = None
     """
     Document metadata.
     """
 
 
 class QueryVectorStoreOut(BaseModel):
-    class Config:
-        extra = Extra.allow
-
     results: List[List[VectorStoreQueryResult]]
     """
     Query results.
     """
     collection_name: Optional[str] = None
     """
     Vector store name.
```

### Comparing `substrate-120240418.0.10/substrate/core/sb.py` & `substrate-120240430.0.0/substrate/core/sb.py`

 * *Files identical despite different names*

### Comparing `substrate-120240418.0.10/substrate/dataclass_models.py` & `substrate-120240430.0.0/substrate/dataclass_models.py`

 * *Files identical despite different names*

### Comparing `substrate-120240418.0.10/substrate/future_dataclass_models.py` & `substrate-120240430.0.0/substrate/future_dataclass_models.py`

 * *Files identical despite different names*

### Comparing `substrate-120240418.0.10/substrate/nodes.py` & `substrate-120240430.0.0/substrate/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 ꩜ Substrate
 @GENERATED FILE
-20240418.20240429
+20240430.20240430
 """
 
 from .core.models import (
     CLIPOut,
     JinaV2Out,
     XTTSV2Out,
     BigLaMaOut,
```

### Comparing `substrate-120240418.0.10/substrate/substrate.py` & `substrate-120240430.0.0/substrate/substrate.py`

 * *Files identical despite different names*

### Comparing `substrate-120240418.0.10/substrate/substrate_response.py` & `substrate-120240430.0.0/substrate/substrate_response.py`

 * *Files identical despite different names*

### Comparing `substrate-120240418.0.10/substrate/typeddict_models.py` & `substrate-120240430.0.0/substrate/typeddict_models.py`

 * *Files identical despite different names*

### Comparing `substrate-120240418.0.10/PKG-INFO` & `substrate-120240430.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: substrate
-Version: 120240418.0.10
+Version: 120240430.0.0
 Summary: Substrate Python SDK
 Author: vprtwn
 Author-email: ben@substrate.run
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: distro (>=1.8.0)
 Requires-Dist: httpx (>=0.26.0)
 Requires-Dist: networkx (>=3.2.1)
 Requires-Dist: pydantic (>=1.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.10.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # ꩜ Substrate Python SDK
 
 [![PyPI version](https://img.shields.io/pypi/v/substrate.svg)](https://pypi.org/project/substrate/)
 
@@ -74,12 +73,21 @@
 ```python
 response = await substrate.async_run(story, summary)
 ```
 
 Get the output of the summary node by passing it to `response.get`.
 
 ```python
-summary_out = response.get(story)
-print(summary_out.text);
+summary_out = response.get(summary)
+print(summary_out.text)
 // Princess Lily, a kind-hearted young princess, discovers a book of spells and uses it to grant her family and kingdom happiness.
 ```
 
+## Examples
+
+To run the above example as a notebook, navigate to the `examples/notebooks` directory and run:
+
+```sh
+make ensure     # install dependencies
+make basic      # run the notebook
+```
+
```

