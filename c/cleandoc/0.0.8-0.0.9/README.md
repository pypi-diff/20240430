# Comparing `tmp/cleandoc-0.0.8.tar.gz` & `tmp/cleandoc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleandoc-0.0.8.tar", last modified: Mon Nov 13 13:03:54 2023, max compression
+gzip compressed data, was "cleandoc-0.0.9.tar", last modified: Mon Nov 13 22:04:04 2023, max compression
```

## Comparing `cleandoc-0.0.8.tar` & `cleandoc-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-11-13 13:03:54.406527 cleandoc-0.0.8/
--rw-rw-rw-   0        0        0    35821 2023-08-08 21:22:00.000000 cleandoc-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     4598 2023-11-13 13:03:54.406527 cleandoc-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3904 2023-11-12 02:12:01.000000 cleandoc-0.0.8/README.md
--rw-rw-rw-   0        0        0      926 2023-11-13 13:03:41.000000 cleandoc-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-11-13 13:03:54.406527 cleandoc-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-11-13 13:03:54.372691 cleandoc-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-11-13 13:03:54.383098 cleandoc-0.0.8/src/cleandoc/
--rw-rw-rw-   0        0        0     6986 2023-11-13 12:28:44.000000 cleandoc-0.0.8/src/cleandoc/__init__.py
--rw-rw-rw-   0        0        0     2794 2023-11-11 21:04:58.000000 cleandoc-0.0.8/src/cleandoc/clean.py
--rw-rw-rw-   0        0        0     2098 2023-08-18 07:33:01.000000 cleandoc-0.0.8/src/cleandoc/cli.py
--rw-rw-rw-   0        0        0     3081 2023-08-22 21:07:41.000000 cleandoc-0.0.8/src/cleandoc/doq.py
--rw-rw-rw-   0        0        0     6835 2023-11-13 13:02:30.000000 cleandoc-0.0.8/src/cleandoc/helper.py
--rw-rw-rw-   0        0        0        0 2023-11-11 02:46:26.000000 cleandoc-0.0.8/src/cleandoc/py.typed
--rw-rw-rw-   0        0        0    10327 2023-11-11 21:04:48.000000 cleandoc-0.0.8/src/cleandoc/sphinxdoc.py
-drwxrwxrwx   0        0        0        0 2023-11-13 13:03:54.404528 cleandoc-0.0.8/src/cleandoc.egg-info/
--rw-rw-rw-   0        0        0     4598 2023-11-13 13:03:54.000000 cleandoc-0.0.8/src/cleandoc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-11-13 13:03:54.000000 cleandoc-0.0.8/src/cleandoc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-13 13:03:54.000000 cleandoc-0.0.8/src/cleandoc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-11-13 13:03:54.000000 cleandoc-0.0.8/src/cleandoc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       73 2023-11-13 13:03:54.000000 cleandoc-0.0.8/src/cleandoc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-11-13 13:03:54.000000 cleandoc-0.0.8/src/cleandoc.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-11-13 13:03:54.405527 cleandoc-0.0.8/test/
--rw-rw-rw-   0        0        0     1308 2023-11-13 10:47:54.000000 cleandoc-0.0.8/test/test_cleandoc.py
+drwxrwxrwx   0        0        0        0 2023-11-13 22:04:04.594149 cleandoc-0.0.9/
+-rw-rw-rw-   0        0        0    35821 2023-08-08 21:22:00.000000 cleandoc-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     4598 2023-11-13 22:04:04.593132 cleandoc-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3904 2023-11-12 02:12:01.000000 cleandoc-0.0.9/README.md
+-rw-rw-rw-   0        0        0      941 2023-11-13 22:03:51.000000 cleandoc-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-11-13 22:04:04.594149 cleandoc-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-11-13 22:04:04.547909 cleandoc-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-11-13 22:04:04.562275 cleandoc-0.0.9/src/cleandoc/
+-rw-rw-rw-   0        0        0     6986 2023-11-13 12:28:44.000000 cleandoc-0.0.9/src/cleandoc/__init__.py
+-rw-rw-rw-   0        0        0     2794 2023-11-11 21:04:58.000000 cleandoc-0.0.9/src/cleandoc/clean.py
+-rw-rw-rw-   0        0        0     2098 2023-08-18 07:33:01.000000 cleandoc-0.0.9/src/cleandoc/cli.py
+-rw-rw-rw-   0        0        0     3081 2023-08-22 21:07:41.000000 cleandoc-0.0.9/src/cleandoc/doq.py
+-rw-rw-rw-   0        0        0     6861 2023-11-13 22:02:59.000000 cleandoc-0.0.9/src/cleandoc/helper.py
+-rw-rw-rw-   0        0        0        0 2023-11-11 02:46:26.000000 cleandoc-0.0.9/src/cleandoc/py.typed
+-rw-rw-rw-   0        0        0    10327 2023-11-11 21:04:48.000000 cleandoc-0.0.9/src/cleandoc/sphinxdoc.py
+drwxrwxrwx   0        0        0        0 2023-11-13 22:04:04.585130 cleandoc-0.0.9/src/cleandoc.egg-info/
+-rw-rw-rw-   0        0        0     4598 2023-11-13 22:04:04.000000 cleandoc-0.0.9/src/cleandoc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-11-13 22:04:04.000000 cleandoc-0.0.9/src/cleandoc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-13 22:04:04.000000 cleandoc-0.0.9/src/cleandoc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-11-13 22:04:04.000000 cleandoc-0.0.9/src/cleandoc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       73 2023-11-13 22:04:04.000000 cleandoc-0.0.9/src/cleandoc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-11-13 22:04:04.000000 cleandoc-0.0.9/src/cleandoc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-11-13 22:04:04.592131 cleandoc-0.0.9/test/
+-rw-rw-rw-   0        0        0     1308 2023-11-13 10:47:54.000000 cleandoc-0.0.9/test/test_cleandoc.py
```

### Comparing `cleandoc-0.0.8/LICENSE.txt` & `cleandoc-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cleandoc-0.0.8/PKG-INFO` & `cleandoc-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleandoc
-Version: 0.0.8
+Version: 0.0.9
 Author-email: Jason Krist <jkrist2696@gmail.com>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/jkrist2696/cleandoc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
