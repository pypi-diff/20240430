# Comparing `tmp/gofeatureflag_python_provider-0.1.2.tar.gz` & `tmp/gofeatureflag_python_provider-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gofeatureflag_python_provider-0.1.2.tar", max compression
+gzip compressed data, was "gofeatureflag_python_provider-0.2.0.tar", max compression
```

## Comparing `gofeatureflag_python_provider-0.1.2.tar` & `gofeatureflag_python_provider-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     2705 2024-03-19 09:18:08.550915 gofeatureflag_python_provider-0.1.2/README.md
--rw-r--r--   0        0        0       22 2024-03-19 09:18:08.550915 gofeatureflag_python_provider-0.1.2/gofeatureflag_python_provider/__init__.py
--rw-r--r--   0        0        0     5276 2024-03-19 09:18:08.550915 gofeatureflag_python_provider-0.1.2/gofeatureflag_python_provider/data_collector_hook.py
--rw-r--r--   0        0        0      172 2024-03-19 09:18:08.550915 gofeatureflag_python_provider-0.1.2/gofeatureflag_python_provider/metadata.py
--rw-r--r--   0        0        0     1863 2024-03-19 09:18:08.550915 gofeatureflag_python_provider-0.1.2/gofeatureflag_python_provider/options.py
--rw-r--r--   0        0        0    12667 2024-03-19 09:18:08.554915 gofeatureflag_python_provider-0.1.2/gofeatureflag_python_provider/provider.py
--rw-r--r--   0        0        0      181 2024-03-19 09:18:08.554915 gofeatureflag_python_provider-0.1.2/gofeatureflag_python_provider/provider_status.py
--rw-r--r--   0        0        0     2225 2024-03-19 09:18:08.554915 gofeatureflag_python_provider-0.1.2/gofeatureflag_python_provider/request_data_collector.py
--rw-r--r--   0        0        0     1599 2024-03-19 09:18:08.554915 gofeatureflag_python_provider-0.1.2/gofeatureflag_python_provider/request_flag_evaluation.py
--rw-r--r--   0        0        0      512 2024-03-19 09:18:08.554915 gofeatureflag_python_provider-0.1.2/gofeatureflag_python_provider/response_flag_evaluation.py
--rw-r--r--   0        0        0     1514 2024-03-19 09:18:08.934911 gofeatureflag_python_provider-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4242 1970-01-01 00:00:00.000000 gofeatureflag_python_provider-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2705 2024-04-30 10:47:25.769516 gofeatureflag_python_provider-0.2.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-30 10:47:25.769516 gofeatureflag_python_provider-0.2.0/gofeatureflag_python_provider/__init__.py
+-rw-r--r--   0        0        0     5276 2024-04-30 10:47:25.769516 gofeatureflag_python_provider-0.2.0/gofeatureflag_python_provider/data_collector_hook.py
+-rw-r--r--   0        0        0      172 2024-04-30 10:47:25.769516 gofeatureflag_python_provider-0.2.0/gofeatureflag_python_provider/metadata.py
+-rw-r--r--   0        0        0     1863 2024-04-30 10:47:25.769516 gofeatureflag_python_provider-0.2.0/gofeatureflag_python_provider/options.py
+-rw-r--r--   0        0        0    10682 2024-04-30 10:47:25.769516 gofeatureflag_python_provider-0.2.0/gofeatureflag_python_provider/provider.py
+-rw-r--r--   0        0        0     2225 2024-04-30 10:47:25.769516 gofeatureflag_python_provider-0.2.0/gofeatureflag_python_provider/request_data_collector.py
+-rw-r--r--   0        0        0     1599 2024-04-30 10:47:25.769516 gofeatureflag_python_provider-0.2.0/gofeatureflag_python_provider/request_flag_evaluation.py
+-rw-r--r--   0        0        0      503 2024-04-30 10:47:25.769516 gofeatureflag_python_provider-0.2.0/gofeatureflag_python_provider/response_flag_evaluation.py
+-rw-r--r--   0        0        0     1514 2024-04-30 10:47:26.169520 gofeatureflag_python_provider-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4242 1970-01-01 00:00:00.000000 gofeatureflag_python_provider-0.2.0/PKG-INFO
```

### Comparing `gofeatureflag_python_provider-0.1.2/README.md` & `gofeatureflag_python_provider-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gofeatureflag_python_provider-0.1.2/gofeatureflag_python_provider/data_collector_hook.py` & `gofeatureflag_python_provider-0.2.0/gofeatureflag_python_provider/data_collector_hook.py`

 * *Files identical despite different names*

### Comparing `gofeatureflag_python_provider-0.1.2/gofeatureflag_python_provider/options.py` & `gofeatureflag_python_provider-0.2.0/gofeatureflag_python_provider/options.py`

 * *Files identical despite different names*

### Comparing `gofeatureflag_python_provider-0.1.2/gofeatureflag_python_provider/provider.py` & `gofeatureflag_python_provider-0.2.0/gofeatureflag_python_provider/provider.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,21 +14,20 @@
     GeneralError,
     OpenFeatureError,
     TypeMismatchError,
 )
 from openfeature.flag_evaluation import FlagResolutionDetails, Reason
 from openfeature.hook import Hook
 from openfeature.provider.metadata import Metadata
