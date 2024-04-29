# Comparing `tmp/flexa-0.1.8.tar.gz` & `tmp/flexa-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexa-0.1.8.tar", last modified: Mon Apr 29 15:21:35 2024, max compression
+gzip compressed data, was "flexa-0.1.9.tar", last modified: Mon Apr 29 15:23:09 2024, max compression
```

## Comparing `flexa-0.1.8.tar` & `flexa-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 a.kano     (501) staff       (20)        0 2024-04-29 15:21:35.920631 flexa-0.1.8/
--rw-r--r--   0 a.kano     (501) staff       (20)       49 2024-04-29 15:21:35.920449 flexa-0.1.8/PKG-INFO
--rw-r--r--   0 a.kano     (501) staff       (20)      114 2024-04-29 14:45:31.000000 flexa-0.1.8/README.md
-drwxr-xr-x   0 a.kano     (501) staff       (20)        0 2024-04-29 15:21:35.919139 flexa-0.1.8/flexa/
--rw-r--r--   0 a.kano     (501) staff       (20)       25 2024-04-29 12:49:09.000000 flexa-0.1.8/flexa/__init__.py
--rw-r--r--   0 a.kano     (501) staff       (20)     1103 2024-04-29 14:38:39.000000 flexa-0.1.8/flexa/flexa.py
-drwxr-xr-x   0 a.kano     (501) staff       (20)        0 2024-04-29 15:21:35.920272 flexa-0.1.8/flexa.egg-info/
--rw-r--r--   0 a.kano     (501) staff       (20)       49 2024-04-29 15:21:35.000000 flexa-0.1.8/flexa.egg-info/PKG-INFO
--rw-r--r--   0 a.kano     (501) staff       (20)      187 2024-04-29 15:21:35.000000 flexa-0.1.8/flexa.egg-info/SOURCES.txt
--rw-r--r--   0 a.kano     (501) staff       (20)        1 2024-04-29 15:21:35.000000 flexa-0.1.8/flexa.egg-info/dependency_links.txt
--rw-r--r--   0 a.kano     (501) staff       (20)        6 2024-04-29 15:21:35.000000 flexa-0.1.8/flexa.egg-info/top_level.txt
--rw-r--r--   0 a.kano     (501) staff       (20)       38 2024-04-29 15:21:35.920670 flexa-0.1.8/setup.cfg
--rw-r--r--   0 a.kano     (501) staff       (20)      122 2024-04-29 15:21:26.000000 flexa-0.1.8/setup.py
-drwxr-xr-x   0 a.kano     (501) staff       (20)        0 2024-04-29 15:21:35.920012 flexa-0.1.8/tests/
--rw-r--r--   0 a.kano     (501) staff       (20)      812 2024-04-29 14:38:39.000000 flexa-0.1.8/tests/test_flexa.py
+drwxr-xr-x   0 a.kano     (501) staff       (20)        0 2024-04-29 15:23:09.558512 flexa-0.1.9/
+-rw-r--r--   0 a.kano     (501) staff       (20)       49 2024-04-29 15:23:09.558254 flexa-0.1.9/PKG-INFO
+-rw-r--r--   0 a.kano     (501) staff       (20)      114 2024-04-29 14:45:31.000000 flexa-0.1.9/README.md
+drwxr-xr-x   0 a.kano     (501) staff       (20)        0 2024-04-29 15:23:09.555113 flexa-0.1.9/flexa/
+-rw-r--r--   0 a.kano     (501) staff       (20)       25 2024-04-29 12:49:09.000000 flexa-0.1.9/flexa/__init__.py
+-rw-r--r--   0 a.kano     (501) staff       (20)     1103 2024-04-29 14:38:39.000000 flexa-0.1.9/flexa/flexa.py
+drwxr-xr-x   0 a.kano     (501) staff       (20)        0 2024-04-29 15:23:09.557956 flexa-0.1.9/flexa.egg-info/
+-rw-r--r--   0 a.kano     (501) staff       (20)       49 2024-04-29 15:23:09.000000 flexa-0.1.9/flexa.egg-info/PKG-INFO
+-rw-r--r--   0 a.kano     (501) staff       (20)      187 2024-04-29 15:23:09.000000 flexa-0.1.9/flexa.egg-info/SOURCES.txt
+-rw-r--r--   0 a.kano     (501) staff       (20)        1 2024-04-29 15:23:09.000000 flexa-0.1.9/flexa.egg-info/dependency_links.txt
+-rw-r--r--   0 a.kano     (501) staff       (20)        6 2024-04-29 15:23:09.000000 flexa-0.1.9/flexa.egg-info/top_level.txt
+-rw-r--r--   0 a.kano     (501) staff       (20)       38 2024-04-29 15:23:09.558552 flexa-0.1.9/setup.cfg
+-rw-r--r--   0 a.kano     (501) staff       (20)      122 2024-04-29 15:22:33.000000 flexa-0.1.9/setup.py
+drwxr-xr-x   0 a.kano     (501) staff       (20)        0 2024-04-29 15:23:09.556591 flexa-0.1.9/tests/
+-rw-r--r--   0 a.kano     (501) staff       (20)      812 2024-04-29 14:38:39.000000 flexa-0.1.9/tests/test_flexa.py
```

### Comparing `flexa-0.1.8/flexa/flexa.py` & `flexa-0.1.9/flexa/flexa.py`

 * *Files identical despite different names*

### Comparing `flexa-0.1.8/tests/test_flexa.py` & `flexa-0.1.9/tests/test_flexa.py`

 * *Files identical despite different names*

