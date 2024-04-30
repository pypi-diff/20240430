# Comparing `tmp/pypanasonic-0.0.2.tar.gz` & `tmp/pypanasonic-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypanasonic-0.0.2.tar", last modified: Tue Apr 30 14:19:16 2024, max compression
+gzip compressed data, was "pypanasonic-0.0.3.tar", last modified: Tue Apr 30 14:37:03 2024, max compression
```

## Comparing `pypanasonic-0.0.2.tar` & `pypanasonic-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 14:19:16.880830 pypanasonic-0.0.2/
--rw-rw-rw-   0        0        0     1083 2024-04-30 13:58:47.000000 pypanasonic-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      206 2024-04-30 14:05:37.000000 pypanasonic-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1749 2024-04-30 14:19:16.879830 pypanasonic-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      936 2024-04-30 13:56:36.000000 pypanasonic-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 14:19:16.879830 pypanasonic-0.0.2/pypanasonic.egg-info/
--rw-rw-rw-   0        0        0     1749 2024-04-30 14:19:16.000000 pypanasonic-0.0.2/pypanasonic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2024-04-30 14:19:16.000000 pypanasonic-0.0.2/pypanasonic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 14:19:16.000000 pypanasonic-0.0.2/pypanasonic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2024-04-30 14:19:16.000000 pypanasonic-0.0.2/pypanasonic.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2024-04-30 14:19:16.000000 pypanasonic-0.0.2/pypanasonic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 14:19:16.000000 pypanasonic-0.0.2/pypanasonic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1157 2024-04-30 14:18:00.000000 pypanasonic-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       81 2024-04-30 14:19:16.882831 pypanasonic-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      324 2024-04-30 14:04:03.000000 pypanasonic-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 14:37:03.962743 pypanasonic-0.0.3/
+-rw-rw-rw-   0        0        0     1083 2024-04-30 13:58:47.000000 pypanasonic-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      230 2024-04-30 14:36:01.000000 pypanasonic-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1749 2024-04-30 14:37:03.961744 pypanasonic-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      936 2024-04-30 13:56:36.000000 pypanasonic-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 14:37:03.960744 pypanasonic-0.0.3/pypanasonic.egg-info/
+-rw-rw-rw-   0        0        0     1749 2024-04-30 14:37:03.000000 pypanasonic-0.0.3/pypanasonic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2024-04-30 14:37:03.000000 pypanasonic-0.0.3/pypanasonic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 14:37:03.000000 pypanasonic-0.0.3/pypanasonic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-30 14:37:03.000000 pypanasonic-0.0.3/pypanasonic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 14:37:03.000000 pypanasonic-0.0.3/pypanasonic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1920 2024-04-30 13:46:19.000000 pypanasonic-0.0.3/pypanasonic.py
+-rw-rw-rw-   0        0        0      981 2024-04-30 14:35:27.000000 pypanasonic-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2024-04-30 14:37:03.970739 pypanasonic-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      324 2024-04-30 14:04:03.000000 pypanasonic-0.0.3/setup.py
```

### Comparing `pypanasonic-0.0.2/LICENSE` & `pypanasonic-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypanasonic-0.0.2/PKG-INFO` & `pypanasonic-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypanasonic
-Version: 0.0.2
+Version: 0.0.3
 Summary: Panasonic PLC mewtocol lib via serial port
 Author-email: Wei-zhao Lu <luweizhao09@gmail.com>, Hua lu <hualu0305@gmail.com>
 Maintainer-email: Wei-zhao lu <luweizhao09@gmail.com>
 Project-URL: Homepage, https://github.com/hy1stax/pypanasonic
 Project-URL: Documentation, https://github.com/hy1stax/pypanasonic/README.md
 Project-URL: Repository, https://github.com/hy1stax/pypanasonic.git
 Project-URL: Bug Tracker, https://github.com/hy1stax/pypanasonic/issues
```

### Comparing `pypanasonic-0.0.2/README.md` & `pypanasonic-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pypanasonic-0.0.2/pypanasonic.egg-info/PKG-INFO` & `pypanasonic-0.0.3/pypanasonic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypanasonic
-Version: 0.0.2
+Version: 0.0.3
 Summary: Panasonic PLC mewtocol lib via serial port
 Author-email: Wei-zhao Lu <luweizhao09@gmail.com>, Hua lu <hualu0305@gmail.com>
 Maintainer-email: Wei-zhao lu <luweizhao09@gmail.com>
 Project-URL: Homepage, https://github.com/hy1stax/pypanasonic
 Project-URL: Documentation, https://github.com/hy1stax/pypanasonic/README.md
 Project-URL: Repository, https://github.com/hy1stax/pypanasonic.git
 Project-URL: Bug Tracker, https://github.com/hy1stax/pypanasonic/issues
```

