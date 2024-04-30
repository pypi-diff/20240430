# Comparing `tmp/dsws_client-1.1.0.tar.gz` & `tmp/dsws_client-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsws_client-1.1.0.tar", last modified: Tue Apr 30 09:09:48 2024, max compression
+gzip compressed data, was "dsws_client-1.1.1.tar", last modified: Tue Apr 30 13:55:26 2024, max compression
```

## Comparing `dsws_client-1.1.0.tar` & `dsws_client-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      753 2024-04-30 09:09:30.575347 dsws_client-1.1.0/README.md
--rw-r--r--   0        0        0      319 2024-04-30 09:09:30.575347 dsws_client-1.1.0/dsws_client/__init__.py
--rw-r--r--   0        0        0    12687 2024-04-30 09:09:30.575347 dsws_client-1.1.0/dsws_client/client.py
--rw-r--r--   0        0        0     1589 2024-04-30 09:09:30.575347 dsws_client-1.1.0/dsws_client/config.py
--rw-r--r--   0        0        0      757 2024-04-30 09:09:30.575347 dsws_client-1.1.0/dsws_client/converters.py
--rw-r--r--   0        0        0     9523 2024-04-30 09:09:30.575347 dsws_client-1.1.0/dsws_client/ds_request.py
--rw-r--r--   0        0        0     5417 2024-04-30 09:09:30.579347 dsws_client-1.1.0/dsws_client/ds_response.py
--rw-r--r--   0        0        0      510 2024-04-30 09:09:30.579347 dsws_client-1.1.0/dsws_client/exceptions.py
--rw-r--r--   0        0        0     5907 2024-04-30 09:09:30.579347 dsws_client-1.1.0/dsws_client/parse.py
--rw-r--r--   0        0        0        0 2024-04-30 09:09:30.579347 dsws_client-1.1.0/dsws_client/py.typed
--rw-r--r--   0        0        0      508 2024-04-30 09:09:30.579347 dsws_client-1.1.0/dsws_client/value_objects/__init__.py
--rw-r--r--   0        0        0     1603 2024-04-30 09:09:30.579347 dsws_client-1.1.0/dsws_client/value_objects/enums.py
--rw-r--r--   0        0        0      563 2024-04-30 09:09:30.579347 dsws_client-1.1.0/dsws_client/value_objects/types.py
--rw-r--r--   0        0        0       77 2024-04-30 09:09:30.579347 dsws_client-1.1.0/dsws_client/version.py
--rw-r--r--   0        0        0     3206 2024-04-30 09:09:48.399275 dsws_client-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       18 2024-04-30 09:09:30.579347 dsws_client-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0     2940 2024-04-30 09:09:30.579347 dsws_client-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0     2567 2024-04-30 09:09:30.579347 dsws_client-1.1.0/tests/test_client.py
--rw-r--r--   0        0        0     1248 2024-04-30 09:09:30.579347 dsws_client-1.1.0/tests/test_parsing.py
--rw-r--r--   0        0        0     4935 2024-04-30 09:09:30.579347 dsws_client-1.1.0/tests/test_requests.py
--rw-r--r--   0        0        0     1784 2024-04-30 09:09:30.579347 dsws_client-1.1.0/tests/test_responses.py
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 dsws_client-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      753 2024-04-30 13:55:07.989594 dsws_client-1.1.1/README.md
+-rw-r--r--   0        0        0      319 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/__init__.py
+-rw-r--r--   0        0        0    13127 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/client.py
+-rw-r--r--   0        0        0     1589 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/config.py
+-rw-r--r--   0        0        0      757 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/converters.py
+-rw-r--r--   0        0        0     9523 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/ds_request.py
+-rw-r--r--   0        0        0     5417 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/ds_response.py
+-rw-r--r--   0        0        0      510 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/exceptions.py
+-rw-r--r--   0        0        0     5907 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/parse.py
+-rw-r--r--   0        0        0        0 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/py.typed
+-rw-r--r--   0        0        0      508 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/value_objects/__init__.py
+-rw-r--r--   0        0        0     1603 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/value_objects/enums.py
+-rw-r--r--   0        0        0      563 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/value_objects/types.py
+-rw-r--r--   0        0        0       77 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/version.py
+-rw-r--r--   0        0        0     3206 2024-04-30 13:55:26.597586 dsws_client-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       18 2024-04-30 13:55:07.989594 dsws_client-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     2940 2024-04-30 13:55:07.989594 dsws_client-1.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     2567 2024-04-30 13:55:07.989594 dsws_client-1.1.1/tests/test_client.py
+-rw-r--r--   0        0        0     1248 2024-04-30 13:55:07.989594 dsws_client-1.1.1/tests/test_parsing.py
+-rw-r--r--   0        0        0     4935 2024-04-30 13:55:07.989594 dsws_client-1.1.1/tests/test_requests.py
+-rw-r--r--   0        0        0     1784 2024-04-30 13:55:07.989594 dsws_client-1.1.1/tests/test_responses.py
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 dsws_client-1.1.1/PKG-INFO
```

### Comparing `dsws_client-1.1.0/README.md` & `dsws_client-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.0/dsws_client/client.py` & `dsws_client-1.1.1/dsws_client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,97 +82,107 @@
     @property
     def token(self) -> str:
         """Get a token."""
         if self._token is None or self._token.is_expired:
             self._token = self.fetch_token()
         return self._token.token_value
 
