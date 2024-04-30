# Comparing `tmp/pycocos-0.2.8.tar.gz` & `tmp/pycocos-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycocos-0.2.8.tar", last modified: Fri Apr 19 05:57:54 2024, max compression
+gzip compressed data, was "pycocos-0.2.9.tar", last modified: Fri Apr 19 15:34:19 2024, max compression
```

## Comparing `pycocos-0.2.8.tar` & `pycocos-0.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:57:54.963013 pycocos-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 05:57:51.000000 pycocos-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-04-19 05:57:54.963013 pycocos-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-19 05:57:51.000000 pycocos-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 05:57:54.963013 pycocos-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-19 05:57:51.000000 pycocos-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:57:54.959012 pycocos-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:57:54.963013 pycocos-0.2.8/src/pyCocos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-04-19 05:57:54.000000 pycocos-0.2.8/src/pyCocos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-19 05:57:54.000000 pycocos-0.2.8/src/pyCocos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 05:57:54.000000 pycocos-0.2.8/src/pyCocos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 05:57:54.000000 pycocos-0.2.8/src/pyCocos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 05:57:54.000000 pycocos-0.2.8/src/pyCocos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:57:54.959012 pycocos-0.2.8/src/pycocos/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 05:57:51.000000 pycocos-0.2.8/src/pycocos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:57:54.963013 pycocos-0.2.8/src/pycocos/components/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-19 05:57:51.000000 pycocos-0.2.8/src/pycocos/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15891 2024-04-19 05:57:51.000000 pycocos-0.2.8/src/pycocos/components/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-19 05:57:51.000000 pycocos-0.2.8/src/pycocos/components/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-19 05:57:51.000000 pycocos-0.2.8/src/pycocos/components/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-19 05:57:51.000000 pycocos-0.2.8/src/pycocos/components/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    53080 2024-04-19 05:57:51.000000 pycocos-0.2.8/src/pycocos/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:34:19.622514 pycocos-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 15:34:16.000000 pycocos-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-04-19 15:34:19.622514 pycocos-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-19 15:34:16.000000 pycocos-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 15:34:19.622514 pycocos-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-19 15:34:16.000000 pycocos-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:34:19.618514 pycocos-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:34:19.622514 pycocos-0.2.9/src/pyCocos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-04-19 15:34:19.000000 pycocos-0.2.9/src/pyCocos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-19 15:34:19.000000 pycocos-0.2.9/src/pyCocos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 15:34:19.000000 pycocos-0.2.9/src/pyCocos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 15:34:19.000000 pycocos-0.2.9/src/pyCocos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 15:34:19.000000 pycocos-0.2.9/src/pyCocos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:34:19.622514 pycocos-0.2.9/src/pycocos/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 15:34:16.000000 pycocos-0.2.9/src/pycocos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:34:19.622514 pycocos-0.2.9/src/pycocos/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-19 15:34:16.000000 pycocos-0.2.9/src/pycocos/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15891 2024-04-19 15:34:16.000000 pycocos-0.2.9/src/pycocos/components/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-19 15:34:16.000000 pycocos-0.2.9/src/pycocos/components/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-19 15:34:16.000000 pycocos-0.2.9/src/pycocos/components/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-19 15:34:16.000000 pycocos-0.2.9/src/pycocos/components/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53118 2024-04-19 15:34:16.000000 pycocos-0.2.9/src/pycocos/main.py
```

### Comparing `pycocos-0.2.8/LICENSE` & `pycocos-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pycocos-0.2.8/PKG-INFO` & `pycocos-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCocos
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python connector for Cocos Capital's Rest APIs.
 Home-page: https://github.com/nacho-herrera/pyCocos
 Author: Nacho Herrera
 Author-email: github@nachoherrera.com.ar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pycocos-0.2.8/README.md` & `pycocos-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pycocos-0.2.8/setup.py` & `pycocos-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyCocos",
-    version="0.2.8",
+    version="0.2.9",
     author="Nacho Herrera",
     author_email="github@nachoherrera.com.ar",
     description="Python connector for Cocos Capital's Rest APIs.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nacho-herrera/pyCocos",
     packages=setuptools.find_packages(where='src'),
```

### Comparing `pycocos-0.2.8/src/pyCocos.egg-info/PKG-INFO` & `pycocos-0.2.9/src/pyCocos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCocos
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python connector for Cocos Capital's Rest APIs.
 Home-page: https://github.com/nacho-herrera/pyCocos
 Author: Nacho Herrera
 Author-email: github@nachoherrera.com.ar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pycocos-0.2.8/src/pycocos/components/client.py` & `pycocos-0.2.9/src/pycocos/components/client.py`

 * *Files identical despite different names*

### Comparing `pycocos-0.2.8/src/pycocos/components/enums.py` & `pycocos-0.2.9/src/pycocos/components/enums.py`

 * *Files identical despite different names*

### Comparing `pycocos-0.2.8/src/pycocos/components/urls.py` & `pycocos-0.2.9/src/pycocos/components/urls.py`

 * *Files identical despite different names*

### Comparing `pycocos-0.2.8/src/pycocos/main.py` & `pycocos-0.2.9/src/pycocos/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1171,21 +1171,22 @@
 
         Args:
             long_ticker (str): The long ticker of the instrument.
 
         Returns:
             str: The instrument code, or "" if not found.
         """
+        short_ticker = long_ticker.split("-")[0]
         ticker_search: List[Dict[str, Any]] = self.search_ticker(
-            long_ticker.split("-")[0]
+            short_ticker
         )
         for ticker in ticker_search:
             for subtype in ticker["instrument_subtypes"]:
                 for data in subtype["market_data"]:
-                    if data.get("long_ticker") == long_ticker:
+                    if data.get("short_ticker") == short_ticker:
                         return data["instrument_code"]
         return ""
 
     def _get_instrument_snapshot_value_by_key(self, instrument_code: str, long_ticker:str, segment: Segment, key: str) -> Any:
         """Retrieves the value of a specified key in the instrument snapshot list
 
         Args:
```

