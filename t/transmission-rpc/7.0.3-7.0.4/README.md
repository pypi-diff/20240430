# Comparing `tmp/transmission_rpc-7.0.3.tar.gz` & `tmp/transmission_rpc-7.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transmission_rpc-7.0.3.tar", max compression
+gzip compressed data, was "transmission_rpc-7.0.4.tar", max compression
```

## Comparing `transmission_rpc-7.0.3.tar` & `transmission_rpc-7.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1127 2023-10-16 06:14:38.349616 transmission_rpc-7.0.3/LICENSE
--rw-r--r--   0        0        0     2277 2023-10-16 06:14:38.349616 transmission_rpc-7.0.3/README.md
--rw-r--r--   0        0        0     3109 2023-10-16 06:14:38.349616 transmission_rpc-7.0.3/pyproject.toml
--rw-r--r--   0        0        0     1893 2023-10-16 06:14:38.349616 transmission_rpc-7.0.3/transmission_rpc/__init__.py
--rw-r--r--   0        0        0    43674 2023-10-16 06:14:38.349616 transmission_rpc-7.0.3/transmission_rpc/client.py
--rw-r--r--   0        0        0    10069 2023-10-16 06:14:38.349616 transmission_rpc-7.0.3/transmission_rpc/constants.py
--rw-r--r--   0        0        0     1639 2023-10-16 06:14:38.349616 transmission_rpc-7.0.3/transmission_rpc/error.py
--rw-r--r--   0        0        0        0 2023-10-16 06:14:38.349616 transmission_rpc-7.0.3/transmission_rpc/py.typed
--rw-r--r--   0        0        0    12493 2023-10-16 06:14:38.349616 transmission_rpc-7.0.3/transmission_rpc/session.py
--rw-r--r--   0        0        0    23203 2023-10-16 06:14:38.349616 transmission_rpc-7.0.3/transmission_rpc/torrent.py
--rw-r--r--   0        0        0     1484 2023-10-16 06:14:38.349616 transmission_rpc-7.0.3/transmission_rpc/types.py
--rw-r--r--   0        0        0     2669 2023-10-16 06:14:38.349616 transmission_rpc-7.0.3/transmission_rpc/utils.py
--rw-r--r--   0        0        0     3412 1970-01-01 00:00:00.000000 transmission_rpc-7.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1127 2024-04-30 20:39:54.562527 transmission_rpc-7.0.4/LICENSE
+-rw-r--r--   0        0        0     2277 2024-04-30 20:39:54.562527 transmission_rpc-7.0.4/README.md
+-rw-r--r--   0        0        0     3091 2024-04-30 20:39:54.562527 transmission_rpc-7.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1893 2024-04-30 20:39:54.566527 transmission_rpc-7.0.4/transmission_rpc/__init__.py
+-rw-r--r--   0        0        0    43856 2024-04-30 20:39:54.566527 transmission_rpc-7.0.4/transmission_rpc/client.py
+-rw-r--r--   0        0        0    10069 2024-04-30 20:39:54.566527 transmission_rpc-7.0.4/transmission_rpc/constants.py
+-rw-r--r--   0        0        0     1640 2024-04-30 20:39:54.566527 transmission_rpc-7.0.4/transmission_rpc/error.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:39:54.566527 transmission_rpc-7.0.4/transmission_rpc/py.typed
+-rw-r--r--   0        0        0    12493 2024-04-30 20:39:54.566527 transmission_rpc-7.0.4/transmission_rpc/session.py
+-rw-r--r--   0        0        0    23203 2024-04-30 20:39:54.566527 transmission_rpc-7.0.4/transmission_rpc/torrent.py
+-rw-r--r--   0        0        0     1484 2024-04-30 20:39:54.566527 transmission_rpc-7.0.4/transmission_rpc/types.py
+-rw-r--r--   0        0        0     2669 2024-04-30 20:39:54.566527 transmission_rpc-7.0.4/transmission_rpc/utils.py
+-rw-r--r--   0        0        0     3412 1970-01-01 00:00:00.000000 transmission_rpc-7.0.4/PKG-INFO
```

### Comparing `transmission_rpc-7.0.3/LICENSE` & `transmission_rpc-7.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.3/README.md` & `transmission_rpc-7.0.4/README.md`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.3/pyproject.toml` & `transmission_rpc-7.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "transmission-rpc"
-version = "7.0.3"
+version = "7.0.4"
 description = "Python module that implements the Transmission bittorent client JSON-RPC protocol"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'README.md'
 repository = 'https://github.com/Trim21/transmission-rpc'
 license = 'MIT'
 packages = [{ include = 'transmission_rpc' }]
 keywords = ['transmission', 'rpc']
@@ -30,31 +30,30 @@
 python = "^3.8"
 # dependencies
 requests = "^2.23.0"
 typing-extensions = "*"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = { version = "^7.0.0", python = "^3.9" }
-furo = { version = "2023.9.10", python = "^3.9" }
+furo = { version = "2024.4.27", python = "^3.9" }
 
 [tool.poetry.group.dev.dependencies]
-yarl = "==1.9.2"
+yarl = "==1.9.4"
 # tests
-pytest = "==7.4.2"
+pytest = "==8.2.0"
 pytest-github-actions-annotate-failures = "==0.2.0"
-coverage = "==7.3.1"
+coverage = "==7.5.0"
 
 # linter and formatter
-pre-commit = { version = "==3.4.0", markers = "implementation_name != 'pypy'", python = "^3.9" }
-mypy = { version = "==1.5.1", markers = "implementation_name != 'pypy'", python = "^3.9" }
-ruff = "0.0.291"
+pre-commit = { version = "==3.7.0", markers = "implementation_name != 'pypy'", python = "^3.9" }
+mypy = { version = "==1.10.0", markers = "implementation_name != 'pypy'", python = "^3.9" }
+ruff = "0.4.2"
 
 # stubs
-types-requests = "==2.31.0.7"
-pytz = "==2023.3.post1"
+types-requests = "==2.31.0.20240406"
 
 [tool.poetry-plugin-bump]
 commit_msg = 'bump: v{version}'
 
 [tool.isort]
 default_section = 'THIRDPARTY'
 indent = '    '
```

