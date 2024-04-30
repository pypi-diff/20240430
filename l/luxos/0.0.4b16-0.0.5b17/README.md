# Comparing `tmp/luxos-0.0.4b16.tar.gz` & `tmp/luxos-0.0.5b17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luxos-0.0.4b16.tar", last modified: Wed Apr 24 18:18:20 2024, max compression
+gzip compressed data, was "luxos-0.0.5b17.tar", last modified: Tue Apr 30 18:43:38 2024, max compression
```

## Comparing `luxos-0.0.4b16.tar` & `luxos-0.0.5b17.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:18:20.534219 luxos-0.0.4b16/
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-24 18:18:20.534219 luxos-0.0.4b16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-24 18:17:50.000000 luxos-0.0.4b16/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-24 18:18:18.000000 luxos-0.0.4b16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 18:18:20.538219 luxos-0.0.4b16/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:18:20.530219 luxos-0.0.4b16/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:18:20.534219 luxos-0.0.4b16/src/luxos/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-24 18:18:18.000000 luxos-0.0.4b16/src/luxos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 18:17:50.000000 luxos-0.0.4b16/src/luxos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-24 18:17:50.000000 luxos-0.0.4b16/src/luxos/api.json
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-24 18:17:50.000000 luxos-0.0.4b16/src/luxos/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10212 2024-04-24 18:17:50.000000 luxos-0.0.4b16/src/luxos/asyncops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:18:20.534219 luxos-0.0.4b16/src/luxos/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:17:50.000000 luxos-0.0.4b16/src/luxos/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-24 18:17:50.000000 luxos-0.0.4b16/src/luxos/cli/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-24 18:17:50.000000 luxos-0.0.4b16/src/luxos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-24 18:17:50.000000 luxos-0.0.4b16/src/luxos/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:17:50.000000 luxos-0.0.4b16/src/luxos/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:18:20.534219 luxos-0.0.4b16/src/luxos/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:17:50.000000 luxos-0.0.4b16/src/luxos/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-24 18:17:50.000000 luxos-0.0.4b16/src/luxos/scripts/async_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-04-24 18:17:50.000000 luxos-0.0.4b16/src/luxos/scripts/health_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-24 18:17:50.000000 luxos-0.0.4b16/src/luxos/scripts/luxos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:18:20.534219 luxos-0.0.4b16/src/luxos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-24 18:18:20.000000 luxos-0.0.4b16/src/luxos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-24 18:18:20.000000 luxos-0.0.4b16/src/luxos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:18:20.000000 luxos-0.0.4b16/src/luxos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-24 18:18:20.000000 luxos-0.0.4b16/src/luxos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-24 18:18:20.000000 luxos-0.0.4b16/src/luxos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 18:18:20.000000 luxos-0.0.4b16/src/luxos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:18:20.534219 luxos-0.0.4b16/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-24 18:17:50.000000 luxos-0.0.4b16/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-24 18:17:50.000000 luxos-0.0.4b16/tests/test_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-04-24 18:17:50.000000 luxos-0.0.4b16/tests/test_luxos_asyncops.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-24 18:17:50.000000 luxos-0.0.4b16/tests/test_luxos_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:43:38.070597 luxos-0.0.5b17/
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-30 18:43:38.066597 luxos-0.0.5b17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-30 18:43:07.000000 luxos-0.0.5b17/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-30 18:43:35.000000 luxos-0.0.5b17/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 18:43:38.070597 luxos-0.0.5b17/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:43:38.062597 luxos-0.0.5b17/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:43:38.066597 luxos-0.0.5b17/src/luxos/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-30 18:43:35.000000 luxos-0.0.5b17/src/luxos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 18:43:07.000000 luxos-0.0.5b17/src/luxos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-30 18:43:07.000000 luxos-0.0.5b17/src/luxos/api.json
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-30 18:43:07.000000 luxos-0.0.5b17/src/luxos/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-04-30 18:43:07.000000 luxos-0.0.5b17/src/luxos/asyncops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:43:38.066597 luxos-0.0.5b17/src/luxos/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:43:07.000000 luxos-0.0.5b17/src/luxos/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-30 18:43:07.000000 luxos-0.0.5b17/src/luxos/cli/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-30 18:43:07.000000 luxos-0.0.5b17/src/luxos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-30 18:43:07.000000 luxos-0.0.5b17/src/luxos/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:43:07.000000 luxos-0.0.5b17/src/luxos/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:43:38.066597 luxos-0.0.5b17/src/luxos/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:43:07.000000 luxos-0.0.5b17/src/luxos/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-30 18:43:07.000000 luxos-0.0.5b17/src/luxos/scripts/async_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-04-30 18:43:07.000000 luxos-0.0.5b17/src/luxos/scripts/health_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-30 18:43:07.000000 luxos-0.0.5b17/src/luxos/scripts/luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-30 18:43:07.000000 luxos-0.0.5b17/src/luxos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:43:38.066597 luxos-0.0.5b17/src/luxos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-30 18:43:38.000000 luxos-0.0.5b17/src/luxos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-30 18:43:38.000000 luxos-0.0.5b17/src/luxos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:43:38.000000 luxos-0.0.5b17/src/luxos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-30 18:43:38.000000 luxos-0.0.5b17/src/luxos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-30 18:43:38.000000 luxos-0.0.5b17/src/luxos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 18:43:38.000000 luxos-0.0.5b17/src/luxos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:43:38.066597 luxos-0.0.5b17/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-30 18:43:07.000000 luxos-0.0.5b17/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-30 18:43:07.000000 luxos-0.0.5b17/tests/test_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-04-30 18:43:07.000000 luxos-0.0.5b17/tests/test_luxos_asyncops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-30 18:43:07.000000 luxos-0.0.5b17/tests/test_luxos_misc.py
```

### Comparing `luxos-0.0.4b16/PKG-INFO` & `luxos-0.0.5b17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.4b16
+Version: 0.0.5b17
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.4b16/README.md` & `luxos-0.0.5b17/README.md`

 * *Files identical despite different names*

### Comparing `luxos-0.0.4b16/pyproject.toml` & `luxos-0.0.5b17/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "luxos"
-version = "0.0.4b16"
+version = "0.0.5b17"
 description = "The all encompassing LuxOS python library."
 readme = "README.md"
 license = { text = "MIT" }  # TODO I don't think this is a MIT??
 requires-python = ">= 3.9"
 
 authors = [
   { name = "Antonio Cavallo", email = "antonio.cavallo@luxor.tech" },
```

### Comparing `luxos-0.0.4b16/src/luxos/api.json` & `luxos-0.0.5b17/src/luxos/api.json`

 * *Files identical despite different names*

### Comparing `luxos-0.0.4b16/src/luxos/api.py` & `luxos-0.0.5b17/src/luxos/api.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.4b16/src/luxos/asyncops.py` & `luxos-0.0.5b17/src/luxos/asyncops.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,33 +272,33 @@
             try:
                 if cmd == "logon":
                     return {"sid": await logon(host, port, timeout)}
                 else:
                     return await logoff(host, port, parameters[0])
             except Exception as exc:
                 failure = exc
-            if retry_delay:
+            if retry and (i < retry) and retry_delay:
                 await asyncio.sleep(retry_delay)
         if isinstance(failure, Exception):
             raise failure
 
     failure = None
     sid = ""
-    for i in range(retry or 1):
+    for i in range(retry + 1):
         if not api.logon_required(cmd):
             log.debug("no logon required for command '%s' on %s:%i", cmd, host, port)
             break
         try:
             sid = await logon(host, port, timeout)
             parameters = [sid, *parameters]
             log.info("session id requested & obtained for %s:%i (%s)", host, port, sid)
             break
         except Exception as exc:
             failure = exc
-        if retry_delay:
+        if retry and (i < retry) and retry_delay:
             await asyncio.sleep(retry_delay)
 
     if isinstance(failure, Exception):
         raise failure
 
     packet = {"command": cmd}
     if parameters:
@@ -308,23 +308,24 @@
         cmd,
         host,
         port,
         packet.get("parameter", ""),
     )
 
     failure = None
