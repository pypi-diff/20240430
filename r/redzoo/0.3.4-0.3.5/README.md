# Comparing `tmp/redzoo-0.3.4.tar.gz` & `tmp/redzoo-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redzoo-0.3.4.tar", last modified: Tue Apr 30 06:29:54 2024, max compression
+gzip compressed data, was "redzoo-0.3.5.tar", last modified: Tue Apr 30 06:35:51 2024, max compression
```

## Comparing `redzoo-0.3.4.tar` & `redzoo-0.3.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:54.566892 redzoo-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 06:29:46.000000 redzoo-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-30 06:29:54.566892 redzoo-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 06:29:46.000000 redzoo-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-30 06:29:46.000000 redzoo-0.3.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:54.562892 redzoo-0.3.4/redzoo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:46.000000 redzoo-0.3.4/redzoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:54.566892 redzoo-0.3.4/redzoo/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:46.000000 redzoo-0.3.4/redzoo/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-30 06:29:46.000000 redzoo-0.3.4/redzoo/database/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:54.566892 redzoo-0.3.4/redzoo/math/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:46.000000 redzoo-0.3.4/redzoo/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-30 06:29:46.000000 redzoo-0.3.4/redzoo/math/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:54.566892 redzoo-0.3.4/redzoo/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:46.000000 redzoo-0.3.4/redzoo/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-04-30 06:29:46.000000 redzoo-0.3.4/redzoo/metrics/consumption.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:54.566892 redzoo-0.3.4/redzoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-30 06:29:54.000000 redzoo-0.3.4/redzoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 06:29:54.000000 redzoo-0.3.4/redzoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:29:54.000000 redzoo-0.3.4/redzoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 06:29:54.000000 redzoo-0.3.4/redzoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 06:29:54.000000 redzoo-0.3.4/redzoo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 06:29:54.566892 redzoo-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:29:54.566892 redzoo-0.3.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-30 06:29:46.000000 redzoo-0.3.4/test/test_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-30 06:29:46.000000 redzoo-0.3.4/test/test_simpledb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:35:51.422457 redzoo-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 06:35:45.000000 redzoo-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-30 06:35:51.422457 redzoo-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 06:35:45.000000 redzoo-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-30 06:35:45.000000 redzoo-0.3.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:35:51.418457 redzoo-0.3.5/redzoo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:35:45.000000 redzoo-0.3.5/redzoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:35:51.418457 redzoo-0.3.5/redzoo/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:35:45.000000 redzoo-0.3.5/redzoo/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-30 06:35:45.000000 redzoo-0.3.5/redzoo/database/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:35:51.418457 redzoo-0.3.5/redzoo/math/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:35:45.000000 redzoo-0.3.5/redzoo/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-30 06:35:45.000000 redzoo-0.3.5/redzoo/math/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:35:51.418457 redzoo-0.3.5/redzoo/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:35:45.000000 redzoo-0.3.5/redzoo/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-04-30 06:35:45.000000 redzoo-0.3.5/redzoo/metrics/consumption.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:35:51.422457 redzoo-0.3.5/redzoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-30 06:35:51.000000 redzoo-0.3.5/redzoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 06:35:51.000000 redzoo-0.3.5/redzoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:35:51.000000 redzoo-0.3.5/redzoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 06:35:51.000000 redzoo-0.3.5/redzoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 06:35:51.000000 redzoo-0.3.5/redzoo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 06:35:51.422457 redzoo-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:35:51.422457 redzoo-0.3.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-30 06:35:45.000000 redzoo-0.3.5/test/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-30 06:35:45.000000 redzoo-0.3.5/test/test_simpledb.py
```

### Comparing `redzoo-0.3.4/LICENSE` & `redzoo-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `redzoo-0.3.4/redzoo/database/simple.py` & `redzoo-0.3.5/redzoo/database/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         self.__name = name
         if directory is None:
             self.__directory = site_data_dir("simpledb", appauthor=False)
         else:
             self.__directory = directory
         self.__data = self.__load()
         self.__last_time_stored = datetime.now() - timedelta(days=2)
-        logging.info("simple db: using " + self.filename + " (" + str(len(self.__data)) + " entries; " + size(os.stat(self.filename).st_size) )
+        logging.info("simple db: using " + self.filename + " (" + str(len(self.__data)) + " entries; " + size(os.stat(self.filename).st_size) + ")")
 
     @property
     def filename(self):
         if not os.path.exists(self.__directory):
             logging.info("directory " + self.__directory + " does not exits. Creating it")
             os.makedirs(self.__directory)
         return os.path.join(self.__directory, self.__name + ".json.gz")
```

### Comparing `redzoo-0.3.4/redzoo/math/display.py` & `redzoo-0.3.5/redzoo/math/display.py`

 * *Files identical despite different names*

### Comparing `redzoo-0.3.4/redzoo/metrics/consumption.py` & `redzoo-0.3.5/redzoo/metrics/consumption.py`

 * *Files identical despite different names*

### Comparing `redzoo-0.3.4/test/test_simpledb.py` & `redzoo-0.3.5/test/test_simpledb.py`

 * *Files identical despite different names*

