# Comparing `tmp/zibai_server-0.9.5.tar.gz` & `tmp/zibai_server-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zibai_server-0.9.5.tar", last modified: Fri Feb 23 08:12:01 2024, max compression
+gzip compressed data, was "zibai_server-0.9.6.tar", last modified: Wed Mar  6 03:07:05 2024, max compression
```

## Comparing `zibai_server-0.9.5.tar` & `zibai_server-0.9.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11340 2024-02-23 08:11:50.018384 zibai_server-0.9.5/LICENCE
--rw-r--r--   0        0        0     7687 2024-02-23 08:11:50.018384 zibai_server-0.9.5/README.md
--rw-r--r--   0        0        0     1191 2024-02-23 08:12:01.978402 zibai_server-0.9.5/pyproject.toml
--rw-r--r--   0        0        0      374 2024-02-23 08:11:50.018384 zibai_server-0.9.5/src/zibai/__init__.py
--rw-r--r--   0        0        0       78 2024-02-23 08:11:50.018384 zibai_server-0.9.5/src/zibai/__main__.py
--rw-r--r--   0        0        0    12283 2024-02-23 08:11:50.018384 zibai_server-0.9.5/src/zibai/cli.py
--rw-r--r--   0        0        0       42 2024-02-23 08:11:50.018384 zibai_server-0.9.5/src/zibai/const.py
--rw-r--r--   0        0        0     3492 2024-02-23 08:11:50.018384 zibai_server-0.9.5/src/zibai/core.py
--rw-r--r--   0        0        0     9512 2024-02-23 08:11:50.018384 zibai_server-0.9.5/src/zibai/h11.py
--rw-r--r--   0        0        0      848 2024-02-23 08:11:50.018384 zibai_server-0.9.5/src/zibai/logger.py
--rw-r--r--   0        0        0        0 2024-02-23 08:11:50.018384 zibai_server-0.9.5/src/zibai/middlewares/__init__.py
--rw-r--r--   0        0        0      548 2024-02-23 08:11:50.018384 zibai_server-0.9.5/src/zibai/middlewares/limit_request_count.py
--rw-r--r--   0        0        0     9097 2024-02-23 08:11:50.018384 zibai_server-0.9.5/src/zibai/multiprocess.py
--rw-r--r--   0        0        0     1610 2024-02-23 08:11:50.018384 zibai_server-0.9.5/src/zibai/reloader.py
--rw-r--r--   0        0        0     2410 2024-02-23 08:11:50.018384 zibai_server-0.9.5/src/zibai/utils.py
--rw-r--r--   0        0        0     7901 2024-02-23 08:11:50.018384 zibai_server-0.9.5/src/zibai/wsgi_typing.py
--rw-r--r--   0        0        0        0 2024-02-23 08:11:50.018384 zibai_server-0.9.5/tests/__init__.py
--rw-r--r--   0        0        0      574 2024-02-23 08:11:50.018384 zibai_server-0.9.5/tests/conftest.py
--rw-r--r--   0        0        0     1771 2024-02-23 08:11:50.018384 zibai_server-0.9.5/tests/test_core.py
--rw-r--r--   0        0        0        0 2024-02-23 08:11:50.022384 zibai_server-0.9.5/tests/test_multiprocess.py
--rw-r--r--   0        0        0      650 2024-02-23 08:11:50.022384 zibai_server-0.9.5/tests/utils.py
--rw-r--r--   0        0        0     8164 1970-01-01 00:00:00.000000 zibai_server-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0    11340 2024-03-06 03:06:51.543546 zibai_server-0.9.6/LICENCE
+-rw-r--r--   0        0        0     7687 2024-03-06 03:06:51.543546 zibai_server-0.9.6/README.md
+-rw-r--r--   0        0        0     1191 2024-03-06 03:07:05.115564 zibai_server-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0      374 2024-03-06 03:06:51.543546 zibai_server-0.9.6/src/zibai/__init__.py
+-rw-r--r--   0        0        0       78 2024-03-06 03:06:51.543546 zibai_server-0.9.6/src/zibai/__main__.py
+-rw-r--r--   0        0        0    12283 2024-03-06 03:06:51.543546 zibai_server-0.9.6/src/zibai/cli.py
+-rw-r--r--   0        0        0       42 2024-03-06 03:06:51.543546 zibai_server-0.9.6/src/zibai/const.py
+-rw-r--r--   0        0        0     3492 2024-03-06 03:06:51.543546 zibai_server-0.9.6/src/zibai/core.py
+-rw-r--r--   0        0        0     9512 2024-03-06 03:06:51.543546 zibai_server-0.9.6/src/zibai/h11.py
+-rw-r--r--   0        0        0      848 2024-03-06 03:06:51.543546 zibai_server-0.9.6/src/zibai/logger.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:06:51.543546 zibai_server-0.9.6/src/zibai/middlewares/__init__.py
+-rw-r--r--   0        0        0      548 2024-03-06 03:06:51.543546 zibai_server-0.9.6/src/zibai/middlewares/limit_request_count.py
+-rw-r--r--   0        0        0     9084 2024-03-06 03:06:51.543546 zibai_server-0.9.6/src/zibai/multiprocess.py
+-rw-r--r--   0        0        0     1610 2024-03-06 03:06:51.543546 zibai_server-0.9.6/src/zibai/reloader.py
+-rw-r--r--   0        0        0     2410 2024-03-06 03:06:51.543546 zibai_server-0.9.6/src/zibai/utils.py
+-rw-r--r--   0        0        0     7901 2024-03-06 03:06:51.543546 zibai_server-0.9.6/src/zibai/wsgi_typing.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:06:51.543546 zibai_server-0.9.6/tests/__init__.py
+-rw-r--r--   0        0        0      574 2024-03-06 03:06:51.543546 zibai_server-0.9.6/tests/conftest.py
+-rw-r--r--   0        0        0     1771 2024-03-06 03:06:51.543546 zibai_server-0.9.6/tests/test_core.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:06:51.543546 zibai_server-0.9.6/tests/test_multiprocess.py
+-rw-r--r--   0        0        0      650 2024-03-06 03:06:51.543546 zibai_server-0.9.6/tests/utils.py
+-rw-r--r--   0        0        0     8164 1970-01-01 00:00:00.000000 zibai_server-0.9.6/PKG-INFO
```

### Comparing `zibai_server-0.9.5/LICENCE` & `zibai_server-0.9.6/LICENCE`

 * *Files identical despite different names*

### Comparing `zibai_server-0.9.5/README.md` & `zibai_server-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `zibai_server-0.9.5/pyproject.toml` & `zibai_server-0.9.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "zibai-server"
-version = "0.9.5"
+version = "0.9.6"
 description = "A modern high-performance Python WSGI server."
 authors = [
     { name = "abersheeran", email = "me@abersheeran.com" },
 ]
 dependencies = [
     "h11>=0.14.0",
 ]
```

