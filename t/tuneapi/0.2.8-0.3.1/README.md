# Comparing `tmp/tuneapi-0.2.8.tar.gz` & `tmp/tuneapi-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneapi-0.2.8.tar", max compression
+gzip compressed data, was "tuneapi-0.3.1.tar", max compression
```

## Comparing `tuneapi-0.2.8.tar` & `tuneapi-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0       30 2024-03-02 10:46:47.727709 tuneapi-0.2.8/README.md
--rw-r--r--   0        0        0      696 2024-04-12 08:21:20.179027 tuneapi-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       78 2024-04-12 08:21:15.818709 tuneapi-0.2.8/tuneapi/__init__.py
--rw-r--r--   0        0        0      230 2024-04-12 08:19:21.664606 tuneapi-0.2.8/tuneapi/apis/__init__.py
--rw-r--r--   0        0        0     6710 2024-04-12 08:20:50.001225 tuneapi-0.2.8/tuneapi/apis/model_anthropic.py
--rw-r--r--   0        0        0     3064 2024-04-12 08:08:55.997351 tuneapi-0.2.8/tuneapi/apis/model_grok.py
--rw-r--r--   0        0        0     3082 2024-04-12 08:19:03.799303 tuneapi-0.2.8/tuneapi/apis/model_mistral.py
--rw-r--r--   0        0        0     8309 2024-03-30 16:56:55.006134 tuneapi-0.2.8/tuneapi/apis/model_openai.py
--rw-r--r--   0        0        0     5519 2024-04-12 08:20:35.218980 tuneapi-0.2.8/tuneapi/apis/model_tune.py
--rw-r--r--   0        0        0      659 2024-04-07 20:07:56.771955 tuneapi-0.2.8/tuneapi/apis/threads.py
--rw-r--r--   0        0        0      183 2024-03-30 04:57:08.088526 tuneapi-0.2.8/tuneapi/types/__init__.py
--rw-r--r--   0        0        0    14666 2024-04-03 06:38:04.010933 tuneapi-0.2.8/tuneapi/types/chats.py
--rw-r--r--   0        0        0     1032 2024-04-07 05:56:12.541307 tuneapi-0.2.8/tuneapi/utils/__init__.py
--rw-r--r--   0        0        0      279 2024-02-29 16:50:59.822352 tuneapi-0.2.8/tuneapi/utils/env.py
--rw-r--r--   0        0        0     2389 2024-03-17 09:04:09.851851 tuneapi-0.2.8/tuneapi/utils/fs.py
--rw-r--r--   0        0        0      958 2024-02-29 04:52:05.321819 tuneapi-0.2.8/tuneapi/utils/logger.py
--rw-r--r--   0        0        0    33461 2024-02-28 18:58:17.252019 tuneapi-0.2.8/tuneapi/utils/mime.py
--rw-r--r--   0        0        0     3712 2024-04-07 20:01:31.642080 tuneapi-0.2.8/tuneapi/utils/misc.py
--rw-r--r--   0        0        0     2065 2024-02-28 18:58:23.839022 tuneapi-0.2.8/tuneapi/utils/networking.py
--rw-r--r--   0        0        0     4653 2024-04-02 03:55:14.556441 tuneapi-0.2.8/tuneapi/utils/parallel.py
--rw-r--r--   0        0        0      400 2024-03-08 09:25:58.748478 tuneapi-0.2.8/tuneapi/utils/randomness.py
--rw-r--r--   0        0        0     2430 2024-04-07 05:56:29.001597 tuneapi-0.2.8/tuneapi/utils/serdeser.py
--rw-r--r--   0        0        0     5297 2024-03-28 07:17:07.821045 tuneapi-0.2.8/tuneapi/utils/subway.py
--rw-r--r--   0        0        0      535 2024-03-15 08:31:32.392327 tuneapi-0.2.8/tuneapi/utils/terminal.py
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 tuneapi-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-23 08:29:50.671125 tuneapi-0.3.1/LICENSE
+-rw-r--r--   0        0        0       30 2024-03-02 10:46:47.727709 tuneapi-0.3.1/README.md
+-rw-r--r--   0        0        0      712 2024-04-30 05:40:45.011463 tuneapi-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-04-30 05:40:42.068157 tuneapi-0.3.1/tuneapi/__init__.py
+-rw-r--r--   0        0        0      291 2024-04-23 00:52:16.205178 tuneapi-0.3.1/tuneapi/apis/__init__.py
+-rw-r--r--   0        0        0     6805 2024-04-18 21:09:12.184663 tuneapi-0.3.1/tuneapi/apis/model_anthropic.py
+-rw-r--r--   0        0        0     3159 2024-04-25 05:37:07.370133 tuneapi-0.3.1/tuneapi/apis/model_groq.py
+-rw-r--r--   0        0        0     3177 2024-04-18 21:08:27.197387 tuneapi-0.3.1/tuneapi/apis/model_mistral.py
+-rw-r--r--   0        0        0     6328 2024-04-26 00:29:23.039606 tuneapi-0.3.1/tuneapi/apis/model_openai.py
+-rw-r--r--   0        0        0     5822 2024-04-22 20:41:11.558482 tuneapi-0.3.1/tuneapi/apis/model_tune.py
+-rw-r--r--   0        0        0     3714 2024-04-23 01:23:26.207221 tuneapi-0.3.1/tuneapi/apis/threads.py
+-rw-r--r--   0        0        0      183 2024-04-25 04:12:26.606262 tuneapi-0.3.1/tuneapi/types/__init__.py
+-rw-r--r--   0        0        0    15414 2024-04-24 21:00:11.105695 tuneapi-0.3.1/tuneapi/types/chats.py
+-rw-r--r--   0        0        0     1065 2024-04-24 17:41:16.006098 tuneapi-0.3.1/tuneapi/utils/__init__.py
+-rw-r--r--   0        0        0      279 2024-02-29 16:50:59.822352 tuneapi-0.3.1/tuneapi/utils/env.py
+-rw-r--r--   0        0        0     2460 2024-04-24 17:41:09.928391 tuneapi-0.3.1/tuneapi/utils/fs.py
+-rw-r--r--   0        0        0      958 2024-02-29 04:52:05.321819 tuneapi-0.3.1/tuneapi/utils/logger.py
+-rw-r--r--   0        0        0    33461 2024-02-28 18:58:17.252019 tuneapi-0.3.1/tuneapi/utils/mime.py
+-rw-r--r--   0        0        0     3712 2024-04-07 20:01:31.642080 tuneapi-0.3.1/tuneapi/utils/misc.py
+-rw-r--r--   0        0        0     2065 2024-02-28 18:58:23.839022 tuneapi-0.3.1/tuneapi/utils/networking.py
+-rw-r--r--   0        0        0     4846 2024-04-25 22:30:49.313201 tuneapi-0.3.1/tuneapi/utils/parallel.py
+-rw-r--r--   0        0        0     1154 2024-04-30 05:41:11.504281 tuneapi-0.3.1/tuneapi/utils/randomness.py
+-rw-r--r--   0        0        0     2430 2024-04-07 05:56:29.001597 tuneapi-0.3.1/tuneapi/utils/serdeser.py
+-rw-r--r--   0        0        0     5772 2024-04-23 00:48:09.361152 tuneapi-0.3.1/tuneapi/utils/subway.py
+-rw-r--r--   0        0        0      535 2024-03-15 08:31:32.392327 tuneapi-0.3.1/tuneapi/utils/terminal.py
+-rw-r--r--   0        0        0      973 1970-01-01 00:00:00.000000 tuneapi-0.3.1/PKG-INFO
```

### Comparing `tuneapi-0.2.8/pyproject.toml` & `tuneapi-0.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "tuneapi"
-version = "0.2.8"
+version = "0.3.1"
 description = "Tune AI APIs."
 authors = ["Frello Technology Private Limited <engineering@nimblebox.ai>"]
