# Comparing `tmp/pylinweb-1.6.tar.gz` & `tmp/pylinweb-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylinweb-1.6.tar", last modified: Mon Apr 29 20:52:43 2024, max compression
+gzip compressed data, was "pylinweb-1.7.tar", last modified: Mon Apr 29 21:14:37 2024, max compression
```

## Comparing `pylinweb-1.6.tar` & `pylinweb-1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 20:52:43.111726 pylinweb-1.6/
--rw-rw-rw-   0        0        0       34 2024-04-29 20:50:14.000000 pylinweb-1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2053 2024-04-29 20:52:43.110603 pylinweb-1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1581 2024-04-26 00:01:05.000000 pylinweb-1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 20:52:43.049863 pylinweb-1.6/pylinweb/
--rw-rw-rw-   0        0        0       63 2024-04-29 20:52:26.000000 pylinweb-1.6/pylinweb/__init__.py
--rw-rw-rw-   0        0        0     3297 2024-04-29 20:49:24.000000 pylinweb-1.6/pylinweb/functions.py
--rw-rw-rw-   0        0        0     1544 2024-04-29 20:51:43.000000 pylinweb-1.6/pylinweb/main.py
--rw-rw-rw-   0        0        0      115 2024-04-29 20:45:38.000000 pylinweb-1.6/pylinweb/variables.py
-drwxrwxrwx   0        0        0        0 2024-04-29 20:52:43.108815 pylinweb-1.6/pylinweb.egg-info/
--rw-rw-rw-   0        0        0     2053 2024-04-29 20:52:42.000000 pylinweb-1.6/pylinweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-04-29 20:52:42.000000 pylinweb-1.6/pylinweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 20:52:42.000000 pylinweb-1.6/pylinweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-29 20:52:42.000000 pylinweb-1.6/pylinweb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      334 2024-04-29 20:52:42.000000 pylinweb-1.6/pylinweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-29 20:52:42.000000 pylinweb-1.6/pylinweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 20:52:43.112301 pylinweb-1.6/setup.cfg
--rw-rw-rw-   0        0        0     1575 2024-04-29 20:52:40.000000 pylinweb-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 21:14:37.633606 pylinweb-1.7/
+-rw-rw-rw-   0        0        0       34 2024-04-29 20:50:14.000000 pylinweb-1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2053 2024-04-29 21:14:37.633606 pylinweb-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1581 2024-04-26 00:01:05.000000 pylinweb-1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 21:14:37.592510 pylinweb-1.7/pylinweb/
+-rw-rw-rw-   0        0        0       63 2024-04-29 20:52:26.000000 pylinweb-1.7/pylinweb/__init__.py
+-rw-rw-rw-   0        0        0     3297 2024-04-29 20:49:24.000000 pylinweb-1.7/pylinweb/functions.py
+-rw-rw-rw-   0        0        0     1544 2024-04-29 20:51:43.000000 pylinweb-1.7/pylinweb/main.py
+-rw-rw-rw-   0        0        0      113 2024-04-29 21:13:39.000000 pylinweb-1.7/pylinweb/variables.py
+drwxrwxrwx   0        0        0        0 2024-04-29 21:14:37.631054 pylinweb-1.7/pylinweb.egg-info/
+-rw-rw-rw-   0        0        0     2053 2024-04-29 21:14:37.000000 pylinweb-1.7/pylinweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-04-29 21:14:37.000000 pylinweb-1.7/pylinweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 21:14:37.000000 pylinweb-1.7/pylinweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-29 21:14:37.000000 pylinweb-1.7/pylinweb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      334 2024-04-29 21:14:37.000000 pylinweb-1.7/pylinweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-29 21:14:37.000000 pylinweb-1.7/pylinweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 21:14:37.633606 pylinweb-1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1534 2024-04-29 21:13:20.000000 pylinweb-1.7/setup.py
```

### Comparing `pylinweb-1.6/PKG-INFO` & `pylinweb-1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylinweb
-Version: 1.6
+Version: 1.7
 Summary: A simple functional test library using Python and Selenium
 Home-page: UNKNOWN
 Author: Linda Lopez
 License: UNKNOWN
 Keywords: selenium,testing,web,chrome
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pylinweb-1.6/README.md` & `pylinweb-1.7/README.md`

 * *Files identical despite different names*

### Comparing `pylinweb-1.6/pylinweb/functions.py` & `pylinweb-1.7/pylinweb/functions.py`

 * *Files identical despite different names*

### Comparing `pylinweb-1.6/pylinweb/main.py` & `pylinweb-1.7/pylinweb/main.py`

 * *Files identical despite different names*

### Comparing `pylinweb-1.6/pylinweb.egg-info/PKG-INFO` & `pylinweb-1.7/pylinweb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylinweb
-Version: 1.6
+Version: 1.7
 Summary: A simple functional test library using Python and Selenium
 Home-page: UNKNOWN
 Author: Linda Lopez
 License: UNKNOWN
 Keywords: selenium,testing,web,chrome
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pylinweb-1.6/setup.py` & `pylinweb-1.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         "docxtpl==0.16.8",
         "playwright==1.42.0",
         "psutil==5.9.2",
         "PyPDF2==3.0.1",
         "python-docx==1.1.0",
         "pycparser==2.21",
         "screeninfo==0.8",
-        "selenium==4.12", #TODO cambiar version para mobile!! 4.12
+        "selenium==4.12",
         "webdriver-manager==4.0.1",
         "webdrivermanager==0.10.0",
         "keyboard==0.13.5"
     ],
     entry_points={
         'console_scripts': [
             'pylinweb=pylinweb.main:main',
```

