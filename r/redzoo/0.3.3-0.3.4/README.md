# Comparing `tmp/redzoo-0.3.3.tar.gz` & `tmp/redzoo-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redzoo-0.3.3.tar", last modified: Tue Apr 30 05:34:54 2024, max compression
+gzip compressed data, was "redzoo-0.3.4.tar", last modified: Tue Apr 30 06:29:54 2024, max compression
```

## Comparing `redzoo-0.3.3.tar` & `redzoo-0.3.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:34:54.315768 redzoo-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 05:34:48.000000 redzoo-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-30 05:34:54.315768 redzoo-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 05:34:48.000000 redzoo-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-30 05:34:48.000000 redzoo-0.3.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:34:54.311768 redzoo-0.3.3/redzoo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 05:34:48.000000 redzoo-0.3.3/redzoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:34:54.315768 redzoo-0.3.3/redzoo/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 05:34:48.000000 redzoo-0.3.3/redzoo/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-04-30 05:34:48.000000 redzoo-0.3.3/redzoo/database/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:34:54.315768 redzoo-0.3.3/redzoo/math/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 05:34:48.000000 redzoo-0.3.3/redzoo/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-30 05:34:48.000000 redzoo-0.3.3/redzoo/math/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:34:54.315768 redzoo-0.3.3/redzoo/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 05:34:48.000000 redzoo-0.3.3/redzoo/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-04-30 05:34:48.000000 redzoo-0.3.3/redzoo/metrics/consumption.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:34:54.315768 redzoo-0.3.3/redzoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-30 05:34:54.000000 redzoo-0.3.3/redzoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 05:34:54.000000 redzoo-0.3.3/redzoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 05:34:54.000000 redzoo-0.3.3/redzoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 05:34:54.000000 redzoo-0.3.3/redzoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 05:34:54.000000 redzoo-0.3.3/redzoo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 05:34:54.315768 redzoo-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 05:34:54.315768 redzoo-0.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-30 05:34:48.000000 redzoo-0.3.3/test/test_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-30 05:34:48.000000 redzoo-0.3.3/test/test_simpledb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:54.566892 redzoo-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 06:29:46.000000 redzoo-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-30 06:29:54.566892 redzoo-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 06:29:46.000000 redzoo-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-30 06:29:46.000000 redzoo-0.3.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:54.562892 redzoo-0.3.4/redzoo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:46.000000 redzoo-0.3.4/redzoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:54.566892 redzoo-0.3.4/redzoo/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:46.000000 redzoo-0.3.4/redzoo/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-30 06:29:46.000000 redzoo-0.3.4/redzoo/database/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:54.566892 redzoo-0.3.4/redzoo/math/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:46.000000 redzoo-0.3.4/redzoo/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-30 06:29:46.000000 redzoo-0.3.4/redzoo/math/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:54.566892 redzoo-0.3.4/redzoo/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:46.000000 redzoo-0.3.4/redzoo/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-04-30 06:29:46.000000 redzoo-0.3.4/redzoo/metrics/consumption.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:54.566892 redzoo-0.3.4/redzoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-30 06:29:54.000000 redzoo-0.3.4/redzoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 06:29:54.000000 redzoo-0.3.4/redzoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:29:54.000000 redzoo-0.3.4/redzoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 06:29:54.000000 redzoo-0.3.4/redzoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 06:29:54.000000 redzoo-0.3.4/redzoo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 06:29:54.566892 redzoo-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:54.566892 redzoo-0.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-30 06:29:46.000000 redzoo-0.3.4/test/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-30 06:29:46.000000 redzoo-0.3.4/test/test_simpledb.py
```

### Comparing `redzoo-0.3.3/LICENSE` & `redzoo-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `redzoo-0.3.3/redzoo/database/simple.py` & `redzoo-0.3.4/redzoo/database/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import gzip
 import shutil
 import logging
 from random import randint
 from datetime import datetime, timedelta
 from appdirs import site_data_dir
 from typing import Any, Dict, List
+from redzoo.math.display import size
 
 
 
 class Entry:
 
     def __init__(self, value: Any, expire_date: datetime):
         self.expire_date = expire_date
@@ -41,17 +42,15 @@
         self.__name = name
         if directory is None:
             self.__directory = site_data_dir("simpledb", appauthor=False)
         else:
             self.__directory = directory
         self.__data = self.__load()
         self.__last_time_stored = datetime.now() - timedelta(days=2)
-
-        file_size_kb = int(os.stat(self.filename).st_size / 1024)
-        logging.info("simple db: using " + self.filename + " (" + str(len(self.__data)) + " entries; " + str(file_size_kb) + " KB)")
+        logging.info("simple db: using " + self.filename + " (" + str(len(self.__data)) + " entries; " + size(os.stat(self.filename).st_size) )
 
     @property
     def filename(self):
         if not os.path.exists(self.__directory):
             logging.info("directory " + self.__directory + " does not exits. Creating it")
             os.makedirs(self.__directory)
         return os.path.join(self.__directory, self.__name + ".json.gz")
@@ -96,15 +95,15 @@
         entry = self.__data.get(key, None)
         if entry is None or entry.is_expired():
             return default_value
         else:
             return self.__copy(entry.value)
 
     def get_values(self) -> List:
-        logging.warning("SimpleDB#get_values is deprecated. Use SimpleDB#get_values instead")
+        logging.warning("SimpleDB#get_values is deprecated. Use SimpleDB#values instead")
         return self.values()
 
     def values(self) -> List:
         values = []
         for key in list(self.__data.keys()):
             entry = self.__data[key]
             if not entry.is_expired():
```

### Comparing `redzoo-0.3.3/redzoo/metrics/consumption.py` & `redzoo-0.3.4/redzoo/metrics/consumption.py`

 * *Files identical despite different names*

### Comparing `redzoo-0.3.3/test/test_simpledb.py` & `redzoo-0.3.4/test/test_simpledb.py`

 * *Files identical despite different names*