-license = "Apache 2.0"
+license = "MIT"
 readme = "README.md"
 repository = "https://github.com/NimbleBoxAI/tuneapi"
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 fire = "0.5.0"
 requests = "^2.31.0"
 cloudpickle = "3.0.0"
 protobuf = "^4.25.3"
 cryptography = ">=42.0.5"
 tqdm = "^4.66.1"
+snowflake_id = "1.0.2"
 boto3 = { version = "1.29.6", optional = true }
 
 [tool.poetry.extras]
 boto3 = ["boto3"]
 
 [tool.poetry.group.dev.dependencies]
 sphinx = "7.2.5"
```

### Comparing `tuneapi-0.2.8/tuneapi/apis/model_anthropic.py` & `tuneapi-0.3.1/tuneapi/apis/model_anthropic.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,21 @@
 from typing import Optional, Dict, Any, Tuple, List
 
 from tuneapi.utils import ENV, SimplerTimes as stime, from_json, to_json
 from tuneapi.types import Thread, human, Message
 
 
 class Anthropic:
-    def __init__(self, model: Optional[str] = "claude-3-haiku-20240307"):
+    def __init__(
+        self,
+        model: Optional[str] = "claude-3-haiku-20240307",
+        base_url: str = "https://api.anthropic.com/v1/messages",
+    ):
         self.anthropic_model = model
