# Comparing `tmp/dsws_client-1.0.0.tar.gz` & `tmp/dsws_client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsws_client-1.0.0.tar", last modified: Sun Apr 28 23:15:27 2024, max compression
+gzip compressed data, was "dsws_client-1.1.0.tar", last modified: Tue Apr 30 09:09:48 2024, max compression
```

## Comparing `dsws_client-1.0.0.tar` & `dsws_client-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      753 2024-04-28 23:15:09.255058 dsws_client-1.0.0/README.md
--rw-r--r--   0        0        0      319 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/__init__.py
--rw-r--r--   0        0        0    11479 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/client.py
--rw-r--r--   0        0        0     1589 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/config.py
--rw-r--r--   0        0        0      757 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/converters.py
--rw-r--r--   0        0        0     9523 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/ds_request.py
--rw-r--r--   0        0        0     5417 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/ds_response.py
--rw-r--r--   0        0        0      510 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/exceptions.py
--rw-r--r--   0        0        0     5698 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/parse.py
--rw-r--r--   0        0        0        0 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/py.typed
--rw-r--r--   0        0        0      508 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/value_objects/__init__.py
--rw-r--r--   0        0        0     1603 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/value_objects/enums.py
--rw-r--r--   0        0        0      563 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/value_objects/types.py
--rw-r--r--   0        0        0       77 2024-04-28 23:15:09.255058 dsws_client-1.0.0/dsws_client/version.py
--rw-r--r--   0        0        0     3206 2024-04-28 23:15:27.647108 dsws_client-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       18 2024-04-28 23:15:09.255058 dsws_client-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2940 2024-04-28 23:15:09.255058 dsws_client-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0     2567 2024-04-28 23:15:09.255058 dsws_client-1.0.0/tests/test_client.py
--rw-r--r--   0        0        0     1248 2024-04-28 23:15:09.255058 dsws_client-1.0.0/tests/test_parsing.py
--rw-r--r--   0        0        0     4935 2024-04-28 23:15:09.255058 dsws_client-1.0.0/tests/test_requests.py
--rw-r--r--   0        0        0     1784 2024-04-28 23:15:09.255058 dsws_client-1.0.0/tests/test_responses.py
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 dsws_client-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      753 2024-04-30 09:09:30.575347 dsws_client-1.1.0/README.md
+-rw-r--r--   0        0        0      319 2024-04-30 09:09:30.575347 dsws_client-1.1.0/dsws_client/__init__.py
+-rw-r--r--   0        0        0    12687 2024-04-30 09:09:30.575347 dsws_client-1.1.0/dsws_client/client.py
+-rw-r--r--   0        0        0     1589 2024-04-30 09:09:30.575347 dsws_client-1.1.0/dsws_client/config.py
+-rw-r--r--   0        0        0      757 2024-04-30 09:09:30.575347 dsws_client-1.1.0/dsws_client/converters.py
+-rw-r--r--   0        0        0     9523 2024-04-30 09:09:30.575347 dsws_client-1.1.0/dsws_client/ds_request.py
+-rw-r--r--   0        0        0     5417 2024-04-30 09:09:30.579347 dsws_client-1.1.0/dsws_client/ds_response.py
+-rw-r--r--   0        0        0      510 2024-04-30 09:09:30.579347 dsws_client-1.1.0/dsws_client/exceptions.py
+-rw-r--r--   0        0        0     5907 2024-04-30 09:09:30.579347 dsws_client-1.1.0/dsws_client/parse.py
+-rw-r--r--   0        0        0        0 2024-04-30 09:09:30.579347 dsws_client-1.1.0/dsws_client/py.typed
+-rw-r--r--   0        0        0      508 2024-04-30 09:09:30.579347 dsws_client-1.1.0/dsws_client/value_objects/__init__.py
+-rw-r--r--   0        0        0     1603 2024-04-30 09:09:30.579347 dsws_client-1.1.0/dsws_client/value_objects/enums.py
+-rw-r--r--   0        0        0      563 2024-04-30 09:09:30.579347 dsws_client-1.1.0/dsws_client/value_objects/types.py
+-rw-r--r--   0        0        0       77 2024-04-30 09:09:30.579347 dsws_client-1.1.0/dsws_client/version.py
+-rw-r--r--   0        0        0     3206 2024-04-30 09:09:48.399275 dsws_client-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       18 2024-04-30 09:09:30.579347 dsws_client-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2940 2024-04-30 09:09:30.579347 dsws_client-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     2567 2024-04-30 09:09:30.579347 dsws_client-1.1.0/tests/test_client.py
+-rw-r--r--   0        0        0     1248 2024-04-30 09:09:30.579347 dsws_client-1.1.0/tests/test_parsing.py
+-rw-r--r--   0        0        0     4935 2024-04-30 09:09:30.579347 dsws_client-1.1.0/tests/test_requests.py
+-rw-r--r--   0        0        0     1784 2024-04-30 09:09:30.579347 dsws_client-1.1.0/tests/test_responses.py
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 dsws_client-1.1.0/PKG-INFO
```

### Comparing `dsws_client-1.0.0/README.md` & `dsws_client-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dsws_client-1.0.0/dsws_client/client.py` & `dsws_client-1.1.0/dsws_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     DSGetDataResponse,
     DSGetTokenResponse,
 )
 from dsws_client.exceptions import (
     InvalidResponseError,
     RequestFailedError,
 )
-from dsws_client.parse import ParsedResponse, responses_to_records
+from dsws_client.parse import ParsedResponse, aggregate_responses, responses_to_records
 from dsws_client.value_objects import DateType, DSStringKVPair, Token
 
 logger = logging.getLogger(__name__)
 
 ResponseCls = TypeVar("ResponseCls")
 
 
