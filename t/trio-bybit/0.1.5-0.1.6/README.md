# Comparing `tmp/trio_bybit-0.1.5.tar.gz` & `tmp/trio_bybit-0.1.6.tar.gz`

## Comparing `trio_bybit-0.1.5.tar` & `trio_bybit-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/pytest.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/tests/test_async_client.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/tests/test_streams.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/trio_bybit/__init__.py
--rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/trio_bybit/client.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/trio_bybit/enums.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/trio_bybit/exceptions.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/trio_bybit/helpers.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/trio_bybit/streams.py
--rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/LICENSE
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/README.md
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 trio_bybit-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/pytest.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/tests/test_async_client.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/tests/test_streams.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/trio_bybit/__init__.py
+-rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/trio_bybit/client.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/trio_bybit/enums.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/trio_bybit/exceptions.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/trio_bybit/helpers.py
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/trio_bybit/streams.py
+-rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/LICENSE
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/README.md
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/PKG-INFO
```

### Comparing `trio_bybit-0.1.5/tests/test_async_client.py` & `trio_bybit-0.1.6/tests/test_async_client.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.5/tests/test_streams.py` & `trio_bybit-0.1.6/tests/test_streams.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,45 +2,56 @@
 
 import trio
 import pytest_trio
 
 from trio_bybit.streams import BybitSocketManager
 
 
+async def pub_stream_check(socket):
+    async for msg in socket.get_next_message():
+        assert "ts" in msg
+        assert "type" in msg
+        assert "data" in msg
+
+
+async def pub_unsub(socket):
+    unsub = {
+        "op": "unsubscribe",
+        "args": ["orderbook.1.BTCUSDT", "publicTrade.BTCUSDT"],
+    }
+    await socket.subscribe(unsub)
+
+
 async def test_public_stream():
     socket = BybitSocketManager()
     async with socket.connect():
         subscription = {
             "op": "subscribe",
             "args": ["orderbook.1.BTCUSDT", "publicTrade.BTCUSDT"],
         }
         await socket.subscribe(subscription)
 
-        count = 0
-        async for msg in socket.get_next_message():
-            count += 1
-            assert "ts" in msg
-            assert "type" in msg
-            assert "data" in msg
-            if count >= 500:
-                break
+        with trio.move_on_after(12):
+            async with trio.open_nursery() as nursery:
+                nursery.start_soon(pub_stream_check, socket)
+                await trio.sleep(10)
+                nursery.start_soon(pub_unsub, socket)
 
 
 async def test_public_linear_stream():
     socket = BybitSocketManager(endpoint="linear")
     async with socket.connect():
         subscription = {
             "op": "subscribe",
             "args": ["orderbook.1.BTCUSDT", "publicTrade.BTCUSDT"],
         }
         await socket.subscribe(subscription)
 
         count = 0
         async for msg in socket.get_next_message():
-            print(msg)
             count += 1
             if msg.get("topic") == "orderbook.1.BTCUSDT":
                 assert "topic" in msg
                 assert "type" in msg
                 assert "data" in msg
                 assert "s" in msg["data"]
                 assert "a" in msg["data"]
@@ -48,17 +59,14 @@
             elif msg.get("topic") == "publicTrade.BTCUSDT":
                 assert "topic" in msg
                 assert "type" in msg
                 assert "data" in msg
                 assert "S" in msg["data"][0]
                 assert "v" in msg["data"][0]
                 assert "p" in msg["data"][0]