+        self.base_url = base_url
         self.anthropic_api_token = ENV.ANTHROPIC_TOKEN("")
 
     def set_api_token(self, token: str) -> None:
         self.anthropic_api_token = token
 
     def tool_to_claude_xml(self, tool):
         tool_signature = ""
@@ -155,15 +160,15 @@
             "messages": claude_messages,
             "temperature": temperature,
             "system": system,
             "stream": True,
             **kwargs,
         }
         r = requests.post(
-            "https://api.anthropic.com/v1/messages",
+            self.base_url,
             headers=headers,
             json=data,
             timeout=timeout,
         )
         try:
             r.raise_for_status()
         except Exception as e:
```

### Comparing `tuneapi-0.2.8/tuneapi/apis/model_grok.py` & `tuneapi-0.3.1/tuneapi/apis/model_groq.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,21 @@
 from typing import Optional, Dict, Any, Tuple, List
 
 from tuneapi.utils import ENV, SimplerTimes as stime, from_json, to_json
 from tuneapi.types import Thread, human, Message
 
 
 class Groq:
-    def __init__(self, id: Optional[str] = "mixtral-8x7b-32768"):
+    def __init__(
+        self,
+        id: Optional[str] = "mixtral-8x7b-32768",
+        base_url: str = "https://api.groq.com/openai/v1/chat/completions",
+    ):
         self.groq_model_id = id
+        self.base_url = base_url
         self.groq_api_token = ENV.GROQ_TOKEN("")
 
     def set_api_token(self, token: str) -> None:
         self.groq_api_token = token
 
     def _process_input(self, chats, token: Optional[str] = None):
         if not token and not self.groq_api_token:  # type: ignore
@@ -73,15 +78,15 @@
             "model": model or self.groq_model_id,
             "stream": True,
             "max_tokens": max_tokens,
         }
         # for m in messages:
         #     print(m)
         response = requests.post(
-            "https://api.groq.com/openai/v1/chat/completions",
+            self.base_url,
             headers=headers,
             json=data,
             stream=True,
             timeout=timeout,
         )
         try:
             response.raise_for_status()
```

### Comparing `tuneapi-0.2.8/tuneapi/apis/model_mistral.py` & `tuneapi-0.3.1/tuneapi/apis/model_mistral.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,21 @@
 from typing import Optional, Dict, Any, Tuple, List
 
 from tuneapi.utils import ENV, SimplerTimes as stime, from_json, to_json
 from tuneapi.types import Thread, human, Message
 
 
 class Mistral:
-    def __init__(self, id: Optional[str] = "mistral-small-latest"):
+    def __init__(
+        self,
+        id: Optional[str] = "mistral-small-latest",
+        base_url: str = "https://api.mistral.ai/v1/chat/completions",
+    ):
         self.groq_model_id = id
+        self.base_url = base_url
         self.mistral_api_token = ENV.MISTRAL_TOKEN("")
 
     def set_api_token(self, token: str) -> None:
         self.mistral_api_token = token
 
     def _process_input(self, chats, token: Optional[str] = None):
         if not token and not self.mistral_api_token:  # type: ignore
