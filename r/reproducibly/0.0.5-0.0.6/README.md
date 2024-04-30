# Comparing `tmp/reproducibly-0.0.5.tar.gz` & `tmp/reproducibly-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reproducibly-0.0.5.tar", last modified: Tue Jan  1 00:00:00 1980, max compression
+gzip compressed data, was "reproducibly-0.0.6.tar", last modified: Tue Jan  1 00:00:00 1980, max compression
```

## Comparing `reproducibly-0.0.5.tar` & `reproducibly-0.0.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 1980-01-01 00:00:00.000000 reproducibly-0.0.5/
--rw-r--r--   0 root         (0) root         (0)     2851 1980-01-01 00:00:00.000000 reproducibly-0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2238 1980-01-01 00:00:00.000000 reproducibly-0.0.5/README.md
--rw-r--r--   0 root         (0) root         (0)      855 1980-01-01 00:00:00.000000 reproducibly-0.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)    13359 1980-01-01 00:00:00.000000 reproducibly-0.0.5/reproducibly.py
+drwxr-xr-x   0 root         (0) root         (0)        0 1980-01-01 00:00:00.000000 reproducibly-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)     2851 1980-01-01 00:00:00.000000 reproducibly-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2238 1980-01-01 00:00:00.000000 reproducibly-0.0.6/README.md
+-rw-r--r--   0 root         (0) root         (0)      855 1980-01-01 00:00:00.000000 reproducibly-0.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)    13359 1980-01-01 00:00:00.000000 reproducibly-0.0.6/reproducibly.py
```

### Comparing `reproducibly-0.0.5/PKG-INFO` & `reproducibly-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: reproducibly
-Version: 0.0.5
+Version: 0.0.6
 Summary: Reproducibly build Python packages
 Author-email: Keith Maxwell <keith.maxwell@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Dist: build==1.2.1
 Requires-Dist: cibuildwheel==2.17.0
 Requires-Dist: packaging==24.0
-Requires-Dist: pyproject_hooks==1.0.0
+Requires-Dist: pyproject_hooks==1.1.0
 Project-URL: Homepage, https://github.com/maxwell-k/reproducibly/
 Project-URL: Issues, https://github.com/maxwell-k/reproducibly/issues
 
 # reproducibly.py
 
 ## Introduction / Reproducibly build Python packages.
```

### Comparing `reproducibly-0.0.5/README.md` & `reproducibly-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `reproducibly-0.0.5/pyproject.toml` & `reproducibly-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
 ]
 dependencies = [
   "build==1.2.1",
   "cibuildwheel==2.17.0",
   "packaging==24.0",
-  "pyproject_hooks==1.0.0",
+  "pyproject_hooks==1.1.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/maxwell-k/reproducibly/"
 Issues = "https://github.com/maxwell-k/reproducibly/issues"
 
 [project.scripts]
```

### Comparing `reproducibly-0.0.5/reproducibly.py` & `reproducibly-0.0.6/reproducibly.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 # ]]]
 # /// script
 # requires-python = ">=3.11"
 # dependencies = [
 #   "build==1.2.1",
 #   "cibuildwheel==2.17.0",
 #   "packaging==24.0",
-#   "pyproject_hooks==1.0.0",
+#   "pyproject_hooks==1.1.0",
 # ]
 # ///
 # [[[end]]]
 
 
 # - Built distributions are created from source distributions
 # - Source distributions are typically gzipped tar files
@@ -77,15 +77,15 @@
     # for line in Path("constraints.txt").read_text().splitlines():
     #   cog.outl(f'"{line}",')
     # ]]]
     "wheel==0.43.0",
     # [[[end]]]
 }
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 
 def _build(srcdir: Path, output: Path, distribution: str) -> Path:
     """Call the build API
 
     Returns the path to the built distribution"""
     with DefaultIsolatedEnv() as env:
```