@@ -90,14 +90,30 @@
         self,
         identifiers: List[str],
         fields: List[str],
         start: Optional[DateType] = None,
         tag: Optional[str] = None,
     ) -> ParsedResponse:
         """Fetch snapshot data."""
+        data_responses = self.fetch_snapshot_data_iter(
+            identifiers=identifiers,
+            fields=fields,
+            start=start,
+            tag=tag,
+        )
+        return aggregate_responses(data_responses)
+
+    def fetch_snapshot_data_iter(
+        self,
+        identifiers: List[str],
+        fields: List[str],
+        start: Optional[DateType] = None,
+        tag: Optional[str] = None,
+    ) -> Iterator[ParsedResponse]:
+        """Fetch snapshot data, returning an iterator over responses."""
         request_bundles = self.construct_request_bundles(
             identifiers=identifiers,
             fields=fields,
             start=start,
             end=None,
             frequency=None,
             kind=0,
@@ -117,14 +133,34 @@
         fields: List[str],
         start: Optional[DateType] = None,
         end: Optional[DateType] = None,
         frequency: str = "D",
         tag: Optional[str] = None,
     ) -> ParsedResponse:
         """Fetch timeseries data."""
+        data_responses = self.fetch_timeseries_data_iter(
+            identifiers=identifiers,
+            fields=fields,
+            start=start,
+            end=end,
+            frequency=frequency,
+            tag=tag,
+        )
+        return aggregate_responses(data_responses)
+
+    def fetch_timeseries_data_iter(  # noqa: PLR0913
+        self,
+        identifiers: List[str],
+        fields: List[str],
+        start: Optional[DateType] = None,
+        end: Optional[DateType] = None,
+        frequency: str = "D",
+        tag: Optional[str] = None,
+    ) -> Iterator[ParsedResponse]:
+        """Fetch timeseries data, returning an iterator over responses."""
         request_bundles = self.construct_request_bundles(
             identifiers=identifiers,
             fields=fields,
             start=start,
             end=end,
             frequency=frequency,
             kind=1,
```

### Comparing `dsws_client-1.0.0/dsws_client/config.py` & `dsws_client-1.1.0/dsws_client/config.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.0.0/dsws_client/converters.py` & `dsws_client-1.1.0/dsws_client/converters.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.0.0/dsws_client/ds_request.py` & `dsws_client-1.1.0/dsws_client/ds_request.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.0.0/dsws_client/ds_response.py` & `dsws_client-1.1.0/dsws_client/ds_response.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.0.0/dsws_client/parse.py` & `dsws_client-1.1.0/dsws_client/parse.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import collections
 import datetime as dt
 import logging
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Any, Dict, Iterable, Iterator, List, Optional, Tuple, Union
 
 import msgspec
 
 from dsws_client.ds_response import (
     DSDataResponse,
     DSError,
     DSString,
@@ -59,27 +59,33 @@
     meta: Meta = msgspec.field(default_factory=Meta)
 
 
 def responses_to_records(
     responses: Iterable[DSDataResponse],
     *,
     process_strings: bool = True,
-) -> ParsedResponse:
+) -> Iterator[ParsedResponse]:
     """Parse a list of DSDataResponse objects into a list of records."""
-    parsed_response = ParsedResponse()
     for response in responses:
         try:
-            _parsed_response = parse_response(response, process_strings=process_strings)
+            parsed_response = parse_response(response, process_strings=process_strings)
         except InvalidResponseError as exc:
             logger.warning("Invalid response, skipping")
             logger.debug(exc)
             continue
-        parsed_response.records.extend(_parsed_response.records)
-        parsed_response.errors.extend(_parsed_response.errors)
-        parsed_response.meta = parsed_response.meta.merge(_parsed_response.meta)
+        yield parsed_response
+
+
+def aggregate_responses(responses: Iterable[ParsedResponse]) -> ParsedResponse:
+    """Aggregate a list of parsed responses into a single response."""
+    parsed_response = ParsedResponse()
+    for response in responses:
+        parsed_response.records.extend(response.records)
+        parsed_response.errors.extend(response.errors)
+        parsed_response.meta = parsed_response.meta.merge(response.meta)
     return parsed_response
 
 
 def parse_response(
     response: DSDataResponse,
     *,
     process_strings: bool = True,
```

### Comparing `dsws_client-1.0.0/dsws_client/value_objects/enums.py` & `dsws_client-1.1.0/dsws_client/value_objects/enums.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.0.0/dsws_client/value_objects/types.py` & `dsws_client-1.1.0/dsws_client/value_objects/types.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.0.0/pyproject.toml` & `dsws_client-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dsws-client"
-version = "1.0.0"
+version = "1.1.0"
 description = "Python client for the Datastream Web Service API (DSWS)"
 readme = "README.md"
 authors = [
     { name = "ljnsn", email = "info@ljnsn.com" },
 ]
 requires-python = ">=3.8,<4.0"
 dependencies = [
```

### Comparing `dsws_client-1.0.0/tests/conftest.py` & `dsws_client-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.0.0/tests/test_client.py` & `dsws_client-1.1.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.0.0/tests/test_parsing.py` & `dsws_client-1.1.0/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.0.0/tests/test_requests.py` & `dsws_client-1.1.0/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.0.0/tests/test_responses.py` & `dsws_client-1.1.0/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.0.0/PKG-INFO` & `dsws_client-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsws-client
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python client for the Datastream Web Service API (DSWS)
 Author-Email: ljnsn <info@ljnsn.com>
 License: MIT
 Requires-Python: <4.0,>=3.8
 Requires-Dist: attrs>=23.1.0
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: msgspec>=0.18.6
```