@@ -73,15 +78,15 @@
             "model": model or self.groq_model_id,
             "stream": True,
             "max_tokens": max_tokens,
         }
         # for m in messages:
         #     print(m)
         response = requests.post(
-            "https://api.mistral.ai/v1/chat/completions",
+            self.base_url,
             headers=headers,
             json=data,
             stream=True,
             timeout=timeout,
         )
         try:
             response.raise_for_status()
```

### Comparing `tuneapi-0.2.8/tuneapi/apis/model_tune.py` & `tuneapi-0.3.1/tuneapi/apis/model_tune.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,30 @@
 from tuneapi.utils import ENV, SimplerTimes as stime, from_json, to_json
 from tuneapi.types import Thread, human, Message
 
 
 class TuneModel:
     """Defines the model used in tune.app. See [Tune Studio](https://studio.tune.app/) for more information."""
 
-    def __init__(self, id: Optional[str] = "rohan/mixtral-8x7b-inst-v0-1-32k"):
+    def __init__(
+        self,
+        id: Optional[str] = "rohan/mixtral-8x7b-inst-v0-1-32k",
+        base_url: str = "https://proxy.tune.app/chat/completions",
+    ):
         self.tune_model_id = id
+        self.base_url = base_url
         self.tune_api_token = ENV.TUNEAPI_TOKEN("")
+        self.tune_org_id = ENV.TUNEORG_ID("")
 
     def set_api_token(self, token: str) -> None:
         self.tune_api_token = token
 
+    def set_org_id(self, org_id: str) -> None:
+        self.tune_org_id = org_id
+
     def _process_input(self, chats, token: Optional[str] = None):
         if not token and not self.tune_api_token:  # type: ignore
             raise Exception(
                 "Tune API key not found. Please set TUNEAPI_TOKEN environment variable or pass through function"
             )
         token = token or self.tune_api_token
         if isinstance(chats, Thread):
@@ -31,14 +40,16 @@
         else:
             messages = chats
 
         headers = {
             "Authorization": token,
             "Content-Type": "application/json",
         }
+        if self.tune_org_id:
+            headers["X-Org-Id"] = self.tune_org_id
         return headers, messages
 
     def chat(
         self,
         chats: Thread | str,
         model: Optional[str] = None,
         max_tokens: int = 1024,
@@ -68,15 +79,15 @@
             "temperature": temperature,
             "messages": messages,
             "model": model or self.tune_model_id,
             "stream": False,
             "max_tokens": max_tokens,
         }
         response = requests.post(
-            "https://proxy.tune.app/chat/completions",
+            self.base_url,
             headers=headers,
             json=data,
             timeout=timeout,
         )
         try:
             response.raise_for_status()
         except Exception as e:
```

### Comparing `tuneapi-0.2.8/tuneapi/types/chats.py` & `tuneapi-0.3.1/tuneapi/types/chats.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,23 +38,24 @@
         "function-resp": FUNCTION_RESP,
         # tools
         "tools": TOOLS,
         "tool": TOOLS,
     }
 
     # start initialization here
-    def __init__(self, value: str | float | List[Dict[str, Any]], role: str):
+    def __init__(self, value: str | float | List[Dict[str, Any]], role: str, **kwargs):
         if role not in self.KNOWN_ROLES:
             raise ValueError(f"Unknown role: {role}. Update dictionary `KNOWN_ROLES`")
         if value is None:
             raise ValueError("value cannot be None")
 
         self.role = role
         self.value = value
         self._unq_value = get_random_string(6)
+        self.metadata = kwargs
 
     def __str__(self) -> str:
         try:
             idx = max(os.get_terminal_size().columns - len(self.role) - 40, 10)
         except OSError:
             idx = 50
         return f"<{self.role}: {json.dumps(self.value)[:idx]}>"
@@ -69,43 +70,59 @@
         return str(self.value)
 
     def __getitem__(self, x):
         if x == "content":
             return self.value
         return getattr(self, x)
 