### Comparing `zibai_server-0.9.5/src/zibai/cli.py` & `zibai_server-0.9.6/src/zibai/cli.py`

 * *Files identical despite different names*

### Comparing `zibai_server-0.9.5/src/zibai/core.py` & `zibai_server-0.9.6/src/zibai/core.py`

 * *Files identical despite different names*

### Comparing `zibai_server-0.9.5/src/zibai/h11.py` & `zibai_server-0.9.6/src/zibai/h11.py`

 * *Files identical despite different names*

### Comparing `zibai_server-0.9.5/src/zibai/logger.py` & `zibai_server-0.9.6/src/zibai/logger.py`

 * *Files identical despite different names*

### Comparing `zibai_server-0.9.5/src/zibai/middlewares/limit_request_count.py` & `zibai_server-0.9.6/src/zibai/middlewares/limit_request_count.py`

 * *Files identical despite different names*

### Comparing `zibai_server-0.9.5/src/zibai/multiprocess.py` & `zibai_server-0.9.6/src/zibai/multiprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self.kwargs = kwargs
 
 
 class Process:
     def __init__(self, parameters: ProcessParameters) -> None:
         self.parameters = parameters
         self.parent_conn, self.child_conn = Pipe()
-        self.process = SpawnProcess(target=self.target, daemon=True)
+        self.process = SpawnProcess(target=self.target)
 
     def ping(self, timeout: float = 5) -> bool:
         try:
             self.parent_conn.send(b"ping")
             if self.parent_conn.poll(timeout):
                 self.parent_conn.recv()
                 return True
```

### Comparing `zibai_server-0.9.5/src/zibai/reloader.py` & `zibai_server-0.9.6/src/zibai/reloader.py`

 * *Files identical despite different names*

### Comparing `zibai_server-0.9.5/src/zibai/utils.py` & `zibai_server-0.9.6/src/zibai/utils.py`

 * *Files identical despite different names*

### Comparing `zibai_server-0.9.5/src/zibai/wsgi_typing.py` & `zibai_server-0.9.6/src/zibai/wsgi_typing.py`

 * *Files identical despite different names*

### Comparing `zibai_server-0.9.5/tests/conftest.py` & `zibai_server-0.9.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zibai_server-0.9.5/tests/test_core.py` & `zibai_server-0.9.6/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `zibai_server-0.9.5/tests/utils.py` & `zibai_server-0.9.6/tests/utils.py`

 * *Files identical despite different names*

### Comparing `zibai_server-0.9.5/PKG-INFO` & `zibai_server-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibai-server
-Version: 0.9.5
+Version: 0.9.6
 Summary: A modern high-performance Python WSGI server.
 Author-Email: abersheeran <me@abersheeran.com>
 License: Apache-2.0
 Project-URL: Repository, https://github.com/abersheeran/zibai
 Requires-Python: >=3.10
 Requires-Dist: h11>=0.14.0
 Requires-Dist: gevent>=23.9.1; extra == "gevent"
```

