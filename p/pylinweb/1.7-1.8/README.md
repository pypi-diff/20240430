# Comparing `tmp/pylinweb-1.7.tar.gz` & `tmp/pylinweb-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylinweb-1.7.tar", last modified: Mon Apr 29 21:14:37 2024, max compression
+gzip compressed data, was "pylinweb-1.8.tar", last modified: Mon Apr 29 22:04:59 2024, max compression
```

## Comparing `pylinweb-1.7.tar` & `pylinweb-1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 21:14:37.633606 pylinweb-1.7/
--rw-rw-rw-   0        0        0       34 2024-04-29 20:50:14.000000 pylinweb-1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2053 2024-04-29 21:14:37.633606 pylinweb-1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1581 2024-04-26 00:01:05.000000 pylinweb-1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 21:14:37.592510 pylinweb-1.7/pylinweb/
--rw-rw-rw-   0        0        0       63 2024-04-29 20:52:26.000000 pylinweb-1.7/pylinweb/__init__.py
--rw-rw-rw-   0        0        0     3297 2024-04-29 20:49:24.000000 pylinweb-1.7/pylinweb/functions.py
--rw-rw-rw-   0        0        0     1544 2024-04-29 20:51:43.000000 pylinweb-1.7/pylinweb/main.py
--rw-rw-rw-   0        0        0      113 2024-04-29 21:13:39.000000 pylinweb-1.7/pylinweb/variables.py
-drwxrwxrwx   0        0        0        0 2024-04-29 21:14:37.631054 pylinweb-1.7/pylinweb.egg-info/
--rw-rw-rw-   0        0        0     2053 2024-04-29 21:14:37.000000 pylinweb-1.7/pylinweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-04-29 21:14:37.000000 pylinweb-1.7/pylinweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 21:14:37.000000 pylinweb-1.7/pylinweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-29 21:14:37.000000 pylinweb-1.7/pylinweb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      334 2024-04-29 21:14:37.000000 pylinweb-1.7/pylinweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-29 21:14:37.000000 pylinweb-1.7/pylinweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 21:14:37.633606 pylinweb-1.7/setup.cfg
--rw-rw-rw-   0        0        0     1534 2024-04-29 21:13:20.000000 pylinweb-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 22:04:59.910918 pylinweb-1.8/
+-rw-rw-rw-   0        0        0       34 2024-04-29 20:50:14.000000 pylinweb-1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2518 2024-04-29 22:04:59.909919 pylinweb-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1581 2024-04-26 00:01:05.000000 pylinweb-1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 22:04:59.864294 pylinweb-1.8/pylinweb/
+-rw-rw-rw-   0        0        0       63 2024-04-29 20:52:26.000000 pylinweb-1.8/pylinweb/__init__.py
+-rw-rw-rw-   0        0        0     3297 2024-04-29 20:49:24.000000 pylinweb-1.8/pylinweb/functions.py
+-rw-rw-rw-   0        0        0     1544 2024-04-29 20:51:43.000000 pylinweb-1.8/pylinweb/main.py
+-rw-rw-rw-   0        0        0      113 2024-04-29 21:59:09.000000 pylinweb-1.8/pylinweb/variables.py
+drwxrwxrwx   0        0        0        0 2024-04-29 22:04:59.907928 pylinweb-1.8/pylinweb.egg-info/
+-rw-rw-rw-   0        0        0     2518 2024-04-29 22:04:59.000000 pylinweb-1.8/pylinweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-04-29 22:04:59.000000 pylinweb-1.8/pylinweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 22:04:59.000000 pylinweb-1.8/pylinweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-29 22:04:59.000000 pylinweb-1.8/pylinweb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      284 2024-04-29 22:04:59.000000 pylinweb-1.8/pylinweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-29 22:04:59.000000 pylinweb-1.8/pylinweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 22:04:59.910918 pylinweb-1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1460 2024-04-29 21:35:21.000000 pylinweb-1.8/setup.py
```

### Comparing `pylinweb-1.7/PKG-INFO` & `pylinweb-1.8/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pylinweb
-Version: 1.7
-Summary: A simple functional test library using Python and Selenium
-Home-page: UNKNOWN
-Author: Linda Lopez
-License: UNKNOWN
-Keywords: selenium,testing,web,chrome
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown
-
 # Pylinweb
 
 Pylinweb es una biblioteca de pruebas funcionales simple que utiliza Python, Selenium y Chrome driver.
 
 ## Pre-requisitos
 
 Antes de instalar Pylinweb, asegúrate de tener instalado lo siguiente:
@@ -69,9 +54,8 @@
 ```
 Y para generar un informe, puedes usar:
 
 ```bash
 pylinweb --report
 ```
 
-Reemplaza version con la versión específica de Pylinweb que deseas instalar.
-
+Reemplaza version con la versión específica de Pylinweb que deseas instalar.
```

### Comparing `pylinweb-1.7/pylinweb/functions.py` & `pylinweb-1.8/pylinweb/functions.py`

 * *Files identical despite different names*

### Comparing `pylinweb-1.7/pylinweb/main.py` & `pylinweb-1.8/pylinweb/main.py`

 * *Files identical despite different names*

### Comparing `pylinweb-1.7/setup.py` & `pylinweb-1.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,16 +23,14 @@
         "playwright==1.42.0",
         "psutil==5.9.2",
         "PyPDF2==3.0.1",
         "python-docx==1.1.0",
         "pycparser==2.21",
         "screeninfo==0.8",
         "selenium==4.12",
-        "webdriver-manager==4.0.1",
-        "webdrivermanager==0.10.0",
         "keyboard==0.13.5"
     ],
     entry_points={
         'console_scripts': [
             'pylinweb=pylinweb.main:main',
         ],
     },
```