-    def to_dict(self, ft: bool = False):
+    def to_dict(
+        self,
+        format: Optional[str] = None,
+        meta: bool = False,
+    ):  #  ft: bool = False
         """
-        if `ft` then export to following format: `{"from": "system/human/gpt", "value": "..."}`
+        if format == `ft` then export to following format: `{"from": "system/human/gpt", "value": "..."}`
+        elif format == `api` then `{"role": "system/user/assistant", "content": [{"type": "text", "text": {"value": "..."}]}`
         else export to following format: `{"role": "system/user/assistant", "content": "..."}`
         """
         role = self.role
+
+        ft = format == "ft"
+        api = format == "api"
+
         if not ft:
             if self.role == self.HUMAN:
                 role = "user"
             elif self.role == self.GPT:
                 role = "assistant"
 
         chat_message: Dict[str, str | float]
         if ft:
             chat_message = {"from": role}
         else:
             chat_message = {"role": role}
 
-        if not ft:
-            chat_message["content"] = self.value
-        else:
+        if ft:
             chat_message["value"] = self.value
+        elif api:
+            chat_message["content"] = [{"type": "text", "text": {"value": self.value}}]
+        else:
+            chat_message["content"] = self.value
+
+        if meta:
+            chat_message["metadata"] = self.metadata
+
         return chat_message
 
     @classmethod
     def from_dict(cls, data):
         return cls(
             value=data.get("value") or data.get("content"),
             role=data.get("from") or data.get("role"),
+            **data.get("metadata", {}),
         )  # type: ignore
 
 
 ### Aliases
 human = partial(Message, role=Message.HUMAN)
 system = partial(Message, role=Message.SYSTEM)
 assistant = partial(Message, role=Message.GPT)
@@ -122,21 +139,23 @@
     """
 
     def __init__(
         self,
         *chats: Union[List[Message], Message],
         jl: Optional[Dict[str, Any]] = None,
         model: Optional[str] = None,
-        i: str = "",
+        id: str = "",
+        title: str = "",
         **kwargs,
     ):
         self.chats = list(chats)
         self.jl = jl
         self.model = model
-        self.id = i
+        self.id = id
+        self.title = title
 
         #
         kwargs = {k: v for k, v in sorted(kwargs.items())}
         self.meta = kwargs
         self.keys = list(kwargs.keys())
         self.values = tuple(kwargs.values())
 
@@ -171,51 +190,55 @@
     def to_dict(self, full: bool = False):
         if full:
             return {
                 "chats": [x.to_dict() for x in self.chats],
                 "jl": self.jl,
                 "model": self.model,
                 "meta": self.meta,
+                "title": self.title,
+                "id": self.id,
             }
         return {
             "chats": [x.to_dict() for x in self.chats],
         }
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "Thread":
         chats = data.get("chats", []) or data.get("conversations", [])
         if not chats:
             raise ValueError("No chats found")
         return cls(
             *[Message.from_dict(x) for x in chats],
-            i=data.get("id", ""),
+            id=data.get("id", ""),
             jl=data.get("jl", ""),
             model=data.get("model", ""),
+            title=data.get("title", ""),
             **data.get("meta", {}),
         )
 
     def to_ft(
         self, id: Any = None, drop_last: bool = False
     ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         chats = self.chats if not drop_last else self.chats[:-1]
         ft_dict = {
             "id": id or get_random_string(6),
-            "conversations": [x.to_dict(ft=True) for x in chats],
+            "conversations": [x.to_dict(format="ft") for x in chats],
         }
         if drop_last:
-            ft_dict["last"] = self.chats[-1].to_dict(ft=True)
+            ft_dict["last"] = self.chats[-1].to_dict(format="ft")
         return ft_dict, self.meta
 
     # modifications
 
     def copy(self) -> "Thread":
         return Thread(
             chats=[x for x in self.chats],
             jl=self.jl,
             model=self.model,
+            title="Copy: " + self.title,
             **self.meta,
         )
 
     def add(self, message: Message):
         self.chats.append(message)
 
     def append(self, message: Message):
```

### Comparing `tuneapi-0.2.8/tuneapi/utils/__init__.py` & `tuneapi-0.3.1/tuneapi/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,18 @@
 )
 from tuneapi.utils.parallel import (
     batched,
     threaded_map,
 )
 from tuneapi.utils.randomness import (
     get_random_string,
+    get_snowflake,
 )
 from tuneapi.utils.fs import (
+    list_dir,
     get_files_in_folder,
     folder,
     joinp,
     load_module_from_path,
 )
 from tuneapi.utils.terminal import (
     hr,
```

### Comparing `tuneapi-0.2.8/tuneapi/utils/fs.py` & `tuneapi-0.3.1/tuneapi/utils/fs.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,14 +59,18 @@
                     _fp = joinp(folder_abs, f)
                     if not ignore_pat.search(_fp).group():
                         all_paths.append(_fp)
 
     return all_paths
 
 
+list_dir = get_files_in_folder
+"""Alias for `get_files_in_folder`"""
+
+
 def folder(x: str) -> str:
     """get the folder of this file path"""
     return os.path.split(os.path.abspath(x))[0]
 
 
 def joinp(x: str, *args) -> str:
     """convienience function for os.path.join"""
```

### Comparing `tuneapi-0.2.8/tuneapi/utils/logger.py` & `tuneapi-0.3.1/tuneapi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.8/tuneapi/utils/mime.py` & `tuneapi-0.3.1/tuneapi/utils/mime.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.8/tuneapi/utils/misc.py` & `tuneapi-0.3.1/tuneapi/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.8/tuneapi/utils/networking.py` & `tuneapi-0.3.1/tuneapi/utils/networking.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.8/tuneapi/utils/parallel.py` & `tuneapi-0.3.1/tuneapi/utils/parallel.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 """
 
 # Copyright © 2024- Frello Technology Private Limited
 
 import time
 from uuid import uuid4
 from tqdm import trange