### Comparing `transmission_rpc-7.0.3/transmission_rpc/__init__.py` & `transmission_rpc-7.0.4/transmission_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.3/transmission_rpc/client.py` & `transmission_rpc-7.0.4/transmission_rpc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,15 @@
                 "paused": paused,
                 "peer-limit": peer_limit,
                 "priority-high": priority_high,
                 "priority-low": priority_low,
                 "priority-normal": priority_normal,
                 "bandwidthPriority": bandwidthPriority,
                 "cookies": cookies,
-                "labels": list_or_none(labels),
+                "labels": list_or_none(_single_str_as_list(labels)),
             }
         )
 
         torrent_data = _try_read_torrent(torrent)
         if torrent_data:
             kwargs["metainfo"] = torrent_data
         else:
@@ -714,15 +714,15 @@
                 "seedIdleLimit": seed_idle_limit,
                 "seedIdleMode": seed_idle_mode,
                 "seedRatioLimit": seed_ratio_limit,
                 "seedRatioMode": seed_ratio_mode,
                 "trackerAdd": tracker_add,
                 "trackerRemove": tracker_remove,
                 "trackerReplace": tracker_replace,
-                "labels": list_or_none(labels),
+                "labels": list_or_none(_single_str_as_list(labels)),
                 "trackerList": None if tracker_list is None else "\n".join("\n\n".join(x) for x in tracker_list),
                 "group": group,
             }
         )
 
         args.update(kwargs)
 
@@ -1106,26 +1106,27 @@
 
         self._request(RpcMethod.GroupSet, arguments, timeout=timeout)
 
     def get_group(self, name: str, *, timeout: Optional[_Timeout] = None) -> Optional[Group]:
         self._rpc_version_warning(17)
         result: Dict[str, Any] = self._request(RpcMethod.GroupGet, {"group": name}, timeout=timeout)
 
-        if result["arguments"]["group"]:
-            return Group(fields=result["arguments"]["group"][0])
+        if result["group"]:
+            return Group(fields=result["group"][0])
+
         return None
 
     def get_groups(self, name: Optional[List[str]] = None, *, timeout: Optional[_Timeout] = None) -> Dict[str, Group]:
         payload = {}
         if name is not None:
             payload = {"group": name}
 
         result: Dict[str, Any] = self._request(RpcMethod.GroupGet, payload, timeout=timeout)
 
-        return {x["name"]: Group(fields=x) for x in result["arguments"]["group"]}
+        return {x["name"]: Group(fields=x) for x in result["group"]}
 
     def __enter__(self) -> "Client":
         return self
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
@@ -1134,14 +1135,22 @@
     ) -> None:
         self._http_session.close()
 
 
 T = TypeVar("T")
 
 
+def _single_str_as_list(v: Optional[Iterable[str]]) -> Optional[List[str]]:
+    if v is None:
+        return v
+    if isinstance(v, str):
+        return [v]
+    return list(v)
+
+
 def list_or_none(v: Optional[Iterable[T]]) -> Optional[List[T]]:
     if v is None:
         return None
     return list(v)
 
 
 def remove_unset_value(data: Dict[str, Any]) -> Dict[str, Any]:
```

### Comparing `transmission_rpc-7.0.3/transmission_rpc/constants.py` & `transmission_rpc-7.0.4/transmission_rpc/constants.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.3/transmission_rpc/error.py` & `transmission_rpc-7.0.4/transmission_rpc/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 exception raise by this package
 """
+
 from typing import Any, Optional
 
 from requests.models import Response
 
 
 class TransmissionError(Exception):
     """
```

### Comparing `transmission_rpc-7.0.3/transmission_rpc/session.py` & `transmission_rpc-7.0.4/transmission_rpc/session.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.3/transmission_rpc/torrent.py` & `transmission_rpc-7.0.4/transmission_rpc/torrent.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.3/transmission_rpc/types.py` & `transmission_rpc-7.0.4/transmission_rpc/types.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.3/transmission_rpc/utils.py` & `transmission_rpc-7.0.4/transmission_rpc/utils.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.3/PKG-INFO` & `transmission_rpc-7.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transmission-rpc
-Version: 7.0.3
+Version: 7.0.4
 Summary: Python module that implements the Transmission bittorent client JSON-RPC protocol
 Home-page: https://github.com/Trim21/transmission-rpc
 License: MIT
 Keywords: transmission,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.8,<4.0
@@ -12,16 +12,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: requests (>=2.23.0,<3.0.0)
 Requires-Dist: typing-extensions
 Project-URL: Repository, https://github.com/Trim21/transmission-rpc
 Description-Content-Type: text/markdown
```

