# Comparing `tmp/mfprocess-0.0.5.tar.gz` & `tmp/mfprocess-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfprocess-0.0.5.tar", last modified: Mon Apr 29 20:18:13 2024, max compression
+gzip compressed data, was "mfprocess-0.0.6.tar", last modified: Mon Apr 29 20:23:24 2024, max compression
```

## Comparing `mfprocess-0.0.5.tar` & `mfprocess-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:18:13.475211 mfprocess-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-29 20:18:09.000000 mfprocess-0.0.5/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-29 20:18:13.475211 mfprocess-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 20:18:09.000000 mfprocess-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:18:13.475211 mfprocess-0.0.5/mfprocess/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 20:18:09.000000 mfprocess-0.0.5/mfprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 20:18:09.000000 mfprocess-0.0.5/mfprocess/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:18:13.475211 mfprocess-0.0.5/mfprocess.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-29 20:18:13.000000 mfprocess-0.0.5/mfprocess.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-29 20:18:13.000000 mfprocess-0.0.5/mfprocess.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 20:18:13.000000 mfprocess-0.0.5/mfprocess.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 20:18:13.000000 mfprocess-0.0.5/mfprocess.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 20:18:13.000000 mfprocess-0.0.5/mfprocess.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 20:18:13.475211 mfprocess-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-29 20:18:11.000000 mfprocess-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:23:24.806404 mfprocess-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-29 20:23:20.000000 mfprocess-0.0.6/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-29 20:23:24.806404 mfprocess-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 20:23:20.000000 mfprocess-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:23:24.806404 mfprocess-0.0.6/mfprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 20:23:20.000000 mfprocess-0.0.6/mfprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-29 20:23:20.000000 mfprocess-0.0.6/mfprocess/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:23:24.806404 mfprocess-0.0.6/mfprocess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-29 20:23:24.000000 mfprocess-0.0.6/mfprocess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-29 20:23:24.000000 mfprocess-0.0.6/mfprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 20:23:24.000000 mfprocess-0.0.6/mfprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 20:23:24.000000 mfprocess-0.0.6/mfprocess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 20:23:24.000000 mfprocess-0.0.6/mfprocess.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 20:23:24.806404 mfprocess-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-29 20:23:22.000000 mfprocess-0.0.6/setup.py
```

### Comparing `mfprocess-0.0.5/LICENCE` & `mfprocess-0.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `mfprocess-0.0.5/PKG-INFO` & `mfprocess-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfprocess
-Version: 0.0.5
+Version: 0.0.6
 Summary: Data Process
 Home-page: https://github.com/agustinbustosbarton/mfprocess
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `mfprocess-0.0.5/mfprocess.egg-info/PKG-INFO` & `mfprocess-0.0.6/mfprocess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfprocess
-Version: 0.0.5
+Version: 0.0.6
 Summary: Data Process
 Home-page: https://github.com/agustinbustosbarton/mfprocess
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `mfprocess-0.0.5/setup.py` & `mfprocess-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="mfprocess",
-    version= '0.0.5',  #'0.0.4',   #
+    version= '0.0.6',  #'0.0.4',   #
     author="Agustin Bustos Barton",
     author_email="agustinbustosbarton@gmail.com",
     description="Data Process",
     url = "https://github.com/agustinbustosbarton/mfprocess",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