-    def fetch_snapshot_data(
+    def fetch_snapshot_data(  # noqa: PLR0913
         self,
         identifiers: List[str],
         fields: List[str],
         start: Optional[DateType] = None,
         tag: Optional[str] = None,
+        *,
+        concurrent_requests: bool = False,
     ) -> ParsedResponse:
         """Fetch snapshot data."""
         data_responses = self.fetch_snapshot_data_iter(
             identifiers=identifiers,
             fields=fields,
             start=start,
             tag=tag,
+            concurrent_requests=concurrent_requests,
         )
         return aggregate_responses(data_responses)
 
-    def fetch_snapshot_data_iter(
+    def fetch_snapshot_data_iter(  # noqa: PLR0913
         self,
         identifiers: List[str],
         fields: List[str],
         start: Optional[DateType] = None,
         tag: Optional[str] = None,
+        *,
+        concurrent_requests: bool = False,
     ) -> Iterator[ParsedResponse]:
         """Fetch snapshot data, returning an iterator over responses."""
         request_bundles = self.construct_request_bundles(
             identifiers=identifiers,
             fields=fields,
             start=start,
             end=None,
             frequency=None,
             kind=0,
             tag=tag,
             return_symbol_names=True,
             return_field_names=True,
         )
-        responses = self.fetch_all(request_bundles)
+        responses = self.fetch_all(request_bundles, threaded=concurrent_requests)
         data_responses = itertools.chain.from_iterable(
             response.data_responses for response in responses
         )
         return responses_to_records(data_responses)
 
     def fetch_timeseries_data(  # noqa: PLR0913
         self,
         identifiers: List[str],
         fields: List[str],
         start: Optional[DateType] = None,
         end: Optional[DateType] = None,
         frequency: str = "D",
         tag: Optional[str] = None,
+        *,
+        concurrent_requests: bool = False,
     ) -> ParsedResponse:
         """Fetch timeseries data."""
         data_responses = self.fetch_timeseries_data_iter(
             identifiers=identifiers,
             fields=fields,
             start=start,
             end=end,
             frequency=frequency,
             tag=tag,
+            concurrent_requests=concurrent_requests,
         )
         return aggregate_responses(data_responses)
 
     def fetch_timeseries_data_iter(  # noqa: PLR0913
         self,
         identifiers: List[str],
         fields: List[str],
         start: Optional[DateType] = None,
         end: Optional[DateType] = None,
         frequency: str = "D",
         tag: Optional[str] = None,
+        *,
+        concurrent_requests: bool = False,
     ) -> Iterator[ParsedResponse]:
         """Fetch timeseries data, returning an iterator over responses."""
         request_bundles = self.construct_request_bundles(
             identifiers=identifiers,
             fields=fields,
             start=start,
             end=end,
             frequency=frequency,
             kind=1,
             tag=tag,
             return_symbol_names=True,
             return_field_names=True,
         )
-        responses = self.fetch_all(request_bundles)
+        responses = self.fetch_all(request_bundles, threaded=concurrent_requests)
         data_responses = itertools.chain.from_iterable(
             response.data_responses for response in responses
         )
         return responses_to_records(data_responses)
 
     def fetch_one(
         self,
@@ -227,23 +237,25 @@
             ),
             DSGetDataBundleResponse,
         )
 
     def fetch_all(
         self,
         request_bundles: List[List[DSDataRequest]],
+        *,
+        threaded: bool = False,
     ) -> Iterator[DSGetDataBundleResponse]:
         """Fetch as many bundles as needed to get all items."""
-        if self._max_concurrency > 1:
-            yield from self._fetch_all_threaded(request_bundles)
+        if threaded:
+            yield from self.fetch_all_threaded(request_bundles)
         else:
             for bundle in request_bundles:
                 yield self.fetch_bundle(bundle)
 
-    def _fetch_all_threaded(
+    def fetch_all_threaded(
         self,
         request_bundles: List[List[DSDataRequest]],
     ) -> Iterator[DSGetDataBundleResponse]:
         """Fetch as many bundles as needed to get all items (concurrently)."""
         with concurrent.futures.ThreadPoolExecutor(
             max_workers=self._max_concurrency
         ) as executor:
```

### Comparing `dsws_client-1.1.0/dsws_client/config.py` & `dsws_client-1.1.1/dsws_client/config.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.0/dsws_client/converters.py` & `dsws_client-1.1.1/dsws_client/converters.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.0/dsws_client/ds_request.py` & `dsws_client-1.1.1/dsws_client/ds_request.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.0/dsws_client/ds_response.py` & `dsws_client-1.1.1/dsws_client/ds_response.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.0/dsws_client/parse.py` & `dsws_client-1.1.1/dsws_client/parse.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.0/dsws_client/value_objects/enums.py` & `dsws_client-1.1.1/dsws_client/value_objects/enums.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.0/dsws_client/value_objects/types.py` & `dsws_client-1.1.1/dsws_client/value_objects/types.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.0/pyproject.toml` & `dsws_client-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dsws-client"
-version = "1.1.0"
+version = "1.1.1"
 description = "Python client for the Datastream Web Service API (DSWS)"
 readme = "README.md"
 authors = [
     { name = "ljnsn", email = "info@ljnsn.com" },
 ]
 requires-python = ">=3.8,<4.0"
 dependencies = [
```

### Comparing `dsws_client-1.1.0/tests/conftest.py` & `dsws_client-1.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.0/tests/test_client.py` & `dsws_client-1.1.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.0/tests/test_parsing.py` & `dsws_client-1.1.1/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.0/tests/test_requests.py` & `dsws_client-1.1.1/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.0/tests/test_responses.py` & `dsws_client-1.1.1/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.0/PKG-INFO` & `dsws_client-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsws-client
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python client for the Datastream Web Service API (DSWS)
 Author-Email: ljnsn <info@ljnsn.com>
 License: MIT
 Requires-Python: <4.0,>=3.8
 Requires-Dist: attrs>=23.1.0
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: msgspec>=0.18.6
```