-from typing import Any, Dict, List, Union, Tuple
+from typing import Any, Dict, List, Union, Tuple, Generator
 
 from concurrent.futures import ThreadPoolExecutor, as_completed, Future
 
 
 def threaded_map(
     fn,
-    inputs: List[Tuple],
+    inputs: List[Tuple] | Generator,
     wait: bool = True,
     max_threads=20,
     post_fn=None,
     _name: str = "",
     safe: bool = False,
     pbar: bool = False,
 ) -> Union[Dict[Future, int], List[Any]]:
@@ -28,31 +28,34 @@
     Args:
         fn (function): The function to call
         inputs (List[Tuple[Any]]): All the inputs to the function, can be a generator
         wait (bool, optional): If true, wait for all the threads to finish, otherwise return a dict of futures. Defaults to True.
         max_threads (int, optional): The maximum number of threads to use. Defaults to 20.
         post_fn (function, optional): A function to call with the result. Defaults to None.
         _name (str, optional): The name of the thread pool. Defaults to "".
-        safe (bool, optional): If true, all caughts exceptions are in the results. Defaults to False.
+        safe (bool, optional): If true, all exceptions are caught and returned with results. Defaults to False.
+        pbar (bool, optional): If true, show a progress bar. Defaults to False.
     """
     _name = _name or str(uuid4())
+    if isinstance(inputs, Generator):
+        inputs = list(inputs)
     results = [None for _ in range(len(inputs))]
     errors = []
     _pbar = trange(len(inputs), desc="Processing", unit="input") if pbar else None
     with ThreadPoolExecutor(max_workers=max_threads, thread_name_prefix=_name) as exe:
         _fn = lambda i, x: [i, fn(*x)]
         futures = {exe.submit(_fn, i, x): i for i, x in enumerate(inputs)}
         if not wait:
             return futures
         for future in as_completed(futures):
             try:
                 if _pbar:
                     _pbar.update(1)
                 i, res = future.result()
-                if post_fn:
+                if post_fn is not None:
                     res = post_fn(res)
                 results[i] = res
             except Exception as e:
                 if safe:
                     errors.append(e)
                 else:
                     raise e
```

### Comparing `tuneapi-0.2.8/tuneapi/utils/serdeser.py` & `tuneapi-0.3.1/tuneapi/utils/serdeser.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.8/tuneapi/utils/subway.py` & `tuneapi-0.3.1/tuneapi/utils/subway.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright © 2024- Frello Technology Private Limited
 
 from requests import Session
 from pydantic import BaseModel
 from typing import Dict, Any, Optional, Tuple
 
 from tuneapi.utils.logger import logger
+from tuneapi.utils.misc import SimplerTimes
 
 
 class SubwayClientError(Exception):
     """Raised if 399 < status_code < 500"""
 
     def __init__(self, *args, code: str):
         self.code = code
@@ -19,20 +20,26 @@
     """Raised if 499 < status_code < 600"""
 
     def __init__(self, *args, code: str):
         self.code = code
         super().__init__(*args)
 
 
-def get_session(token: Optional[str] = "", bearer: Optional[str] = "") -> Session:
+def get_session(
+    token: Optional[str] = "",
+    bearer: Optional[str] = "",
+    **headers,
+) -> Session:
     sess = Session()
     if token:
         sess.headers.update({"token": token})
     if bearer:
         sess.headers.update({"Authorization": f"Bearer {bearer}"})
+    if headers:
+        sess.headers.update(headers)
     return sess
 
 
 class Subway:
     """
     Simple code that allows writing APIs by `.attr.ing` them. This is inspired from gRPC style functional calls which
     hides the complexity of underlying networking. This is useful when you are trying to debug live server directly.
