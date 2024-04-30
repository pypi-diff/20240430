# Comparing `tmp/mllm-0.1.4.tar.gz` & `tmp/mllm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mllm-0.1.4.tar", max compression
+gzip compressed data, was "mllm-0.1.5.tar", max compression
```

## Comparing `mllm-0.1.4.tar` & `mllm-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2024-04-27 16:19:02.140835 mllm-0.1.4/LICENSE
--rw-r--r--   0        0        0     2221 2024-04-29 21:12:11.290383 mllm-0.1.4/README.md
--rw-r--r--   0        0        0      154 2024-04-27 21:30:57.109430 mllm-0.1.4/mllm/__init__.py
--rw-r--r--   0        0        0     1981 2024-04-27 22:13:37.479726 mllm-0.1.4/mllm/db/conn.py
--rw-r--r--   0        0        0      541 2024-04-27 16:19:02.141445 mllm-0.1.4/mllm/db/models.py
--rw-r--r--   0        0        0      866 2024-04-27 21:28:03.888370 mllm-0.1.4/mllm/models.py
--rw-r--r--   0        0        0     5625 2024-04-27 21:29:28.486764 mllm-0.1.4/mllm/prompt.py
--rw-r--r--   0        0        0     8327 2024-04-27 21:28:31.215289 mllm-0.1.4/mllm/router.py
--rw-r--r--   0        0        0      793 2024-04-27 21:31:01.883780 mllm-0.1.4/mllm/util.py
--rw-r--r--   0        0        0      390 2024-04-29 21:12:15.343851 mllm-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2790 1970-01-01 00:00:00.000000 mllm-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-27 16:19:02.140835 mllm-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2221 2024-04-29 21:12:11.290383 mllm-0.1.5/README.md
+-rw-r--r--   0        0        0      149 2024-04-29 21:17:19.261017 mllm-0.1.5/mllm/__init__.py
+-rw-r--r--   0        0        0     1981 2024-04-27 22:13:37.479726 mllm-0.1.5/mllm/db/conn.py
+-rw-r--r--   0        0        0      541 2024-04-27 16:19:02.141445 mllm-0.1.5/mllm/db/models.py
+-rw-r--r--   0        0        0      846 2024-04-29 21:16:16.874384 mllm-0.1.5/mllm/models.py
+-rw-r--r--   0        0        0     5605 2024-04-29 21:16:42.671629 mllm-0.1.5/mllm/prompt.py
+-rw-r--r--   0        0        0     8299 2024-04-29 21:17:12.773037 mllm-0.1.5/mllm/router.py
+-rw-r--r--   0        0        0      793 2024-04-29 21:17:15.851578 mllm-0.1.5/mllm/util.py
+-rw-r--r--   0        0        0      390 2024-04-29 21:17:25.763718 mllm-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2790 1970-01-01 00:00:00.000000 mllm-0.1.5/PKG-INFO
```

### Comparing `mllm-0.1.4/LICENSE` & `mllm-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mllm-0.1.4/README.md` & `mllm-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mllm-0.1.4/mllm/db/conn.py` & `mllm-0.1.5/mllm/db/conn.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.4/mllm/db/models.py` & `mllm-0.1.5/mllm/db/models.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.4/mllm/models.py` & `mllm-0.1.5/mllm/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from typing import Optional, Dict, Any, List
 
 from pydantic import BaseModel
 from threadmem.server.models import RoleThreadModel, RoleMessageModel
 
 
-class V1PromptModel(BaseModel):
+class V1Prompt(BaseModel):
     """An LLM prompt model"""
 
     id: Optional[str] = None
     thread: RoleThreadModel
     response: RoleMessageModel
     namespace: str = "default"
     metadata: Dict[str, Any] = {}
     created: Optional[float] = None
     approved: bool = False
     flagged: bool = False
 
 
