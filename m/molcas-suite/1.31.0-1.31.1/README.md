# Comparing `tmp/molcas_suite-1.31.0.tar.gz` & `tmp/molcas_suite-1.31.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molcas_suite-1.31.0.tar", last modified: Wed Apr 10 13:50:58 2024, max compression
+gzip compressed data, was "molcas_suite-1.31.1.tar", last modified: Tue Apr 30 14:21:10 2024, max compression
```

## Comparing `molcas_suite-1.31.0.tar` & `molcas_suite-1.31.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 h21027rm   (502) staff       (20)        0 2024-04-10 13:50:58.200200 molcas_suite-1.31.0/
--rw-r--r--   0 h21027rm   (502) staff       (20)    35072 2024-03-12 11:49:12.000000 molcas_suite-1.31.0/LICENSE
--rw-r--r--   0 h21027rm   (502) staff       (20)     3803 2024-04-10 13:50:58.198803 molcas_suite-1.31.0/PKG-INFO
--rwxr-xr-x   0 h21027rm   (502) staff       (20)     2952 2024-03-12 11:49:12.000000 molcas_suite-1.31.0/README.md
-drwxr-xr-x   0 h21027rm   (502) staff       (20)        0 2024-04-10 13:50:58.191725 molcas_suite-1.31.0/molcas_suite/
--rw-r--r--   0 h21027rm   (502) staff       (20)       31 2024-03-12 11:49:12.000000 molcas_suite-1.31.0/molcas_suite/__init__.py
--rw-r--r--   0 h21027rm   (502) staff       (20)      107 2024-04-10 13:43:53.000000 molcas_suite-1.31.0/molcas_suite/__version__.py
--rw-r--r--   0 h21027rm   (502) staff       (20)     6311 2024-03-12 11:49:12.000000 molcas_suite-1.31.0/molcas_suite/barrier.py
--rw-r--r--   0 h21027rm   (502) staff       (20)     1440 2024-03-12 11:49:12.000000 molcas_suite-1.31.0/molcas_suite/cfp.py
--rw-r--r--   0 h21027rm   (502) staff       (20)    31129 2024-04-10 13:21:22.000000 molcas_suite-1.31.0/molcas_suite/cli.py
--rw-r--r--   0 h21027rm   (502) staff       (20)    34861 2024-03-12 11:49:12.000000 molcas_suite-1.31.0/molcas_suite/extractor.py
--rw-r--r--   0 h21027rm   (502) staff       (20)    18445 2024-03-12 11:49:12.000000 molcas_suite-1.31.0/molcas_suite/generate_input.py
--rw-r--r--   0 h21027rm   (502) staff       (20)    25242 2024-03-12 11:49:12.000000 molcas_suite-1.31.0/molcas_suite/generate_job.py
--rw-r--r--   0 h21027rm   (502) staff       (20)     6412 2024-03-12 11:49:12.000000 molcas_suite-1.31.0/molcas_suite/h5tools.py
--rw-r--r--   0 h21027rm   (502) staff       (20)    27067 2024-04-10 13:21:22.000000 molcas_suite-1.31.0/molcas_suite/orbs.py
-drwxr-xr-x   0 h21027rm   (502) staff       (20)        0 2024-04-10 13:50:58.197327 molcas_suite-1.31.0/molcas_suite.egg-info/
--rw-r--r--   0 h21027rm   (502) staff       (20)     3803 2024-04-10 13:50:58.000000 molcas_suite-1.31.0/molcas_suite.egg-info/PKG-INFO
--rw-r--r--   0 h21027rm   (502) staff       (20)      507 2024-04-10 13:50:58.000000 molcas_suite-1.31.0/molcas_suite.egg-info/SOURCES.txt
--rw-r--r--   0 h21027rm   (502) staff       (20)        1 2024-04-10 13:50:58.000000 molcas_suite-1.31.0/molcas_suite.egg-info/dependency_links.txt
--rw-r--r--   0 h21027rm   (502) staff       (20)       55 2024-04-10 13:50:58.000000 molcas_suite-1.31.0/molcas_suite.egg-info/entry_points.txt
--rw-r--r--   0 h21027rm   (502) staff       (20)       80 2024-04-10 13:50:58.000000 molcas_suite-1.31.0/molcas_suite.egg-info/requires.txt
--rw-r--r--   0 h21027rm   (502) staff       (20)       13 2024-04-10 13:50:58.000000 molcas_suite-1.31.0/molcas_suite.egg-info/top_level.txt
--rw-r--r--   0 h21027rm   (502) staff       (20)     1116 2024-04-10 13:46:40.000000 molcas_suite-1.31.0/pyproject.toml
--rw-r--r--   0 h21027rm   (502) staff       (20)       38 2024-04-10 13:50:58.200263 molcas_suite-1.31.0/setup.cfg
--rw-r--r--   0 h21027rm   (502) staff       (20)     1458 2024-04-10 13:44:17.000000 molcas_suite-1.31.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:21:10.426656 molcas_suite-1.31.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35072 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3803 2024-04-30 14:21:10.426656 molcas_suite-1.31.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2952 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:21:10.425656 molcas_suite-1.31.1/molcas_suite/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/molcas_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-30 14:21:05.000000 molcas_suite-1.31.1/molcas_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6311 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/molcas_suite/barrier.py
+-rw-rw-rw-   0 root         (0) root         (0)     1440 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/molcas_suite/cfp.py
+-rw-rw-rw-   0 root         (0) root         (0)    31142 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/molcas_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    34861 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/molcas_suite/extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)    18445 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/molcas_suite/generate_input.py
+-rw-rw-rw-   0 root         (0) root         (0)    25242 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/molcas_suite/generate_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     6412 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/molcas_suite/h5tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    27067 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/molcas_suite/orbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:21:10.426656 molcas_suite-1.31.1/molcas_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3803 2024-04-30 14:21:10.000000 molcas_suite-1.31.1/molcas_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      507 2024-04-30 14:21:10.000000 molcas_suite-1.31.1/molcas_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 14:21:10.000000 molcas_suite-1.31.1/molcas_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2024-04-30 14:21:10.000000 molcas_suite-1.31.1/molcas_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-30 14:21:10.000000 molcas_suite-1.31.1/molcas_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-30 14:21:10.000000 molcas_suite-1.31.1/molcas_suite.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-04-30 14:20:39.000000 molcas_suite-1.31.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 14:21:10.426656 molcas_suite-1.31.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1458 2024-04-30 14:21:05.000000 molcas_suite-1.31.1/setup.py
```

### Comparing `molcas_suite-1.31.0/LICENSE` & `molcas_suite-1.31.1/LICENSE`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.31.0/PKG-INFO` & `molcas_suite-1.31.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molcas_suite
-Version: 1.31.0
+Version: 1.31.1
 Summary: A package for dealing with OpenMOLCAS input and output files
 Home-page: https://gitlab.com/chilton-group/molcas_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/molcas_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/molcas_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molcas_suite-1.31.0/README.md` & `molcas_suite-1.31.1/README.md`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.31.0/molcas_suite/barrier.py` & `molcas_suite-1.31.1/molcas_suite/barrier.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.31.0/molcas_suite/cfp.py` & `molcas_suite-1.31.1/molcas_suite/cfp.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.31.0/molcas_suite/cli.py` & `molcas_suite-1.31.1/molcas_suite/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         command line arguments
 
     Returns
     -------
     None
 
     """
-    labels, coords = xyzp.load_xyz(args.xyz_input, capitalise=False)
+    labels, coords = xyzp.load_xyz(args.xyz_input, capitalise=False, check=False)
 
     # set output to stem of xyz_input if not supplied
     path = args.xyz_input
     abs_stem = os.path.splitext(path)[0]
 
     name = args.output if args.output else abs_stem + '.input'
```

### Comparing `molcas_suite-1.31.0/molcas_suite/extractor.py` & `molcas_suite-1.31.1/molcas_suite/extractor.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.31.0/molcas_suite/generate_input.py` & `molcas_suite-1.31.1/molcas_suite/generate_input.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.31.0/molcas_suite/generate_job.py` & `molcas_suite-1.31.1/molcas_suite/generate_job.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.31.0/molcas_suite/h5tools.py` & `molcas_suite-1.31.1/molcas_suite/h5tools.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.31.0/molcas_suite/orbs.py` & `molcas_suite-1.31.1/molcas_suite/orbs.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.31.0/molcas_suite.egg-info/PKG-INFO` & `molcas_suite-1.31.1/molcas_suite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molcas_suite
-Version: 1.31.0
+Version: 1.31.1
 Summary: A package for dealing with OpenMOLCAS input and output files
 Home-page: https://gitlab.com/chilton-group/molcas_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/molcas_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/molcas_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molcas_suite-1.31.0/pyproject.toml` & `molcas_suite-1.31.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+
 [tool.semantic_release]
 commit_message = "{version}\n\nAutomatically generated by python-semantic-release"
 commit_parser = "angular"
 logging_use_named_masks = false
 major_on_zero = true
 tag_format = "v{version}"
-version_variable = [
+version_variables = [
     'setup.py:__version__',
     'molcas_suite/__version__.py:__version__'
     ]
 upload_to_pypi=true
 branch = "master"
 hvcs="gitlab"
 
@@ -36,8 +37,8 @@
 hvcs = "gitlab"
 
 [tool.semantic_release.remote.token]
 env = "GL_TOKEN"
 
 [tool.semantic_release.publish]
 dist_glob_patterns = ["dist/*"]
-upload_to_vcs_release = true
+upload_to_vcs_release = true
```

### Comparing `molcas_suite-1.31.0/setup.py` & `molcas_suite-1.31.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "1.31.0"
+__version__ = "1.31.1"
 
 setuptools.setup(
     name='molcas_suite',
     version=__version__,
     author='Chilton Group',
     author_email='nicholas.chilton@manchester.ac.uk',
     description='A package for dealing with OpenMOLCAS input and output files',
```

