# Comparing `tmp/proxylib-0.1.1.tar.gz` & `tmp/proxylib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxylib-0.1.1.tar", last modified: Fri May 20 10:39:09 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `proxylib-0.1.1.tar` & `proxylib-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-05-20 10:39:09.375172 proxylib-0.1.1/
--rw-rw-rw-   0        0        0      477 2022-05-20 10:39:09.375172 proxylib-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2022-05-20 10:39:09.375172 proxylib-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2242 2022-04-18 03:36:37.000000 proxylib-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-20 10:39:09.343930 proxylib-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2022-05-20 10:39:09.359627 proxylib-0.1.1/src/proxylib/
--rw-rw-rw-   0        0        0       74 2022-05-12 22:27:52.000000 proxylib-0.1.1/src/proxylib/__init__.py
--rw-rw-rw-   0        0        0     2885 2022-04-23 06:24:39.000000 proxylib-0.1.1/src/proxylib/_jscontext.py
--rw-rw-rw-   0        0        0     2155 2022-05-12 22:27:52.000000 proxylib-0.1.1/src/proxylib/_models.py
--rw-rw-rw-   0        0        0      420 2022-04-23 03:50:40.000000 proxylib-0.1.1/src/proxylib/_re.py
-drwxrwxrwx   0        0        0        0 2022-05-20 10:39:09.371596 proxylib-0.1.1/src/proxylib/discovery/
--rw-rw-rw-   0        0        0      524 2022-05-12 22:27:52.000000 proxylib-0.1.1/src/proxylib/discovery/__init__.py
--rw-rw-rw-   0        0        0     1834 2022-05-12 22:27:52.000000 proxylib-0.1.1/src/proxylib/discovery/common.py
--rw-rw-rw-   0        0        0      954 2022-05-12 22:27:52.000000 proxylib-0.1.1/src/proxylib/discovery/windows.py
--rw-rw-rw-   0        0        0     4491 2022-05-20 10:38:56.000000 proxylib-0.1.1/src/proxylib/pac.py
--rw-rw-rw-   0        0        0     1244 2022-05-12 22:27:52.000000 proxylib-0.1.1/src/proxylib/utils.py
-drwxrwxrwx   0        0        0        0 2022-05-20 10:39:09.369230 proxylib-0.1.1/src/proxylib.egg-info/
--rw-rw-rw-   0        0        0      477 2022-05-20 10:39:09.000000 proxylib-0.1.1/src/proxylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2022-05-20 10:39:09.000000 proxylib-0.1.1/src/proxylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-20 10:39:09.000000 proxylib-0.1.1/src/proxylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-05-20 10:39:09.000000 proxylib-0.1.1/src/proxylib.egg-info/top_level.txt
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/example.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/proxylib/__init__.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/proxylib/env.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/proxylib/netutils.py
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/proxylib/proxy.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/proxylib/utils.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/proxylib/os/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/proxylib/os/nt.py
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/proxylib/pac/__init__.py
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 proxylib-0.5.0/src/proxylib/pac/javascript.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 proxylib-0.5.0/tests/test_pac.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 proxylib-0.5.0/tests/test_proxy.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 proxylib-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 proxylib-0.5.0/LICENSE
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 proxylib-0.5.0/README.md
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 proxylib-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 proxylib-0.5.0/PKG-INFO
```

### Comparing `proxylib-0.1.1/src/proxylib/_jscontext.py` & `proxylib-0.5.0/src/proxylib/pac/javascript.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from abc import ABCMeta
 from typing import OrderedDict, Sequence
+
 from dukpy import JSInterpreter
 
+__all__ = ["JSContext"]
+
+
 class JSContextMeta(ABCMeta):
     def __new__(
         metaclass: "type[JSContext]",
         cls_name: str,
         base_classes: Sequence[object],
         cls_builder: OrderedDict[str, object],
     ):
@@ -16,15 +20,17 @@
                 jsContext.setdefault(key, val)
 
         for cls in reversed(base_classes):
             exclude.extend(getattr(cls, "_JSCONTEXT_EXCLUDE", []))
             if hasattr(cls, "_JSCONTEXT"):
                 update: dict = cls._JSCONTEXT
             else:
-                update = {key: getattr(cls, key) for key in dir(cls) if key[0].isalpha()}
+                update = {
+                    key: getattr(cls, key) for key in dir(cls) if key[0].isalpha()
+                }
             for key, val in update.items():
                 jsContext.setdefault(key, staticmethod(val))
 
         return type.__new__(
             metaclass,
             cls_name,
             base_classes,
@@ -40,16 +46,16 @@
                     if (key[0].isalpha() and key[0] not in exclude)
                 },
             },
         )
 
 
 class JSContext(metaclass=JSContextMeta):