-from openfeature.provider.provider import AbstractProvider
+from openfeature.provider import AbstractProvider
 from pydantic import PrivateAttr, ValidationError
 
 from gofeatureflag_python_provider.data_collector_hook import DataCollectorHook
 from gofeatureflag_python_provider.metadata import GoFeatureFlagMetadata
 from gofeatureflag_python_provider.options import BaseModel, GoFeatureFlagOptions
-from gofeatureflag_python_provider.provider_status import ProviderStatus
 from gofeatureflag_python_provider.request_flag_evaluation import (
     RequestFlagEvaluation,
     convert_evaluation_context,
 )
 from gofeatureflag_python_provider.response_flag_evaluation import (
     JsonType,
     ResponseFlagEvaluation,
@@ -42,15 +41,14 @@
     pass
 
 
 class GoFeatureFlagProvider(BaseModel, AbstractProvider, metaclass=CombinedMetaclass):
     options: GoFeatureFlagOptions
     _http_client: urllib3.PoolManager = PrivateAttr()
     _cache: pylru.lrucache = PrivateAttr()
-    _status: ProviderStatus = PrivateAttr(ProviderStatus.NOT_READY)
     _data_collector_hook: Optional[DataCollectorHook] = PrivateAttr()
     _ws: websocket.WebSocketApp = PrivateAttr()
     _ws_thread: Thread = PrivateAttr()
 
     def __init__(self, **data):
         """
         Constructor of the provider.
@@ -71,55 +69,41 @@
             options=self.options,
             http_client=self._http_client,
         )
         websocket.enableTrace(self.options.debug)
         self._ws = websocket.WebSocketApp(
             self._build_websocket_uri(),
             on_message=self._websocket_message_handler,
-            on_open=self._websocket_open_handler,
-            on_close=self._websocket_close_handler,
-            on_error=self._websocket_error_handler,
         )
 
-    def get_status(self) -> ProviderStatus:
-        """
-        get_status returns the status of the provider
-        :return: the status of the provider
-        """
-        return self._status
-
     def initialize(self, evaluation_context: EvaluationContext) -> None:
         """
         initialize is called when the provider is initialized.
         :param evaluation_context: the evaluation context
         :return: None
         """
         self._cache = pylru.lrucache(self.options.cache_size)
         self._data_collector_hook.initialize()
         # start the websocket thread
         if self.options.disable_cache_invalidation is False:
             self._ws_thread = Thread(target=self.run_websocket)
             self._ws_thread.start()
-        else:
-            self._status = ProviderStatus.READY
 
     def shutdown(self):
         if self.options.disable_cache_invalidation is False:
             self._ws.close(status=websocket.STATUS_NORMAL)
             self._ws_thread.join()
 
         if self._cache is not None:
             self._cache.clear()
 
         if self._data_collector_hook is not None:
             self._data_collector_hook.shutdown()
             self._data_collector_hook = None
 
-        self._status = ProviderStatus.NOT_READY
-
     def get_metadata(self) -> Metadata:
         return GoFeatureFlagMetadata()
 
     def get_provider_hooks(self) -> List[Hook]:
         if self._data_collector_hook is None:
             return []
         return [self._data_collector_hook]
@@ -188,22 +172,14 @@
         :param original_type: type of the request
         :param flag_key:  name of the flag
         :param default_value: default value of the flag
         :param evaluation_context: context to evaluate the flag
         :return: a FlagResolutionDetails object containing the response for the SDK.
         """
         try:
-            if self._status != ProviderStatus.READY:
-                return FlagResolutionDetails[original_type](
-                    value=default_value,
-                    reason=Reason.ERROR,
-                    error_code=ErrorCode.PROVIDER_NOT_READY,
-                    error_message="GO Feature Flag provider is not ready",
-                )
-
             goff_evaluation_context = convert_evaluation_context(evaluation_context)
             goff_request = RequestFlagEvaluation(
                 user=goff_evaluation_context,
                 defaultValue=default_value,
             )
             evaluation_context_hash = goff_evaluation_context.hash()
             is_from_cache = False
@@ -306,36 +282,9 @@
         :param wsapp: the websocket app
         :param message: the message received
         :return: None
         """
         # when we receive a message from go-feature-flag server, we clear the cache.
         self._cache.clear()
 
-    def _websocket_open_handler(self, ws_app) -> None:
-        """
-        websocket_open_handler is the handler called when the websocket is open
-        :param ws app: the websocket app
-        :return: None
-        """
-        self._status = ProviderStatus.READY
-
-    def _websocket_error_handler(self, ws_app, error) -> None:
-        """
-        websocket_error_handler is the handler called when we receive an error from the GO Feature Flag server
-        :param ws_app: the websocket app
-        :param error: error received
-        :return: None
-        """
-        self._status = ProviderStatus.ERROR
-
-    def _websocket_close_handler(self, ws_app, close_status_code, close_msg) -> None:
-        """
-        websocket_close_handler is the handler called when the websocket is closed
-        :param wsapp: the websocket app
-        :param close_status_code: the status code of the close
-        :param close_msg: the message of the close
-        :return: None
-        """
-        self._status = ProviderStatus.STALE
-
     def __hash__(self):
         return id(self)
```

### Comparing `gofeatureflag_python_provider-0.1.2/gofeatureflag_python_provider/request_data_collector.py` & `gofeatureflag_python_provider-0.2.0/gofeatureflag_python_provider/request_data_collector.py`

 * *Files identical despite different names*

### Comparing `gofeatureflag_python_provider-0.1.2/gofeatureflag_python_provider/request_flag_evaluation.py` & `gofeatureflag_python_provider-0.2.0/gofeatureflag_python_provider/request_flag_evaluation.py`

 * *Files identical despite different names*

### Comparing `gofeatureflag_python_provider-0.1.2/pyproject.toml` & `gofeatureflag_python_provider-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gofeatureflag-python-provider"
-version = "0.1.2"
+version = "0.2.0"
 description = "GO Feature Flag provider for OpenFeature"
 license = "Apache-2.0"
 authors = [ "Thomas Poignant" ]
 readme = "README.md"
 homepage = "https://gofeatureflag.org"
 repository = "https://github.com/thomaspoignant/go-feature-flag"
 documentation = "https://github.com/thomaspoignant/go-feature-flag/tree/main/openfeature/providers/python-provider"
@@ -24,15 +24,15 @@
   [tool.poetry.urls]
   "Bug Tracker" = "https://github.com/thomaspoignant/go-feature-flag/issues"
   "Source Code" = "https://github.com/thomaspoignant/go-feature-flag/tree/main/openfeature/providers/python-provider"
   Documentation = "https://github.com/thomaspoignant/go-feature-flag/tree/main/openfeature/providers/python-provider"
 
   [tool.poetry.dependencies]
   python = "^3.9"
-  openfeature-sdk = ">=0.5.0,<0.6.0"
+  openfeature-sdk = ">=0.5.0,<0.8.0"
   pydantic = "^2.5.2"
   urllib3 = "^2.1.0"
   pylru = "^1.2.1"
   websocket-client = "^1.6.4"
   rel = "^0.4.9"
   asyncio = "^3.4.3"
```

### Comparing `gofeatureflag_python_provider-0.1.2/PKG-INFO` & `gofeatureflag_python_provider-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gofeatureflag-python-provider
-Version: 0.1.2
+Version: 0.2.0
 Summary: GO Feature Flag provider for OpenFeature
 Home-page: https://gofeatureflag.org
 License: Apache-2.0
 Keywords: feature flags,feature toggles,go-feature-flag,gofeatureflag,openfeature,open-feature
 Author: Thomas Poignant
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
-Requires-Dist: openfeature-sdk (>=0.5.0,<0.6.0)
+Requires-Dist: openfeature-sdk (>=0.5.0,<0.8.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Requires-Dist: pylru (>=1.2.1,<2.0.0)
 Requires-Dist: rel (>=0.4.9,<0.5.0)
 Requires-Dist: urllib3 (>=2.1.0,<3.0.0)
 Requires-Dist: websocket-client (>=1.6.4,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/thomaspoignant/go-feature-flag/issues
 Project-URL: Documentation, https://github.com/thomaspoignant/go-feature-flag/tree/main/openfeature/providers/python-provider
```

