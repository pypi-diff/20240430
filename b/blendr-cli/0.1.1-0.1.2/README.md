# Comparing `tmp/blendr_cli-0.1.1.tar.gz` & `tmp/blendr_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blendr_cli-0.1.1.tar", last modified: Mon Apr 29 20:29:35 2024, max compression
+gzip compressed data, was "blendr_cli-0.1.2.tar", last modified: Tue Apr 30 06:44:49 2024, max compression
```

## Comparing `blendr_cli-0.1.1.tar` & `blendr_cli-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-29 20:29:35.988284 blendr_cli-0.1.1/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     3012 2024-04-29 20:29:35.988072 blendr_cli-0.1.1/PKG-INFO
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     2677 2024-04-29 20:20:22.000000 blendr_cli-0.1.1/README.md
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-29 20:29:35.985316 blendr_cli-0.1.1/blendr/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-20 16:49:51.000000 blendr_cli-0.1.1/blendr/__init__.py
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-29 20:29:35.985810 blendr_cli-0.1.1/blendr/auth/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-21 17:20:43.000000 blendr_cli-0.1.1/blendr/auth/__init__.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     2021 2024-04-28 21:02:26.000000 blendr_cli-0.1.1/blendr/auth/authenticate.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     1867 2024-04-29 18:25:08.000000 blendr_cli-0.1.1/blendr/cli.py
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-29 20:29:35.986640 blendr_cli-0.1.1/blendr/config/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-21 17:20:41.000000 blendr_cli-0.1.1/blendr/config/__init__.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)      119 2024-04-29 18:47:00.000000 blendr_cli-0.1.1/blendr/config/settings.py
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     3440 2024-04-29 18:27:36.000000 blendr_cli-0.1.1/blendr/config/setup.py
-drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-29 20:29:35.987803 blendr_cli-0.1.1/blendr_cli.egg-info/
--rw-r--r--   0 stefanshiloh   (501) staff       (20)     3012 2024-04-29 20:29:35.000000 blendr_cli-0.1.1/blendr_cli.egg-info/PKG-INFO
--rw-r--r--   0 stefanshiloh   (501) staff       (20)      384 2024-04-29 20:29:35.000000 blendr_cli-0.1.1/blendr_cli.egg-info/SOURCES.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        1 2024-04-29 20:29:35.000000 blendr_cli-0.1.1/blendr_cli.egg-info/dependency_links.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)       43 2024-04-29 20:29:35.000000 blendr_cli-0.1.1/blendr_cli.egg-info/entry_points.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)       24 2024-04-29 20:29:35.000000 blendr_cli-0.1.1/blendr_cli.egg-info/requires.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)        7 2024-04-29 20:29:35.000000 blendr_cli-0.1.1/blendr_cli.egg-info/top_level.txt
--rw-r--r--   0 stefanshiloh   (501) staff       (20)       38 2024-04-29 20:29:35.988333 blendr_cli-0.1.1/setup.cfg
--rw-r--r--   0 stefanshiloh   (501) staff       (20)      746 2024-04-29 20:28:38.000000 blendr_cli-0.1.1/setup.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 06:44:49.185078 blendr_cli-0.1.2/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     3079 2024-04-30 06:44:49.184860 blendr_cli-0.1.2/PKG-INFO
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     2677 2024-04-29 20:20:22.000000 blendr_cli-0.1.2/README.md
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 06:44:49.181828 blendr_cli-0.1.2/blendr/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-20 16:49:51.000000 blendr_cli-0.1.2/blendr/__init__.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 06:44:49.182221 blendr_cli-0.1.2/blendr/auth/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-21 17:20:43.000000 blendr_cli-0.1.2/blendr/auth/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     2021 2024-04-28 21:02:26.000000 blendr_cli-0.1.2/blendr/auth/authenticate.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     1867 2024-04-29 18:25:08.000000 blendr_cli-0.1.2/blendr/cli.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 06:44:49.182844 blendr_cli-0.1.2/blendr/config/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-21 17:20:41.000000 blendr_cli-0.1.2/blendr/config/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      119 2024-04-29 18:47:00.000000 blendr_cli-0.1.2/blendr/config/settings.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     3440 2024-04-29 18:27:36.000000 blendr_cli-0.1.2/blendr/config/setup.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 06:44:49.183217 blendr_cli-0.1.2/blendr/gpu_manager/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-29 22:27:38.000000 blendr_cli-0.1.2/blendr/gpu_manager/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      190 2024-04-29 20:05:17.000000 blendr_cli-0.1.2/blendr/gpu_manager/detect.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 06:44:49.183581 blendr_cli-0.1.2/blendr/task_manager/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        0 2024-04-29 22:27:33.000000 blendr_cli-0.1.2/blendr/task_manager/__init__.py
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     2245 2024-04-29 20:05:25.000000 blendr_cli-0.1.2/blendr/task_manager/listen.py
+drwxr-xr-x   0 stefanshiloh   (501) staff       (20)        0 2024-04-30 06:44:49.184632 blendr_cli-0.1.2/blendr_cli.egg-info/
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)     3079 2024-04-30 06:44:49.000000 blendr_cli-0.1.2/blendr_cli.egg-info/PKG-INFO
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      506 2024-04-30 06:44:49.000000 blendr_cli-0.1.2/blendr_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        1 2024-04-30 06:44:49.000000 blendr_cli-0.1.2/blendr_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)       43 2024-04-30 06:44:49.000000 blendr_cli-0.1.2/blendr_cli.egg-info/entry_points.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)       46 2024-04-30 06:44:49.000000 blendr_cli-0.1.2/blendr_cli.egg-info/requires.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)        7 2024-04-30 06:44:49.000000 blendr_cli-0.1.2/blendr_cli.egg-info/top_level.txt
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)       38 2024-04-30 06:44:49.185125 blendr_cli-0.1.2/setup.cfg
+-rw-r--r--   0 stefanshiloh   (501) staff       (20)      797 2024-04-30 06:44:43.000000 blendr_cli-0.1.2/setup.py
```

### Comparing `blendr_cli-0.1.1/PKG-INFO` & `blendr_cli-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: blendr-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: Blendr CLI tool for GPU Lending
 Home-page: https://www.blendr.network
 Author: Blendr Network
 Author-email: tech@blendr.network
 License: MIT
 Keywords: blendr cli
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: requests
 Requires-Dist: colorama
