# Comparing `tmp/git_fastcdc-0.4.0.tar.gz` & `tmp/git_fastcdc-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_fastcdc-0.4.0.tar", max compression
+gzip compressed data, was "git_fastcdc-0.5.0.tar", max compression
```

## Comparing `git_fastcdc-0.4.0.tar` & `git_fastcdc-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    34523 2024-03-28 16:09:33.984653 git_fastcdc-0.4.0/LICENSE
--rw-r--r--   0        0        0     1927 2024-03-29 15:39:11.766309 git_fastcdc-0.4.0/README.md
--rw-r--r--   0        0        0    16458 2024-03-31 12:41:39.115237 git_fastcdc-0.4.0/git_fastcdc.py
--rw-r--r--   0        0        0      721 2024-04-10 10:42:15.108265 git_fastcdc-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2646 1970-01-01 00:00:00.000000 git_fastcdc-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-28 16:09:33.984653 git_fastcdc-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1927 2024-03-29 15:39:11.766309 git_fastcdc-0.5.0/README.md
+-rw-r--r--   0        0        0    16458 2024-04-10 10:47:48.689734 git_fastcdc-0.5.0/git_fastcdc.py
+-rw-r--r--   0        0        0      721 2024-04-30 12:00:32.503249 git_fastcdc-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2646 1970-01-01 00:00:00.000000 git_fastcdc-0.5.0/PKG-INFO
```

### Comparing `git_fastcdc-0.4.0/LICENSE` & `git_fastcdc-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git_fastcdc-0.4.0/README.md` & `git_fastcdc-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `git_fastcdc-0.4.0/git_fastcdc.py` & `git_fastcdc-0.5.0/git_fastcdc.py`

 * *Files 1% similar despite different names*

```diff
@@ -641,16 +641,16 @@
             "config",
             "--unset",
             "core.bigFileThreshold",
         ],
     )
 
 
-@delta.command()
-def disable_delta(name="disable"):
+@delta.command(name="disable")
+def disable_delta():
     """Disable delta-compression."""
     run(
         [
             "git",
             "config",
             "--local",
             "core.bigFileThreshold",
```

### Comparing `git_fastcdc-0.4.0/pyproject.toml` & `git_fastcdc-0.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "git-fastcdc"
-version = "0.4.0"
+version = "0.5.0"
 description = "FastCDC for large git files"
 authors = ["Jean-Louis Fuchs <jean-louis.fuchs@adfinis.com>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.scripts]
 git-fastcdc = 'git_fastcdc:cli'
```

### Comparing `git_fastcdc-0.4.0/PKG-INFO` & `git_fastcdc-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-fastcdc
-Version: 0.4.0
+Version: 0.5.0
 Summary: FastCDC for large git files
 License: AGPL-3.0-or-later
 Author: Jean-Louis Fuchs
 Author-email: jean-louis.fuchs@adfinis.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

