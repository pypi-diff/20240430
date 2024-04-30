# Comparing `tmp/substrate-120240416.0.9.tar.gz` & `tmp/substrate-120240418.0.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrate-120240416.0.9.tar", max compression
+gzip compressed data, was "substrate-120240418.0.10.tar", max compression
```

## Comparing `substrate-120240416.0.9.tar` & `substrate-120240418.0.10.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240416.0.9/LICENSE
--rw-r--r--   0        0        0       45 2024-03-19 21:55:57.200047 substrate-120240416.0.9/README.md
--rw-r--r--   0        0        0     2044 2024-04-19 04:11:24.008444 substrate-120240416.0.9/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 19:17:25.000000 substrate-120240416.0.9/substrate/.keep
--rw-r--r--   0        0        0       17 2024-04-19 03:17:45.451119 substrate-120240416.0.9/substrate/GEN_VERSION
--rw-r--r--   0        0        0     2010 2024-04-19 03:17:45.451616 substrate-120240416.0.9/substrate/__init__.py
--rw-r--r--   0        0        0     6459 2024-04-19 04:08:42.427085 substrate-120240416.0.9/substrate/_client.py
--rw-r--r--   0        0        0       30 2024-03-13 14:46:31.829473 substrate-120240416.0.9/substrate/_version.py
--rw-r--r--   0        0        0        1 2024-04-19 01:11:58.982501 substrate-120240416.0.9/substrate/core/__init__.py
--rw-r--r--   0        0        0       27 2024-04-19 01:11:58.982373 substrate-120240416.0.9/substrate/core/_version.py
--rw-r--r--   0        0        0     1535 2024-04-19 01:11:58.982766 substrate-120240416.0.9/substrate/core/base_future.py
--rw-r--r--   0        0        0        0 2024-04-19 01:11:58.983463 substrate-120240416.0.9/substrate/core/client/__init__.py
--rw-r--r--   0        0        0     1750 2024-04-19 01:11:58.983609 substrate-120240416.0.9/substrate/core/client/find_futures_client.py
--rw-r--r--   0        0        0     2697 2024-04-19 01:11:58.983753 substrate-120240416.0.9/substrate/core/client/future.py
--rw-r--r--   0        0        0     1212 2024-04-19 01:11:58.983077 substrate-120240416.0.9/substrate/core/client/graph.py
--rw-r--r--   0        0        0     1149 2024-04-19 01:11:58.982639 substrate-120240416.0.9/substrate/core/coregraph.py
--rw-r--r--   0        0        0     2138 2024-04-19 03:17:45.452478 substrate-120240416.0.9/substrate/core/corenode.py
--rw-r--r--   0        0        0     1227 2024-04-19 01:11:58.982867 substrate-120240416.0.9/substrate/core/future_directive.py
--rw-r--r--   0        0        0      894 2024-04-19 01:11:58.981394 substrate-120240416.0.9/substrate/core/id_generator.py
--rw-r--r--   0        0        0    38416 2024-04-19 03:17:45.452857 substrate-120240416.0.9/substrate/core/models.py
--rw-r--r--   0        0        0     2332 2024-04-19 01:11:58.981258 substrate-120240416.0.9/substrate/core/sb.py
--rw-r--r--   0        0        0    32553 2024-04-19 03:17:45.454302 substrate-120240416.0.9/substrate/dataclass_models.py
--rw-r--r--   0        0        0    43544 2024-04-19 03:17:45.454909 substrate-120240416.0.9/substrate/future_dataclass_models.py
--rw-r--r--   0        0        0    41746 2024-04-19 03:17:45.455305 substrate-120240416.0.9/substrate/nodes.py
--rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240416.0.9/substrate/py.typed
--rw-r--r--   0        0        0     1645 2024-04-19 03:55:44.473974 substrate-120240416.0.9/substrate/substrate.py
--rw-r--r--   0        0        0     1034 2024-04-16 21:25:37.775283 substrate-120240416.0.9/substrate/substrate_response.py
--rw-r--r--   0        0        0    34066 2024-04-19 03:17:45.455741 substrate-120240416.0.9/substrate/typeddict_models.py
--rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 substrate-120240416.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240418.0.10/LICENSE
+-rw-r--r--   0        0        0     2479 2024-04-30 15:07:37.029522 substrate-120240418.0.10/README.md
+-rw-r--r--   0        0        0     2066 2024-04-30 16:05:26.952395 substrate-120240418.0.10/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 19:17:25.000000 substrate-120240418.0.10/substrate/.keep
+-rw-r--r--   0        0        0       17 2024-04-30 15:27:43.000000 substrate-120240418.0.10/substrate/GEN_VERSION
+-rw-r--r--   0        0        0     2280 2024-04-30 15:27:45.000000 substrate-120240418.0.10/substrate/__init__.py
+-rw-r--r--   0        0        0     6443 2024-04-19 14:16:03.281048 substrate-120240418.0.10/substrate/_client.py
+-rw-r--r--   0        0        0       30 2024-03-13 14:46:31.829473 substrate-120240418.0.10/substrate/_version.py
+-rw-r--r--   0        0        0        1 2024-04-30 15:34:56.208304 substrate-120240418.0.10/substrate/core/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-30 15:34:56.207625 substrate-120240418.0.10/substrate/core/_version.py
+-rw-r--r--   0        0        0     1535 2024-04-30 15:34:56.210898 substrate-120240418.0.10/substrate/core/base_future.py
+-rw-r--r--   0        0        0        0 2024-04-30 15:34:56.215661 substrate-120240418.0.10/substrate/core/client/__init__.py
+-rw-r--r--   0        0        0     1750 2024-04-30 15:34:56.215875 substrate-120240418.0.10/substrate/core/client/find_futures_client.py
+-rw-r--r--   0        0        0     2697 2024-04-30 15:34:56.216120 substrate-120240418.0.10/substrate/core/client/future.py
+-rw-r--r--   0        0        0     1212 2024-04-30 15:34:56.215460 substrate-120240418.0.10/substrate/core/client/graph.py
+-rw-r--r--   0        0        0     1149 2024-04-30 15:34:56.209209 substrate-120240418.0.10/substrate/core/coregraph.py
+-rw-r--r--   0        0        0     2212 2024-04-30 15:34:56.206329 substrate-120240418.0.10/substrate/core/corenode.py
+-rw-r--r--   0        0        0     1227 2024-04-30 15:34:56.211147 substrate-120240418.0.10/substrate/core/future_directive.py
+-rw-r--r--   0        0        0      894 2024-04-30 15:34:56.206094 substrate-120240418.0.10/substrate/core/id_generator.py
+-rw-r--r--   0        0        0    43544 2024-04-30 15:34:56.206734 substrate-120240418.0.10/substrate/core/models.py
+-rw-r--r--   0        0        0     2332 2024-04-30 15:34:56.205783 substrate-120240418.0.10/substrate/core/sb.py
+-rw-r--r--   0        0        0    32553 2024-04-19 00:53:25.000000 substrate-120240418.0.10/substrate/dataclass_models.py
+-rw-r--r--   0        0        0    49125 2024-04-29 23:13:38.000000 substrate-120240418.0.10/substrate/future_dataclass_models.py
+-rw-r--r--   0        0        0    45754 2024-04-30 15:27:44.000000 substrate-120240418.0.10/substrate/nodes.py
+-rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240418.0.10/substrate/py.typed
+-rw-r--r--   0        0        0     2132 2024-04-30 15:31:40.067652 substrate-120240418.0.10/substrate/substrate.py
+-rw-r--r--   0        0        0     1015 2024-04-30 15:26:11.836346 substrate-120240418.0.10/substrate/substrate_response.py
+-rw-r--r--   0        0        0    38598 2024-04-29 23:13:36.000000 substrate-120240418.0.10/substrate/typeddict_models.py
+-rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 substrate-120240418.0.10/PKG-INFO
```

### Comparing `substrate-120240416.0.9/LICENSE` & `substrate-120240418.0.10/LICENSE`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.9/pyproject.toml` & `substrate-120240418.0.10/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "substrate"
-version = "120240416.0.9"
+version = "120240418.0.10"
 description = "Substrate Python SDK"
 readme = "README.md"
 authors = [ "vprtwn <ben@substrate.run>", "liamgriffiths <liam@substrate.run>",]
 [[tool.poetry.packages]]
 include = "substrate"
 
 [tool.pyright]
@@ -44,14 +44,15 @@
 [tool.poetry.dependencies]
 python = ">=3.9"
 networkx = ">=3.2.1"
 httpx = ">=0.26.0"
 distro = ">=1.8.0"
 typing-extensions = "^4.10.0"
 requests = "^2.31.0"
+pydantic = ">=1.0.0"
 
 [tool.ruff.lint]
 ignore-init-module-imports = true
 ignore = [ "B006", "T201", "T203", "ARG002", "ARG001",]
 unfixable = [ "T201", "T203",]
 select = [ "I", "B", "F401", "E722", "ARG", "TCH004",]
```

### Comparing `substrate-120240416.0.9/substrate/__init__.py` & `substrate-120240418.0.10/substrate/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 ꩜ Substrate Python SDK
 
-20240416.20240418
+20240418.20240429
 """
 
 from .nodes import (
     CLIP,
     XTTSV2,
     JinaV2,
     BigLaMa,
+    RunCode,
     DISISNet,
     FillMask,
     EmbedText,
     EmbedImage,
     RealESRGAN,
     FetchVectors,
     Firellava13B,
@@ -24,26 +25,31 @@
     UpdateVectors,
     GenerateSpeech,
     MultiEmbedText,
     MultiEmbedImage,
     SegmentAnything,
     TranscribeMedia,
     ListVectorStores,
+    Llama3Instruct8B,
     QueryVectorStore,
     RemoveBackground,
+    BatchGenerateJSON,
+    BatchGenerateText,
     CreateVectorStore,
     DeleteVectorStore,
+    Llama3Instruct70B,
     Mistral7BInstruct,
     MultiGenerateJSON,
     MultiGenerateText,
     SegmentUnderPoint,
     StableDiffusionXL,
     GenerateTextVision,
     MultiGenerateImage,
     GenerativeEditImage,
+    Mixtral8x7BInstruct,
     MultiGenerativeEditImage,
     StableDiffusionXLInpaint,
     StableDiffusionXLIPAdapter,
     StableDiffusionXLLightning,
     StableDiffusionXLControlNet,
 )
 from .core.sb import sb
@@ -51,20 +57,26 @@
 from .substrate import Substrate, SubstrateResponse
 
 __all__ = [
     "__version__",
     "SubstrateResponse",
     "sb",
     "Substrate",
+    "RunCode",
     "GenerateText",
     "MultiGenerateText",
+    "BatchGenerateText",
+    "BatchGenerateJSON",
     "GenerateJSON",
     "MultiGenerateJSON",
     "GenerateTextVision",
     "Mistral7BInstruct",
+    "Mixtral8x7BInstruct",
+    "Llama3Instruct8B",
+    "Llama3Instruct70B",
     "Firellava13B",
     "GenerateImage",
     "MultiGenerateImage",
     "GenerativeEditImage",
     "MultiGenerativeEditImage",
     "StableDiffusionXL",
     "StableDiffusionXLLightning",
```

### Comparing `substrate-120240416.0.9/substrate/_client.py` & `substrate-120240418.0.10/substrate/_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import datetime
 import platform
 from typing import Any, Dict, Union, Optional
 from typing_extensions import Literal
 
 import httpx
 import distro
```

### Comparing `substrate-120240416.0.9/substrate/core/base_future.py` & `substrate-120240418.0.10/substrate/core/base_future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.9/substrate/core/client/find_futures_client.py` & `substrate-120240418.0.10/substrate/core/client/find_futures_client.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.9/substrate/core/client/future.py` & `substrate-120240418.0.10/substrate/core/client/future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.9/substrate/core/client/graph.py` & `substrate-120240418.0.10/substrate/core/client/graph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.9/substrate/core/coregraph.py` & `substrate-120240418.0.10/substrate/core/coregraph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.9/substrate/core/corenode.py` & `substrate-120240418.0.10/substrate/core/corenode.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """
 CORE ꩜ SUBSTRATE
 """
-from typing import Any, List, Type, Optional
+from typing import Any, List, Type, Generic, TypeVar, Optional
 
 import networkx as nx
 
 from .base_future import BaseFuture
 from .id_generator import IDGenerator
 from .client.future import TracedFuture
 from .future_directive import TraceDirective
 from .client.find_futures_client import find_futures_client
 
+OT = TypeVar("OT")
 
-class CoreNode:
-    def __init__(self, hide: bool = True, **attr):
+
+class CoreNode(Generic[OT]):
+    def __init__(self, out_type: Type[OT] = Type[Any], hide: bool = True, **attr):
+        self._out_type = out_type
         self.node = self.__class__.__name__
         self.args = attr
         generator_instance = IDGenerator.get_instance(self.__class__.__name__)
         self.id = generator_instance.get_next_id()
         self._global_output_keys = None
         self._should_output_globally: bool = not hide
         self.SG = nx.DiGraph()
@@ -25,19 +28,19 @@
             self.args = BaseFuture.replace_futures_with_placeholder(attr)
         else:
             self.args = {}
         self.SG.add_node(self, **self.args)
         self.futures_from_args: List[BaseFuture] = find_futures_client(attr)
 
     @property
-    def out_type(self) -> Type[Any]:
+    def out_type(self) -> Type[OT]:
         """
-        Get the typed output of this node using `response.get(node, node.out_type)`
+        The output type of this node.
         """
-        return Type[None]
+        return self._out_type
 
     def to_dict(self):
         return {
             "id": self.id,
             "node": self.node,
             "args": self.args,
             **({"_should_output_globally": self._should_output_globally} if self._should_output_globally else {}),
```

### Comparing `substrate-120240416.0.9/substrate/core/future_directive.py` & `substrate-120240418.0.10/substrate/core/future_directive.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.9/substrate/core/id_generator.py` & `substrate-120240418.0.10/substrate/core/id_generator.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.9/substrate/core/models.py` & `substrate-120240418.0.10/substrate/core/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,50 @@
     """
     request_id: Optional[str] = None
     """
     A unique identifier for the request.
     """
 
 