-    def __init__(self, js:str) -> None:
-        context:dict = object.__getattribute__(self, "_JSCONTEXT")
+    def __init__(self, js: str) -> None:
+        context: dict = object.__getattribute__(self, "_JSCONTEXT")
         engine = JSInterpreter()
         for key, val in context.items():
             if isinstance(val, staticmethod):
                 val = val.__func__
             elif isinstance(val, classmethod):
                 val = val.__get__(self.__class__)
             elif isinstance(val, property):
@@ -61,15 +67,17 @@
             _js = f"function {key}(){{ return call_python.apply(null, ['{key}'].concat(Array.prototype.slice.call(arguments))); }}"
             engine.evaljs(_js)
         engine.evaljs(js)
 
         object.__setattr__(self, "_jsengine", engine)
 
     def __getattribute__(self, name: str):
-        engine:JSInterpreter = object.__getattribute__(self, "_jsengine")
-        context:dict = object.__getattribute__(self, "_JSCONTEXT")
+        engine: JSInterpreter = object.__getattribute__(self, "_jsengine")
+        context: dict = object.__getattribute__(self, "_JSCONTEXT")
         if name in context:
+
             def jsFunction(*args):
-                return engine.evaljs(f"{name}.apply(null, dukpy.args)", args = list(args))
+                return engine.evaljs(f"{name}.apply(null, dukpy.args)", args=list(args))
+
             return jsFunction
         else:
             return object.__getattribute__(self, name)
```

### Comparing `proxylib-0.1.1/src/proxylib/discovery/common.py` & `proxylib-0.5.0/src/proxylib/env.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import os
-from typing import Iterable as _Iter
 import re
-from .._models import Proxy, ProxyMap, URL
-from ..pac import load_pac, PAC
-from ..utils import SingleProxyMap, get_proxymap_for, get_addresses
+from typing import Iterable as _Iter
+
+from .netutils import get_ip, get_local_interfaces
+from .proxy import URL, Proxy, ProxyMap
+from .utils import get_proxymap_for
+
+__all__ = ("EnvProxyConfig",)
 
 
 class EnvProxyConfig(ProxyMap):
     __slots__ = ("http_proxy", "https_proxy", "no_proxy")
 
     def __init__(
         self,
@@ -25,18 +28,19 @@
             if no_proxy
             else []
         )
 
     def __getitem__(self, url: str) -> _Iter[Proxy]:
         uri = URL.from_str(url)
         url = f"{uri.scheme}://{uri.netloc}"
+        ip = get_ip(uri.host)
         for _no in self.no_proxy:
             if _no is None:
-                for addr in get_addresses():
-                    if PAC.isInNet(url, addr["addr"], addr["netmask"]):
+                for _if in get_local_interfaces():
+                    if ip in _if.network:
                         return [None]
             else:
                 if _no.match(url):
                     return [None]
         return self.https_proxy[url] if uri.scheme == "https" else self.http_proxy[url]
 
     @staticmethod
```

### Comparing `proxylib-0.1.1/src/proxylib/discovery/windows.py` & `proxylib-0.5.0/src/proxylib/os/nt.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 import winreg as _reg
-from .common import  EnvProxyConfig
-from ..utils import SingleProxyMap
-def _queryvalue(key:_reg.HKEYType, subkey:str)->str:
+
+from ..env import EnvProxyConfig
+from ..utils import SimpleProxyMap
+
+
+def _queryvalue(key: _reg.HKEYType, subkey: str) -> str:
     try:
         value, type = _reg.QueryValueEx(key, subkey)
         return value
     except:
         return None
 
-_WINREG_INTERNET_SETTINGS = r"SOFTWARE\Microsoft\Windows\CurrentVersion\Internet Settings"
+
+_WINREG_INTERNET_SETTINGS = (
+    r"SOFTWARE\Microsoft\Windows\CurrentVersion\Internet Settings"
+)
+
 
 def system_proxy():
     settings = _reg.OpenKey(_reg.HKEY_CURRENT_USER, _WINREG_INTERNET_SETTINGS)
     pac = _queryvalue(settings, "AutoConfigURL")
     if pac:
         return pac
     if _queryvalue(settings, "ProxyEnable"):
         env_proxy = _queryvalue(settings, "ProxyServer")
         overrides = _queryvalue(settings, "ProxyOverride")
         if env_proxy:
