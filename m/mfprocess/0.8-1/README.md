# Comparing `tmp/mfprocess-0.8.tar.gz` & `tmp/mfprocess-1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfprocess-0.8.tar", last modified: Tue Apr 30 13:55:22 2024, max compression
+gzip compressed data, was "mfprocess-1.tar", last modified: Tue Apr 30 13:57:53 2024, max compression
```

## Comparing `mfprocess-0.8.tar` & `mfprocess-1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:55:22.806764 mfprocess-0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-30 13:55:18.000000 mfprocess-0.8/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-30 13:55:22.806764 mfprocess-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 13:55:18.000000 mfprocess-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:55:22.802764 mfprocess-0.8/mfprocess/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 13:55:18.000000 mfprocess-0.8/mfprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-30 13:55:18.000000 mfprocess-0.8/mfprocess/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-30 13:55:18.000000 mfprocess-0.8/mfprocess/update_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:55:22.806764 mfprocess-0.8/mfprocess.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-30 13:55:22.000000 mfprocess-0.8/mfprocess.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-30 13:55:22.000000 mfprocess-0.8/mfprocess.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:55:22.000000 mfprocess-0.8/mfprocess.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 13:55:22.000000 mfprocess-0.8/mfprocess.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 13:55:22.000000 mfprocess-0.8/mfprocess.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:55:22.806764 mfprocess-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-30 13:55:20.000000 mfprocess-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:57:53.442423 mfprocess-1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-30 13:57:48.000000 mfprocess-1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-30 13:57:53.442423 mfprocess-1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-30 13:57:48.000000 mfprocess-1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:57:53.442423 mfprocess-1/mfprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 13:57:48.000000 mfprocess-1/mfprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-30 13:57:48.000000 mfprocess-1/mfprocess/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-30 13:57:48.000000 mfprocess-1/mfprocess/update_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:57:53.442423 mfprocess-1/mfprocess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-30 13:57:53.000000 mfprocess-1/mfprocess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-30 13:57:53.000000 mfprocess-1/mfprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:57:53.000000 mfprocess-1/mfprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 13:57:53.000000 mfprocess-1/mfprocess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 13:57:53.000000 mfprocess-1/mfprocess.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:57:53.442423 mfprocess-1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-30 13:57:50.000000 mfprocess-1/setup.py
```

### Comparing `mfprocess-0.8/LICENCE` & `mfprocess-1/LICENCE`

 * *Files identical despite different names*

### Comparing `mfprocess-0.8/PKG-INFO` & `mfprocess-1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfprocess
-Version: 0.8
+Version: 1
 Summary: Data Process
 Home-page: https://github.com/agustinbustosbarton/mfprocess
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `mfprocess-0.8/mfprocess.egg-info/PKG-INFO` & `mfprocess-1/mfprocess.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfprocess
-Version: 0.8
+Version: 1
 Summary: Data Process
 Home-page: https://github.com/agustinbustosbarton/mfprocess
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `mfprocess-0.8/setup.py` & `mfprocess-1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="mfprocess",
-    version= '0.08',  #'0.0.4',   #
+    version= '1',  #'0.0.4',   #
     author="Agustin Bustos Barton",
     author_email="agustinbustosbarton@gmail.com",
     description="Data Process",
     url = "https://github.com/agustinbustosbarton/mfprocess",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

