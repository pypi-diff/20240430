# Comparing `tmp/cheeseapi-1.1.2.tar.gz` & `tmp/cheeseapi-1.1.3.tar.gz`

## Comparing `cheeseapi-1.1.2.tar` & `cheeseapi-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/__init__.py
--rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/app.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/cors.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/exception.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/file.py
--rw-r--r--   0        0        0    32439 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/handle.py
--rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/protocol.py
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/request.py
--rw-r--r--   0        0        0    17621 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/response.py
--rw-r--r--   0        0        0    11145 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/route.py
--rw-r--r--   0        0        0    10335 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/schedule.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/server.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/signal.py
--rw-r--r--   0        0        0     8509 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/text.py
--rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/validator.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/websocket.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/CheeseAPI/workspace.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/LICENSE
--rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 cheeseapi-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/CheeseAPI/__init__.py
+-rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/CheeseAPI/app.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/CheeseAPI/cors.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/CheeseAPI/exception.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/CheeseAPI/file.py
+-rw-r--r--   0        0        0    32435 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/CheeseAPI/handle.py
+-rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/CheeseAPI/protocol.py
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/CheeseAPI/request.py
+-rw-r--r--   0        0        0    17621 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/CheeseAPI/response.py
+-rw-r--r--   0        0        0    13129 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/CheeseAPI/route.py
+-rw-r--r--   0        0        0    10335 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/CheeseAPI/schedule.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/CheeseAPI/server.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/CheeseAPI/signal.py
+-rw-r--r--   0        0        0     8558 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/CheeseAPI/text.py
+-rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/CheeseAPI/validator.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/CheeseAPI/websocket.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/CheeseAPI/workspace.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/LICENSE
+-rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 cheeseapi-1.1.3/PKG-INFO
```

### Comparing `cheeseapi-1.1.2/CheeseAPI/app.py` & `cheeseapi-1.1.3/CheeseAPI/app.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.2/CheeseAPI/cors.py` & `cheeseapi-1.1.3/CheeseAPI/cors.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.2/CheeseAPI/exception.py` & `cheeseapi-1.1.3/CheeseAPI/exception.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.2/CheeseAPI/file.py` & `cheeseapi-1.1.3/CheeseAPI/file.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.2/CheeseAPI/handle.py` & `cheeseapi-1.1.3/CheeseAPI/handle.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,15 @@
                         'response': protocol.response,
                         **protocol.kwargs
                     })
                 await self.http_response(protocol)
                 return
 
             try:
-                func, protocol.kwargs = self._app.routeBus._match(protocol.request.path, protocol.request.method)
+                fn, protocol.kwargs = self._app.routeBus._match(protocol.request.path, protocol.request.method)
             except Route_404_Exception as e:
                 await self.http_afterRequest(protocol)
                 if self._app.signal.http_afterRequest.receivers:
                     await self._app.signal.http_afterRequest.async_send(**{
                         'request': protocol.request,
                         **protocol.kwargs
                     })
@@ -327,15 +327,15 @@
             await self.http_afterRequest(protocol)
             if self._app.signal.http_afterRequest.receivers:
                 await self._app.signal.http_afterRequest.async_send(**{
                     'request': protocol.request,
                     **protocol.kwargs
             })
 
