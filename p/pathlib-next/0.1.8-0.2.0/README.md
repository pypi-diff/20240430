# Comparing `tmp/pathlib_next-0.1.8.tar.gz` & `tmp/pathlib_next-0.2.0.tar.gz`

## Comparing `pathlib_next-0.1.8.tar` & `pathlib_next-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/src/example.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/src/pathlib_next/__init__.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/src/pathlib_next/fspath.py
--rw-r--r--   0        0        0     5174 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/src/pathlib_next/mempath.py
--rw-r--r--   0        0        0    18030 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/src/pathlib_next/path.py
--rw-r--r--   0        0        0    15459 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/src/pathlib_next/uri/__init__.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/src/pathlib_next/uri/query.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/src/pathlib_next/uri/source.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/src/pathlib_next/uri/schemes/__init__.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/src/pathlib_next/uri/schemes/file.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/src/pathlib_next/uri/schemes/http.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/src/pathlib_next/uri/schemes/sftp.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/src/pathlib_next/utils/__init__.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/src/pathlib_next/utils/glob.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/src/pathlib_next/utils/stat.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/src/pathlib_next/utils/sync.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/tests/test_local.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/tests/test_uri.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/LICENSE
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/README.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pathlib_next-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/src/example.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/src/pathlib_next/__init__.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/src/pathlib_next/fspath.py
+-rw-r--r--   0        0        0     5174 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/src/pathlib_next/mempath.py
+-rw-r--r--   0        0        0    18038 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/src/pathlib_next/path.py
+-rw-r--r--   0        0        0    15590 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/src/pathlib_next/uri/__init__.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/src/pathlib_next/uri/query.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/src/pathlib_next/uri/source.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/src/pathlib_next/uri/schemes/__init__.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/src/pathlib_next/uri/schemes/file.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/src/pathlib_next/uri/schemes/http.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/src/pathlib_next/uri/schemes/sftp.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/src/pathlib_next/utils/__init__.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/src/pathlib_next/utils/glob.py
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/src/pathlib_next/utils/stat.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/src/pathlib_next/utils/sync.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/tests/test_local.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/tests/test_uri.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/LICENSE
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/README.md
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 pathlib_next-0.2.0/PKG-INFO
```

### Comparing `pathlib_next-0.1.8/src/example.py` & `pathlib_next-0.2.0/src/example.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+import os
+
 from pathlib_next import Path, glob
 from pathlib_next.mempath import MemPath
-from pathlib_next.uri import Query, Source, UriPath
-from pathlib_next.uri.schemes import *
+from pathlib_next.uri import Query, Source, Uri, UriPath
 from pathlib_next.utils.sync import PathSyncer
 
+rootless = Uri("sftp://root@sftpexample")
+rootless.source
+authkeys = rootless / "root/.ssh/authorized_keys"
+keys = authkeys.as_uri()
+
+local = Path("./_ssh")
+
 mempath = MemPath("test/test3") / "subpath"
 mempath.parent.mkdir(parents=True, exist_ok=True)
 mempath.write_text("test")
 check = mempath.read_text()
 mempath.parent.rm(recursive=True)
 
-pass
-
-local = Path("./_ssh")
+test = list(os.scandir(local))
 print(list(local.iterdir()))
 query = Query({"test": "://$#!1", "test2&": [1, 2]})
 q2 = Query(str(query)).to_dict()
 for name, value in query:
     print(f"{name}: {value}")
 src = Source(scheme="scheme", userinfo="user", host="123.com", port=0)
 test = {**src}
```

### Comparing `pathlib_next-0.1.8/src/pathlib_next/fspath.py` & `pathlib_next-0.2.0/src/pathlib_next/fspath.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import pathlib as _path
-import os as _os
 import functools as _func
+import os as _os
+import pathlib as _path
+import re as _re
 import typing as _ty
+
 from . import path as _proto
-import re as _re
 
 
 @_func.cache
 def _is_case_sensitive(flavour: _os.path) -> bool:
     return flavour.normcase("Aa") == "Aa"
 
 
@@ -28,15 +29,15 @@
     @property
     def _is_case_sensitive(self) -> bool:
         return _is_case_sensitive(self._parser)
 
     @property
     def segments(self):
         return self.parts
