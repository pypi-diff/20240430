# Comparing `tmp/sfdmap2-0.2.2.post1.tar.gz` & `tmp/sfdmap2-0.2.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfdmap2-0.2.2.post1.tar", max compression
+gzip compressed data, was "sfdmap2-0.2.2.post2.tar", max compression
```

## Comparing `sfdmap2-0.2.2.post1.tar` & `sfdmap2-0.2.2.post2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     6028 2023-10-20 09:37:53.710639 sfdmap2-0.2.2.post1/README.md
--rw-r--r--   0        0        0      631 2023-10-20 09:37:53.710639 sfdmap2-0.2.2.post1/pyproject.toml
--rw-r--r--   0        0        0    12432 2023-10-20 09:37:53.710639 sfdmap2-0.2.2.post1/sfdmap2/sfdmap.py
--rw-r--r--   0        0        0     6829 1970-01-01 00:00:00.000000 sfdmap2-0.2.2.post1/PKG-INFO
+-rw-r--r--   0        0        0     6028 2024-04-30 09:21:18.123091 sfdmap2-0.2.2.post2/README.md
+-rw-r--r--   0        0        0      624 2024-04-30 09:21:18.123091 sfdmap2-0.2.2.post2/pyproject.toml
+-rw-r--r--   0        0        0    12432 2024-04-30 09:21:18.123091 sfdmap2-0.2.2.post2/sfdmap2/sfdmap.py
+-rw-r--r--   0        0        0     6861 1970-01-01 00:00:00.000000 sfdmap2-0.2.2.post2/PKG-INFO
```

### Comparing `sfdmap2-0.2.2.post1/README.md` & `sfdmap2-0.2.2.post2/README.md`

 * *Files identical despite different names*

### Comparing `sfdmap2-0.2.2.post1/pyproject.toml` & `sfdmap2-0.2.2.post2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "sfdmap2"
-version = "0.2.2-1"
+version = "0.2.2-2"
 description = "Get E(B-V) values from SFD dust map data"
 authors = ["Kyle Barbary"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/simeonreusch/sfdmap2"
 maintainers = [
     "Simeon Reusch <simeon.reusch@desy.de>"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.24.2"
-astropy = "^5.2.1"
-fitsio = {version="^1.1.8", optional=true}
+astropy = ">=5"
+fitsio = {version="^1", optional=true}
 
 [tool.poetry.extras]
 fits = ["fitsio"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 coveralls = "^3.3.1"
```

### Comparing `sfdmap2-0.2.2.post1/sfdmap2/sfdmap.py` & `sfdmap2-0.2.2.post2/sfdmap2/sfdmap.py`

 * *Files identical despite different names*

### Comparing `sfdmap2-0.2.2.post1/PKG-INFO` & `sfdmap2-0.2.2.post2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: sfdmap2
-Version: 0.2.2.post1
+Version: 0.2.2.post2
 Summary: Get E(B-V) values from SFD dust map data
 Home-page: https://github.com/simeonreusch/sfdmap2
 License: MIT
 Author: Kyle Barbary
 Maintainer: Simeon Reusch
 Maintainer-email: simeon.reusch@desy.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: fits
-Requires-Dist: astropy (>=5.2.1,<6.0.0)
-Requires-Dist: fitsio (>=1.1.8,<2.0.0) ; extra == "fits"
+Requires-Dist: astropy (>=5)
+Requires-Dist: fitsio (>=1,<2) ; extra == "fits"
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Project-URL: Repository, https://github.com/simeonreusch/sfdmap2
 Description-Content-Type: text/markdown
 
 # sfdmap2
 This is a fork of [sfdmap](https://github.com/kbarbary/sfdmap), as the original repository is no longer maintained.
```