-    for i in range(retry or 1):
+    for i in range(retry + 1):
         try:
             ret = await roundtrip(host, port, packet, timeout=timeout)
             log.debug("received from %s:%s: %s", host, port, str(ret))
             if sid:
                 await logoff(host, port, sid)
             return ret
         except Exception as exc:
             failure = exc
-        if retry_delay:
+        if retry and (i < retry) and retry_delay:
+            log.debug("failed attempt %i (out of %i)", i + 1, retry)
             await asyncio.sleep(retry_delay)
 
     if sid:
         await logoff(host, port, sid)
     if isinstance(failure, Exception):
         raise failure
```

### Comparing `luxos-0.0.4b16/src/luxos/cli/v1.py` & `luxos-0.0.5b17/src/luxos/cli/v1.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.4b16/src/luxos/exceptions.py` & `luxos-0.0.5b17/src/luxos/exceptions.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.4b16/src/luxos/misc.py` & `luxos-0.0.5b17/src/luxos/misc.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.4b16/src/luxos/scripts/async_luxos.py` & `luxos-0.0.5b17/src/luxos/scripts/async_luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.4b16/src/luxos/scripts/health_checker.py` & `luxos-0.0.5b17/src/luxos/scripts/health_checker.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.4b16/src/luxos/scripts/luxos.py` & `luxos-0.0.5b17/src/luxos/scripts/luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.4b16/src/luxos.egg-info/PKG-INFO` & `luxos-0.0.5b17/src/luxos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.4b16
+Version: 0.0.5b17
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.4b16/src/luxos.egg-info/SOURCES.txt` & `luxos-0.0.5b17/src/luxos.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 src/luxos/__main__.py
 src/luxos/api.json
 src/luxos/api.py
 src/luxos/asyncops.py
 src/luxos/exceptions.py
 src/luxos/misc.py
 src/luxos/py.typed
+src/luxos/utils.py
 src/luxos.egg-info/PKG-INFO
 src/luxos.egg-info/SOURCES.txt
 src/luxos.egg-info/dependency_links.txt
 src/luxos.egg-info/entry_points.txt
 src/luxos.egg-info/requires.txt
 src/luxos.egg-info/top_level.txt
 src/luxos/cli/__init__.py
```

### Comparing `luxos-0.0.4b16/tests/test_cli.py` & `luxos-0.0.5b17/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.4b16/tests/test_luxos_asyncops.py` & `luxos-0.0.5b17/tests/test_luxos_asyncops.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.4b16/tests/test_luxos_misc.py` & `luxos-0.0.5b17/tests/test_luxos_misc.py`

 * *Files identical despite different names*

