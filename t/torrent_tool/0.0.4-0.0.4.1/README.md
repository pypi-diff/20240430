# Comparing `tmp/torrent_tool-0.0.4.tar.gz` & `tmp/torrent_tool-0.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torrent_tool-0.0.4.tar", max compression
+gzip compressed data, was "torrent_tool-0.0.4.1.tar", max compression
```

## Comparing `torrent_tool-0.0.4.tar` & `torrent_tool-0.0.4.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 torrent_tool-0.0.4/LICENSE
--rw-r--r--   0        0        0     1136 2024-04-21 15:59:37.449290 torrent_tool-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1811 2024-03-26 14:59:41.100942 torrent_tool-0.0.4/readme.md
--rwxr-xr-x   0        0        0     5794 2024-04-21 16:01:38.509603 torrent_tool-0.0.4/torrent_tool/__init__.py
--rwxr-xr-x   0        0        0     1192 2024-04-21 16:03:51.411148 torrent_tool-0.0.4/torrent_tool/__main__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 torrent_tool-0.0.4/torrent_tool/py.typed
--rw-r--r--   0        0        0     2924 1970-01-01 00:00:00.000000 torrent_tool-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 torrent_tool-0.0.4.1/LICENSE
+-rw-r--r--   0        0        0     1138 2024-04-30 16:39:22.363384 torrent_tool-0.0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1811 2024-03-26 14:59:41.100942 torrent_tool-0.0.4.1/readme.md
+-rwxr-xr-x   0        0        0     5794 2024-04-21 16:01:38.509603 torrent_tool-0.0.4.1/torrent_tool/__init__.py
+-rwxr-xr-x   0        0        0     1624 2024-04-30 16:50:28.032600 torrent_tool-0.0.4.1/torrent_tool/__main__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 torrent_tool-0.0.4.1/torrent_tool/py.typed
+-rw-r--r--   0        0        0     2926 1970-01-01 00:00:00.000000 torrent_tool-0.0.4.1/PKG-INFO
```

### Comparing `torrent_tool-0.0.4/LICENSE` & `torrent_tool-0.0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torrent_tool-0.0.4/pyproject.toml` & `torrent_tool-0.0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torrent_tool"
-version = "0.0.4"
+version = "0.0.4.1"
 description = "torrent tool."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/torrent_tool"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/torrent_tool"
 keywords = ["torrent", "magnet"]
```

### Comparing `torrent_tool-0.0.4/readme.md` & `torrent_tool-0.0.4.1/readme.md`

 * *Files identical despite different names*

### Comparing `torrent_tool-0.0.4/torrent_tool/__init__.py` & `torrent_tool-0.0.4.1/torrent_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `torrent_tool-0.0.4/torrent_tool/__main__.py` & `torrent_tool-0.0.4.1/torrent_tool/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,41 +3,54 @@
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
 __doc__ = "torrent to magnet"
 
 from argparse import ArgumentParser
 
 parser = ArgumentParser(description=__doc__)
-parser.add_argument("files", nargs="*", help="paths to torrent files")
-parser.add_argument("-f", "--full", action="store_true", help="append more detailed queries")
+parser.add_argument("paths", nargs="*", metavar="path", help="paths to torrent files, use stdin as default")
+parser.add_argument("-f", "--full", action="store_true", help="more detailed query string")
+parser.add_argument("-v", "--version", action="store_true", help="print the current version")
 args = parser.parse_args()
 if args.version:
     from torrent_tool import __version__
     print(".".join(map(str, __version__)))
     raise SystemExit(0)
-if not args.files:
-    parser.parse_args(["-h"])
 
+from collections import deque
 from os import scandir
 from os.path import isdir
 from sys import stdout
 
 from torrent_tool import torrent_to_magnet
 
-write = stdout.buffer.raw.write # type: ignore
-files = args.files
 full = args.full
+paths = args.paths
+if not paths:
+    from sys import stdin
+    paths = (line.removesuffix("\n") for line in stdin)
+
+dq: deque[str] = deque(paths)
+get = dq.popleft
+write = stdout.buffer.raw.write # type: ignore
+
 try:
-    for file in files:
-        if isdir(file):
-            files.extend(scandir(file))
-        else:
-            try:
-                data = open(file, "rb").read()
-                write(torrent_to_magnet(data, full=full).encode("utf-8"))
-                write(b"\n")
-            except (ValueError, LookupError):
-                pass
+    while dq:
+        path = get()
+        try:
+            if isdir(path):
+                dq.extend(p.path for p in scandir(path))
+            elif path.endswith(".torrent"):
+                try:
+                    data = open(path, "rb").read()
+                    write(torrent_to_magnet(data, full=full).encode("utf-8"))
+                    write(b"\n")
+                except (ValueError, LookupError):
+                    pass
+        except OSError:
+            pass
 except BrokenPipeError:
     from sys import stderr
     stderr.close()
+except KeyboardInterrupt:
+    pass
```

### Comparing `torrent_tool-0.0.4/PKG-INFO` & `torrent_tool-0.0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torrent_tool
-Version: 0.0.4
+Version: 0.0.4.1
 Summary: torrent tool.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/torrent_tool
 License: MIT
 Keywords: torrent,magnet
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

