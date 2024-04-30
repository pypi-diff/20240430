# Comparing `tmp/fast_tts-0.0.1.tar.gz` & `tmp/fast_tts-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_tts-0.0.1.tar", last modified: Tue Apr 30 19:22:14 2024, max compression
+gzip compressed data, was "fast_tts-0.0.2.tar", last modified: Tue Apr 30 19:49:09 2024, max compression
```

## Comparing `fast_tts-0.0.1.tar` & `fast_tts-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:22:14.991873 fast_tts-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-30 19:22:11.000000 fast_tts-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-30 19:22:14.991873 fast_tts-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 19:22:11.000000 fast_tts-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:22:14.991873 fast_tts-0.0.1/fast_tts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-30 19:22:14.000000 fast_tts-0.0.1/fast_tts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-30 19:22:14.000000 fast_tts-0.0.1/fast_tts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:22:14.000000 fast_tts-0.0.1/fast_tts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-30 19:22:14.000000 fast_tts-0.0.1/fast_tts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:22:14.000000 fast_tts-0.0.1/fast_tts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:22:14.991873 fast_tts-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-30 19:22:11.000000 fast_tts-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:49:09.120856 fast_tts-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-30 19:49:05.000000 fast_tts-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-30 19:49:09.120856 fast_tts-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-30 19:49:05.000000 fast_tts-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:49:09.120856 fast_tts-0.0.2/fast_tts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-30 19:49:09.000000 fast_tts-0.0.2/fast_tts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-30 19:49:09.000000 fast_tts-0.0.2/fast_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:49:09.000000 fast_tts-0.0.2/fast_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-30 19:49:09.000000 fast_tts-0.0.2/fast_tts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:49:09.000000 fast_tts-0.0.2/fast_tts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:49:09.120856 fast_tts-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-30 19:49:05.000000 fast_tts-0.0.2/setup.py
```

### Comparing `fast_tts-0.0.1/LICENSE` & `fast_tts-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_tts-0.0.1/setup.py` & `fast_tts-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     description = f.read()
 
 setup(
-    name='fast-tts',
-    version='0.0.1',
+    name='fast_tts',
+    version='0.0.2',
     long_description=description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'torch',
         'transformers',
```