-            return EnvProxyConfig(env_proxy, env_proxy, overrides.split(";") if overrides else [] )
-    
+            return EnvProxyConfig(
+                env_proxy, env_proxy, overrides.split(";") if overrides else []
+            )
+
     if _queryvalue(settings, "EnableNegotiate"):
-        #TODO
+        # TODO
         pass
-    return SingleProxyMap()
-
+    return SimpleProxyMap()
```

### Comparing `proxylib-0.1.1/src/proxylib/pac.py` & `proxylib-0.5.0/src/proxylib/pac/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-from typing import (
-    Iterable as _Iter,
-    Literal as _Literal,
-    get_args as _args,
-    cast as _cast,
-    overload as _overload,
-)
-import socket as _socket
+import datetime as _datetime
 import ipaddress as _ip
+import socket as _socket
 from fnmatch import fnmatch as _shexpmatch
-import datetime as _datetime
+from typing import Iterable as _Iter
+from typing import Literal as _Literal
+from typing import cast as _cast
+from typing import get_args as _args
+from typing import overload as _overload
 from urllib.request import urlopen as _urlopen
 from warnings import warn as _warn
-from ._models import ProxyMap, Proxy
-from ._re import _PAC_REGEX, _URI_REGEX
 
+from ..proxy import Proxy, ProxyMap, UriSplit
 
 _WEEKDAY = _Literal["SUN", "MON", "TUE", "WED", "THU", "FRI", "SAT"]
 _WEEKDAYS = ("SUN", "MON", "TUE", "WED", "THU", "FRI", "SAT")
 
+__all__ = ("PAC", "load")
+
 
-class PAC(ProxyMap):
+class PAC(object):
 
     #### UTILITY FUNCTIONS ####
     @staticmethod
     def dnsResolve(host: str, /):
         try:
             return _socket.gethostbyname(host)
         except:
@@ -43,22 +42,20 @@
 
     @staticmethod
     def shExpMatch(test: str, shexp: str, /):
         return _shexpmatch(test, shexp)
 
     #### TIME FUNCTIONS ####
     @_overload
-    def weekdayRange(wd1: _WEEKDAY, gmt: 'None|_Literal["GMT"]' = None, /):
-        ...
+    def weekdayRange(wd1: _WEEKDAY, gmt: 'None|_Literal["GMT"]' = None, /): ...
 
     @_overload
     def weekdayRange(
         wd1: _WEEKDAY, wd2: _WEEKDAY, gmt: 'None|_Literal["GMT"]' = None, /
-    ):
-        ...
+    ): ...
 
     @staticmethod
     def weekdayRange(wd1: _WEEKDAY, /, *args: '_WEEKDAY|_Literal["GMT"]'):
         start = _WEEKDAYS.index(wd1.upper())
         if args:
             wd2 = args[0].upper()
             if len(args) == 2:
@@ -123,41 +120,41 @@
         return ip in net
 
     @staticmethod
     def FindProxyForURL(url: str, host: str, /) -> str:
         return "DIRECT"
 
     def __getitem__(self, url: str) -> _Iter[Proxy]:
-        parsed = _URI_REGEX.match(url)
+        parsed = UriSplit.Default.match(url)
         if not parsed:
             raise ValueError(url)
         scheme, user, p, host, port = parsed.groups()
         pac_proxies = self.FindProxyForURL(
             f"{scheme}://{host}{f':{port}' if port else ''}", host
         )
-        return (Proxy(*proxy) for proxy in _PAC_REGEX.findall(pac_proxies))
+        return Proxy.find_all(pac_proxies, UriSplit.PAC)
 
 
 try:
-    from ._jscontext import JSContext as _JSContext
+    from .javascript import JSContext
 
-    class JSProxyAutoConfig(PAC, _JSContext):
-        ...
+    class JSProxyAutoConfig(PAC, JSContext): ...
 
     _jspac = True
 except ImportError:
 
     _jspac = False
+    JSProxyAutoConfig = None
 
 
-def load_pac(url: str, **urllib_kwds):
+def load(url: str, **urllib_kwds):
     if "://" not in url:
         url = ("file://" if url.startswith("/") else "https://") + url
     with _urlopen(url, **urllib_kwds) as resp:
         js = _cast(bytes, resp.read()).decode()
     if "FindProxyForURL" not in js:
         raise Exception("Not FindProxyForURL found int response from: " + url)
     if not _jspac:
-        _warn(f"Can not load js from: {url} as pac. Install libproxy[jspac]")
+        _warn(f"Can not load js from: {url} as pac. Install proxylib[pac]")
         return PAC()
     else:
         return JSProxyAutoConfig(js)
```

