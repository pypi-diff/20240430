# Comparing `tmp/bot_station_client-0.0.5.tar.gz` & `tmp/bot_station_client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bot_station_client-0.0.5.tar", last modified: Wed Apr  3 20:14:12 2024, max compression
+gzip compressed data, was "bot_station_client-0.1.0.tar", last modified: Tue Apr 30 19:21:55 2024, max compression
```

## Comparing `bot_station_client-0.0.5.tar` & `bot_station_client-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-04-03 20:14:12.657272 bot_station_client-0.0.5/
--rw-r--r--   0 mrmx       (501) staff       (20)     1070 2024-03-22 14:52:19.000000 bot_station_client-0.0.5/LICENSE
--rw-r--r--   0 mrmx       (501) staff       (20)      438 2024-04-03 20:14:12.656507 bot_station_client-0.0.5/PKG-INFO
--rw-r--r--   0 mrmx       (501) staff       (20)       24 2024-03-22 14:41:22.000000 bot_station_client-0.0.5/README.md
-drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-04-03 20:14:12.652495 bot_station_client-0.0.5/bot_station_client/
--rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-03-22 14:38:45.000000 bot_station_client-0.0.5/bot_station_client/__init__.py
--rw-r--r--   0 mrmx       (501) staff       (20)     2704 2024-04-03 19:49:02.000000 bot_station_client-0.0.5/bot_station_client/client.py
-drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-04-03 20:14:12.655023 bot_station_client-0.0.5/bot_station_client/model/
--rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-03-22 15:15:24.000000 bot_station_client-0.0.5/bot_station_client/model/__init__.py
--rw-r--r--   0 mrmx       (501) staff       (20)      100 2024-03-22 15:23:15.000000 bot_station_client-0.0.5/bot_station_client/model/config.py
-drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-04-03 20:14:12.655826 bot_station_client-0.0.5/bot_station_client.egg-info/
--rw-r--r--   0 mrmx       (501) staff       (20)      438 2024-04-03 20:14:12.000000 bot_station_client-0.0.5/bot_station_client.egg-info/PKG-INFO
--rw-r--r--   0 mrmx       (501) staff       (20)      367 2024-04-03 20:14:12.000000 bot_station_client-0.0.5/bot_station_client.egg-info/SOURCES.txt
--rw-r--r--   0 mrmx       (501) staff       (20)        1 2024-04-03 20:14:12.000000 bot_station_client-0.0.5/bot_station_client.egg-info/dependency_links.txt
--rw-r--r--   0 mrmx       (501) staff       (20)       32 2024-04-03 20:14:12.000000 bot_station_client-0.0.5/bot_station_client.egg-info/requires.txt
--rw-r--r--   0 mrmx       (501) staff       (20)       19 2024-04-03 20:14:12.000000 bot_station_client-0.0.5/bot_station_client.egg-info/top_level.txt
--rw-r--r--   0 mrmx       (501) staff       (20)       38 2024-04-03 20:14:12.657414 bot_station_client-0.0.5/setup.cfg
--rw-r--r--   0 mrmx       (501) staff       (20)      780 2024-04-03 20:13:54.000000 bot_station_client-0.0.5/setup.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-04-30 19:21:55.470237 bot_station_client-0.1.0/
+-rw-r--r--   0 mrmx       (501) staff       (20)     1070 2024-03-22 14:52:19.000000 bot_station_client-0.1.0/LICENSE
+-rw-r--r--   0 mrmx       (501) staff       (20)      438 2024-04-30 19:21:55.469142 bot_station_client-0.1.0/PKG-INFO
+-rw-r--r--   0 mrmx       (501) staff       (20)       24 2024-03-22 14:41:22.000000 bot_station_client-0.1.0/README.md
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-04-30 19:21:55.462852 bot_station_client-0.1.0/bot_station_client/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-03-22 14:38:45.000000 bot_station_client-0.1.0/bot_station_client/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)     3561 2024-04-30 19:10:20.000000 bot_station_client-0.1.0/bot_station_client/client.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-04-30 19:21:55.466359 bot_station_client-0.1.0/bot_station_client/model/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-03-22 15:15:24.000000 bot_station_client-0.1.0/bot_station_client/model/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      237 2024-04-29 11:58:01.000000 bot_station_client-0.1.0/bot_station_client/model/call_result.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      100 2024-03-22 15:23:15.000000 bot_station_client-0.1.0/bot_station_client/model/config.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      241 2024-04-30 19:18:13.000000 bot_station_client-0.1.0/bot_station_client/model/document.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-04-30 19:21:55.468182 bot_station_client-0.1.0/bot_station_client.egg-info/
+-rw-r--r--   0 mrmx       (501) staff       (20)      438 2024-04-30 19:21:55.000000 bot_station_client-0.1.0/bot_station_client.egg-info/PKG-INFO
+-rw-r--r--   0 mrmx       (501) staff       (20)      499 2024-04-30 19:21:55.000000 bot_station_client-0.1.0/bot_station_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mrmx       (501) staff       (20)        1 2024-04-30 19:21:55.000000 bot_station_client-0.1.0/bot_station_client.egg-info/dependency_links.txt
+-rw-r--r--   0 mrmx       (501) staff       (20)       32 2024-04-30 19:21:55.000000 bot_station_client-0.1.0/bot_station_client.egg-info/requires.txt
+-rw-r--r--   0 mrmx       (501) staff       (20)       25 2024-04-30 19:21:55.000000 bot_station_client-0.1.0/bot_station_client.egg-info/top_level.txt
+-rw-r--r--   0 mrmx       (501) staff       (20)       38 2024-04-30 19:21:55.470415 bot_station_client-0.1.0/setup.cfg
+-rw-r--r--   0 mrmx       (501) staff       (20)      780 2024-04-30 19:21:39.000000 bot_station_client-0.1.0/setup.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-04-30 19:21:55.467326 bot_station_client-0.1.0/tests/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-04-29 10:41:42.000000 bot_station_client-0.1.0/tests/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)     1947 2024-04-30 19:19:28.000000 bot_station_client-0.1.0/tests/bot_station_client_e2e_test.py
```

### Comparing `bot_station_client-0.0.5/LICENSE` & `bot_station_client-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bot_station_client-0.0.5/bot_station_client/client.py` & `bot_station_client-0.1.0/bot_station_client/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import json
-from typing import Dict, Any
+import logging
+import uuid
+from typing import Dict
 
 import aiohttp
