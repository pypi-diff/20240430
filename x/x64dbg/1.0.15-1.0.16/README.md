# Comparing `tmp/x64dbg-1.0.15.tar.gz` & `tmp/x64dbg-1.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x64dbg-1.0.15.tar", last modified: Wed Apr 17 09:21:22 2024, max compression
+gzip compressed data, was "x64dbg-1.0.16.tar", last modified: Tue Apr 30 07:01:31 2024, max compression
```

## Comparing `x64dbg-1.0.15.tar` & `x64dbg-1.0.16.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 09:21:22.951877 x64dbg-1.0.15/
--r--r--r--   0        0        0    35613 2022-10-01 07:57:15.000000 x64dbg-1.0.15/LICENSE
--rw-rw-rw-   0        0        0      245 2024-04-17 09:21:22.909950 x64dbg-1.0.15/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-17 09:21:22.952853 x64dbg-1.0.15/setup.cfg
--rw-rw-rw-   0        0        0      392 2024-04-17 09:19:59.000000 x64dbg-1.0.15/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 09:21:22.613449 x64dbg-1.0.15/x64dbg/
--rw-rw-rw-   0        0        0    70956 2024-04-17 09:20:36.000000 x64dbg-1.0.15/x64dbg/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 09:21:22.869975 x64dbg-1.0.15/x64dbg.egg-info/
--rw-rw-rw-   0        0        0      245 2024-04-17 09:21:22.000000 x64dbg-1.0.15/x64dbg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      155 2024-04-17 09:21:22.000000 x64dbg-1.0.15/x64dbg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 09:21:22.000000 x64dbg-1.0.15/x64dbg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-17 09:21:22.000000 x64dbg-1.0.15/x64dbg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 07:01:31.281049 x64dbg-1.0.16/
+-r--r--r--   0        0        0    35613 2022-10-01 07:57:15.000000 x64dbg-1.0.16/LICENSE
+-rw-rw-rw-   0        0        0     1036 2024-04-30 07:01:31.219207 x64dbg-1.0.16/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2024-04-30 05:50:44.000000 x64dbg-1.0.16/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-30 07:01:31.281975 x64dbg-1.0.16/setup.cfg
+-rw-rw-rw-   0        0        0      992 2024-04-30 07:00:27.000000 x64dbg-1.0.16/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 07:01:30.902155 x64dbg-1.0.16/x64dbg/
+-rw-rw-rw-   0        0        0   199447 2024-04-30 06:59:47.000000 x64dbg-1.0.16/x64dbg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 07:01:31.176355 x64dbg-1.0.16/x64dbg.egg-info/
+-rw-rw-rw-   0        0        0     1036 2024-04-30 07:01:30.000000 x64dbg-1.0.16/x64dbg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      165 2024-04-30 07:01:30.000000 x64dbg-1.0.16/x64dbg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 07:01:30.000000 x64dbg-1.0.16/x64dbg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-30 07:01:30.000000 x64dbg-1.0.16/x64dbg.egg-info/top_level.txt
```

### Comparing `x64dbg-1.0.15/LICENSE` & `x64dbg-1.0.16/LICENSE`

 * *Files identical despite different names*

