# Comparing `tmp/egrader-0.0.7.tar.gz` & `tmp/egrader-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "egrader-0.0.7.tar", last modified: Fri Mar  8 18:14:04 2024, max compression
+gzip compressed data, was "egrader-0.0.8.tar", last modified: Tue Apr 30 12:14:18 2024, max compression
```

## Comparing `egrader-0.0.7.tar` & `egrader-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:14:04.051741 egrader-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-08 18:13:55.000000 egrader-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-03-08 18:14:04.051741 egrader-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-08 18:13:55.000000 egrader-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:14:04.051741 egrader-0.0.7/egrader/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-08 18:13:55.000000 egrader-0.0.7/egrader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-03-08 18:13:55.000000 egrader-0.0.7/egrader/assess.py
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-03-08 18:13:55.000000 egrader-0.0.7/egrader/cli_bin.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-08 18:13:55.000000 egrader-0.0.7/egrader/cli_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-03-08 18:13:55.000000 egrader-0.0.7/egrader/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-08 18:13:55.000000 egrader-0.0.7/egrader/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-08 18:13:55.000000 egrader-0.0.7/egrader/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-03-08 18:13:55.000000 egrader-0.0.7/egrader/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-08 18:13:55.000000 egrader-0.0.7/egrader/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-03-08 18:13:55.000000 egrader-0.0.7/egrader/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-08 18:13:55.000000 egrader-0.0.7/egrader/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 18:14:04.051741 egrader-0.0.7/egrader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-03-08 18:14:04.000000 egrader-0.0.7/egrader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-08 18:14:04.000000 egrader-0.0.7/egrader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 18:14:04.000000 egrader-0.0.7/egrader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-08 18:14:04.000000 egrader-0.0.7/egrader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-08 18:14:04.000000 egrader-0.0.7/egrader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-08 18:14:04.000000 egrader-0.0.7/egrader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-03-08 18:13:55.000000 egrader-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 18:14:04.051741 egrader-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:14:18.107191 egrader-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-30 12:14:08.000000 egrader-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-30 12:14:18.107191 egrader-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-30 12:14:08.000000 egrader-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:14:18.103191 egrader-0.0.8/egrader/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-30 12:14:08.000000 egrader-0.0.8/egrader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-04-30 12:14:08.000000 egrader-0.0.8/egrader/assess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-30 12:14:08.000000 egrader-0.0.8/egrader/cli_bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-30 12:14:08.000000 egrader-0.0.8/egrader/cli_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-30 12:14:08.000000 egrader-0.0.8/egrader/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-30 12:14:08.000000 egrader-0.0.8/egrader/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-30 12:14:08.000000 egrader-0.0.8/egrader/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-30 12:14:08.000000 egrader-0.0.8/egrader/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-30 12:14:08.000000 egrader-0.0.8/egrader/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-04-30 12:14:08.000000 egrader-0.0.8/egrader/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-30 12:14:08.000000 egrader-0.0.8/egrader/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:14:18.107191 egrader-0.0.8/egrader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-30 12:14:18.000000 egrader-0.0.8/egrader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-30 12:14:18.000000 egrader-0.0.8/egrader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 12:14:18.000000 egrader-0.0.8/egrader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-30 12:14:18.000000 egrader-0.0.8/egrader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-30 12:14:18.000000 egrader-0.0.8/egrader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 12:14:18.000000 egrader-0.0.8/egrader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-30 12:14:08.000000 egrader-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 12:14:18.107191 egrader-0.0.8/setup.cfg
```

### Comparing `egrader-0.0.7/LICENSE` & `egrader-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `egrader-0.0.7/PKG-INFO` & `egrader-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: egrader
-Version: 0.0.7
+Version: 0.0.8
 Summary: Auto-grader for Git-based programming exercises
 Author-email: Nuno Fachada <nuno.fachada@ulusofona.pt>
 License: GPL-3
 Project-URL: Bug Reports, https://github.com/VideojogosLusofona/egrader/issues
 Project-URL: Documentation, https://videojogoslusofona.github.io/egrader/
 Project-URL: Source, https://github.com/VideojogosLusofona/egrader
 Keywords: aat,education,autograder,programming,computer science education
```