+
+from bot_station_client.model.call_result import CallResult
 from bot_station_client.model.config import BotStationClientConfig
 
 
 class BotStationClient:
     config: BotStationClientConfig = ""
 
     def __init__(self, config: BotStationClientConfig):
@@ -35,55 +39,74 @@
                 "description": description,
                 "prompt_intro": prompt_intro,
                 "add_external_context_to_prompt": str(add_external_context_to_prompt).lower(),
                 "add_messages_history_to_prompt": str(add_messages_history_to_prompt).lower(),
                 "temperature": temperature,
             }
         )
-        return response_json["id"]
+        return str(response_json["id"])
 
     async def train(self,
                     bot_id: str,
-                    text: str
+                    text: str,
+                    id: str = str(uuid.uuid4()),
+                    source_link: str | None = None,
+                    metadata: dict[str, str] | None = None,
                     ):
+        content = {"bot_id": bot_id, "data": text, "id": id}
+
+        if source_link is not None:
+            content["source_link"] = source_link
+        if metadata is not None:
+            content["metadata"] = metadata
+
         await self.__post(
-            method="create",
-            content={
-                "id": bot_id,
-                "data": text,
-            }
+            method="train",
+            content=content
         )
 
     async def call(self,
                    bot_id: str,
                    chat_id: int | str,
                    text: str
-                   ) -> str:
+                   ) -> CallResult:
         """
         :param bot_id:
         :param chat_id:
         :param text:
         :return: bot's response
         """
-        response_json = await self.__post(
+        response_dict = await self.__post(
             method="call",
             content={
                 "bot_id": bot_id,
                 "chat_id": chat_id,
                 "data": text
             }
         )
-        return response_json["text"]
+        response_str = json.dumps(response_dict)
+        result = CallResult(response_str)
+
+        return result
 
     async def __post(self,
                      method: str,
                      content: Dict[str, str | int],
-                     ) -> Any:
+                     ) -> dict[str, object]:
         """
         Returns response json body
         """
         headers: Dict[str, str] = {'content-type': 'application/json'}
         session = aiohttp.ClientSession(headers=headers)
         url = f'{self.config.base_uri}/{method}'
+        logging.debug(f"POST /{method}  {content}")
         response = await session.post(url=url, data=json.dumps(content))
-        data = await response.json()
-        return data
+        if response.status == 200:
+            if response.content_type == 'application/json':
+                data = await response.json()
+            else:
+                data = {}
+            await session.close()
+            return data
+        else:
+            await session.close()
+            raise Exception(f"{response.status} {response.content}")
```

### Comparing `bot_station_client-0.0.5/setup.py` & `bot_station_client-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="bot_station_client",
-    version="0.0.5",
+    version="0.1.0",
     author="Maxim Marashan",
     # author_email="ericjaychi@gmail.com",
     description="Bot Station client SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://github.com/ericjaychi/sample-pypi-package",
     packages=setuptools.find_packages(),
```