@@ -45,14 +52,15 @@
       _url (str): The url to use for the client
       _session (requests.Session): The session to use for the client
     """
 
     def __init__(self, _url: str, _session: Session):
         self._url = _url.rstrip("/")
         self._session = _session
+        self._last_update = SimplerTimes.get_now_i64()
 
     def __repr__(self):
         return self._url
 
     def __getattr__(self, attr: str):
         # https://stackoverflow.com/questions/3278077/difference-between-getattr-vs-getattribute
         return Subway(f"{self._url}/{attr}", self._session)
@@ -73,17 +81,25 @@
         """
         return getattr(self, attr)
 
     def _renew_session(self):
         """Renew the session"""
         _session = Session()
         if "token" in self._session.headers:
-            _session.headers.update({"token": self._session.headers["token"]})
+            _session.headers.update(**self._session.headers)
         self._session = _session
 
+    @staticmethod
+    def _get_session(
+        token: Optional[str] = "",
+        bearer: Optional[str] = "",
+        **headers,
+    ) -> Session:
+        return get_session(token=token, bearer=bearer, **headers)
+
     def __call__(
         self,
         method="get",
         json={},
         trailing="",
         data=None,
         params: Dict = {},
@@ -128,14 +144,17 @@
             if isinstance(json, BaseModel):
                 json = json.model_dump()
             items["json"] = json
         if data:
             items["data"] = data
         if params:
             items["params"] = params
+
+        if SimplerTimes.get_now_i64() - self._last_update > 120:
+            self._renew_session()
         r = fn(url, **items, **kwargs)
         if 399 < r.status_code < 500:
             raise SubwayClientError(r.content.decode(), code=r.status_code)
         if 499 < r.status_code < 600:
             raise SubwayServerError(r.content.decode(), code=r.status_code)
 
         try:
```

### Comparing `tuneapi-0.2.8/tuneapi/utils/terminal.py` & `tuneapi-0.3.1/tuneapi/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.8/PKG-INFO` & `tuneapi-0.3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: tuneapi
-Version: 0.2.8
+Version: 0.3.1
 Summary: Tune AI APIs.
 Home-page: https://github.com/NimbleBoxAI/tuneapi
-License: Apache 2.0
+License: MIT
 Author: Frello Technology Private Limited
 Author-email: engineering@nimblebox.ai
 Requires-Python: >=3.9,<3.12
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: boto3
 Requires-Dist: boto3 (==1.29.6) ; extra == "boto3"
 Requires-Dist: cloudpickle (==3.0.0)
 Requires-Dist: cryptography (>=42.0.5)
 Requires-Dist: fire (==0.5.0)
 Requires-Dist: protobuf (>=4.25.3,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: snowflake_id (==1.0.2)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Project-URL: Repository, https://github.com/NimbleBoxAI/tuneapi
 Description-Content-Type: text/markdown
 
 # Tune API
 
 Package for using
```