### Comparing `egrader-0.0.7/README.md` & `egrader-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `egrader-0.0.7/egrader/assess.py` & `egrader-0.0.8/egrader/assess.py`

 * *Files identical despite different names*

### Comparing `egrader-0.0.7/egrader/cli_bin.py` & `egrader-0.0.8/egrader/cli_bin.py`

 * *Files identical despite different names*

### Comparing `egrader-0.0.7/egrader/cli_lib.py` & `egrader-0.0.8/egrader/cli_lib.py`

 * *Files identical despite different names*

### Comparing `egrader-0.0.7/egrader/fetch.py` & `egrader-0.0.8/egrader/fetch.py`

 * *Files identical despite different names*

### Comparing `egrader-0.0.7/egrader/git.py` & `egrader-0.0.8/egrader/git.py`

 * *Files identical despite different names*

### Comparing `egrader-0.0.7/egrader/paths.py` & `egrader-0.0.8/egrader/paths.py`

 * *Files identical despite different names*

### Comparing `egrader-0.0.7/egrader/plugin.py` & `egrader-0.0.8/egrader/plugin.py`

 * *Files identical despite different names*

### Comparing `egrader-0.0.7/egrader/report.py` & `egrader-0.0.8/egrader/report.py`

 * *Files identical despite different names*

### Comparing `egrader-0.0.7/egrader/types.py` & `egrader-0.0.8/egrader/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Classes used in egrader."""
 
 from pathlib import Path
 from typing import Any, Dict, List
 from urllib.parse import urlparse
 
-import requests
+# import requests
 import validators
 from yarl import URL
 
 
 class StudentGit:
     """A student and his Git repositories."""
 
@@ -28,15 +28,15 @@
             p = Path(u.netloc, u.path)
             if p.exists() and p.is_dir():
                 self.url_type = "file"
                 self._url = str(p)
         elif (
             u.scheme in {"http", "https"}  # Is it a HTTP/HTTPS URL?
             and validators.url(url)  # Is it a well-formed URL?
-            and requests.head(url).status_code < 400  # Valid net resource (200)?
+            # and requests.head(url).status_code < 400  # Valid net resource (200)?
         ):
             self.url_type = u.scheme
             self._url = url
 
     def __repr__(self) -> str:
         """String representation of this instance for YAML serialization."""
         return "%s(sid=%r, email=%r, url=%r, url_type=%r, repos=%r)" % (
```

### Comparing `egrader-0.0.7/egrader/yaml.py` & `egrader-0.0.8/egrader/yaml.py`

 * *Files identical despite different names*

### Comparing `egrader-0.0.7/egrader.egg-info/PKG-INFO` & `egrader-0.0.8/egrader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: egrader
-Version: 0.0.7
+Version: 0.0.8
 Summary: Auto-grader for Git-based programming exercises
 Author-email: Nuno Fachada <nuno.fachada@ulusofona.pt>
 License: GPL-3
 Project-URL: Bug Reports, https://github.com/VideojogosLusofona/egrader/issues
 Project-URL: Documentation, https://videojogoslusofona.github.io/egrader/
 Project-URL: Source, https://github.com/VideojogosLusofona/egrader
 Keywords: aat,education,autograder,programming,computer science education
```

### Comparing `egrader-0.0.7/egrader.egg-info/entry_points.txt` & `egrader-0.0.8/egrader.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `egrader-0.0.7/pyproject.toml` & `egrader-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "setuptools" ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "egrader"
 description = "Auto-grader for Git-based programming exercises"
-version = "0.0.7"
+version = "0.0.8"
 authors = [ { name = "Nuno Fachada", email = "nuno.fachada@ulusofona.pt" } ]
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = [
     "aat",
     "education",
     "autograder",
```