```

### Comparing `cleandoc-0.0.8/README.md` & `cleandoc-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cleandoc-0.0.8/pyproject.toml` & `cleandoc-0.0.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -11,20 +11,20 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     'Operating System :: Microsoft :: Windows',
     'Operating System :: Unix',
 ]
 
 name = "cleandoc"
-version = "0.0.8"
+version = "0.0.9"
 authors = [{ name = "Jason Krist", email = "jkrist2696@gmail.com" }]
 description = ""
 requires-python = ">=3.12.0"
 dependencies = ["black>=23.3.0","Sphinx>=6.2.1","doq>=0.9.1","m2r2","sphinx_rtd_theme","pylint","mypy"]
 [tool.setuptools.package-data]
 cleandoc = ["*.typed", ".template"]
 [tool.setuptools.exclude-package-data]
-cleandoc = ["__pycache__/*"]
+cleandoc = ["__pycache__/*", "__pycache__"]
 [project.scripts]
 cleandoc="cleandoc:cli_main"
 [project.urls]
 "Homepage" = "https://github.com/jkrist2696/cleandoc"
```

### Comparing `cleandoc-0.0.8/src/cleandoc/__init__.py` & `cleandoc-0.0.9/src/cleandoc/__init__.py`

 * *Files identical despite different names*

### Comparing `cleandoc-0.0.8/src/cleandoc/clean.py` & `cleandoc-0.0.9/src/cleandoc/clean.py`

 * *Files identical despite different names*

### Comparing `cleandoc-0.0.8/src/cleandoc/cli.py` & `cleandoc-0.0.9/src/cleandoc/cli.py`

 * *Files identical despite different names*

### Comparing `cleandoc-0.0.8/src/cleandoc/doq.py` & `cleandoc-0.0.9/src/cleandoc/doq.py`

 * *Files identical despite different names*

### Comparing `cleandoc-0.0.8/src/cleandoc/helper.py` & `cleandoc-0.0.9/src/cleandoc/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
     results = findall_infile(regex, logpath, skip_exist=True)
     for result in results:
         if not check_modified(result[1], result[0]):
             clean_pyfiles.append(result[1])
     return clean_pyfiles
 
 
-def config_log(file: str = "", level=logging.INFO):
+def config_log(file: str = "", level=logging.DEBUG):
     """Configure log file using logging module
 
     Parameters
     ----------
     file : str = ""
         Path to logfile to write
     level
@@ -217,27 +217,27 @@
     logger object
 
     """
     logname = "cleandoc"
     logger = logging.getLogger(logname)
     if logger.hasHandlers():
         return logger
-    logging.basicConfig(level=logging.WARN)  # level=logging.WARN
     fs = "%(asctime)s | %(name)s | %(levelname)s | %(message)s"
     dfs = "%d-%m-%y | %H:%M:%S"
+    logging.basicConfig(stream=stdout, format=fs, datefmt=dfs, level=logging.INFO)
     if len(file) > 0:
         if path.exists(file):
             remove(file)
         file_handler = logging.FileHandler(file)
         print(f"logfile path: {path.realpath(file)}\n")
         file_handler.setFormatter(logging.Formatter(fs, dfs, "%"))
         file_handler.setLevel(logging.DEBUG)
         logger.addHandler(file_handler)
-    stdout_handler = logging.StreamHandler(stdout)
-    stdout_handler.setFormatter(logging.Formatter(fs, dfs, "%"))
-    logger.addHandler(stdout_handler)
-    logger.propagate = False
+    # stdout_handler = logging.StreamHandler(stdout)
+    # stdout_handler.setFormatter(logging.Formatter(fs, dfs, "%"))
+    # logger.addHandler(stdout_handler)
+    # logger.propagate = False
     logger.setLevel(level)
     return logger
 
 
 # if __name__ == "__main__":
```

### Comparing `cleandoc-0.0.8/src/cleandoc/sphinxdoc.py` & `cleandoc-0.0.9/src/cleandoc/sphinxdoc.py`

 * *Files identical despite different names*

### Comparing `cleandoc-0.0.8/src/cleandoc.egg-info/PKG-INFO` & `cleandoc-0.0.9/src/cleandoc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleandoc
-Version: 0.0.8
+Version: 0.0.9
 Author-email: Jason Krist <jkrist2696@gmail.com>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/jkrist2696/cleandoc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
```

### Comparing `cleandoc-0.0.8/test/test_cleandoc.py` & `cleandoc-0.0.9/test/test_cleandoc.py`

 * *Files identical despite different names*