-class V1EnvVarOptModel(BaseModel):
+class V1EnvVarOpt(BaseModel):
     name: str
     description: Optional[str] = None
     required: bool = False
     default: Optional[str] = None
     secret: bool = False
     options: List[str] = []
 
 
 class V1MLLMProviders(BaseModel):
     preference: List[str] = []
 
 
 class V1MLLMOption(BaseModel):
     model: str
-    env_var: V1EnvVarOptModel
+    env_var: V1EnvVarOpt
 
 
-class V1MLLMModel(BaseModel):
+class V1MLLM(BaseModel):
     options: List[V1MLLMOption]
```

### Comparing `mllm-0.1.4/mllm/prompt.py` & `mllm-0.1.5/mllm/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Dict, Any, List, Optional
 
 from threadmem import RoleThread, RoleMessage
 from threadmem.server.models import RoleMessageModel, RoleThreadModel
 
 from .db.models import PromptRecord
 from .db.conn import WithDB
-from .models import V1PromptModel
+from .models import V1Prompt
 
 logger = logging.getLogger(__name__)
 
 
 class Prompt(WithDB):
     """An LLM prompt"""
 
@@ -140,28 +140,28 @@
         obj._metadata = metadata
         obj._created = record.created
         obj._approved = record.approved
         obj._flagged = record.flagged
 
         return obj
 
-    def to_v1(self) -> V1PromptModel:
-        return V1PromptModel(
+    def to_v1(self) -> V1Prompt:
+        return V1Prompt(
             id=self._id,
             namespace=self._namespace,
             thread=self._thread.to_schema(),
             response=self._response.to_schema(),
             metadata=self._metadata,
             created=self._created,
             approved=self._approved,
             flagged=self._flagged,
         )
 
     @classmethod
-    def from_v1(cls, v1: V1PromptModel) -> "Prompt":
+    def from_v1(cls, v1: V1Prompt) -> "Prompt":
         obj = cls.__new__(cls)
 
         obj._id = v1.id
         obj._namespace = v1.namespace
         obj._thread = RoleThread.from_schema(v1.thread)
         obj._response = RoleMessage.from_schema(v1.response)
         obj._metadata = v1.metadata
```

### Comparing `mllm-0.1.4/mllm/router.py` & `mllm-0.1.5/mllm/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from litellm import Router as LLMRouter, ModelResponse
 from threadmem import RoleThread, RoleMessage
 from litellm._logging import handler
 from pydantic import BaseModel
 from tenacity import retry, stop_after_attempt
 
-from .models import V1EnvVarOptModel, V1MLLMModel, V1MLLMOption
+from .models import V1EnvVarOpt, V1MLLMOption
 from .util import extract_parse_json
 from .prompt import Prompt
 
 
 T = TypeVar("T", bound=BaseModel)
 
 
@@ -106,15 +106,15 @@
     @classmethod
     def all_opts(cls) -> List[V1MLLMOption]:
         out = []
         for model, key in cls.provider_api_keys.items():
             out.append(
                 V1MLLMOption(
                     model=model,
-                    env_var=V1EnvVarOptModel(
+                    env_var=V1EnvVarOpt(
                         name=key,
                         description=f"{model} API key",
                         required=True,
                         secret=True,
                     ),
                 )
             )
@@ -207,15 +207,15 @@
         options = []
         for model_info in self.model_list:
             model_name = model_info["model_name"]
             api_key_env = self.provider_api_keys.get(model_name)
             if api_key_env:
                 option = V1MLLMOption(
                     model=model_name,
-                    env_var=V1EnvVarOptModel(
+                    env_var=V1EnvVarOpt(
                         name=api_key_env,
                         description=f"{model_name} API key",
                         required=True,
                         secret=True,
                     ),
                 )
                 options.append(option)
```

### Comparing `mllm-0.1.4/mllm/util.py` & `mllm-0.1.5/mllm/util.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.4/PKG-INFO` & `mllm-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mllm
-Version: 0.1.4
+Version: 0.1.5
 Summary: Multimodal Large Language Models
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