-    
+
     def with_segments(self, *args: str | _proto.FsPathLike):
         return type(self)(*args)
 
 
 class PosixPathname(_path.PurePosixPath, _BaseFSPathname):
     __slots__ = ()
 
@@ -75,8 +76,8 @@
         yield from _proto.Path.glob(
             self,
             pattern,
             case_sensitive=case_sensitive,
             include_hidden=include_hidden,
             recursive=recursive,
             dironly=dironly,
-        )
+        )
```

### Comparing `pathlib_next-0.1.8/src/pathlib_next/mempath.py` & `pathlib_next-0.2.0/src/pathlib_next/mempath.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.8/src/pathlib_next/path.py` & `pathlib_next-0.2.0/src/pathlib_next/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         cls = type(self)
         other = other if isinstance(other, cls) else cls(self, other)
         return other == self or other in self.parents
 
     def __truediv__(self, key: _ty.Self | str) -> _ty.Self:
         try:
             return type(self)(self, key)
-        except (TypeError, NotImplementedError):
+        except (TypeError, NotImplementedError) as _err:
             return NotImplemented
 
     @property
     @_abc.abstractmethod
     def parent(self) -> _ty.Self:
         """The logical parent of the path."""
```

### Comparing `pathlib_next-0.1.8/src/pathlib_next/uri/__init__.py` & `pathlib_next-0.2.0/src/pathlib_next/uri/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,21 @@
                 elif _path:
                     _path = f"{path}/{_path}"
                 else:
                     _path = path
                 if _path.startswith("/"):
                     break
 
+        if (
+            (source.host or source.userinfo or source.port)
+            and _path
+            and not _path.startswith("/")
+        ):
+            _path = "/" + _path
+
         self._init(source, _path, query, fragment)
 
     def _init(self, source: Source, path: str, query: str, fragment: str, **kwargs):
         if self._initiated:
             pass
             # raise Exception(f"Uri._init should only be called once")
         self._initiated = True
@@ -197,15 +204,18 @@
                 return f"//{self.source.host}/{self.path.removeprefix('/')}"
             else:
                 raise NotImplementedError(f"OS Support for not local fspath")
 
         raise NotImplementedError(f"fspath for {self.source.scheme}")
 
     def __repr__(self):
-        return "{}({!r})".format(type(self).__name__, str(self))
+        if self._initiated:
+            return "{}({!r})".format(type(self).__name__, str(self))
+        else:
+            return super().__repr__()
 
     def as_uri(self, /, sanitize=False):
         if self._uri is None or sanitize:
             uri = self._format_parsed_parts(
                 self.source, self.path, self.query, self.fragment, sanitize=sanitize
             )
             if not sanitize:
@@ -394,14 +404,21 @@
             if cls is UriPath:
                 inst = Uri.__new__(cls, *args, **kwargs)
             else:
                 inst = cls.__new__(cls, *args, **kwargs)
             inst._init(uri.source, uri.path, uri.query, uri.fragment, **kwargs)
         else:
             inst = Uri.__new__(cls, *args, **kwargs)