-            protocol.response = await func(**{
+            protocol.response = await fn(**{
                 'request': protocol.request,
                 **protocol.kwargs
             })
 
             if self._app.signal.http_custom.receivers:
                 await self._app.signal.http_custom.async_send(**{
                     'request': protocol.request,
```

### Comparing `cheeseapi-1.1.2/CheeseAPI/protocol.py` & `cheeseapi-1.1.3/CheeseAPI/protocol.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.2/CheeseAPI/request.py` & `cheeseapi-1.1.3/CheeseAPI/request.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.2/CheeseAPI/response.py` & `cheeseapi-1.1.3/CheeseAPI/response.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.2/CheeseAPI/schedule.py` & `cheeseapi-1.1.3/CheeseAPI/schedule.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.2/CheeseAPI/server.py` & `cheeseapi-1.1.3/CheeseAPI/server.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, socket
+import os
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from CheeseAPI.app import App
 
 class Server:
     def __init__(self, app: 'App'):
```

### Comparing `cheeseapi-1.1.2/CheeseAPI/signal.py` & `cheeseapi-1.1.3/CheeseAPI/signal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Callable
+from typing import TYPE_CHECKING
 
 from CheeseSignal import Signal
 
 if TYPE_CHECKING:
     from CheeseAPI.app import App
 
 class _Signal:
```

### Comparing `cheeseapi-1.1.2/CheeseAPI/text.py` & `cheeseapi-1.1.3/CheeseAPI/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,19 @@
     def server_information(self) -> List[Tuple[str, str]]:
         return [
             (f'The master process {os.getpid()} started', f'The master process <blue>{os.getpid()}</blue> started'),
             (f'''Workspace Information:
 Base: {self._app.workspace.base}''' + (f'''
 Static: {self._app.workspace.static}''' if self._app.workspace.static and self._app.server.static else '') + (f'''
 Log: {self._app.workspace.log}''' if self._app.workspace.log and self._app.workspace.logger else '') + (f'''
-Logger: {self._app.workspace.logger}''' if self._app.workspace.log and self._app.workspace.logger else ''), f'''Workspace Information:
+Logger: {logger.encode(self._app.workspace.logger)}''' if self._app.workspace.log and self._app.workspace.logger else ''), f'''Workspace Information:
 Base: <cyan><underline>{self._app.workspace.base}</underline></cyan>''' + (f'''
 Static: <cyan><underline>{self._app.workspace.static}</underline></cyan>''' if self._app.workspace.static and self._app.server.static else '') + (f'''
 Log: <cyan><underline>{self._app.workspace.log}</underline></cyan>''' if self._app.workspace.log and self._app.workspace.logger else '') + (f'''
-Logger: <cyan><underline>{self._app.workspace.logger}</underline></cyan>''' if self._app.workspace.log and self._app.workspace.logger else '')),
+Logger: <cyan><underline>{logger.encode(self._app.workspace.logger)}</underline></cyan>''' if self._app.workspace.log and self._app.workspace.logger else '')),
             (f'''Server Information:
 Host: {self._app.server.host}
 Port: {self._app.server.port}
 Workers: {self._app.server.workers}
 Backlog: {self._app.server.backlog}''' + (f'''
 Static: {self._app.server.static}''' if self._app.workspace.static and self._app.server.static else ''), f'''Server Information:
 Host: <cyan>{self._app.server.host}</cyan>
@@ -147,30 +147,30 @@
         styledMessage += '<blue>{:.6f}</blue> seconds'.format(timer % 60)
 
         return [
             (message, styledMessage)
         ]
 
     def validator_requiredMessage(self, scope: str, key: str) -> str:
-        return f'参数{scope}.{key}是必要的'
+        return f'The {scope}.{key} is required'
 
     def validator_typeMessage(self, scope: str, key: str, expected_type: object) -> str:
-        return f'参数{scope}.{key}无法转换为{expected_type.__name__}'
+        return f'The {scope}.{key} cannot be converted to {expected_type.__name__}'
 
     def validator_patternMessage(self, scope: str, key: str) -> str:
-        return f'参数{scope}.{key}正则校验错误'
+        return f'The {scope}.{key} regular check error'
 
     def validator_minMessage(self, scope: str, key: str, min: object) -> str:
-        return f'参数{scope}.{key}不允许小于{min}'
+        return f'The {scope}.{key} cannot be less than {min}'
 
     def validator_maxMessage(self, scope: str, key: str, max: object) -> str:
-        return f'参数{scope}.{key}不允许大于{max}'
+        return f'The {scope}.{key} cannot be larger than {max}'
 
     def validator_enumMessage(self, scope: str, key: str, enum: List[Any]) -> str:
-        return f'参数{scope}.{key}不允许为{enum}之外的值'
+        return f'The {scope}.{key} cannot be a value other than {enum}'
 
     @property
     def process_title(self) -> str:
         return self._process_title
 
     @process_title.setter
     def process_title(self, value: str):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cheeseapi-1.1.2/CheeseAPI/validator.py` & `cheeseapi-1.1.3/CheeseAPI/validator.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.2/CheeseAPI/websocket.py` & `cheeseapi-1.1.3/CheeseAPI/websocket.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.2/CheeseAPI/workspace.py` & `cheeseapi-1.1.3/CheeseAPI/workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         return self._log
 
     @log.setter
     def log(self, value: str):
         self._log = value
 
         if self.log and self.logger:
-            logger.filePath = os.path.join(self.log, self.logger)
+            logger.filePath = os.path.join(self.base, self.log, self.logger)
         else:
             logger.filePath = ''
 
     @property
     def logger(self) -> str:
         return self._logger
 
@@ -94,10 +94,10 @@
             self._logger = self._app._text.logger
         elif value is False:
             self._logger = ''
         else:
             self._logger = value
 
         if self.log and self.logger:
-            logger.filePath = os.path.join(self.log, self.logger)
+            logger.filePath = os.path.join(self.base, self.log, self.logger)
         else:
             logger.filePath = ''
```

### Comparing `cheeseapi-1.1.2/LICENSE` & `cheeseapi-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.2/README.md` & `cheeseapi-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.1.2/pyproject.toml` & `cheeseapi-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "CheeseAPI"
-version = "1.1.2"
+version = "1.1.3"
 description = "一款web协程框架。"
 readme = "README.md"
 license-files = { paths = [ "LICENSE" ] }
 authors = [
     { name = "Cheese Unknown", email = "cheese@cheese.ren" }
 ]
 keywords = [ 'API', 'BackEnd' ]
```

### Comparing `cheeseapi-1.1.2/PKG-INFO` & `cheeseapi-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: CheeseAPI
-Version: 1.1.2
+Version: 1.1.3
 Summary: 一款web协程框架。
 Project-URL: Source, https://github.com/CheeseUnknown/CheeseAPI
 Author-email: Cheese Unknown <cheese@cheese.ren>
 License-File: LICENSE
 Keywords: API,BackEnd
 Requires-Dist: cheeselog==1.0.*
 Requires-Dist: cheesesignal==1.1.*
```