-            else:  # this endpoint responses subscription asynchronously with actual data
-                assert msg["op"] == "subscribe"
-                assert msg["success"]
             if count >= 5000:
                 break
 
 
 async def test_private_stream():
     socket = BybitSocketManager(
         endpoint="private",
```

### Comparing `trio_bybit-0.1.5/trio_bybit/client.py` & `trio_bybit-0.1.6/trio_bybit/client.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.5/trio_bybit/exceptions.py` & `trio_bybit-0.1.6/trio_bybit/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,11 +66,16 @@
         super().__init__(-1013, message)
 
 
 class BybitWebsocketUnableToConnect(Exception):
     pass
 
 
+class BybitWebsocketOpError(Exception):
+    def __init__(self, message):
+        self.message = message
+
+
 class NotImplementedException(Exception):
     def __init__(self, value):
         message = f"Not implemented: {value}"
         super().__init__(message)
```

### Comparing `trio_bybit-0.1.5/trio_bybit/helpers.py` & `trio_bybit-0.1.6/trio_bybit/helpers.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.5/trio_bybit/streams.py` & `trio_bybit-0.1.6/trio_bybit/streams.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from contextlib import asynccontextmanager
 
 import trio
 import orjson
 import trio_websocket
 from trio_websocket import open_websocket_url
 
+from trio_bybit.exceptions import BybitWebsocketOpError
+
 
 class BybitSocketManager:
     URLS = {
         "main": {
             "spot": "wss://stream.bybit.com/v5/public/spot",
             "linear": "wss://stream.bybit.com/v5/public/linear",
             "inverse": "wss://stream.bybit.com/v5/public/inverse",
@@ -49,14 +51,16 @@
             url = self.URLS[self.alternative_net][self.endpoint]
         except KeyError:
             raise ValueError(f"endpoint {self.endpoint} with net {self.alternative_net} not supported")
         async with open_websocket_url(url) as ws:
             self.ws = ws
             async with trio.open_nursery() as nursery:
                 nursery.start_soon(self.heartbeat)
+                if self.endpoint == "private":
+                    await self._send_signature()
                 yield self.ws
                 nursery.cancel_scope.cancel()
 
     async def heartbeat(self):
         while True:
             with trio.fail_after(5):
                 await self.ws.send_message('{"op": "ping"}')
@@ -67,30 +71,29 @@
         signature = str(
             hmac.new(
                 self.api_secret.encode("utf-8"), f"GET/realtime{expires}".encode("utf-8"), digestmod="sha256"
             ).hexdigest()
         )
         await self.ws.send_message(orjson.dumps({"op": "auth", "args": [self.api_key, expires, signature]}))
         auth_ret = orjson.loads(await self.ws.get_message())
-        print(auth_ret)
         if auth_ret["op"] == "auth":
             assert auth_ret["success"]
             self.conn_id = auth_ret["conn_id"]
 
-    async def subscribe(self, subscription):
-        if self.endpoint == "private":
-            await self._send_signature()
+    async def subscribe(self, subscription: dict):
+        """
+        Subscribe or unsubscribe to a websocket stream.
+        :param subscription: (un)subscription message, e.g. {"op": "subscribe", "args": ["publicTrade.BTCUSDT"]}
+        """
         await self.ws.send_message(orjson.dumps(subscription))
-        if self.endpoint == "spot":  # seems only spot has an immediate response
-            subscribed = orjson.loads(await self.ws.get_message())
-            assert subscribed["op"] == "subscribe"
-            assert subscribed["ret_msg"] == "subscribe"
-            assert subscribed["success"]
-            assert "conn_id" in subscribed
 
     async def get_next_message(self):
         while True:
             raw_message = await self.ws.get_message()
             message = orjson.loads(raw_message)
-            if message.get("ret_msg") == "pong":
-                continue
-            yield message
+            if "topic" in message and "data" in message:
+                yield message
+            elif "op" in message:
+                if message["op"] == "pong":
+                    continue
+                if not message.get("success"):  # probably a subscription error
+                    raise BybitWebsocketOpError(raw_message)
```

### Comparing `trio_bybit-0.1.5/.gitignore` & `trio_bybit-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.5/LICENSE` & `trio_bybit-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.5/README.md` & `trio_bybit-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.5/pyproject.toml` & `trio_bybit-0.1.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "trio-bybit"
-version = "0.1.5"
+version = "0.1.6"
 description = "Python bybit async SDK based on trio."
 authors = [
     { name = "Shu Wang", email = "halfelf.ronin@gmail.com" }
 ]
 dependencies = [
     "trio>=0.25.0",
     "httpx[http2]>=0.27.0",
```

### Comparing `trio_bybit-0.1.5/PKG-INFO` & `trio_bybit-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: trio-bybit
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python bybit async SDK based on trio.
 Project-URL: Repository, https://github.com/halfelf/trio-bybit
 Author-email: Shu Wang <halfelf.ronin@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Shu Wang <halfelf.ronin@gmail.com>
```