+class RunCodeIn(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    code: str
+    """
+    Code to execute.
+    """
+    args: Optional[List[str]] = None
+    """
+    List of command line arguments.
+    """
+    language: Literal["python", "typescript", "javascript"] = "python"
+    """
+    Interpreter to use.
+    """
+
+
+class RunCodeOut(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    output: Optional[str] = None
+    """
+    Contents of `stdout` after executing the code.
+    """
+    json_output: Dict[str, Any]
+    """
+    `output` as parsed JSON. Print serialized json to `stdout` to receive JSON.
+    """
+    error: Optional[str] = None
+    """
+    Contents of `stderr` after executing the code.
+    """
+
+
 class GenerateTextIn(BaseModel):
     class Config:
         extra = Extra.allow
 
     prompt: str
     """
     Input prompt.
@@ -43,15 +79,20 @@
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
-    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
+    node: Literal[
+        "Mistral7BInstruct",
+        "Mixtral8x7BInstruct",
+        "Llama3Instruct8B",
+        "Llama3Instruct70B",
+    ] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 class GenerateTextOut(BaseModel):
     class Config:
@@ -79,15 +120,15 @@
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
-    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct", "Mixtral8x7BInstruct"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 class GenerateJSONOut(BaseModel):
     class Config:
@@ -99,134 +140,175 @@
     """
 
 
 class MultiGenerateTextIn(BaseModel):
     class Config:
         extra = Extra.allow
 
-    prompt: Optional[str] = None
+    prompt: str
     """
     Input prompt.
     """
-    batch_prompts: Optional[List[str]] = None
-    """
-    Batch input prompts.
-    """
-    num_choices: Annotated[int, Field(ge=1, le=8)] = 1
+    num_choices: Annotated[int, Field(ge=1, le=8)]
     """
     Number of choices to generate.
     """
     temperature: Annotated[float, Field(ge=0.0, le=1.0)] = 0.4
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
-    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
+    node: Literal[
+        "Mistral7BInstruct",
+        "Mixtral8x7BInstruct",
+        "Llama3Instruct8B",
+        "Llama3Instruct70B",
+    ] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
-class MultiGenerateTextOutput(BaseModel):
+class MultiGenerateTextOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     choices: List[GenerateTextOut]
     """
     Response choices.
     """
 
 
-class MultiGenerateTextOut(BaseModel):
+class BatchGenerateTextIn(BaseModel):
     class Config:
         extra = Extra.allow
 
-    outputs: List[MultiGenerateTextOutput]
+    prompts: List[str]
+    """
+    Batch input prompts.
+    """
+    temperature: Annotated[float, Field(ge=0.0, le=1.0)] = 0.4
     """
-    A single output for `prompt`, or multiple outputs for `batch_prompts`.
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: Optional[int] = None
+    """
+    Maximum number of tokens to generate.
+    """
+    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
+    """
+    Selected node.
+    """
+
+
+class BatchGenerateTextOut(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    outputs: List[GenerateTextOut]
+    """
+    Batch outputs.
     """
 
 
 class MultiGenerateJSONIn(BaseModel):
     class Config:
         extra = Extra.allow
 
-    prompt: Optional[str] = None
+    prompt: str
     """
     Input prompt.
     """
     json_schema: Dict[str, Any]
     """
     JSON schema to guide `json_object` response.
     """
-    batch_prompts: Optional[List[str]] = None
-    """
-    Batch input prompts.
-    """
-    num_choices: Annotated[int, Field(ge=1, le=8)] = 2
+    num_choices: Annotated[int, Field(ge=1, le=8)]
     """
     Number of choices to generate.
     """
     temperature: Annotated[float, Field(ge=0.0, le=1.0)] = 0.4
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
-    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct", "Mixtral8x7BInstruct"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
-class MultiGenerateJSONOutput(BaseModel):
+class MultiGenerateJSONOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     choices: List[GenerateJSONOut]
     """
     Response choices.
     """
 
 
-class MultiGenerateJSONOut(BaseModel):
+class BatchGenerateJSONIn(BaseModel):
     class Config:
         extra = Extra.allow
 
-    outputs: List[MultiGenerateJSONOutput]
+    prompts: List[str]
+    """
+    Batch input prompts.
+    """
+    json_schema: Dict[str, Any]
     """
-    A single output for `prompt`, or multiple outputs for `batch_prompts`.
+    JSON schema to guide `json_object` response.
+    """
+    temperature: Annotated[float, Field(ge=0.0, le=1.0)] = 0.4
+    """
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: Optional[int] = None
+    """
+    Maximum number of tokens to generate.
+    """
+    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
+    """
+    Selected node.
+    """
+
+
+class BatchGenerateJSONOut(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    outputs: List[GenerateJSONOut]
+    """
+    Batch outputs.
     """
 
 
 class Mistral7BInstructIn(BaseModel):
     class Config:
         extra = Extra.allow
 
-    prompt: Optional[str] = None
+    prompt: str
     """
     Input prompt.
     """
     num_choices: Annotated[int, Field(ge=1, le=8)] = 1
     """
     Number of choices to generate.
     """
     json_schema: Optional[Dict[str, Any]] = None
     """
     JSON schema to guide response.
     """
-    batch_prompts: Optional[List[str]] = None
-    """
-    Batch input prompts.
-    """
     temperature: Annotated[Optional[float], Field(ge=0.0, le=1.0)] = None
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
@@ -243,31 +325,155 @@
     """
     json_object: Optional[Dict[str, Any]] = None
     """
     JSON response, if `json_schema` was provided.
     """
 
 
-class Mistral7BInstructOutput(BaseModel):
+class Mistral7BInstructOut(BaseModel):
     class Config:
         extra = Extra.allow
 
     choices: List[Mistral7BInstructChoice]
     """
     Response choices.
     """
 
 
-class Mistral7BInstructOut(BaseModel):
+class Mixtral8x7BInstructIn(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    prompt: str
+    """
+    Input prompt.
+    """
+    num_choices: Annotated[int, Field(ge=1, le=8)] = 1
+    """
+    Number of choices to generate.
+    """
+    json_schema: Optional[Dict[str, Any]] = None
+    """
+    JSON schema to guide response.
+    """
+    temperature: Annotated[Optional[float], Field(ge=0.0, le=1.0)] = None
+    """
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: Optional[int] = None
+    """
+    Maximum number of tokens to generate.
+    """
+
+
+class Mixtral8x7BChoice(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    text: Optional[str] = None
+    """
+    Text response, if `json_schema` was not provided.
+    """
+    json_object: Optional[Dict[str, Any]] = None
+    """
+    JSON response, if `json_schema` was provided.
+    """
+
+
+class Mixtral8x7BInstructOut(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    choices: List[Mixtral8x7BChoice]
+    """
+    Response choices.
+    """
+
+
+class Llama3Instruct8BIn(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    prompt: str
+    """
+    Input prompt.
+    """
+    num_choices: Annotated[int, Field(ge=1, le=8)] = 1
+    """
+    Number of choices to generate.
+    """
+    temperature: Annotated[Optional[float], Field(ge=0.0, le=1.0)] = None
+    """
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: Optional[int] = None
+    """
+    Maximum number of tokens to generate.
+    """
+
+
+class Llama3Instruct8BChoice(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    text: Optional[str] = None
+    """
+    Text response.
+    """
+
+
+class Llama3Instruct8BOut(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    choices: List[Llama3Instruct8BChoice]
+    """
+    Response choices.
+    """
+
+
+class Llama3Instruct70BIn(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    prompt: str
+    """
+    Input prompt.
+    """
+    num_choices: Annotated[int, Field(ge=1, le=8)] = 1
+    """
+    Number of choices to generate.
+    """
+    temperature: Annotated[Optional[float], Field(ge=0.0, le=1.0)] = None
+    """
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: Optional[int] = None
+    """
+    Maximum number of tokens to generate.
+    """
+
+
+class Llama3Instruct70BChoice(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    text: Optional[str] = None
+    """
+    Text response.
+    """
+
+
+class Llama3Instruct70BOut(BaseModel):
     class Config:
         extra = Extra.allow
 
-    outputs: List[Mistral7BInstructOutput]
+    choices: List[Llama3Instruct70BChoice]
     """
-    A single output for `prompt`, or multiple outputs for `batch_prompts`.
+    Response choices.
     """
 
 
 class GenerateTextVisionIn(BaseModel):
     class Config:
         extra = Extra.allow
 
@@ -333,15 +539,15 @@
 
     prompt: str
     """
     Text prompt.
     """
     store: Optional[str] = None
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: Literal["StableDiffusionXL"] = "StableDiffusionXL"
     """
     Selected node.
     """
 
 
@@ -365,15 +571,15 @@
     """
     num_images: Annotated[int, Field(ge=1, le=8)]
     """
     Number of images to generate.
     """
     store: Optional[str] = None
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: Literal["StableDiffusionXL"] = "StableDiffusionXL"
     """
     Selected node.
     """
 
 
@@ -405,15 +611,15 @@
     """
     num_images: Annotated[int, Field(ge=1, le=8)]
     """
     Number of images to generate.
     """
     store: Optional[str] = None
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     height: Annotated[int, Field(ge=256, le=1536)] = 1024
     """
     Height of output image, in pixels.
     """
     width: Annotated[int, Field(ge=256, le=1536)] = 1024
     """
@@ -467,15 +673,15 @@
     """
     num_images: Annotated[int, Field(ge=1, le=8)] = 1
     """
     Number of images to generate.
     """
     store: Optional[str] = None
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     height: Annotated[int, Field(ge=256, le=1536)] = 1024
     """
     Height of output image, in pixels.
     """
     width: Annotated[int, Field(ge=256, le=1536)] = 1024
     """
@@ -519,15 +725,15 @@
     """
     negative_prompt: Optional[str] = None
     """
     Negative input prompt.
     """
     store: Optional[str] = None
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     width: Annotated[int, Field(ge=640, le=1536)] = 1024
     """
     Width of output image, in pixels.
     """
     height: Annotated[int, Field(ge=640, le=1536)] = 1024
     """
@@ -575,15 +781,15 @@
     """
     negative_prompt: Optional[str] = None
     """
     Negative input prompt.
     """
     store: Optional[str] = None
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     conditioning_scale: Annotated[float, Field(ge=0.0, le=1.0)] = 0.5
     """
     Controls the influence of the input image on the generated output.
     """
     seeds: Optional[List[int]] = None
     """
@@ -615,15 +821,15 @@
     """
     mask_image_uri: Optional[str] = None
     """
     Mask image that controls which pixels are inpainted. If unset, the entire image is edited (image-to-image).
     """
     store: Optional[str] = None
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: Literal["StableDiffusionXLInpaint"] = "StableDiffusionXLInpaint"
     """
     Selected node.
     """
 
 
@@ -655,15 +861,15 @@
     """
     num_images: Annotated[int, Field(ge=1, le=8)]
     """
     Number of images to generate.
     """
     store: Optional[str] = None
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: Literal["StableDiffusionXLInpaint"] = "StableDiffusionXLInpaint"
     """
     Selected node.
     """
 
 
@@ -703,15 +909,15 @@
     """
     negative_prompt: Optional[str] = None
     """
     Negative input prompt.
     """
     store: Optional[str] = None
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     strength: Annotated[float, Field(ge=0.0, le=1.0)] = 0.8
     """
     Controls the strength of the generation process.
     """
     seeds: Optional[List[int]] = None
     """
@@ -775,15 +981,15 @@
     """
     mask_image_uri: str
     """
     Mask image that controls which pixels are inpainted.
     """
     store: Optional[str] = None
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: Literal["BigLaMa"] = "BigLaMa"
     """
     Selected node.
     """
 
 
@@ -807,15 +1013,15 @@
     """
     mask_image_uri: str
     """
     Mask image that controls which pixels are inpainted.
     """
     store: Optional[str] = None
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 class BigLaMaOut(BaseModel):
     class Config:
         extra = Extra.allow
 
@@ -839,15 +1045,15 @@
     """
     background_color: Optional[str] = None
     """
     Hex value background color. Transparent if unset.
     """
     store: Optional[str] = None
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: Literal["DISISNet"] = "DISISNet"
     """
     Selected node.
     """
 
 
@@ -867,15 +1073,15 @@
 
     image_uri: str
     """
     Input image.
     """
     store: Optional[str] = None
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 class DISISNetOut(BaseModel):
     class Config:
         extra = Extra.allow
 
@@ -891,15 +1097,15 @@
 
     image_uri: str
     """
     Input image.
     """
     store: Optional[str] = None
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: Literal["RealESRGAN"] = "RealESRGAN"
     """
     Selected node.
     """
 
 
@@ -919,15 +1125,15 @@
 
     image_uri: str
     """
     Input image.
     """
     store: Optional[str] = None
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 class RealESRGANOut(BaseModel):
     class Config:
         extra = Extra.allow
 
@@ -947,15 +1153,15 @@
     """
     point: Point
     """
     Point prompt.
     """
     store: Optional[str] = None
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: Literal["SegmentAnything"] = "SegmentAnything"
     """
     Selected node.
     """
 
 
@@ -983,15 +1189,15 @@
     """
     box_prompts: Optional[List[BoundingBox]] = None
     """
     Box prompts, to detect a segment within the bounding box. One of `point_prompts` or `box_prompts` must be set.
     """
     store: Optional[str] = None
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 class SegmentAnythingOut(BaseModel):
     class Config:
         extra = Extra.allow
 
@@ -1121,15 +1327,15 @@
 
     text: str
     """
     Input text.
     """
     store: Optional[str] = None
     """
-    Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
+    Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the audio data will be returned as a base64-encoded string.
     """
     node: Literal["XTTSV2"] = "XTTSV2"
     """
     Selected node.
     """
 
 
@@ -1157,15 +1363,15 @@
     """
     language: str = "en"
     """
     Language of input text. Supported languages: `en, de, fr, es, it, pt, pl, zh, ar, cs, ru, nl, tr, hu, ko`.
     """
     store: Optional[str] = None
     """
-    Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
+    Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the audio data will be returned as a base64-encoded string.
     """
 
 
 class XTTSV2Out(BaseModel):
     class Config:
         extra = Extra.allow
 
@@ -1197,33 +1403,33 @@
     class Config:
         extra = Extra.allow
 
     text: str
     """
     Text to embed.
     """
-    store: Optional[str] = None
+    collection_name: Optional[str] = None
     """
-    [Vector store](/docs/vector-stores) identifier.
+    Vector store name.
     """
     metadata: Optional[Dict[str, Any]] = None
     """
     Metadata that can be used to query the vector store. Ignored if `store` is unset.
     """
     embedded_metadata_keys: Optional[List[str]] = None
     """
     Choose keys from `metadata` to embed with text.
     """
     doc_id: Optional[str] = None
     """
     Vector store document ID. Ignored if `store` is unset.
     """
-    node: Literal["JinaV2", "CLIP"] = "JinaV2"
+    model: Literal["jina-v2", "clip"] = "jina-v2"
     """
-    Selected node.
+    Selected embedding model.
     """
 
 
 class EmbedTextOut(BaseModel):
     class Config:
         extra = Extra.allow
 
@@ -1255,25 +1461,25 @@
     class Config:
         extra = Extra.allow
 
     items: List[EmbedTextItem]
     """
     Items to embed.
     """
-    store: Optional[str] = None
+    collection_name: Optional[str] = None
     """
-    [Vector store](/docs/vector-stores) identifier.
+    Vector store name.
     """
     embedded_metadata_keys: Optional[List[str]] = None
     """
     Choose keys from `metadata` to embed with text.
     """
-    node: Literal["JinaV2", "CLIP"] = "JinaV2"
+    model: Literal["jina-v2", "clip"] = "jina-v2"
     """
-    Selected node.
+    Selected embedding model.
     """
 
 
 class MultiEmbedTextOut(BaseModel):
     class Config:
         extra = Extra.allow
 
@@ -1287,17 +1493,17 @@
     class Config:
         extra = Extra.allow
 
     items: List[EmbedTextItem]
     """
     Items to embed.
     """
-    store: Optional[str] = None
+    collection_name: Optional[str] = None
     """
-    [Vector store](/docs/vector-stores) identifier.
+    Vector store name.
     """
     embedded_metadata_keys: Optional[List[str]] = None
     """
     Choose keys from `metadata` to embed with text.
     """
 
 
@@ -1315,25 +1521,25 @@
     class Config:
         extra = Extra.allow
 
     image_uri: str
     """
     Image to embed.
     """
-    store: Optional[str] = None
+    collection_name: Optional[str] = None
     """
-    [Vector store](/docs/vector-stores) identifier.
+    Vector store name.
     """
     doc_id: Optional[str] = None
     """
     Vector store document ID. Ignored if `store` is unset.
     """
-    node: Literal["CLIP"] = "CLIP"
+    model: Literal["clip"] = "clip"
     """
-    Selected node.
+    Selected embedding model.
     """
 
 
 class EmbedImageOut(BaseModel):
     class Config:
         extra = Extra.allow
 
@@ -1383,21 +1589,21 @@
     class Config:
         extra = Extra.allow
 
     items: List[EmbedImageItem]
     """
     Items to embed.
     """
-    store: Optional[str] = None
+    collection_name: Optional[str] = None
     """
-    [Vector store](/docs/vector-stores) identifier.
+    Vector store name.
     """
-    node: Literal["CLIP"] = "CLIP"
+    model: Literal["clip"] = "clip"
     """
-    Selected node.
+    Selected embedding model.
     """
 
 
 class MultiEmbedImageOut(BaseModel):
     class Config:
         extra = Extra.allow
 
@@ -1411,17 +1617,21 @@
     class Config:
         extra = Extra.allow
 
     items: List[EmbedTextOrImageItem]
     """
     Items to embed.
     """
-    store: Optional[str] = None
+    collection_name: Optional[str] = None
+    """
+    Vector store name.
     """
-    [Vector store](/docs/vector-stores) identifier.
+    embedded_metadata_keys: Optional[List[str]] = None
+    """
+    Choose keys from `metadata` to embed with text. Only applies to text items.
     """
 
 
 class CLIPOut(BaseModel):
     class Config:
         extra = Extra.allow
 
@@ -1431,15 +1641,15 @@
     """
 
 
 class CreateVectorStoreIn(BaseModel):
     class Config:
         extra = Extra.allow
 
-    name: Annotated[str, Field(max_length=63, min_length=1)]
+    collection_name: Annotated[str, Field(max_length=63, min_length=1)]
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model.
     """
@@ -1457,15 +1667,15 @@
     """
 
 
 class CreateVectorStoreOut(BaseModel):
     class Config:
         extra = Extra.allow
 
-    name: Annotated[str, Field(max_length=63, min_length=1)]
+    collection_name: Annotated[str, Field(max_length=63, min_length=1)]
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model.
     """
@@ -1490,39 +1700,39 @@
         extra = Extra.allow
 
 
 class ListVectorStoresOut(BaseModel):
     class Config:
         extra = Extra.allow
 
-    stores: Optional[List[CreateVectorStoreOut]] = None
+    items: Optional[List[CreateVectorStoreOut]] = None
     """
     List of vector stores.
     """
 
 
 class DeleteVectorStoreIn(BaseModel):
     class Config:
         extra = Extra.allow
 
-    name: str
+    collection_name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model.
     """
 
 
 class DeleteVectorStoreOut(BaseModel):
     class Config:
         extra = Extra.allow
 
-    name: str
+    collection_name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model.
     """
@@ -1550,15 +1760,15 @@
     """
 
 
 class FetchVectorsIn(BaseModel):
     class Config:
         extra = Extra.allow
 
-    name: str
+    collection_name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model.
     """
@@ -1616,15 +1826,15 @@
     """
 
 
 class UpdateVectorsIn(BaseModel):
     class Config:
         extra = Extra.allow
 
-    name: str
+    collection_name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model.
     """
@@ -1634,15 +1844,15 @@
     """
 
 
 class DeleteVectorsIn(BaseModel):
     class Config:
         extra = Extra.allow
 
-    name: str
+    collection_name: str
     """
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model.
     """
@@ -1652,15 +1862,15 @@
     """
 
 
 class QueryVectorStoreIn(BaseModel):
     class Config:
         extra = Extra.allow
 
-    name: str
+    collection_name: str
     """
     Vector store to query against.
     """
     model: Literal["jina-v2", "clip"]
     """
     Selected embedding model.
     """
@@ -1696,18 +1906,14 @@
     """
     Include the metadata of the vectors in the response.
     """
     filters: Optional[Dict[str, Any]] = None
     """
     Filter metadata by key-value pairs.
     """
-    metric: Optional[Literal["cosine", "l2", "inner"]] = None
-    """
-    The distance metric used for the query. Defaults to the distance metric the vector store was created with.
-    """
 
 
 class VectorStoreQueryResult(BaseModel):
     class Config:
         extra = Extra.allow
 
     id: str
@@ -1732,15 +1938,15 @@
     class Config:
         extra = Extra.allow
 
     results: List[List[VectorStoreQueryResult]]
     """
     Query results.
     """
-    name: Optional[str] = None
+    collection_name: Optional[str] = None
     """
     Vector store name.
     """
     model: Optional[Literal["jina-v2", "clip"]] = None
     """
     Selected embedding model.
     """
```

### Comparing `substrate-120240416.0.9/substrate/core/sb.py` & `substrate-120240418.0.10/substrate/core/sb.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.9/substrate/dataclass_models.py` & `substrate-120240418.0.10/substrate/dataclass_models.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.9/substrate/future_dataclass_models.py` & `substrate-120240418.0.10/substrate/future_dataclass_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,60 @@
     """
     (Future reference)
     A unique identifier for the request.
     """
 
 
 @dataclass
+class FutureRunCodeIn:
+    """
+    (Future reference)
+    """
+
+    code: str
+    """
+    (Future reference)
+    Code to execute.
+    """
+    args: Optional[List[str]] = None
+    """
+    (Future reference)
+    List of command line arguments.
+    """
+    language: Literal["python", "typescript", "javascript"] = "python"
+    """
+    (Future reference)
+    Interpreter to use.
+    """
+
+
+@dataclass
+class FutureRunCodeOut:
+    """
+    (Future reference)
+    """
+
+    json_output: Dict[str, Any]
+    """
+    (Future reference)
+    `output` as parsed JSON. Print serialized json to `stdout` to receive JSON.
+    """
+    output: Optional[str] = None
+    """
+    (Future reference)
+    Contents of `stdout` after executing the code.
+    """
+    error: Optional[str] = None
+    """
+    (Future reference)
+    Contents of `stderr` after executing the code.
+    """
+
+
+@dataclass
 class FutureGenerateTextIn:
     """
     (Future reference)
     """
 
     prompt: str
     """
@@ -52,15 +98,20 @@
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
-    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
+    node: Literal[
+        "Mistral7BInstruct",
+        "Mixtral8x7BInstruct",
+        "Llama3Instruct8B",
+        "Llama3Instruct70B",
+    ] = "Mistral7BInstruct"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
@@ -98,15 +149,15 @@
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
-    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct", "Mixtral8x7BInstruct"] = "Mistral7BInstruct"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
@@ -124,181 +175,296 @@
 
 @dataclass
 class FutureMultiGenerateTextIn:
     """
     (Future reference)
     """
 
-    prompt: Optional[str] = None
+    prompt: str
     """
     (Future reference)
     Input prompt.
     """
-    batch_prompts: Optional[List[str]] = None
-    """
-    (Future reference)
-    Batch input prompts.
-    """
-    num_choices: int = 1
+    num_choices: int
     """
     (Future reference)
     Number of choices to generate.
     """
     temperature: float = 0.4
     """
     (Future reference)
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
-    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
+    node: Literal[
+        "Mistral7BInstruct",
+        "Mixtral8x7BInstruct",
+        "Llama3Instruct8B",
+        "Llama3Instruct70B",
+    ] = "Mistral7BInstruct"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
-class MultiGenerateTextOutput:
+class FutureMultiGenerateTextOut:
     """
     (Future reference)
     """
 
     choices: List[FutureGenerateTextOut]
     """
     (Future reference)
     Response choices.
     """
 
 
 @dataclass
-class FutureMultiGenerateTextOut:
+class FutureBatchGenerateTextIn:
     """
     (Future reference)
     """
 
-    outputs: List[MultiGenerateTextOutput]
+    prompts: List[str]
     """
     (Future reference)
-    A single output for `prompt`, or multiple outputs for `batch_prompts`.
+    Batch input prompts.
+    """
+    temperature: float = 0.4
+    """
+    (Future reference)
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: Optional[int] = None
+    """
+    (Future reference)
+    Maximum number of tokens to generate.
+    """
+    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
+    """
+    (Future reference)
+    Selected node.
     """
 
 
 @dataclass
-class FutureMultiGenerateJSONIn:
+class FutureBatchGenerateTextOut:
     """
     (Future reference)
     """
 
-    json_schema: Dict[str, Any]
+    outputs: List[FutureGenerateTextOut]
     """
     (Future reference)
-    JSON schema to guide `json_object` response.
+    Batch outputs.
     """
-    prompt: Optional[str] = None
+
+
+@dataclass
+class FutureMultiGenerateJSONIn:
+    """
+    (Future reference)
+    """
+
+    prompt: str
     """
     (Future reference)
     Input prompt.
     """
-    batch_prompts: Optional[List[str]] = None
+    json_schema: Dict[str, Any]
     """
     (Future reference)
-    Batch input prompts.
+    JSON schema to guide `json_object` response.
     """
-    num_choices: int = 2
+    num_choices: int
     """
     (Future reference)
     Number of choices to generate.
     """
     temperature: float = 0.4
     """
     (Future reference)
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
-    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct", "Mixtral8x7BInstruct"] = "Mistral7BInstruct"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
-class MultiGenerateJSONOutput:
+class FutureMultiGenerateJSONOut:
     """
     (Future reference)
     """
 
     choices: List[FutureGenerateJSONOut]
     """
     (Future reference)
     Response choices.
     """
 
 
 @dataclass
-class FutureMultiGenerateJSONOut:
+class FutureBatchGenerateJSONIn:
     """
     (Future reference)
     """
 
-    outputs: List[MultiGenerateJSONOutput]
+    prompts: List[str]
+    """
+    (Future reference)
+    Batch input prompts.
+    """
+    json_schema: Dict[str, Any]
+    """
+    (Future reference)
+    JSON schema to guide `json_object` response.
+    """
+    temperature: float = 0.4
+    """
+    (Future reference)
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: Optional[int] = None
+    """
+    (Future reference)
+    Maximum number of tokens to generate.
+    """
+    node: Literal["Mistral7BInstruct"] = "Mistral7BInstruct"
+    """
+    (Future reference)
+    Selected node.
+    """
+
+
+@dataclass
+class FutureBatchGenerateJSONOut:
     """
     (Future reference)
-    A single output for `prompt`, or multiple outputs for `batch_prompts`.
+    """
+
+    outputs: List[FutureGenerateJSONOut]
+    """
+    (Future reference)
+    Batch outputs.
     """
 
 
 @dataclass
 class FutureMistral7BInstructIn:
     """
     (Future reference)
     """
 
-    prompt: Optional[str] = None
+    prompt: str
     """
     (Future reference)
     Input prompt.
     """
     num_choices: int = 1
     """
     (Future reference)
     Number of choices to generate.
     """
     json_schema: Optional[Dict[str, Any]] = None
     """
     (Future reference)
     JSON schema to guide response.
     """
-    batch_prompts: Optional[List[str]] = None
+    temperature: Optional[float] = None
     """
     (Future reference)
-    Batch input prompts.
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: Optional[int] = None
+    """
+    (Future reference)
+    Maximum number of tokens to generate.
+    """
+
+
+@dataclass
+class Mistral7BInstructChoice:
+    """
+    (Future reference)
+    """
+
+    text: Optional[str] = None
+    """
+    (Future reference)
+    Text response, if `json_schema` was not provided.
+    """
+    json_object: Optional[Dict[str, Any]] = None
+    """
+    (Future reference)
+    JSON response, if `json_schema` was provided.
+    """
+
+
+@dataclass
+class FutureMistral7BInstructOut:
+    """
+    (Future reference)
+    """
+
+    choices: List[Mistral7BInstructChoice]
+    """
+    (Future reference)
+    Response choices.
+    """
+
+
+@dataclass
+class FutureMixtral8x7BInstructIn:
+    """
+    (Future reference)
+    """
+
+    prompt: str
+    """
+    (Future reference)
+    Input prompt.
+    """
+    num_choices: int = 1
+    """
+    (Future reference)
+    Number of choices to generate.
+    """
+    json_schema: Optional[Dict[str, Any]] = None
+    """
+    (Future reference)
+    JSON schema to guide response.
     """
     temperature: Optional[float] = None
     """
     (Future reference)
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
 
 
 @dataclass
-class Mistral7BInstructChoice:
+class Mixtral8x7BChoice:
     """
     (Future reference)
     """
 
     text: Optional[str] = None
     """
     (Future reference)
@@ -308,36 +474,131 @@
     """
     (Future reference)
     JSON response, if `json_schema` was provided.
     """
 
 
 @dataclass
-class Mistral7BInstructOutput:
+class FutureMixtral8x7BInstructOut:
     """
     (Future reference)
     """
 
-    choices: List[Mistral7BInstructChoice]
+    choices: List[Mixtral8x7BChoice]
     """
     (Future reference)
     Response choices.
     """
 
 
 @dataclass
-class FutureMistral7BInstructOut:
+class FutureLlama3Instruct8BIn:
+    """
+    (Future reference)
+    """
+
+    prompt: str
+    """
+    (Future reference)
+    Input prompt.
+    """
+    num_choices: int = 1
+    """
+    (Future reference)
+    Number of choices to generate.
+    """
+    temperature: Optional[float] = None
+    """
+    (Future reference)
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: Optional[int] = None
+    """
+    (Future reference)
+    Maximum number of tokens to generate.
+    """
+
+
+@dataclass
+class Llama3Instruct8BChoice:
+    """
+    (Future reference)
+    """
+
+    text: Optional[str] = None
+    """
+    (Future reference)
+    Text response.
+    """
+
+
+@dataclass
+class FutureLlama3Instruct8BOut:
+    """
+    (Future reference)
+    """
+
+    choices: List[Llama3Instruct8BChoice]
+    """
+    (Future reference)
+    Response choices.
+    """
+
+
+@dataclass
+class FutureLlama3Instruct70BIn:
     """
     (Future reference)
     """
 
-    outputs: List[Mistral7BInstructOutput]
+    prompt: str
+    """
+    (Future reference)
+    Input prompt.
+    """
+    num_choices: int = 1
+    """
+    (Future reference)
+    Number of choices to generate.
+    """
+    temperature: Optional[float] = None
+    """
+    (Future reference)
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: Optional[int] = None
+    """
+    (Future reference)
+    Maximum number of tokens to generate.
+    """
+
+
+@dataclass
+class Llama3Instruct70BChoice:
     """
     (Future reference)
-    A single output for `prompt`, or multiple outputs for `batch_prompts`.
+    """
+
+    text: Optional[str] = None
+    """
+    (Future reference)
+    Text response.
+    """
+
+
+@dataclass
+class FutureLlama3Instruct70BOut:
+    """
+    (Future reference)
+    """
+
+    choices: List[Llama3Instruct70BChoice]
+    """
+    (Future reference)
+    Response choices.
     """
 
 
 @dataclass
 class FutureGenerateTextVisionIn:
     """
     (Future reference)
@@ -424,15 +685,15 @@
     """
     (Future reference)
     Text prompt.
     """
     store: Optional[str] = None
     """
     (Future reference)
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: Literal["StableDiffusionXL"] = "StableDiffusionXL"
     """
     (Future reference)
     Selected node.
     """
 
@@ -465,15 +726,15 @@
     """
     (Future reference)
     Number of images to generate.
     """
     store: Optional[str] = None
     """
     (Future reference)
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: Literal["StableDiffusionXL"] = "StableDiffusionXL"
     """
     (Future reference)
     Selected node.
     """
 
@@ -516,15 +777,15 @@
     """
     (Future reference)
     Number of diffusion steps.
     """
     store: Optional[str] = None
     """
     (Future reference)
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     height: int = 1024
     """
     (Future reference)
     Height of output image, in pixels.
     """
     width: int = 1024
@@ -595,15 +856,15 @@
     """
     (Future reference)
     Number of images to generate.
     """
     store: Optional[str] = None
     """
     (Future reference)
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     height: int = 1024
     """
     (Future reference)
     Height of output image, in pixels.
     """
     width: int = 1024
@@ -661,15 +922,15 @@
     """
     (Future reference)
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     (Future reference)
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     width: int = 1024
     """
     (Future reference)
     Width of output image, in pixels.
     """
     height: int = 1024
@@ -732,15 +993,15 @@
     """
     (Future reference)
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     (Future reference)
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     conditioning_scale: float = 0.5
     """
     (Future reference)
     Controls the influence of the input image on the generated output.
     """
     seeds: Optional[List[int]] = None
@@ -783,15 +1044,15 @@
     """
     (Future reference)
     Mask image that controls which pixels are inpainted. If unset, the entire image is edited (image-to-image).
     """
     store: Optional[str] = None
     """
     (Future reference)
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: Literal["StableDiffusionXLInpaint"] = "StableDiffusionXLInpaint"
     """
     (Future reference)
     Selected node.
     """
 
@@ -834,15 +1095,15 @@
     """
     (Future reference)
     Mask image that controls which pixels are edited (inpainting). If unset, the entire image is edited (image-to-image).
     """
     store: Optional[str] = None
     """
     (Future reference)
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: Literal["StableDiffusionXLInpaint"] = "StableDiffusionXLInpaint"
     """
     (Future reference)
     Selected node.
     """
 
@@ -895,15 +1156,15 @@
     """
     (Future reference)
     Negative input prompt.
     """
     store: Optional[str] = None
     """
     (Future reference)
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     strength: float = 0.8
     """
     (Future reference)
     Controls the strength of the generation process.
     """
     seeds: Optional[List[int]] = None
@@ -987,15 +1248,15 @@
     """
     (Future reference)
     Mask image that controls which pixels are inpainted.
     """
     store: Optional[str] = None
     """
     (Future reference)
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: Literal["BigLaMa"] = "BigLaMa"
     """
     (Future reference)
     Selected node.
     """
 
@@ -1028,15 +1289,15 @@
     """
     (Future reference)
     Mask image that controls which pixels are inpainted.
     """
     store: Optional[str] = None
     """
     (Future reference)
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
 class FutureBigLaMaOut:
     """
     (Future reference)
@@ -1069,15 +1330,15 @@
     """
     (Future reference)
     Hex value background color. Transparent if unset.
     """
     store: Optional[str] = None
     """
     (Future reference)
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: Literal["DISISNet"] = "DISISNet"
     """
     (Future reference)
     Selected node.
     """
 
@@ -1105,15 +1366,15 @@
     """
     (Future reference)
     Input image.
     """
     store: Optional[str] = None
     """
     (Future reference)
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
 class FutureDISISNetOut:
     """
     (Future reference)
@@ -1136,15 +1397,15 @@
     """
     (Future reference)
     Input image.
     """
     store: Optional[str] = None
     """
     (Future reference)
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: Literal["RealESRGAN"] = "RealESRGAN"
     """
     (Future reference)
     Selected node.
     """
 
@@ -1172,15 +1433,15 @@
     """
     (Future reference)
     Input image.
     """
     store: Optional[str] = None
     """
     (Future reference)
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
 class FutureRealESRGANOut:
     """
     (Future reference)
@@ -1208,15 +1469,15 @@
     """
     (Future reference)
     Point prompt.
     """
     store: Optional[str] = None
     """
     (Future reference)
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: Literal["SegmentAnything"] = "SegmentAnything"
     """
     (Future reference)
     Selected node.
     """
 
@@ -1254,15 +1515,15 @@
     """
     (Future reference)
     Box prompts, to detect a segment within the bounding box. One of `point_prompts` or `box_prompts` must be set.
     """
     store: Optional[str] = None
     """
     (Future reference)
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
 class FutureSegmentAnythingOut:
     """
     (Future reference)
@@ -1430,15 +1691,15 @@
     """
     (Future reference)
     Input text.
     """
     store: Optional[str] = None
     """
     (Future reference)
-    Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
+    Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the audio data will be returned as a base64-encoded string.
     """
     node: Literal["XTTSV2"] = "XTTSV2"
     """
     (Future reference)
     Selected node.
     """
 
@@ -1476,15 +1737,15 @@
     """
     (Future reference)
     Language of input text. Supported languages: `en, de, fr, es, it, pt, pl, zh, ar, cs, ru, nl, tr, hu, ko`.
     """
     store: Optional[str] = None
     """
     (Future reference)
-    Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
+    Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the audio data will be returned as a base64-encoded string.
     """
 
 
 @dataclass
 class FutureXTTSV2Out:
     """
     (Future reference)
@@ -1527,18 +1788,18 @@
     """
 
     text: str
     """
     (Future reference)
     Text to embed.
     """
-    store: Optional[str] = None
+    collection_name: Optional[str] = None
     """
     (Future reference)
-    [Vector store](/docs/vector-stores) identifier.
+    Vector store name.
     """
     metadata: Optional[Dict[str, Any]] = None
     """
     (Future reference)
     Metadata that can be used to query the vector store. Ignored if `store` is unset.
     """
     embedded_metadata_keys: Optional[List[str]] = None
@@ -1547,18 +1808,18 @@
     Choose keys from `metadata` to embed with text.
     """
     doc_id: Optional[str] = None
     """
     (Future reference)
     Vector store document ID. Ignored if `store` is unset.
     """
-    node: Literal["JinaV2", "CLIP"] = "JinaV2"
+    model: Literal["jina-v2", "clip"] = "jina-v2"
     """
     (Future reference)
-    Selected node.
+    Selected embedding model.
     """
 
 
 @dataclass
 class FutureEmbedTextOut:
     """
     (Future reference)
@@ -1601,28 +1862,28 @@
     """
 
     items: List[EmbedTextItem]
     """
     (Future reference)
     Items to embed.
     """
-    store: Optional[str] = None
+    collection_name: Optional[str] = None
     """
     (Future reference)
-    [Vector store](/docs/vector-stores) identifier.
+    Vector store name.
     """
     embedded_metadata_keys: Optional[List[str]] = None
     """
     (Future reference)
     Choose keys from `metadata` to embed with text.
     """
-    node: Literal["JinaV2", "CLIP"] = "JinaV2"
+    model: Literal["jina-v2", "clip"] = "jina-v2"
     """
     (Future reference)
-    Selected node.
+    Selected embedding model.
     """
 
 
 @dataclass
 class FutureMultiEmbedTextOut:
     """
     (Future reference)
@@ -1642,18 +1903,18 @@
     """
 
     items: List[EmbedTextItem]
     """
     (Future reference)
     Items to embed.
     """
-    store: Optional[str] = None
+    collection_name: Optional[str] = None
     """
     (Future reference)
-    [Vector store](/docs/vector-stores) identifier.
+    Vector store name.
     """
     embedded_metadata_keys: Optional[List[str]] = None
     """
     (Future reference)
     Choose keys from `metadata` to embed with text.
     """
 
@@ -1678,28 +1939,28 @@
     """
 
     image_uri: str
     """
     (Future reference)
     Image to embed.
     """
-    store: Optional[str] = None
+    collection_name: Optional[str] = None
     """
     (Future reference)
-    [Vector store](/docs/vector-stores) identifier.
+    Vector store name.
     """
     doc_id: Optional[str] = None
     """
     (Future reference)
     Vector store document ID. Ignored if `store` is unset.
     """
-    node: Literal["CLIP"] = "CLIP"
+    model: Literal["clip"] = "clip"
     """
     (Future reference)
-    Selected node.
+    Selected embedding model.
     """
 
 
 @dataclass
 class FutureEmbedImageOut:
     """
     (Future reference)
@@ -1765,23 +2026,23 @@
     """
 
     items: List[EmbedImageItem]
     """
     (Future reference)
     Items to embed.
     """
-    store: Optional[str] = None
+    collection_name: Optional[str] = None
     """
     (Future reference)
-    [Vector store](/docs/vector-stores) identifier.
+    Vector store name.
     """
-    node: Literal["CLIP"] = "CLIP"
+    model: Literal["clip"] = "clip"
     """
     (Future reference)
-    Selected node.
+    Selected embedding model.
     """
 
 
 @dataclass
 class FutureMultiEmbedImageOut:
     """
     (Future reference)
@@ -1801,18 +2062,23 @@
     """
 
     items: List[EmbedTextOrImageItem]
     """
     (Future reference)
     Items to embed.
     """
-    store: Optional[str] = None
+    collection_name: Optional[str] = None
     """
     (Future reference)
-    [Vector store](/docs/vector-stores) identifier.
+    Vector store name.
+    """
+    embedded_metadata_keys: Optional[List[str]] = None
+    """
+    (Future reference)
+    Choose keys from `metadata` to embed with text. Only applies to text items.
     """
 
 
 @dataclass
 class FutureCLIPOut:
     """
     (Future reference)
@@ -1827,15 +2093,15 @@
 
 @dataclass
 class FutureCreateVectorStoreIn:
     """
     (Future reference)
     """
 
-    name: str
+    collection_name: str
     """
     (Future reference)
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     (Future reference)
@@ -1860,15 +2126,15 @@
 
 @dataclass
 class FutureCreateVectorStoreOut:
     """
     (Future reference)
     """
 
-    name: str
+    collection_name: str
     """
     (Future reference)
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     (Future reference)
@@ -1902,28 +2168,28 @@
 
 @dataclass
 class FutureListVectorStoresOut:
     """
     (Future reference)
     """
 
-    stores: Optional[List[FutureCreateVectorStoreOut]] = None
+    items: Optional[List[FutureCreateVectorStoreOut]] = None
     """
     (Future reference)
     List of vector stores.
     """
 
 
 @dataclass
 class FutureDeleteVectorStoreIn:
     """
     (Future reference)
     """
 
-    name: str
+    collection_name: str
     """
     (Future reference)
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     (Future reference)
@@ -1933,15 +2199,15 @@
 
 @dataclass
 class FutureDeleteVectorStoreOut:
     """
     (Future reference)
     """
 
-    name: str
+    collection_name: str
     """
     (Future reference)
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     (Future reference)
@@ -1975,15 +2241,15 @@
 
 @dataclass
 class FutureFetchVectorsIn:
     """
     (Future reference)
     """
 
-    name: str
+    collection_name: str
     """
     (Future reference)
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     (Future reference)
@@ -2060,15 +2326,15 @@
 
 @dataclass
 class FutureUpdateVectorsIn:
     """
     (Future reference)
     """
 
-    name: str
+    collection_name: str
     """
     (Future reference)
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     (Future reference)
@@ -2083,15 +2349,15 @@
 
 @dataclass
 class FutureDeleteVectorsIn:
     """
     (Future reference)
     """
 
-    name: str
+    collection_name: str
     """
     (Future reference)
     Vector store name.
     """
     model: Literal["jina-v2", "clip"]
     """
     (Future reference)
@@ -2106,15 +2372,15 @@
 
 @dataclass
 class FutureQueryVectorStoreIn:
     """
     (Future reference)
     """
 
-    name: str
+    collection_name: str
     """
     (Future reference)
     Vector store to query against.
     """
     model: Literal["jina-v2", "clip"]
     """
     (Future reference)
@@ -2161,19 +2427,14 @@
     Include the metadata of the vectors in the response.
     """
     filters: Optional[Dict[str, Any]] = None
     """
     (Future reference)
     Filter metadata by key-value pairs.
     """
-    metric: Optional[Literal["cosine", "l2", "inner"]] = None
-    """
-    (Future reference)
-    The distance metric used for the query. Defaults to the distance metric the vector store was created with.
-    """
 
 
 @dataclass
 class VectorStoreQueryResult:
     """
     (Future reference)
     """
@@ -2207,15 +2468,15 @@
     """
 
     results: List[List[VectorStoreQueryResult]]
     """
     (Future reference)
     Query results.
     """
-    name: Optional[str] = None
+    collection_name: Optional[str] = None
     """
     (Future reference)
     Vector store name.
     """
     model: Optional[Literal["jina-v2", "clip"]] = None
     """
     (Future reference)
```

### Comparing `substrate-120240416.0.9/substrate/nodes.py` & `substrate-120240418.0.10/substrate/nodes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 ꩜ Substrate
 @GENERATED FILE
-20240416.20240418
+20240418.20240429
 """
-from typing import Type
 
 from .core.models import (
     CLIPOut,
     JinaV2Out,
     XTTSV2Out,
     BigLaMaOut,
+    RunCodeOut,
     DISISNetOut,
     FillMaskOut,
     EmbedTextOut,
     EmbedImageOut,
     RealESRGANOut,
     FetchVectorsOut,
     Firellava13BOut,
@@ -25,38 +25,44 @@
     UpdateVectorsOut,
     GenerateSpeechOut,
     MultiEmbedTextOut,
     MultiEmbedImageOut,
     SegmentAnythingOut,
     TranscribeMediaOut,
     ListVectorStoresOut,
+    Llama3Instruct8BOut,
     QueryVectorStoreOut,
     RemoveBackgroundOut,
+    BatchGenerateJSONOut,
+    BatchGenerateTextOut,
     CreateVectorStoreOut,
     DeleteVectorStoreOut,
+    Llama3Instruct70BOut,
     Mistral7BInstructOut,
     MultiGenerateJSONOut,
     MultiGenerateTextOut,
     SegmentUnderPointOut,
     StableDiffusionXLOut,
     GenerateTextVisionOut,
     MultiGenerateImageOut,
     GenerativeEditImageOut,
+    Mixtral8x7BInstructOut,
     MultiGenerativeEditImageOut,
     StableDiffusionXLInpaintOut,
     StableDiffusionXLIPAdapterOut,
     StableDiffusionXLLightningOut,
     StableDiffusionXLControlNetOut,
 )
 from .core.corenode import CoreNode
 from .typeddict_models import (
     CLIPIn,
     JinaV2In,
     XTTSV2In,
     BigLaMaIn,
+    RunCodeIn,
     DISISNetIn,
     FillMaskIn,
     EmbedTextIn,
     EmbedImageIn,
     RealESRGANIn,
     FetchVectorsIn,
     Firellava13BIn,
@@ -68,37 +74,43 @@
     UpdateVectorsIn,
     GenerateSpeechIn,
     MultiEmbedTextIn,
     MultiEmbedImageIn,
     SegmentAnythingIn,
     TranscribeMediaIn,
     ListVectorStoresIn,
+    Llama3Instruct8BIn,
     QueryVectorStoreIn,
     RemoveBackgroundIn,
+    BatchGenerateJSONIn,
+    BatchGenerateTextIn,
     CreateVectorStoreIn,
     DeleteVectorStoreIn,
+    Llama3Instruct70BIn,
     Mistral7BInstructIn,
     MultiGenerateJSONIn,
     MultiGenerateTextIn,
     SegmentUnderPointIn,
     StableDiffusionXLIn,
     GenerateTextVisionIn,
     MultiGenerateImageIn,
     GenerativeEditImageIn,
+    Mixtral8x7BInstructIn,
     MultiGenerativeEditImageIn,
     StableDiffusionXLInpaintIn,
     StableDiffusionXLIPAdapterIn,
     StableDiffusionXLLightningIn,
     StableDiffusionXLControlNetIn,
 )
 from .future_dataclass_models import (
     FutureCLIPOut,
     FutureJinaV2Out,
     FutureXTTSV2Out,
     FutureBigLaMaOut,
+    FutureRunCodeOut,
     FutureDISISNetOut,
     FutureFillMaskOut,
     FutureEmbedTextOut,
     FutureEmbedImageOut,
     FutureRealESRGANOut,
     FutureFetchVectorsOut,
     FutureFirellava13BOut,
@@ -110,1383 +122,1408 @@
     FutureUpdateVectorsOut,
     FutureGenerateSpeechOut,
     FutureMultiEmbedTextOut,
     FutureMultiEmbedImageOut,
     FutureSegmentAnythingOut,
     FutureTranscribeMediaOut,
     FutureListVectorStoresOut,
+    FutureLlama3Instruct8BOut,
     FutureQueryVectorStoreOut,
     FutureRemoveBackgroundOut,
+    FutureBatchGenerateJSONOut,
+    FutureBatchGenerateTextOut,
     FutureCreateVectorStoreOut,
     FutureDeleteVectorStoreOut,
+    FutureLlama3Instruct70BOut,
     FutureMistral7BInstructOut,
     FutureMultiGenerateJSONOut,
     FutureMultiGenerateTextOut,
     FutureSegmentUnderPointOut,
     FutureStableDiffusionXLOut,
     FutureGenerateTextVisionOut,
     FutureMultiGenerateImageOut,
     FutureGenerativeEditImageOut,
+    FutureMixtral8x7BInstructOut,
     FutureMultiGenerativeEditImageOut,
     FutureStableDiffusionXLInpaintOut,
     FutureStableDiffusionXLIPAdapterOut,
     FutureStableDiffusionXLLightningOut,
     FutureStableDiffusionXLControlNetOut,
 )
 
 
-class GenerateText(CoreNode):
+class RunCode(CoreNode[RunCodeOut]):
+    """
+    Evaluate code using a code interpreter.
+
+    https://substrate.run/library#RunCode
+    """
+
+    def __init__(self, args: RunCodeIn, hide: bool = False):
+        """
+        Input arguments: `code`, `args` (optional), `language` (optional)
+
+        Output fields: `future.output` (optional), `future.json_output`, `future.error` (optional)
+
+        https://substrate.run/library#RunCode
+        """
+        super().__init__(hide=hide, out_type=RunCodeOut, **args)
+        self.node = "RunCode"
+
+    @property
+    def future(self) -> FutureRunCodeOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.output` (optional), `future.json_output`, `future.error` (optional)
+
+        https://substrate.run/library#RunCode
+        """
+        return super().future  # type: ignore
+
+
+class GenerateText(CoreNode[GenerateTextOut]):
     """
     Generate text using a language model.
 
     https://substrate.run/library#GenerateText
     """
 
     def __init__(self, args: GenerateTextIn, hide: bool = False):
         """
         Input arguments: `prompt`, `temperature` (optional), `max_tokens` (optional), `node` (optional)
 
         Output fields: `future.text`
 
         https://substrate.run/library#GenerateText
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=GenerateTextOut, **args)
         self.node = "GenerateText"
 
     @property
-    def out_type(self) -> Type[GenerateTextOut]:
-        return GenerateTextOut
-
-    @property
     def future(self) -> FutureGenerateTextOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.text`
 
         https://substrate.run/library#GenerateText
         """
         return super().future  # type: ignore
 
 
-class MultiGenerateText(CoreNode):
+class MultiGenerateText(CoreNode[MultiGenerateTextOut]):
     """
     Generate multiple text choices using a language model.
 
     https://substrate.run/library#MultiGenerateText
     """
 
     def __init__(self, args: MultiGenerateTextIn, hide: bool = False):
         """
-        Input arguments: `prompt` (optional), `batch_prompts` (optional), `num_choices` (optional), `temperature` (optional), `max_tokens` (optional), `node` (optional)
+        Input arguments: `prompt`, `num_choices`, `temperature` (optional), `max_tokens` (optional), `node` (optional)
 
-        Output fields: `future.outputs`
+        Output fields: `future.choices`
 
         https://substrate.run/library#MultiGenerateText
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=MultiGenerateTextOut, **args)
         self.node = "MultiGenerateText"
 
     @property
-    def out_type(self) -> Type[MultiGenerateTextOut]:
-        return MultiGenerateTextOut
+    def future(self) -> FutureMultiGenerateTextOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.choices`
+
+        https://substrate.run/library#MultiGenerateText
+        """
+        return super().future  # type: ignore
+
+
+class BatchGenerateText(CoreNode[BatchGenerateTextOut]):
+    """
+    Generate text for multiple prompts in batch using a language model.
+
+    https://substrate.run/library#BatchGenerateText
+    """
+
+    def __init__(self, args: BatchGenerateTextIn, hide: bool = False):
+        """
+        Input arguments: `prompts`, `temperature` (optional), `max_tokens` (optional), `node` (optional)
+
+        Output fields: `future.outputs`
+
+        https://substrate.run/library#BatchGenerateText
+        """
+        super().__init__(hide=hide, out_type=BatchGenerateTextOut, **args)
+        self.node = "BatchGenerateText"
 
     @property
-    def future(self) -> FutureMultiGenerateTextOut:  # type: ignore
+    def future(self) -> FutureBatchGenerateTextOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.outputs`
 
-        https://substrate.run/library#MultiGenerateText
+        https://substrate.run/library#BatchGenerateText
+        """
+        return super().future  # type: ignore
+
+
+class BatchGenerateJSON(CoreNode[BatchGenerateJSONOut]):
+    """
+    Generate JSON for multiple prompts in batch using a language model.
+
+    https://substrate.run/library#BatchGenerateJSON
+    """
+
+    def __init__(self, args: BatchGenerateJSONIn, hide: bool = False):
+        """
+        Input arguments: `prompts`, `json_schema`, `temperature` (optional), `max_tokens` (optional), `node` (optional)
+
+        Output fields: `future.outputs`
+
+        https://substrate.run/library#BatchGenerateJSON
+        """
+        super().__init__(hide=hide, out_type=BatchGenerateJSONOut, **args)
+        self.node = "BatchGenerateJSON"
+
+    @property
+    def future(self) -> FutureBatchGenerateJSONOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.outputs`
+
+        https://substrate.run/library#BatchGenerateJSON
         """
         return super().future  # type: ignore
 
 
-class GenerateJSON(CoreNode):
+class GenerateJSON(CoreNode[GenerateJSONOut]):
     """
     Generate JSON using a language model.
 
     https://substrate.run/library#GenerateJSON
     """
 
     def __init__(self, args: GenerateJSONIn, hide: bool = False):
         """
         Input arguments: `prompt`, `json_schema`, `temperature` (optional), `max_tokens` (optional), `node` (optional)
 
         Output fields: `future.json_object`
 
         https://substrate.run/library#GenerateJSON
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=GenerateJSONOut, **args)
         self.node = "GenerateJSON"
 
     @property
-    def out_type(self) -> Type[GenerateJSONOut]:
-        return GenerateJSONOut
-
-    @property
     def future(self) -> FutureGenerateJSONOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.json_object`
 
         https://substrate.run/library#GenerateJSON
         """
         return super().future  # type: ignore
 
 
-class MultiGenerateJSON(CoreNode):
+class MultiGenerateJSON(CoreNode[MultiGenerateJSONOut]):
     """
     Generate multiple JSON choices using a language model.
 
     https://substrate.run/library#MultiGenerateJSON
     """
 
     def __init__(self, args: MultiGenerateJSONIn, hide: bool = False):
         """
-        Input arguments: `prompt` (optional), `json_schema`, `batch_prompts` (optional), `num_choices` (optional), `temperature` (optional), `max_tokens` (optional), `node` (optional)
+        Input arguments: `prompt`, `json_schema`, `num_choices`, `temperature` (optional), `max_tokens` (optional), `node` (optional)
 
-        Output fields: `future.outputs`
+        Output fields: `future.choices`
 
         https://substrate.run/library#MultiGenerateJSON
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=MultiGenerateJSONOut, **args)
         self.node = "MultiGenerateJSON"
 
     @property
-    def out_type(self) -> Type[MultiGenerateJSONOut]:
-        return MultiGenerateJSONOut
-
-    @property
     def future(self) -> FutureMultiGenerateJSONOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.outputs`
+        Output fields: `future.choices`
 
         https://substrate.run/library#MultiGenerateJSON
         """
         return super().future  # type: ignore
 
 
-class GenerateTextVision(CoreNode):
+class GenerateTextVision(CoreNode[GenerateTextVisionOut]):
     """
     Generate text with image input.
 
     https://substrate.run/library#GenerateTextVision
     """
 
     def __init__(self, args: GenerateTextVisionIn, hide: bool = False):
         """
         Input arguments: `prompt`, `image_uris`, `max_tokens` (optional), `node` (optional)
 
         Output fields: `future.text`
 
         https://substrate.run/library#GenerateTextVision
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=GenerateTextVisionOut, **args)
         self.node = "GenerateTextVision"
 
     @property
-    def out_type(self) -> Type[GenerateTextVisionOut]:
-        return GenerateTextVisionOut
-
-    @property
     def future(self) -> FutureGenerateTextVisionOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.text`
 
         https://substrate.run/library#GenerateTextVision
         """
         return super().future  # type: ignore
 
 
-class Mistral7BInstruct(CoreNode):
+class Mistral7BInstruct(CoreNode[Mistral7BInstructOut]):
     """
     Generate text using [Mistral 7B Instruct](https://mistral.ai/news/announcing-mistral-7b).
 
     https://substrate.run/library#Mistral7BInstruct
     """
 
     def __init__(self, args: Mistral7BInstructIn, hide: bool = False):
         """
-        Input arguments: `prompt` (optional), `num_choices` (optional), `json_schema` (optional), `batch_prompts` (optional), `temperature` (optional), `max_tokens` (optional)
+        Input arguments: `prompt`, `num_choices` (optional), `json_schema` (optional), `temperature` (optional), `max_tokens` (optional)
 
-        Output fields: `future.outputs`
+        Output fields: `future.choices`
 
         https://substrate.run/library#Mistral7BInstruct
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=Mistral7BInstructOut, **args)
         self.node = "Mistral7BInstruct"
 
     @property
-    def out_type(self) -> Type[Mistral7BInstructOut]:
-        return Mistral7BInstructOut
-
-    @property
     def future(self) -> FutureMistral7BInstructOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.outputs`
+        Output fields: `future.choices`
 
         https://substrate.run/library#Mistral7BInstruct
         """
         return super().future  # type: ignore
 
 
-class Firellava13B(CoreNode):
+class Mixtral8x7BInstruct(CoreNode[Mixtral8x7BInstructOut]):
+    """
+    Generate text using instruct-tuned [Mixtral 8x7B](https://mistral.ai/news/mixtral-of-experts/).
+
+    https://substrate.run/library#Mixtral8x7BInstruct
+    """
+
+    def __init__(self, args: Mixtral8x7BInstructIn, hide: bool = False):
+        """
+        Input arguments: `prompt`, `num_choices` (optional), `json_schema` (optional), `temperature` (optional), `max_tokens` (optional)
+
+        Output fields: `future.choices`
+
+        https://substrate.run/library#Mixtral8x7BInstruct
+        """
+        super().__init__(hide=hide, out_type=Mixtral8x7BInstructOut, **args)
+        self.node = "Mixtral8x7BInstruct"
+
+    @property
+    def future(self) -> FutureMixtral8x7BInstructOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.choices`
+
+        https://substrate.run/library#Mixtral8x7BInstruct
+        """
+        return super().future  # type: ignore
+
+
+class Llama3Instruct8B(CoreNode[Llama3Instruct8BOut]):
+    """
+    Generate text using instruct-tuned [Llama 3 8B](https://llama.meta.com/llama3/).
+
+    https://substrate.run/library#Llama3Instruct8B
+    """
+
+    def __init__(self, args: Llama3Instruct8BIn, hide: bool = False):
+        """
+        Input arguments: `prompt`, `num_choices` (optional), `temperature` (optional), `max_tokens` (optional)
+
+        Output fields: `future.choices`
+
+        https://substrate.run/library#Llama3Instruct8B
+        """
+        super().__init__(hide=hide, out_type=Llama3Instruct8BOut, **args)
+        self.node = "Llama3Instruct8B"
+
+    @property
+    def future(self) -> FutureLlama3Instruct8BOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.choices`
+
+        https://substrate.run/library#Llama3Instruct8B
+        """
+        return super().future  # type: ignore
+
+
+class Llama3Instruct70B(CoreNode[Llama3Instruct70BOut]):
+    """
+    Generate text using instruct-tuned [Llama 3 70B](https://llama.meta.com/llama3/).
+
+    https://substrate.run/library#Llama3Instruct70B
+    """
+
+    def __init__(self, args: Llama3Instruct70BIn, hide: bool = False):
+        """
+        Input arguments: `prompt`, `num_choices` (optional), `temperature` (optional), `max_tokens` (optional)
+
+        Output fields: `future.choices`
+
+        https://substrate.run/library#Llama3Instruct70B
+        """
+        super().__init__(hide=hide, out_type=Llama3Instruct70BOut, **args)
+        self.node = "Llama3Instruct70B"
+
+    @property
+    def future(self) -> FutureLlama3Instruct70BOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        Output fields: `future.choices`
+
+        https://substrate.run/library#Llama3Instruct70B
+        """
+        return super().future  # type: ignore
+
+
+class Firellava13B(CoreNode[Firellava13BOut]):
     """
     Generate text with image input using [FireLLaVA 13B](https://fireworks.ai/blog/firellava-the-first-commercially-permissive-oss-llava-model).
 
     https://substrate.run/library#Firellava13B
     """
 
     def __init__(self, args: Firellava13BIn, hide: bool = False):
         """
         Input arguments: `prompt`, `image_uris`, `max_tokens` (optional)
 
         Output fields: `future.text`
 
         https://substrate.run/library#Firellava13B
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=Firellava13BOut, **args)
         self.node = "Firellava13B"
 
     @property
-    def out_type(self) -> Type[Firellava13BOut]:
-        return Firellava13BOut
-
-    @property
     def future(self) -> FutureFirellava13BOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.text`
 
         https://substrate.run/library#Firellava13B
         """
         return super().future  # type: ignore
 
 
-class GenerateImage(CoreNode):
+class GenerateImage(CoreNode[GenerateImageOut]):
     """
     Generate an image.
 
     https://substrate.run/library#GenerateImage
     """
 
     def __init__(self, args: GenerateImageIn, hide: bool = False):
         """
         Input arguments: `prompt`, `store` (optional), `node` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#GenerateImage
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=GenerateImageOut, **args)
         self.node = "GenerateImage"
 
     @property
-    def out_type(self) -> Type[GenerateImageOut]:
-        return GenerateImageOut
-
-    @property
     def future(self) -> FutureGenerateImageOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#GenerateImage
         """
         return super().future  # type: ignore
 
 
-class MultiGenerateImage(CoreNode):
+class MultiGenerateImage(CoreNode[MultiGenerateImageOut]):
     """
     Generate multiple images.
 
     https://substrate.run/library#MultiGenerateImage
     """
 
     def __init__(self, args: MultiGenerateImageIn, hide: bool = False):
         """
         Input arguments: `prompt`, `num_images`, `store` (optional), `node` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#MultiGenerateImage
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=MultiGenerateImageOut, **args)
         self.node = "MultiGenerateImage"
 
     @property
-    def out_type(self) -> Type[MultiGenerateImageOut]:
-        return MultiGenerateImageOut
-
-    @property
     def future(self) -> FutureMultiGenerateImageOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#MultiGenerateImage
         """
         return super().future  # type: ignore
 
 
-class GenerativeEditImage(CoreNode):
+class GenerativeEditImage(CoreNode[GenerativeEditImageOut]):
     """
     Edit an image using image generation.
 
     https://substrate.run/library#GenerativeEditImage
     """
 
     def __init__(self, args: GenerativeEditImageIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `prompt`, `mask_image_uri` (optional), `store` (optional), `node` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#GenerativeEditImage
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=GenerativeEditImageOut, **args)
         self.node = "GenerativeEditImage"
 
     @property
-    def out_type(self) -> Type[GenerativeEditImageOut]:
-        return GenerativeEditImageOut
-
-    @property
     def future(self) -> FutureGenerativeEditImageOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#GenerativeEditImage
         """
         return super().future  # type: ignore
 
 
-class MultiGenerativeEditImage(CoreNode):
+class MultiGenerativeEditImage(CoreNode[MultiGenerativeEditImageOut]):
     """
     Edit multiple images using image generation.
 
     https://substrate.run/library#MultiGenerativeEditImage
     """
 
     def __init__(self, args: MultiGenerativeEditImageIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `prompt`, `mask_image_uri` (optional), `num_images`, `store` (optional), `node` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#MultiGenerativeEditImage
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=MultiGenerativeEditImageOut, **args)
         self.node = "MultiGenerativeEditImage"
 
     @property
-    def out_type(self) -> Type[MultiGenerativeEditImageOut]:
-        return MultiGenerativeEditImageOut
-
-    @property
     def future(self) -> FutureMultiGenerativeEditImageOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#MultiGenerativeEditImage
         """
         return super().future  # type: ignore
 
 
-class StableDiffusionXL(CoreNode):
+class StableDiffusionXL(CoreNode[StableDiffusionXLOut]):
     """
     Generate an image using [Stable Diffusion XL](https://arxiv.org/abs/2307.01952).
 
     https://substrate.run/library#StableDiffusionXL
     """
 
     def __init__(self, args: StableDiffusionXLIn, hide: bool = False):
         """
         Input arguments: `prompt`, `negative_prompt` (optional), `steps` (optional), `num_images`, `store` (optional), `height` (optional), `width` (optional), `seeds` (optional), `guidance_scale` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXL
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=StableDiffusionXLOut, **args)
         self.node = "StableDiffusionXL"
 
     @property
-    def out_type(self) -> Type[StableDiffusionXLOut]:
-        return StableDiffusionXLOut
-
-    @property
     def future(self) -> FutureStableDiffusionXLOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXL
         """
         return super().future  # type: ignore
 
 
-class StableDiffusionXLLightning(CoreNode):
+class StableDiffusionXLLightning(CoreNode[StableDiffusionXLLightningOut]):
     """
     Generate an image using [Stable Diffusion XL Lightning](https://arxiv.org/abs/2402.13929).
 
     https://substrate.run/library#StableDiffusionXLLightning
     """
 
     def __init__(self, args: StableDiffusionXLLightningIn, hide: bool = False):
         """
         Input arguments: `prompt`, `negative_prompt` (optional), `num_images` (optional), `store` (optional), `height` (optional), `width` (optional), `seeds` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXLLightning
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=StableDiffusionXLLightningOut, **args)
         self.node = "StableDiffusionXLLightning"
 
     @property
-    def out_type(self) -> Type[StableDiffusionXLLightningOut]:
-        return StableDiffusionXLLightningOut
-
-    @property
     def future(self) -> FutureStableDiffusionXLLightningOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXLLightning
         """
         return super().future  # type: ignore
 
 
-class StableDiffusionXLInpaint(CoreNode):
+class StableDiffusionXLInpaint(CoreNode[StableDiffusionXLInpaintOut]):
     """
     Edit an image using [Stable Diffusion XL](https://arxiv.org/abs/2307.01952). Supports inpainting (edit part of the image with a mask) and image-to-image (edit the full image).
 
     https://substrate.run/library#StableDiffusionXLInpaint
     """
 
     def __init__(self, args: StableDiffusionXLInpaintIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `prompt`, `mask_image_uri` (optional), `num_images`, `output_resolution` (optional), `negative_prompt` (optional), `store` (optional), `strength` (optional), `seeds` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXLInpaint
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=StableDiffusionXLInpaintOut, **args)
         self.node = "StableDiffusionXLInpaint"
 
     @property
-    def out_type(self) -> Type[StableDiffusionXLInpaintOut]:
-        return StableDiffusionXLInpaintOut
-
-    @property
     def future(self) -> FutureStableDiffusionXLInpaintOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXLInpaint
         """
         return super().future  # type: ignore
 
 
-class StableDiffusionXLControlNet(CoreNode):
+class StableDiffusionXLControlNet(CoreNode[StableDiffusionXLControlNetOut]):
     """
     Generate an image with generation structured by an input image, using Stable Diffusion XL with [ControlNet](https://arxiv.org/abs/2302.05543).
 
     https://substrate.run/library#StableDiffusionXLControlNet
     """
 
     def __init__(self, args: StableDiffusionXLControlNetIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `control_method`, `prompt`, `num_images`, `output_resolution` (optional), `negative_prompt` (optional), `store` (optional), `conditioning_scale` (optional), `seeds` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXLControlNet
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=StableDiffusionXLControlNetOut, **args)
         self.node = "StableDiffusionXLControlNet"
 
     @property
-    def out_type(self) -> Type[StableDiffusionXLControlNetOut]:
-        return StableDiffusionXLControlNetOut
-
-    @property
     def future(self) -> FutureStableDiffusionXLControlNetOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXLControlNet
         """
         return super().future  # type: ignore
 
 
-class StableDiffusionXLIPAdapter(CoreNode):
+class StableDiffusionXLIPAdapter(CoreNode[StableDiffusionXLIPAdapterOut]):
     """
     Generate an image with an image prompt, using Stable Diffusion XL with [IP-Adapter](https://arxiv.org/abs/2308.06721).
 
     https://substrate.run/library#StableDiffusionXLIPAdapter
     """
 
     def __init__(self, args: StableDiffusionXLIPAdapterIn, hide: bool = False):
         """
         Input arguments: `prompt`, `image_prompt_uri` (optional), `num_images`, `ip_adapter_scale` (optional), `negative_prompt` (optional), `store` (optional), `width` (optional), `height` (optional), `seeds` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXLIPAdapter
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=StableDiffusionXLIPAdapterOut, **args)
         self.node = "StableDiffusionXLIPAdapter"
 
     @property
-    def out_type(self) -> Type[StableDiffusionXLIPAdapterOut]:
-        return StableDiffusionXLIPAdapterOut
-
-    @property
     def future(self) -> FutureStableDiffusionXLIPAdapterOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXLIPAdapter
         """
         return super().future  # type: ignore
 
 
-class TranscribeMedia(CoreNode):
+class TranscribeMedia(CoreNode[TranscribeMediaOut]):
     """
     Transcribe speech in an audio or video file.
 
     https://substrate.run/library#TranscribeMedia
     """
 
     def __init__(self, args: TranscribeMediaIn, hide: bool = False):
         """
         Input arguments: `audio_uri`, `prompt` (optional), `language` (optional), `segment` (optional), `align` (optional), `diarize` (optional), `suggest_chapters` (optional)
 
         Output fields: `future.text`, `future.segments` (optional), `future.chapters` (optional)
 
         https://substrate.run/library#TranscribeMedia
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=TranscribeMediaOut, **args)
         self.node = "TranscribeMedia"
 
     @property
-    def out_type(self) -> Type[TranscribeMediaOut]:
-        return TranscribeMediaOut
-
-    @property
     def future(self) -> FutureTranscribeMediaOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.text`, `future.segments` (optional), `future.chapters` (optional)
 
         https://substrate.run/library#TranscribeMedia
         """
         return super().future  # type: ignore
 
 
-class GenerateSpeech(CoreNode):
+class GenerateSpeech(CoreNode[GenerateSpeechOut]):
     """
     Generate speech from text.
 
     https://substrate.run/library#GenerateSpeech
     """
 
     def __init__(self, args: GenerateSpeechIn, hide: bool = False):
         """
         Input arguments: `text`, `store` (optional), `node` (optional)
 
         Output fields: `future.audio_uri`
 
         https://substrate.run/library#GenerateSpeech
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=GenerateSpeechOut, **args)
         self.node = "GenerateSpeech"
 
     @property
-    def out_type(self) -> Type[GenerateSpeechOut]:
-        return GenerateSpeechOut
-
-    @property
     def future(self) -> FutureGenerateSpeechOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.audio_uri`
 
         https://substrate.run/library#GenerateSpeech
         """
         return super().future  # type: ignore
 
 
-class XTTSV2(CoreNode):
+class XTTSV2(CoreNode[XTTSV2Out]):
     """
     Generate speech from text using [XTTS v2](https://docs.coqui.ai/en/latest/models/xtts.html).
 
     https://substrate.run/library#XTTSV2
     """
 
     def __init__(self, args: XTTSV2In, hide: bool = False):
         """
         Input arguments: `text`, `audio_uri` (optional), `language` (optional), `store` (optional)
 
         Output fields: `future.audio_uri`
 
         https://substrate.run/library#XTTSV2
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=XTTSV2Out, **args)
         self.node = "XTTSV2"
 
     @property
-    def out_type(self) -> Type[XTTSV2Out]:
-        return XTTSV2Out
-
-    @property
     def future(self) -> FutureXTTSV2Out:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.audio_uri`
 
         https://substrate.run/library#XTTSV2
         """
         return super().future  # type: ignore
 
 
-class RemoveBackground(CoreNode):
+class RemoveBackground(CoreNode[RemoveBackgroundOut]):
     """
     Remove the background from an image, with the option to return the foreground as a mask.
 
     https://substrate.run/library#RemoveBackground
     """
 
     def __init__(self, args: RemoveBackgroundIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `return_mask` (optional), `background_color` (optional), `store` (optional), `node` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#RemoveBackground
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=RemoveBackgroundOut, **args)
         self.node = "RemoveBackground"
 
     @property
-    def out_type(self) -> Type[RemoveBackgroundOut]:
-        return RemoveBackgroundOut
-
-    @property
     def future(self) -> FutureRemoveBackgroundOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#RemoveBackground
         """
         return super().future  # type: ignore
 
 
-class FillMask(CoreNode):
+class FillMask(CoreNode[FillMaskOut]):
     """
     Fill (inpaint) part of an image, e.g. to 'remove' an object.
 
     https://substrate.run/library#FillMask
     """
 
     def __init__(self, args: FillMaskIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `mask_image_uri`, `store` (optional), `node` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#FillMask
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=FillMaskOut, **args)
         self.node = "FillMask"
 
     @property
-    def out_type(self) -> Type[FillMaskOut]:
-        return FillMaskOut
-
-    @property
     def future(self) -> FutureFillMaskOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#FillMask
         """
         return super().future  # type: ignore
 
 
-class UpscaleImage(CoreNode):
+class UpscaleImage(CoreNode[UpscaleImageOut]):
     """
     Upscale an image.
 
     https://substrate.run/library#UpscaleImage
     """
 
     def __init__(self, args: UpscaleImageIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `store` (optional), `node` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#UpscaleImage
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=UpscaleImageOut, **args)
         self.node = "UpscaleImage"
 
     @property
-    def out_type(self) -> Type[UpscaleImageOut]:
-        return UpscaleImageOut
-
-    @property
     def future(self) -> FutureUpscaleImageOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#UpscaleImage
         """
         return super().future  # type: ignore
 
 
-class SegmentUnderPoint(CoreNode):
+class SegmentUnderPoint(CoreNode[SegmentUnderPointOut]):
     """
     Segment an image under a point and return the segment.
 
     https://substrate.run/library#SegmentUnderPoint
     """
 
     def __init__(self, args: SegmentUnderPointIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `point`, `store` (optional), `node` (optional)
 
         Output fields: `future.mask_image_uri`
 
         https://substrate.run/library#SegmentUnderPoint
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=SegmentUnderPointOut, **args)
         self.node = "SegmentUnderPoint"
 
     @property
-    def out_type(self) -> Type[SegmentUnderPointOut]:
-        return SegmentUnderPointOut
-
-    @property
     def future(self) -> FutureSegmentUnderPointOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.mask_image_uri`
 
         https://substrate.run/library#SegmentUnderPoint
         """
         return super().future  # type: ignore
 
 
-class DISISNet(CoreNode):
+class DISISNet(CoreNode[DISISNetOut]):
     """
     Segment image foreground using [DIS IS-Net](https://github.com/xuebinqin/DIS).
 
     https://substrate.run/library#DISISNet
     """
 
     def __init__(self, args: DISISNetIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `store` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#DISISNet
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=DISISNetOut, **args)
         self.node = "DISISNet"
 
     @property
-    def out_type(self) -> Type[DISISNetOut]:
-        return DISISNetOut
-
-    @property
     def future(self) -> FutureDISISNetOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#DISISNet
         """
         return super().future  # type: ignore
 
 
-class BigLaMa(CoreNode):
+class BigLaMa(CoreNode[BigLaMaOut]):
     """
     Inpaint a mask using [LaMa](https://github.com/advimman/lama).
 
     https://substrate.run/library#BigLaMa
     """
 
     def __init__(self, args: BigLaMaIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `mask_image_uri`, `store` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#BigLaMa
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=BigLaMaOut, **args)
         self.node = "BigLaMa"
 
     @property
-    def out_type(self) -> Type[BigLaMaOut]:
-        return BigLaMaOut
-
-    @property
     def future(self) -> FutureBigLaMaOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#BigLaMa
         """
         return super().future  # type: ignore
 
 
-class RealESRGAN(CoreNode):
+class RealESRGAN(CoreNode[RealESRGANOut]):
     """
     Upscale an image using [RealESRGAN](https://github.com/xinntao/Real-ESRGAN).
 
     https://substrate.run/library#RealESRGAN
     """
 
     def __init__(self, args: RealESRGANIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `store` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#RealESRGAN
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=RealESRGANOut, **args)
         self.node = "RealESRGAN"
 
     @property
-    def out_type(self) -> Type[RealESRGANOut]:
-        return RealESRGANOut
-
-    @property
     def future(self) -> FutureRealESRGANOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#RealESRGAN
         """
         return super().future  # type: ignore
 
 
-class SegmentAnything(CoreNode):
+class SegmentAnything(CoreNode[SegmentAnythingOut]):
     """
     Segment an image using [SegmentAnything](https://github.com/facebookresearch/segment-anything).
 
     https://substrate.run/library#SegmentAnything
     """
 
     def __init__(self, args: SegmentAnythingIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `point_prompts` (optional), `box_prompts` (optional), `store` (optional)
 
         Output fields: `future.mask_image_uri`
 
         https://substrate.run/library#SegmentAnything
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=SegmentAnythingOut, **args)
         self.node = "SegmentAnything"
 
     @property
-    def out_type(self) -> Type[SegmentAnythingOut]:
-        return SegmentAnythingOut
-
-    @property
     def future(self) -> FutureSegmentAnythingOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.mask_image_uri`
 
         https://substrate.run/library#SegmentAnything
         """
         return super().future  # type: ignore
 
 
-class EmbedText(CoreNode):
+class EmbedText(CoreNode[EmbedTextOut]):
     """
     Generate embedding for a text document.
 
     https://substrate.run/library#EmbedText
     """
 
     def __init__(self, args: EmbedTextIn, hide: bool = False):
         """
-        Input arguments: `text`, `store` (optional), `metadata` (optional), `embedded_metadata_keys` (optional), `doc_id` (optional), `node` (optional)
+        Input arguments: `text`, `collection_name` (optional), `metadata` (optional), `embedded_metadata_keys` (optional), `doc_id` (optional), `model` (optional)
 
         Output fields: `future.embedding`
 
         https://substrate.run/library#EmbedText
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=EmbedTextOut, **args)
         self.node = "EmbedText"
 
     @property
-    def out_type(self) -> Type[EmbedTextOut]:
-        return EmbedTextOut
-
-    @property
     def future(self) -> FutureEmbedTextOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.embedding`
 
         https://substrate.run/library#EmbedText
         """
         return super().future  # type: ignore
 
 
-class MultiEmbedText(CoreNode):
+class MultiEmbedText(CoreNode[MultiEmbedTextOut]):
     """
     Generate embeddings for multiple text documents.
 
     https://substrate.run/library#MultiEmbedText
     """
 
     def __init__(self, args: MultiEmbedTextIn, hide: bool = False):
         """
-        Input arguments: `items`, `store` (optional), `embedded_metadata_keys` (optional), `node` (optional)
+        Input arguments: `items`, `collection_name` (optional), `embedded_metadata_keys` (optional), `model` (optional)
 
         Output fields: `future.embeddings`
 
         https://substrate.run/library#MultiEmbedText
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=MultiEmbedTextOut, **args)
         self.node = "MultiEmbedText"
 
     @property
-    def out_type(self) -> Type[MultiEmbedTextOut]:
-        return MultiEmbedTextOut
-
-    @property
     def future(self) -> FutureMultiEmbedTextOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.embeddings`
 
         https://substrate.run/library#MultiEmbedText
         """
         return super().future  # type: ignore
 
 
-class EmbedImage(CoreNode):
+class EmbedImage(CoreNode[EmbedImageOut]):
     """
     Generate embedding for an image.
 
     https://substrate.run/library#EmbedImage
     """
 
     def __init__(self, args: EmbedImageIn, hide: bool = False):
         """
-        Input arguments: `image_uri`, `store` (optional), `doc_id` (optional), `node` (optional)
+        Input arguments: `image_uri`, `collection_name` (optional), `doc_id` (optional), `model` (optional)
 
         Output fields: `future.embedding`
 
         https://substrate.run/library#EmbedImage
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=EmbedImageOut, **args)
         self.node = "EmbedImage"
 
     @property
-    def out_type(self) -> Type[EmbedImageOut]:
-        return EmbedImageOut
-
-    @property
     def future(self) -> FutureEmbedImageOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.embedding`
 
         https://substrate.run/library#EmbedImage
         """
         return super().future  # type: ignore
 
 
-class MultiEmbedImage(CoreNode):
+class MultiEmbedImage(CoreNode[MultiEmbedImageOut]):
     """
     Generate embeddings for multiple images.
 
     https://substrate.run/library#MultiEmbedImage
     """
 
     def __init__(self, args: MultiEmbedImageIn, hide: bool = False):
         """
-        Input arguments: `items`, `store` (optional), `node` (optional)
+        Input arguments: `items`, `collection_name` (optional), `model` (optional)
 
         Output fields: `future.embeddings`
 
         https://substrate.run/library#MultiEmbedImage
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=MultiEmbedImageOut, **args)
         self.node = "MultiEmbedImage"
 
     @property
-    def out_type(self) -> Type[MultiEmbedImageOut]:
-        return MultiEmbedImageOut
-
-    @property
     def future(self) -> FutureMultiEmbedImageOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.embeddings`
 
         https://substrate.run/library#MultiEmbedImage
         """
         return super().future  # type: ignore
 
 
-class JinaV2(CoreNode):
+class JinaV2(CoreNode[JinaV2Out]):
     """
     Generate embeddings for multiple text documents using [Jina Embeddings 2](https://arxiv.org/abs/2310.19923).
 
     https://substrate.run/library#JinaV2
     """
 
     def __init__(self, args: JinaV2In, hide: bool = False):
         """
-        Input arguments: `items`, `store` (optional), `embedded_metadata_keys` (optional)
+        Input arguments: `items`, `collection_name` (optional), `embedded_metadata_keys` (optional)
 
         Output fields: `future.embeddings`
 
         https://substrate.run/library#JinaV2
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=JinaV2Out, **args)
         self.node = "JinaV2"
 
     @property
-    def out_type(self) -> Type[JinaV2Out]:
-        return JinaV2Out
-
-    @property
     def future(self) -> FutureJinaV2Out:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.embeddings`
 
         https://substrate.run/library#JinaV2
         """
         return super().future  # type: ignore
 
 
-class CLIP(CoreNode):
+class CLIP(CoreNode[CLIPOut]):
     """
     Generate embeddings for text or images using [CLIP](https://openai.com/research/clip).
 
     https://substrate.run/library#CLIP
     """
 
     def __init__(self, args: CLIPIn, hide: bool = False):
         """
-        Input arguments: `items`, `store` (optional)
+        Input arguments: `items`, `collection_name` (optional), `embedded_metadata_keys` (optional)
 
         Output fields: `future.embeddings`
 
         https://substrate.run/library#CLIP
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=CLIPOut, **args)
         self.node = "CLIP"
 
     @property
-    def out_type(self) -> Type[CLIPOut]:
-        return CLIPOut
-
-    @property
     def future(self) -> FutureCLIPOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.embeddings`
 
         https://substrate.run/library#CLIP
         """
         return super().future  # type: ignore
 
 
-class CreateVectorStore(CoreNode):
+class CreateVectorStore(CoreNode[CreateVectorStoreOut]):
     """
     Create a vector store for storing and querying embeddings.
 
     https://substrate.run/library#CreateVectorStore
     """
 
     def __init__(self, args: CreateVectorStoreIn, hide: bool = False):
         """
-        Input arguments: `name`, `model`, `m` (optional), `ef_construction` (optional), `metric` (optional)
+        Input arguments: `collection_name`, `model`, `m` (optional), `ef_construction` (optional), `metric` (optional)
 
-        Output fields: `future.name`, `future.model`, `future.m`, `future.ef_construction`, `future.metric`
+        Output fields: `future.collection_name`, `future.model`, `future.m`, `future.ef_construction`, `future.metric`
 
         https://substrate.run/library#CreateVectorStore
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=CreateVectorStoreOut, **args)
         self.node = "CreateVectorStore"
 
     @property
-    def out_type(self) -> Type[CreateVectorStoreOut]:
-        return CreateVectorStoreOut
-
-    @property
     def future(self) -> FutureCreateVectorStoreOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.name`, `future.model`, `future.m`, `future.ef_construction`, `future.metric`
+        Output fields: `future.collection_name`, `future.model`, `future.m`, `future.ef_construction`, `future.metric`
 
         https://substrate.run/library#CreateVectorStore
         """
         return super().future  # type: ignore
 
 
-class ListVectorStores(CoreNode):
+class ListVectorStores(CoreNode[ListVectorStoresOut]):
     """
     List all vector stores.
 
     https://substrate.run/library#ListVectorStores
     """
 
     def __init__(self, args: ListVectorStoresIn, hide: bool = False):
         """
         Input arguments:
 
-        Output fields: `future.stores` (optional)
+        Output fields: `future.items` (optional)
 
         https://substrate.run/library#ListVectorStores
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=ListVectorStoresOut, **args)
         self.node = "ListVectorStores"
 
     @property
-    def out_type(self) -> Type[ListVectorStoresOut]:
-        return ListVectorStoresOut
-
-    @property
     def future(self) -> FutureListVectorStoresOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.stores` (optional)
+        Output fields: `future.items` (optional)
 
         https://substrate.run/library#ListVectorStores
         """
         return super().future  # type: ignore
 
 
-class DeleteVectorStore(CoreNode):
+class DeleteVectorStore(CoreNode[DeleteVectorStoreOut]):
     """
     Delete a vector store.
 
     https://substrate.run/library#DeleteVectorStore
     """
 
     def __init__(self, args: DeleteVectorStoreIn, hide: bool = False):
         """
-        Input arguments: `name`, `model`
+        Input arguments: `collection_name`, `model`
 
-        Output fields: `future.name`, `future.model`
+        Output fields: `future.collection_name`, `future.model`
 
         https://substrate.run/library#DeleteVectorStore
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=DeleteVectorStoreOut, **args)
         self.node = "DeleteVectorStore"
 
     @property
-    def out_type(self) -> Type[DeleteVectorStoreOut]:
-        return DeleteVectorStoreOut
-
-    @property
     def future(self) -> FutureDeleteVectorStoreOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.name`, `future.model`
+        Output fields: `future.collection_name`, `future.model`
 
         https://substrate.run/library#DeleteVectorStore
         """
         return super().future  # type: ignore
 
 
-class QueryVectorStore(CoreNode):
+class QueryVectorStore(CoreNode[QueryVectorStoreOut]):
     """
     Query a vector store for similar vectors.
 
     https://substrate.run/library#QueryVectorStore
     """
 
     def __init__(self, args: QueryVectorStoreIn, hide: bool = False):
         """
-        Input arguments: `name`, `model`, `query_strings` (optional), `query_image_uris` (optional), `query_vectors` (optional), `query_ids` (optional), `top_k` (optional), `ef_search` (optional), `include_values` (optional), `include_metadata` (optional), `filters` (optional), `metric` (optional)
+        Input arguments: `collection_name`, `model`, `query_strings` (optional), `query_image_uris` (optional), `query_vectors` (optional), `query_ids` (optional), `top_k` (optional), `ef_search` (optional), `include_values` (optional), `include_metadata` (optional), `filters` (optional)
 
-        Output fields: `future.results`, `future.name` (optional), `future.model` (optional), `future.metric` (optional)
+        Output fields: `future.results`, `future.collection_name` (optional), `future.model` (optional), `future.metric` (optional)
 
         https://substrate.run/library#QueryVectorStore
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=QueryVectorStoreOut, **args)
         self.node = "QueryVectorStore"
 
     @property
-    def out_type(self) -> Type[QueryVectorStoreOut]:
-        return QueryVectorStoreOut
-
-    @property
     def future(self) -> FutureQueryVectorStoreOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.results`, `future.name` (optional), `future.model` (optional), `future.metric` (optional)
+        Output fields: `future.results`, `future.collection_name` (optional), `future.model` (optional), `future.metric` (optional)
 
         https://substrate.run/library#QueryVectorStore
         """
         return super().future  # type: ignore
 
 
-class FetchVectors(CoreNode):
+class FetchVectors(CoreNode[FetchVectorsOut]):
     """
     Fetch vectors from a vector store.
 
     https://substrate.run/library#FetchVectors
     """
 
     def __init__(self, args: FetchVectorsIn, hide: bool = False):
         """
-        Input arguments: `name`, `model`, `ids`
+        Input arguments: `collection_name`, `model`, `ids`
 
         Output fields: `future.vectors`
 
         https://substrate.run/library#FetchVectors
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=FetchVectorsOut, **args)
         self.node = "FetchVectors"
 
     @property
-    def out_type(self) -> Type[FetchVectorsOut]:
-        return FetchVectorsOut
-
-    @property
     def future(self) -> FutureFetchVectorsOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.vectors`
 
         https://substrate.run/library#FetchVectors
         """
         return super().future  # type: ignore
 
 
-class UpdateVectors(CoreNode):
+class UpdateVectors(CoreNode[UpdateVectorsOut]):
     """
     Update vectors in a vector store.
 
     https://substrate.run/library#UpdateVectors
     """
 
     def __init__(self, args: UpdateVectorsIn, hide: bool = False):
         """
-        Input arguments: `name`, `model`, `vectors`
+        Input arguments: `collection_name`, `model`, `vectors`
 
         Output fields: `future.count`
 
         https://substrate.run/library#UpdateVectors
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=UpdateVectorsOut, **args)
         self.node = "UpdateVectors"
 
     @property
-    def out_type(self) -> Type[UpdateVectorsOut]:
-        return UpdateVectorsOut
-
-    @property
     def future(self) -> FutureUpdateVectorsOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.count`
 
         https://substrate.run/library#UpdateVectors
         """
         return super().future  # type: ignore
 
 
-class DeleteVectors(CoreNode):
+class DeleteVectors(CoreNode[DeleteVectorsOut]):
     """
     Delete vectors in a vector store.
 
     https://substrate.run/library#DeleteVectors
     """
 
     def __init__(self, args: DeleteVectorsIn, hide: bool = False):
         """
-        Input arguments: `name`, `model`, `ids`
+        Input arguments: `collection_name`, `model`, `ids`
 
         Output fields: `future.count`
 
         https://substrate.run/library#DeleteVectors
         """
-        super().__init__(hide=hide, **args)
+        super().__init__(hide=hide, out_type=DeleteVectorsOut, **args)
         self.node = "DeleteVectors"
 
     @property
-    def out_type(self) -> Type[DeleteVectorsOut]:
-        return DeleteVectorsOut
-
-    @property
     def future(self) -> FutureDeleteVectorsOut:  # type: ignore
         """
         Future reference to this node's output.
 
         Output fields: `future.count`
 
         https://substrate.run/library#DeleteVectors
```

### Comparing `substrate-120240416.0.9/substrate/substrate.py` & `substrate-120240418.0.10/substrate/substrate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import json
+import zlib
+import base64
 from typing import Any, Dict
 
 from ._client import APIClient
 from .core.corenode import CoreNode
 from .core.client.graph import Graph
 from .substrate_response import SubstrateResponse
 
@@ -11,45 +14,59 @@
     Substrate client.
     """
 
     def __init__(
         self,
         api_key: str,
         base_url: str = "https://api.substrate.run",
-        backend: str = "v0",
+        backend: str = "v1",
         additional_headers: Dict[str, Any] = {},
     ):
         """
         Initialize the Substrate SDK.
         """
         self.api_key = api_key
         self._client = APIClient(
             api_key=api_key,
             base_url=base_url,
             backend=backend,
             additional_headers=additional_headers,
         )
 
-    def run(self, *nodes: CoreNode, use_requests: bool = False) -> SubstrateResponse:
+    def run(self, *nodes: CoreNode) -> SubstrateResponse:
         """
         Run the given nodes.
         """
-        graph = Graph()
-        for node in nodes:
-            graph.add_node(node)
-        graph_serialized = graph.to_dict()
-        if use_requests:
-            api_response = self._client.post_compose_requests(dag=graph_serialized)
-        else:
-            api_response = self._client.post_compose(dag=graph_serialized)
+        serialized = Substrate.serialize(*nodes)
+        api_response = self._client.post_compose(dag=serialized)
         return SubstrateResponse(api_response=api_response)
 
     async def async_run(self, *nodes: CoreNode) -> SubstrateResponse:
         """
         Asynchronously run the given nodes.
         """
+        serialized = Substrate.serialize(*nodes)
+        api_response = await self._client.async_post_compose(dag=serialized)
+        return SubstrateResponse(api_response=api_response)
+
+    @staticmethod
+    def visualize(*nodes):
+        """
+        Returns a url to visualize the given nodes.
+        """
+        serialized = Substrate.serialize(*nodes)
+        compressed = zlib.compress(json.dumps(serialized).encode("utf-8"), level=9)
+        base64_encoded = base64.b64encode(compressed).decode("utf-8")
+        url_encoded = base64_encoded.replace("+", "-").replace("/", "_").replace("=", "")
+        base_url = "https://explore.substrate.run/s/"
+        return base_url + url_encoded
+
+    @staticmethod
+    def serialize(*nodes):
+        """
+        Serializes the given nodes.
+        """
         graph = Graph()
         for node in nodes:
             graph.add_node(node)
         graph_serialized = graph.to_dict()
-        api_response = await self._client.async_post_compose(dag=graph_serialized)
-        return SubstrateResponse(api_response=api_response)
+        return graph_serialized
```

### Comparing `substrate-120240416.0.9/substrate/substrate_response.py` & `substrate-120240418.0.10/substrate/substrate_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from typing import Any, Dict, Type, TypeVar, Optional
+from typing import Any, Dict, TypeVar, Optional
 
 from ._client import APIResponse
 from .core.corenode import CoreNode
 
-T = TypeVar("T", bound=Any)
+OT = TypeVar("OT", bound=Any)
 
 
 class SubstrateResponse:
     """
     Substrate run response.
     """
 
     def __init__(self, api_response: APIResponse):
         self._api_response = api_response
 
-    def get(self, node: CoreNode, output_type: Type[T]) -> T:
+    def get(self, node: CoreNode[OT]) -> OT:
         """
         Get the output of a specific node.
         """
         if self.json and self.json.get("data"):
             data = self.json["data"]
             if data.get(node.id):
                 node_json = data[node.id]
-                return output_type(**node_json)
+                return node.out_type(**node_json)
         raise ValueError(f"Node {node.id} not found in response")
 
     @property
     def json(self) -> Optional[Dict[str, Any]]:
         """
         The full JSON response.
         """
```

### Comparing `substrate-120240416.0.9/substrate/typeddict_models.py` & `substrate-120240418.0.10/substrate/typeddict_models.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,28 +22,65 @@
     """
     request_id: NotRequired[str]
     """
     A unique identifier for the request.
     """
 
 
+class RunCodeIn(TypedDict):
+    code: NotRequired[str]
+    """
+    Code to execute.
+    """
+    args: NotRequired[List[str]]
+    """
+    List of command line arguments.
+    """
+    language: NotRequired[Literal["python", "typescript", "javascript"]]
+    """
+    Interpreter to use.
+    """
+
+
+class RunCodeOut(TypedDict):
+    output: NotRequired[str]
+    """
+    Contents of `stdout` after executing the code.
+    """
+    json_output: NotRequired[Dict[str, Any]]
+    """
+    `output` as parsed JSON. Print serialized json to `stdout` to receive JSON.
+    """
+    error: NotRequired[str]
+    """
+    Contents of `stderr` after executing the code.
+    """
+
+
 class GenerateTextIn(TypedDict):
     prompt: NotRequired[str]
     """
     Input prompt.
     """
     temperature: NotRequired[float]
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
     Maximum number of tokens to generate.
     """
-    node: NotRequired[Literal["Mistral7BInstruct"]]
+    node: NotRequired[
+        Literal[
+            "Mistral7BInstruct",
+            "Mixtral8x7BInstruct",
+            "Llama3Instruct8B",
+            "Llama3Instruct70B",
+        ]
+    ]
     """
     Selected node.
     """
 
 
 class GenerateTextOut(TypedDict):
     text: NotRequired[str]
@@ -65,15 +102,15 @@
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
     Maximum number of tokens to generate.
     """
-    node: NotRequired[Literal["Mistral7BInstruct"]]
+    node: NotRequired[Literal["Mistral7BInstruct", "Mixtral8x7BInstruct"]]
     """
     Selected node.
     """
 
 
 class GenerateJSONOut(TypedDict):
     json_object: NotRequired[Dict[str, Any]]
@@ -83,92 +120,133 @@
 
 
 class MultiGenerateTextIn(TypedDict):
     prompt: NotRequired[str]
     """
     Input prompt.
     """
-    batch_prompts: NotRequired[List[str]]
-    """
-    Batch input prompts.
-    """
     num_choices: NotRequired[int]
     """
     Number of choices to generate.
     """
     temperature: NotRequired[float]
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
     Maximum number of tokens to generate.
     """
-    node: NotRequired[Literal["Mistral7BInstruct"]]
+    node: NotRequired[
+        Literal[
+            "Mistral7BInstruct",
+            "Mixtral8x7BInstruct",
+            "Llama3Instruct8B",
+            "Llama3Instruct70B",
+        ]
+    ]
     """
     Selected node.
     """
 
 
-class MultiGenerateTextOutput(TypedDict):
+class MultiGenerateTextOut(TypedDict):
     choices: NotRequired[List[GenerateTextOut]]
     """
     Response choices.
     """
 
 
-class MultiGenerateTextOut(TypedDict):
-    outputs: NotRequired[List[MultiGenerateTextOutput]]
+class BatchGenerateTextIn(TypedDict):
+    prompts: NotRequired[List[str]]
     """
-    A single output for `prompt`, or multiple outputs for `batch_prompts`.
+    Batch input prompts.
+    """
+    temperature: NotRequired[float]
+    """
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: NotRequired[int]
+    """
+    Maximum number of tokens to generate.
+    """
+    node: NotRequired[Literal["Mistral7BInstruct"]]
+    """
+    Selected node.
+    """
+
+
+class BatchGenerateTextOut(TypedDict):
+    outputs: NotRequired[List[GenerateTextOut]]
+    """
+    Batch outputs.
     """
 
 
 class MultiGenerateJSONIn(TypedDict):
     prompt: NotRequired[str]
     """
     Input prompt.
     """
     json_schema: NotRequired[Dict[str, Any]]
     """
     JSON schema to guide `json_object` response.
     """
-    batch_prompts: NotRequired[List[str]]
-    """
-    Batch input prompts.
-    """
     num_choices: NotRequired[int]
     """
     Number of choices to generate.
     """
     temperature: NotRequired[float]
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
     Maximum number of tokens to generate.
     """
-    node: NotRequired[Literal["Mistral7BInstruct"]]
+    node: NotRequired[Literal["Mistral7BInstruct", "Mixtral8x7BInstruct"]]
     """
     Selected node.
     """
 
 
-class MultiGenerateJSONOutput(TypedDict):
+class MultiGenerateJSONOut(TypedDict):
     choices: NotRequired[List[GenerateJSONOut]]
     """
     Response choices.
     """
 
 
-class MultiGenerateJSONOut(TypedDict):
-    outputs: NotRequired[List[MultiGenerateJSONOutput]]
+class BatchGenerateJSONIn(TypedDict):
+    prompts: NotRequired[List[str]]
+    """
+    Batch input prompts.
+    """
+    json_schema: NotRequired[Dict[str, Any]]
+    """
+    JSON schema to guide `json_object` response.
+    """
+    temperature: NotRequired[float]
+    """
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: NotRequired[int]
+    """
+    Maximum number of tokens to generate.
+    """
+    node: NotRequired[Literal["Mistral7BInstruct"]]
+    """
+    Selected node.
+    """
+
+
+class BatchGenerateJSONOut(TypedDict):
+    outputs: NotRequired[List[GenerateJSONOut]]
     """
-    A single output for `prompt`, or multiple outputs for `batch_prompts`.
+    Batch outputs.
     """
 
 
 class Mistral7BInstructIn(TypedDict):
     prompt: NotRequired[str]
     """
     Input prompt.
@@ -177,18 +255,14 @@
     """
     Number of choices to generate.
     """
     json_schema: NotRequired[Dict[str, Any]]
     """
     JSON schema to guide response.
     """
-    batch_prompts: NotRequired[List[str]]
-    """
-    Batch input prompts.
-    """
     temperature: NotRequired[float]
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
     Maximum number of tokens to generate.
@@ -202,25 +276,125 @@
     """
     json_object: NotRequired[Dict[str, Any]]
     """
     JSON response, if `json_schema` was provided.
     """
 
 
-class Mistral7BInstructOutput(TypedDict):
+class Mistral7BInstructOut(TypedDict):
     choices: NotRequired[List[Mistral7BInstructChoice]]
     """
     Response choices.
     """
 
 
-class Mistral7BInstructOut(TypedDict):
-    outputs: NotRequired[List[Mistral7BInstructOutput]]
+class Mixtral8x7BInstructIn(TypedDict):
+    prompt: NotRequired[str]
+    """
+    Input prompt.
+    """
+    num_choices: NotRequired[int]
+    """
+    Number of choices to generate.
+    """
+    json_schema: NotRequired[Dict[str, Any]]
+    """
+    JSON schema to guide response.
+    """
+    temperature: NotRequired[float]
+    """
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: NotRequired[int]
+    """
+    Maximum number of tokens to generate.
+    """
+
+
+class Mixtral8x7BChoice(TypedDict):
+    text: NotRequired[str]
     """
-    A single output for `prompt`, or multiple outputs for `batch_prompts`.
+    Text response, if `json_schema` was not provided.
+    """
+    json_object: NotRequired[Dict[str, Any]]
+    """
+    JSON response, if `json_schema` was provided.
+    """
+
+
+class Mixtral8x7BInstructOut(TypedDict):
+    choices: NotRequired[List[Mixtral8x7BChoice]]
+    """
+    Response choices.
+    """
+
+
+class Llama3Instruct8BIn(TypedDict):
+    prompt: NotRequired[str]
+    """
+    Input prompt.
+    """
+    num_choices: NotRequired[int]
+    """
+    Number of choices to generate.
+    """
+    temperature: NotRequired[float]
+    """
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: NotRequired[int]
+    """
+    Maximum number of tokens to generate.
+    """
+
+
+class Llama3Instruct8BChoice(TypedDict):
+    text: NotRequired[str]
+    """
+    Text response.
+    """
+
+
+class Llama3Instruct8BOut(TypedDict):
+    choices: NotRequired[List[Llama3Instruct8BChoice]]
+    """
+    Response choices.
+    """
+
+
+class Llama3Instruct70BIn(TypedDict):
+    prompt: NotRequired[str]
+    """
+    Input prompt.
+    """
+    num_choices: NotRequired[int]
+    """
+    Number of choices to generate.
+    """
+    temperature: NotRequired[float]
+    """
+    Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
+    """
+    max_tokens: NotRequired[int]
+    """
+    Maximum number of tokens to generate.
+    """
+
+
+class Llama3Instruct70BChoice(TypedDict):
+    text: NotRequired[str]
+    """
+    Text response.
+    """
+
+
+class Llama3Instruct70BOut(TypedDict):
+    choices: NotRequired[List[Llama3Instruct70BChoice]]
+    """
+    Response choices.
     """
 
 
 class GenerateTextVisionIn(TypedDict):
     prompt: NotRequired[str]
     """
     Text prompt.
@@ -271,15 +445,15 @@
 class GenerateImageIn(TypedDict):
     prompt: NotRequired[str]
     """
     Text prompt.
     """
     store: NotRequired[str]
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: NotRequired[Literal["StableDiffusionXL"]]
     """
     Selected node.
     """
 
 
@@ -297,15 +471,15 @@
     """
     num_images: NotRequired[int]
     """
     Number of images to generate.
     """
     store: NotRequired[str]
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: NotRequired[Literal["StableDiffusionXL"]]
     """
     Selected node.
     """
 
 
@@ -331,15 +505,15 @@
     """
     num_images: NotRequired[int]
     """
     Number of images to generate.
     """
     store: NotRequired[str]
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     height: NotRequired[int]
     """
     Height of output image, in pixels.
     """
     width: NotRequired[int]
     """
@@ -384,15 +558,15 @@
     """
     num_images: NotRequired[int]
     """
     Number of images to generate.
     """
     store: NotRequired[str]
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     height: NotRequired[int]
     """
     Height of output image, in pixels.
     """
     width: NotRequired[int]
     """
@@ -430,15 +604,15 @@
     """
     negative_prompt: NotRequired[str]
     """
     Negative input prompt.
     """
     store: NotRequired[str]
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     width: NotRequired[int]
     """
     Width of output image, in pixels.
     """
     height: NotRequired[int]
     """
@@ -480,15 +654,15 @@
     """
     negative_prompt: NotRequired[str]
     """
     Negative input prompt.
     """
     store: NotRequired[str]
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     conditioning_scale: NotRequired[float]
     """
     Controls the influence of the input image on the generated output.
     """
     seeds: NotRequired[List[int]]
     """
@@ -514,15 +688,15 @@
     """
     mask_image_uri: NotRequired[str]
     """
     Mask image that controls which pixels are inpainted. If unset, the entire image is edited (image-to-image).
     """
     store: NotRequired[str]
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: NotRequired[Literal["StableDiffusionXLInpaint"]]
     """
     Selected node.
     """
 
 
@@ -548,15 +722,15 @@
     """
     num_images: NotRequired[int]
     """
     Number of images to generate.
     """
     store: NotRequired[str]
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: NotRequired[Literal["StableDiffusionXLInpaint"]]
     """
     Selected node.
     """
 
 
@@ -590,15 +764,15 @@
     """
     negative_prompt: NotRequired[str]
     """
     Negative input prompt.
     """
     store: NotRequired[str]
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     strength: NotRequired[float]
     """
     Controls the strength of the generation process.
     """
     seeds: NotRequired[List[int]]
     """
@@ -650,15 +824,15 @@
     """
     mask_image_uri: NotRequired[str]
     """
     Mask image that controls which pixels are inpainted.
     """
     store: NotRequired[str]
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: NotRequired[Literal["BigLaMa"]]
     """
     Selected node.
     """
 
 
@@ -676,15 +850,15 @@
     """
     mask_image_uri: NotRequired[str]
     """
     Mask image that controls which pixels are inpainted.
     """
     store: NotRequired[str]
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 class BigLaMaOut(TypedDict):
     image_uri: NotRequired[str]
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
@@ -702,15 +876,15 @@
     """
     background_color: NotRequired[str]
     """
     Hex value background color. Transparent if unset.
     """
     store: NotRequired[str]
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: NotRequired[Literal["DISISNet"]]
     """
     Selected node.
     """
 
 
@@ -724,15 +898,15 @@
 class DISISNetIn(TypedDict):
     image_uri: NotRequired[str]
     """
     Input image.
     """
     store: NotRequired[str]
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 class DISISNetOut(TypedDict):
     image_uri: NotRequired[str]
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
@@ -742,15 +916,15 @@
 class UpscaleImageIn(TypedDict):
     image_uri: NotRequired[str]
     """
     Input image.
     """
     store: NotRequired[str]
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: NotRequired[Literal["RealESRGAN"]]
     """
     Selected node.
     """
 
 
@@ -764,15 +938,15 @@
 class RealESRGANIn(TypedDict):
     image_uri: NotRequired[str]
     """
     Input image.
     """
     store: NotRequired[str]
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 class RealESRGANOut(TypedDict):
     image_uri: NotRequired[str]
     """
     Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
@@ -786,15 +960,15 @@
     """
     point: NotRequired[Point]
     """
     Point prompt.
     """
     store: NotRequired[str]
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
     node: NotRequired[Literal["SegmentAnything"]]
     """
     Selected node.
     """
 
 
@@ -816,15 +990,15 @@
     """
     box_prompts: NotRequired[List[BoundingBox]]
     """
     Box prompts, to detect a segment within the bounding box. One of `point_prompts` or `box_prompts` must be set.
     """
     store: NotRequired[str]
     """
-    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the image data will be returned as a base64-encoded string.
+    Use "hosted" to return an image URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the image data will be returned as a base64-encoded string.
     """
 
 
 class SegmentAnythingOut(TypedDict):
     mask_image_uri: NotRequired[str]
     """
     Detected segments in 'mask image' format. Base 64-encoded JPEG image bytes, or a hosted image url if `store` is provided.
@@ -933,15 +1107,15 @@
 class GenerateSpeechIn(TypedDict):
     text: NotRequired[str]
     """
     Input text.
     """
     store: NotRequired[str]
     """
-    Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
+    Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the audio data will be returned as a base64-encoded string.
     """
     node: NotRequired[Literal["XTTSV2"]]
     """
     Selected node.
     """
 
 
@@ -963,15 +1137,15 @@
     """
     language: NotRequired[str]
     """
     Language of input text. Supported languages: `en, de, fr, es, it, pt, pl, zh, ar, cs, ru, nl, tr, hu, ko`.
     """
     store: NotRequired[str]
     """
-    Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](/docs/file-stores). If unset, the audio data will be returned as a base64-encoded string.
+    Use "hosted" to return an audio URL hosted on Substrate. You can also provide a URL to a registered [file store](https://guides.substrate.run/guides/external-file-storage). If unset, the audio data will be returned as a base64-encoded string.
     """
 
 
 class XTTSV2Out(TypedDict):
     audio_uri: NotRequired[str]
     """
     Base 64-encoded WAV audio bytes, or a hosted audio url if `store` is provided.
@@ -994,33 +1168,33 @@
 
 
 class EmbedTextIn(TypedDict):
     text: NotRequired[str]
     """
     Text to embed.
     """
-    store: NotRequired[str]
+    collection_name: NotRequired[str]
     """
-    [Vector store](/docs/vector-stores) identifier.
+    Vector store name.
     """
     metadata: NotRequired[Dict[str, Any]]
     """
     Metadata that can be used to query the vector store. Ignored if `store` is unset.
     """
     embedded_metadata_keys: NotRequired[List[str]]
     """
     Choose keys from `metadata` to embed with text.
     """
     doc_id: NotRequired[str]
     """
     Vector store document ID. Ignored if `store` is unset.
     """
-    node: NotRequired[Literal["JinaV2", "CLIP"]]
+    model: NotRequired[Literal["jina-v2", "clip"]]
     """
-    Selected node.
+    Selected embedding model.
     """
 
 
 class EmbedTextOut(TypedDict):
     embedding: NotRequired[Embedding]
     """
     Generated embedding.
@@ -1043,25 +1217,25 @@
 
 
 class MultiEmbedTextIn(TypedDict):
     items: NotRequired[List[EmbedTextItem]]
     """
     Items to embed.
     """
-    store: NotRequired[str]
+    collection_name: NotRequired[str]
     """
-    [Vector store](/docs/vector-stores) identifier.
+    Vector store name.
     """
     embedded_metadata_keys: NotRequired[List[str]]
     """
     Choose keys from `metadata` to embed with text.
     """
-    node: NotRequired[Literal["JinaV2", "CLIP"]]
+    model: NotRequired[Literal["jina-v2", "clip"]]
     """
-    Selected node.
+    Selected embedding model.
     """
 
 
 class MultiEmbedTextOut(TypedDict):
     embeddings: NotRequired[List[Embedding]]
     """
     Generated embeddings.
@@ -1069,17 +1243,17 @@
 
 
 class JinaV2In(TypedDict):
     items: NotRequired[List[EmbedTextItem]]
     """
     Items to embed.
     """
-    store: NotRequired[str]
+    collection_name: NotRequired[str]
     """
-    [Vector store](/docs/vector-stores) identifier.
+    Vector store name.
     """
     embedded_metadata_keys: NotRequired[List[str]]
     """
     Choose keys from `metadata` to embed with text.
     """
 
 
@@ -1091,25 +1265,25 @@
 
 
 class EmbedImageIn(TypedDict):
     image_uri: NotRequired[str]
     """
     Image to embed.
     """
-    store: NotRequired[str]
+    collection_name: NotRequired[str]
     """
-    [Vector store](/docs/vector-stores) identifier.
+    Vector store name.
     """
     doc_id: NotRequired[str]
     """
     Vector store document ID. Ignored if `store` is unset.
     """
-    node: NotRequired[Literal["CLIP"]]
+    model: NotRequired[Literal["clip"]]
     """
-    Selected node.
+    Selected embedding model.
     """
 
 
 class EmbedImageOut(TypedDict):
     embedding: NotRequired[Embedding]
     """
     Generated embedding.
@@ -1147,21 +1321,21 @@
 
 
 class MultiEmbedImageIn(TypedDict):
     items: NotRequired[List[EmbedImageItem]]
     """
     Items to embed.
     """
-    store: NotRequired[str]
+    collection_name: NotRequired[str]
     """
-    [Vector store](/docs/vector-stores) identifier.
+    Vector store name.
     """
-    node: NotRequired[Literal["CLIP"]]
+    model: NotRequired[Literal["clip"]]
     """
-    Selected node.
+    Selected embedding model.
     """
 
 
 class MultiEmbedImageOut(TypedDict):
     embeddings: NotRequired[List[Embedding]]
     """
     Generated embeddings.
@@ -1169,29 +1343,33 @@
 
 
 class CLIPIn(TypedDict):
     items: NotRequired[List[EmbedTextOrImageItem]]
     """
     Items to embed.
     """
-    store: NotRequired[str]
+    collection_name: NotRequired[str]
+    """
+    Vector store name.
+    """
+    embedded_metadata_keys: NotRequired[List[str]]
     """
-    [Vector store](/docs/vector-stores) identifier.
+    Choose keys from `metadata` to embed with text. Only applies to text items.
     """
 
 
 class CLIPOut(TypedDict):
     embeddings: NotRequired[List[Embedding]]
     """
     Generated embeddings.
     """
 
 
 class CreateVectorStoreIn(TypedDict):
-    name: NotRequired[str]
+    collection_name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
     Selected embedding model.
     """
@@ -1206,15 +1384,15 @@
     metric: NotRequired[Literal["cosine", "l2", "inner"]]
     """
     The distance metric to construct the index with.
     """
 
 
 class CreateVectorStoreOut(TypedDict):
-    name: NotRequired[str]
+    collection_name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
     Selected embedding model.
     """
@@ -1233,33 +1411,33 @@
 
 
 class ListVectorStoresIn(TypedDict):
     pass
 
 
 class ListVectorStoresOut(TypedDict):
-    stores: NotRequired[List[CreateVectorStoreOut]]
+    items: NotRequired[List[CreateVectorStoreOut]]
     """
     List of vector stores.
     """
 
 
 class DeleteVectorStoreIn(TypedDict):
-    name: NotRequired[str]
+    collection_name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
     Selected embedding model.
     """
 
 
 class DeleteVectorStoreOut(TypedDict):
-    name: NotRequired[str]
+    collection_name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
     Selected embedding model.
     """
@@ -1281,15 +1459,15 @@
     metadata: NotRequired[Dict[str, Any]]
     """
     Document metadata.
     """
 
 
 class FetchVectorsIn(TypedDict):
-    name: NotRequired[str]
+    collection_name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
     Selected embedding model.
     """
@@ -1332,45 +1510,45 @@
     metadata: NotRequired[Dict[str, Any]]
     """
     Document metadata.
     """
 
 
 class UpdateVectorsIn(TypedDict):
-    name: NotRequired[str]
+    collection_name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
     Selected embedding model.
     """
     vectors: NotRequired[List[UpdateVectorParams]]
     """
     Vectors to upsert.
     """
 
 
 class DeleteVectorsIn(TypedDict):
-    name: NotRequired[str]
+    collection_name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
     Selected embedding model.
     """
     ids: NotRequired[List[str]]
     """
     Document IDs to delete.
     """
 
 
 class QueryVectorStoreIn(TypedDict):
-    name: NotRequired[str]
+    collection_name: NotRequired[str]
     """
     Vector store to query against.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
     Selected embedding model.
     """
@@ -1406,18 +1584,14 @@
     """
     Include the metadata of the vectors in the response.
     """
     filters: NotRequired[Dict[str, Any]]
     """
     Filter metadata by key-value pairs.
     """
-    metric: NotRequired[Literal["cosine", "l2", "inner"]]
-    """
-    The distance metric used for the query. Defaults to the distance metric the vector store was created with.
-    """
 
 
 class VectorStoreQueryResult(TypedDict):
     id: NotRequired[str]
     """
     Document ID.
     """
@@ -1436,15 +1610,15 @@
 
 
 class QueryVectorStoreOut(TypedDict):
     results: NotRequired[List[List[VectorStoreQueryResult]]]
     """
     Query results.
     """
-    name: NotRequired[str]
+    collection_name: NotRequired[str]
     """
     Vector store name.
     """
     model: NotRequired[Literal["jina-v2", "clip"]]
     """
     Selected embedding model.
     """
```