+            backend = kwargs.get("backend", None)
+            if backend is None:
+                for segment in reversed(args):
+                    if isinstance(segment, cls):
+                        backend = segment.backend
+                        break
+            inst._backend = backend
         return inst
 
     def _initbackend(self):
         return None
 
     def _from_parsed_parts(
         self, source: Source, path: str, query: str, fragment: str, /, **kwargs
@@ -429,38 +446,26 @@
         if self._backend is None:
             self._backend = self._initbackend()
         return self._backend
 
     def with_backend(self, backend):
         return self._from_parsed_parts(*self.parts, backend=backend)
 
-    def _load_parts(self):
-        super()._load_parts()
-        if self.source and self.source.scheme and self._backend is None:
-            for uri in reversed(self._raw_uris):
-                if (
-                    isinstance(uri, UriPath)
-                    and uri.source.scheme == self.source.scheme
-                    and uri._backend
-                ):
-                    self._backend = uri._backend
-                    break
-
     def __truediv__(self, key: str | Uri | os.PathLike):
         try:
             return type(self)(self, key, findclass=True)
         except (TypeError, NotImplementedError):
             return NotImplemented
 
     def with_source(self, source: Source):
         cls = type(self)
         if not source:
             inst = Uri.__new__(UriPath)
         elif source.scheme not in cls._schemes():
-            inst = UriPath.__new__(UriPath, source.scheme + ":")
+            inst = cls.__new__(cls, source.scheme + ":", findclass=True)
         else:
             inst = cls.__new__(cls, backend=self._backend)
         inst._init(source, self.path, self.query, self.fragment)
         return inst
 
     @_utils.notimplemented
     def _listdir(self) -> "_ty.Iterator[str]": ...
```

### Comparing `pathlib_next-0.1.8/src/pathlib_next/uri/query.py` & `pathlib_next-0.2.0/src/pathlib_next/uri/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import typing as _ty
+
 import uritools as _uritools
 
 
 class Query(str):
     __slots__ = ("_encoding", "_separator")
     SEPARATOR = "&"
     ENCODING = "utf-8"
@@ -12,15 +13,15 @@
         query: (
             str
             | _ty.Sequence[tuple[str, str | None]]
             | _ty.Mapping[str, str | None | _ty.Sequence[str | None]]
         ),
         *,
         encoding=ENCODING,
-        separator=SEPARATOR
+        separator=SEPARATOR,
     ):
         if isinstance(query, Query):
             _encoding = query._encoding
             _separator = query._separator
         else:
             _encoding = None
             _separator = None
@@ -40,15 +41,15 @@
         obj._separator = separator
         return obj
 
     def decode(query) -> list[tuple[str, str | None]]:
         return _uritools.SplitResultString("", "", "", str(query), "").getquerylist(
             query._separator, query._encoding
         )
-    
+
     def __iter__(self):
         return iter(self.decode())
 
     def to_dict(query, *, single=False):
         query_: dict[str, list[str | None]] = {}
         for k, v in query.decode():
             if single:
```

### Comparing `pathlib_next-0.1.8/src/pathlib_next/uri/source.py` & `pathlib_next-0.2.0/src/pathlib_next/uri/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import ipaddress as _ip
+import socket as _socket
 import typing as _ty
+
 import uritools as _uritools
-import socket as _socket
-import ipaddress as _ip
 
 from .. import utils as _utils
 
 _IPAddress = _ip.IPv4Address | _ip.IPv6Address
 
 if _ty.TYPE_CHECKING:
     from . import UriPath
@@ -15,15 +16,15 @@
     scheme: str | None
     userinfo: str | None
     host: str | _IPAddress | None
     port: int | None
 
     def __bool__(self):
         for val in self:
-            if val == '' or val is None:
+            if val == "" or val is None:
                 continue
             return True
         return False
 
     def __str__(self) -> str:
         return _uritools.uricompose(
             scheme=self.scheme, userinfo=self.userinfo, host=self.host, port=self.port
```

### Comparing `pathlib_next-0.1.8/src/pathlib_next/uri/schemes/file.py` & `pathlib_next-0.2.0/src/pathlib_next/uri/schemes/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import os as _os
+
 from ...fspath import LocalPath as _Local
 from ...path import FsPathLike
-import os as _os
-from .. import UriPath, Source
+from .. import Source, UriPath
 
 
 class FileUri(UriPath):
     __SCHEMES = ("file",)
     __slots__ = ("_filepath",)
 
     @property
```

### Comparing `pathlib_next-0.1.8/src/pathlib_next/uri/schemes/http.py` & `pathlib_next-0.2.0/src/pathlib_next/uri/schemes/http.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from ...utils.stat import FileStat
-from .. import UriPath
-from ... import utils as _utils
 import io as _io
-import requests as _req
-import typing as _ty
-import bs4 as _bs4
 import time as _time
+import typing as _ty
 
+import bs4 as _bs4
+import requests as _req
 from htmllistparse import parse as _htmlparse
 
+from ... import utils as _utils
+from ...utils.stat import FileStat
+from .. import UriPath
+
 
 class _FileEntry(_ty.NamedTuple):
     name: str
     modified: _ty.Optional[_time.struct_time]
     size: _ty.Optional[int]
     description: _ty.Optional[str]
 
@@ -38,15 +39,15 @@
     if _ty.TYPE_CHECKING:
         backend: HttpBackend
 
     def _initbackend(self):
         return HttpBackend(_req.Session(), {})
 
     def _listdir(self) -> list[_FileEntry]:
-        req = self.backend.session.request("GET", self)
+        req = self.backend.request("GET", self)
         req.raise_for_status()
         soup = _bs4.BeautifulSoup(req.content, "html5lib")
         _, listing = _htmlparse(soup)
         return listing
 
     def iterdir(self):
         _self = self.path.removesuffix("/")
@@ -60,15 +61,15 @@
         return (
             resp.is_redirect
             or resp.url.endswith("/")
             or resp.url.endswith("/..")
             or resp.url.endswith("/.")
         )
 
-    def stat(self):
+    def stat(self, *, follow_symlinks=True, walk_up_last_modified=False):
         check = (
             [self.with_path(self.path.removesuffix("/")), self]
             if self.path.endswith("/")
             else [self]
         )
         for uri in check:
             resp = self.backend.request("HEAD", uri, allow_redirects=False)
@@ -86,15 +87,15 @@
         elif resp.status_code == 403:
             raise PermissionError(self)
         else:
             resp.raise_for_status()
 
         st_size = 0 if self._isdir else int(resp.headers.get("Content-Length", 0))
         lm = resp.headers.get("Last-Modified")
-        if lm is None:
+        if lm is None and walk_up_last_modified:
             parent = self.parent
             if self != parent:
                 try:
                     entry = next(
                         filter(
                             lambda p: p.name.removesuffix("/") == self.name,
                             parent._listdir(),
```

### Comparing `pathlib_next-0.1.8/src/pathlib_next/uri/schemes/sftp.py` & `pathlib_next-0.2.0/src/pathlib_next/uri/schemes/sftp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-import typing as _ty
-from .. import UriPath, Source
-from ... import utils as _utils
 import threading as _thread
+import typing as _ty
+
 import paramiko as _paramiko
 
+from ... import utils as _utils
+from .. import Source, UriPath
+
 
 class BaseSftpBackend(object):
     __slots__ = ()
 
     @_utils.notimplemented
     def client(self, source: Source) -> _paramiko.SFTPClient: ...
 
@@ -73,16 +75,19 @@
             client = _CACHED_CLIENTS.invalidate(self.backend, self.source, thead_id)
         return client
 
     def _listdir(self):
         for path in self._sftpclient.listdir(self.path):
             yield path
 
-    def stat(self):
-        return self._sftpclient.stat(self.path)
+    def stat(self, *, follow_symlinks=True):
+        if follow_symlinks:
+            return self._sftpclient.stat(self.path)
+        else:
+            return self._sftpclient.lstat(self.path)
 
     def _open(self, mode="r", buffering=-1):
         return self._sftpclient.open(self.path, mode, buffering)
 
     def _mkdir(self, mode):
         return self._sftpclient.mkdir(self.path, mode)
```

### Comparing `pathlib_next-0.1.8/src/pathlib_next/utils/__init__.py` & `pathlib_next-0.2.0/src/pathlib_next/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
+import collections
 import functools as _functools
-from threading import RLock
-import typing as _ty
 import time as _time
+import typing as _ty
 from email.utils import parsedate as _parsedate
-
-
-import collections
+from threading import RLock
 
 K = _ty.ParamSpec("K")
 V = _ty.TypeVar("V")
 
 
 class LRU(_ty.Generic[K, V]):
 
@@ -18,15 +16,15 @@
         self.func = func
         self._maxsize = maxsize
         self.lock = RLock()
 
     @property
     def maxsize(self):
         return self._maxsize
-    
+
     @maxsize.setter
     def maxsize(self, maxsize: int):
         cache = self.cache
         with self.lock:
             self._maxsize = maxsize
             while len(cache) > maxsize:
                 cache.pop(last=False)
@@ -74,19 +72,21 @@
 def notimplemented(method):
     @_functools.wraps(method)
     def _notimplemented(*args, **kwargs):
         raise NotImplementedError(f"Not implement method  {method.__name__}")
 
     return _notimplemented
 
-import socket as _socket
+
 import ipaddress as _ip
+import socket as _socket
+
 
 def get_machine_ips():
-    ips:list[_ip.IPv4Address|_ip.IPv6Address] = list()
+    ips: list[_ip.IPv4Address | _ip.IPv6Address] = list()
     for item in _socket.getaddrinfo(_socket.gethostname(), None):
         protocol, *_, (ip, *_) = item
         if protocol == _socket.AddressFamily.AF_INET:
             ips.append(_ip.ip_address(ip))
         elif protocol == _socket.AddressFamily.AF_INET6:
             ips.append(_ip.ip_address(ip))
```

### Comparing `pathlib_next-0.1.8/src/pathlib_next/utils/glob.py` & `pathlib_next-0.2.0/src/pathlib_next/utils/glob.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.8/tests/test_local.py` & `pathlib_next-0.2.0/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.8/tests/test_uri.py` & `pathlib_next-0.2.0/tests/test_uri.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,75 +1,99 @@
+import pathlib
+
 import pytest
+
 import src.pathlib_next as pathlib_next
 from src.pathlib_next.uri import Uri
 
-import pathlib
+test_uris = ["http://user:pass@google.com:80"]
+
+
+# @pytest.mark.parametrize("_uri", test_uris)
+def parse_uri(_uri: str):
+    uri = pathlib_next.Uri(_uri)
+    assert uri.as_uri() == _uri
+    return uri
 
 
 def test_source():
-    uri = pathlib_next.Uri("http://user:pass@google.com:80")
+    uri = parse_uri(test_uris[0])
     assert uri.source.scheme == "http"
     assert uri.source.host == "google.com"
     assert uri.source.port == 80
-    assert uri.source.parsed_userinfo() == ('user','pass')
+    assert uri.source.parsed_userinfo() == ("user", "pass")
 
 
 def test_no_scheme():
-    uri = pathlib_next.Uri("//user:pass@google.com:80/")
+    uri = parse_uri("//user:pass@google.com:80/")
     assert uri.source.scheme == None
     assert uri.source.host == "google.com"
     assert uri.source.port == 80
-    assert uri.source.parsed_userinfo() == ('user','pass')
+    assert uri.source.parsed_userinfo() == ("user", "pass")
+
 
 def test_no_scheme_with_host_no_pass():
-    uri = pathlib_next.Uri("//user@google.com:80/")
+    uri = parse_uri("//user@google.com:80/")
     assert uri.source.scheme == None
     assert uri.source.host == "google.com"
     assert uri.source.port == 80
-    assert uri.source.parsed_userinfo() == ('user', '')
+    assert uri.source.parsed_userinfo() == ("user", "")
+
 
 def test_no_scheme_no_host():
-    uri = pathlib_next.Uri("//user@:80/")
+    uri = parse_uri("//user@:80/")
     assert uri.source.scheme == None
     assert uri.source.host == ""
     assert uri.source.port == 80
-    assert uri.source.parsed_userinfo() == ('user', '')
+    assert uri.source.parsed_userinfo() == ("user", "")
+
 
 def test_no_scheme_no_netloc():
-    uri = pathlib_next.Uri("//user@")
+    uri = parse_uri("//user@")
     assert uri.source.scheme == None
     assert uri.source.host == ""
     assert uri.source.port == None
-    assert uri.source.parsed_userinfo() == ('user', '')
+    assert uri.source.parsed_userinfo() == ("user", "")
+
 
 def test_path():
-    uri = pathlib_next.Uri("http://google.com/root/subroot/filename.ext")
+    uri = parse_uri("http://google.com/root/subroot/filename.ext")
     assert uri.source.scheme == "http"
     assert uri.source.host == "google.com"
     assert uri.source.port == None
-    assert uri.source.parsed_userinfo() == ('','')
-    assert uri.path == '/root/subroot/filename.ext'
+    assert uri.source.parsed_userinfo() == ("", "")
+    assert uri.path == "/root/subroot/filename.ext"
+
 
 def test_encoded_path():
-    uri = pathlib_next.Uri("http://goog%2Fe.com/root/subroot/%3Fquery/%23fragment/%2Fencoded%2Ffilename.ext")
+    uri = pathlib_next.Uri(
+        "http://goog%2Fe.com/root/subroot/%3Fquery/%23fragment/%2Fencoded%2Ffilename.ext"
+    )
     assert uri.source.scheme == "http"
     assert uri.source.host == "goog/e.com"
     assert uri.source.port == None
-    assert uri.source.parsed_userinfo() == ('','')
-    assert uri.path == '/root/subroot/?query/#fragment//encoded/filename.ext'
+    assert uri.source.parsed_userinfo() == ("", "")
+    assert uri.path == "/root/subroot/?query/#fragment//encoded/filename.ext"
 
 
 def test_child():
-    sftp_root = Uri('sftp://root@sftpexample/')
-    authkeys = sftp_root / 'root/.ssh/authorized_keys'
+    sftp_root = Uri("sftp://root@sftpexample/")
+    authkeys = sftp_root / "root/.ssh/authorized_keys"
     uri = authkeys.as_uri()
-    assert uri == 'sftp://root@sftpexample/root/.ssh/authorized_keys'
+    assert uri == "sftp://root@sftpexample/root/.ssh/authorized_keys"
+
 
 def test_truediv_pathlib():
-    sftp_root = Uri('sftp://root@sftpexample/')
-    authkeys = sftp_root / pathlib.PurePosixPath('root/.ssh/authorized_keys')
+    sftp_root = Uri("sftp://root@sftpexample/")
+    authkeys = sftp_root / pathlib.PurePosixPath("root/.ssh/authorized_keys")
     uri = authkeys.as_uri()
-    assert uri == 'sftp://root@sftpexample/root/.ssh/authorized_keys'
-    authkeys = sftp_root / pathlib.Path('root/.ssh/authorized_keys')
+    assert uri == "sftp://root@sftpexample/root/.ssh/authorized_keys"
+
+    authkeys = sftp_root / pathlib.Path("root/.ssh/authorized_keys")
+    uri = authkeys.as_uri()
+    assert uri == "file:/root/.ssh/authorized_keys"
+
+
+def test_join_without_root():
+    authkeys = Uri("sftp://root@sftpexample") / "root/.ssh/authorized_keys"
     uri = authkeys.as_uri()
-    assert uri == 'file:/root/.ssh/authorized_keys'
-    
+    assert uri == "sftp://root@sftpexample/root/.ssh/authorized_keys"
```

### Comparing `pathlib_next-0.1.8/LICENSE` & `pathlib_next-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.8/pyproject.toml` & `pathlib_next-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pathlib_next"
-version = "0.1.8"
+version = "0.2.0"
 authors = [{ name = "Jose A" }]
 description = "Generic Path Protocol based pathlib"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = []
 [project.optional-dependencies]
 uri = ["uritools"]
-http = ["requests", "pathlib_next[uri]"]
+http = ["requests", "pathlib_next[uri]", 'htmllistparse', 'bs4']
 sftp = ["paramiko", "pathlib_next[uri]"]
+dev = ['build', 'twine', 'hatchling']
 
 
 [project.urls]
 Homepage = "https://github.com/jose-pr/pathlib_next/"
 Issues = "https://github.com/jose-pr/pathlib_next/issues"
 
 [tool.hatch.build.targets.sdist]
```

### Comparing `pathlib_next-0.1.8/PKG-INFO` & `pathlib_next-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.3
 Name: pathlib_next
-Version: 0.1.8
+Version: 0.2.0
 Summary: Generic Path Protocol based pathlib
 Project-URL: Homepage, https://github.com/jose-pr/pathlib_next/
 Project-URL: Issues, https://github.com/jose-pr/pathlib_next/issues
 Author: Jose A
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
+Provides-Extra: dev
+Requires-Dist: build; extra == 'dev'
+Requires-Dist: hatchling; extra == 'dev'
+Requires-Dist: twine; extra == 'dev'
 Provides-Extra: http
+Requires-Dist: bs4; extra == 'http'
+Requires-Dist: htmllistparse; extra == 'http'
 Requires-Dist: requests; extra == 'http'
 Requires-Dist: uritools; extra == 'http'
 Provides-Extra: sftp
 Requires-Dist: paramiko; extra == 'sftp'
 Requires-Dist: uritools; extra == 'sftp'
 Provides-Extra: uri
 Requires-Dist: uritools; extra == 'uri'
```

