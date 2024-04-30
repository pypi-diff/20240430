# Comparing `tmp/runseq-0.1.1.tar.gz` & `tmp/runseq-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runseq-0.1.1.tar", last modified: Wed Apr 24 22:28:15 2024, max compression
+gzip compressed data, was "runseq-0.2.0.tar", last modified: Tue Apr 30 15:54:45 2024, max compression
```

## Comparing `runseq-0.1.1.tar` & `runseq-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-04-24 22:28:15.574017 runseq-0.1.1/
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)    35149 2024-04-23 13:58:13.000000 runseq-0.1.1/LICENSE
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)    43112 2024-04-24 22:28:15.574017 runseq-0.1.1/PKG-INFO
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)     2241 2024-04-23 15:48:32.000000 runseq-0.1.1/README.md
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)      469 2024-04-24 22:26:03.000000 runseq-0.1.1/pyproject.toml
-drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-04-24 22:28:15.574017 runseq-0.1.1/runseq.egg-info/
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)    43112 2024-04-24 22:28:15.000000 runseq-0.1.1/runseq.egg-info/PKG-INFO
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)      216 2024-04-24 22:28:15.000000 runseq-0.1.1/runseq.egg-info/SOURCES.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)        1 2024-04-24 22:28:15.000000 runseq-0.1.1/runseq.egg-info/dependency_links.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)       39 2024-04-24 22:28:15.000000 runseq-0.1.1/runseq.egg-info/entry_points.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)        7 2024-04-24 22:28:15.000000 runseq-0.1.1/runseq.egg-info/top_level.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)     4356 2024-04-24 22:25:19.000000 runseq-0.1.1/runseq.py
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)       38 2024-04-24 22:28:15.574017 runseq-0.1.1/setup.cfg
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)       38 2024-04-23 15:30:44.000000 runseq-0.1.1/setup.py
+drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-04-30 15:54:45.482674 runseq-0.2.0/
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)    35149 2024-04-23 13:58:13.000000 runseq-0.2.0/LICENSE
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)    43112 2024-04-30 15:54:45.482674 runseq-0.2.0/PKG-INFO
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)     2241 2024-04-23 15:48:32.000000 runseq-0.2.0/README.md
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)      469 2024-04-30 15:47:28.000000 runseq-0.2.0/pyproject.toml
+drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-04-30 15:54:45.482674 runseq-0.2.0/runseq.egg-info/
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)    43112 2024-04-30 15:54:45.000000 runseq-0.2.0/runseq.egg-info/PKG-INFO
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)      216 2024-04-30 15:54:45.000000 runseq-0.2.0/runseq.egg-info/SOURCES.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)        1 2024-04-30 15:54:45.000000 runseq-0.2.0/runseq.egg-info/dependency_links.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)       39 2024-04-30 15:54:45.000000 runseq-0.2.0/runseq.egg-info/entry_points.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)        7 2024-04-30 15:54:45.000000 runseq-0.2.0/runseq.egg-info/top_level.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)     5782 2024-04-30 15:52:35.000000 runseq-0.2.0/runseq.py
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)       38 2024-04-30 15:54:45.482674 runseq-0.2.0/setup.cfg
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)       38 2024-04-23 15:30:44.000000 runseq-0.2.0/setup.py
```

### Comparing `runseq-0.1.1/LICENSE` & `runseq-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runseq-0.1.1/PKG-INFO` & `runseq-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runseq
-Version: 0.1.1
+Version: 0.2.0
 Summary: Simple job manager to run jobs sequentially in a Linux machine.
 Author-email: Luís Gomes <luismsgomes@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `runseq-0.1.1/README.md` & `runseq-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `runseq-0.1.1/runseq.egg-info/PKG-INFO` & `runseq-0.2.0/runseq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runseq
-Version: 0.1.1
+Version: 0.2.0
 Summary: Simple job manager to run jobs sequentially in a Linux machine.
 Author-email: Luís Gomes <luismsgomes@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