+Requires-Dist: GPUtil
+Requires-Dist: psutil
+Requires-Dist: keyring
 
 # Blendr CLI
 
 Blendr CLI is a command-line interface designed to help users lend their GPU resources for computational tasks on the Blendr platform. This tool allows for easy setup, management, and monitoring of GPU resources from your terminal.
 
 ## Features
```

### Comparing `blendr_cli-0.1.1/README.md` & `blendr_cli-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `blendr_cli-0.1.1/blendr/auth/authenticate.py` & `blendr_cli-0.1.2/blendr/auth/authenticate.py`

 * *Files identical despite different names*

### Comparing `blendr_cli-0.1.1/blendr/cli.py` & `blendr_cli-0.1.2/blendr/cli.py`

 * *Files identical despite different names*

### Comparing `blendr_cli-0.1.1/blendr/config/setup.py` & `blendr_cli-0.1.2/blendr/config/setup.py`

 * *Files identical despite different names*

### Comparing `blendr_cli-0.1.1/blendr_cli.egg-info/PKG-INFO` & `blendr_cli-0.1.2/blendr_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: blendr-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: Blendr CLI tool for GPU Lending
 Home-page: https://www.blendr.network
 Author: Blendr Network
 Author-email: tech@blendr.network
 License: MIT
 Keywords: blendr cli
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: requests
 Requires-Dist: colorama
+Requires-Dist: GPUtil
+Requires-Dist: psutil
+Requires-Dist: keyring
 
 # Blendr CLI
 
 Blendr CLI is a command-line interface designed to help users lend their GPU resources for computational tasks on the Blendr platform. This tool allows for easy setup, management, and monitoring of GPU resources from your terminal.
 
 ## Features
```

