# Comparing `tmp/qfpy-6.0.2.tar.gz` & `tmp/qfpy-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfpy-6.0.2.tar", last modified: Mon Apr 29 16:56:09 2024, max compression
+gzip compressed data, was "qfpy-7.0.0.tar", last modified: Mon Apr 29 17:02:35 2024, max compression
```

## Comparing `qfpy-6.0.2.tar` & `qfpy-7.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 16:56:09.856638 qfpy-6.0.2/
--rw-rw-rw-   0        0        0      159 2024-04-29 16:56:09.853712 qfpy-6.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-29 16:55:56.000000 qfpy-6.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 16:56:09.856638 qfpy-6.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 16:56:09.827781 qfpy-6.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 16:56:09.843403 qfpy-6.0.2/src/qfpy/
--rw-rw-rw-   0        0        0       70 2024-04-29 16:54:46.000000 qfpy-6.0.2/src/qfpy/__init__.py
--rw-rw-rw-   0        0        0      210 2024-04-29 16:48:36.000000 qfpy-6.0.2/src/qfpy/character.py
--rw-rw-rw-   0        0        0     1528 2024-04-29 16:50:05.000000 qfpy-6.0.2/src/qfpy/exif.py
--rw-rw-rw-   0        0        0     3067 2024-04-29 16:52:59.000000 qfpy-6.0.2/src/qfpy/ffmpeg.py
--rw-rw-rw-   0        0        0      700 2024-04-29 16:53:48.000000 qfpy-6.0.2/src/qfpy/folder.py
--rw-rw-rw-   0        0        0      881 2024-04-29 16:55:19.000000 qfpy-6.0.2/src/qfpy/function.py
--rw-rw-rw-   0        0        0      854 2024-04-29 16:55:44.000000 qfpy-6.0.2/src/qfpy/process.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:56:09.852735 qfpy-6.0.2/src/qfpy.egg-info/
--rw-rw-rw-   0        0        0      159 2024-04-29 16:56:09.000000 qfpy-6.0.2/src/qfpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-04-29 16:56:09.000000 qfpy-6.0.2/src/qfpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 16:56:09.000000 qfpy-6.0.2/src/qfpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-29 16:56:09.000000 qfpy-6.0.2/src/qfpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 17:02:35.722128 qfpy-7.0.0/
+-rw-rw-rw-   0        0        0      159 2024-04-29 17:02:35.721150 qfpy-7.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-29 17:02:17.000000 qfpy-7.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 17:02:35.722128 qfpy-7.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 17:02:35.691856 qfpy-7.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 17:02:35.712364 qfpy-7.0.0/src/qfpy/
+-rw-rw-rw-   0        0        0       80 2024-04-29 17:01:22.000000 qfpy-7.0.0/src/qfpy/__init__.py
+-rw-rw-rw-   0        0        0      210 2024-04-29 16:48:36.000000 qfpy-7.0.0/src/qfpy/character.py
+-rw-rw-rw-   0        0        0      131 2024-04-29 17:01:55.000000 qfpy-7.0.0/src/qfpy/crypto.py
+-rw-rw-rw-   0        0        0     1528 2024-04-29 16:50:05.000000 qfpy-7.0.0/src/qfpy/exif.py
+-rw-rw-rw-   0        0        0     3067 2024-04-29 16:52:59.000000 qfpy-7.0.0/src/qfpy/ffmpeg.py
+-rw-rw-rw-   0        0        0      700 2024-04-29 16:53:48.000000 qfpy-7.0.0/src/qfpy/folder.py
+-rw-rw-rw-   0        0        0      881 2024-04-29 16:55:19.000000 qfpy-7.0.0/src/qfpy/function.py
+-rw-rw-rw-   0        0        0      854 2024-04-29 16:55:44.000000 qfpy-7.0.0/src/qfpy/process.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:02:35.720174 qfpy-7.0.0/src/qfpy.egg-info/
+-rw-rw-rw-   0        0        0      159 2024-04-29 17:02:35.000000 qfpy-7.0.0/src/qfpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2024-04-29 17:02:35.000000 qfpy-7.0.0/src/qfpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 17:02:35.000000 qfpy-7.0.0/src/qfpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-29 17:02:35.000000 qfpy-7.0.0/src/qfpy.egg-info/top_level.txt
```

### Comparing `qfpy-6.0.2/src/qfpy/exif.py` & `qfpy-7.0.0/src/qfpy/exif.py`

 * *Files identical despite different names*

### Comparing `qfpy-6.0.2/src/qfpy/ffmpeg.py` & `qfpy-7.0.0/src/qfpy/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `qfpy-6.0.2/src/qfpy/folder.py` & `qfpy-7.0.0/src/qfpy/folder.py`

 * *Files identical despite different names*

### Comparing `qfpy-6.0.2/src/qfpy/function.py` & `qfpy-7.0.0/src/qfpy/function.py`

 * *Files identical despite different names*

### Comparing `qfpy-6.0.2/src/qfpy/process.py` & `qfpy-7.0.0/src/qfpy/process.py`

 * *Files identical despite different names*

