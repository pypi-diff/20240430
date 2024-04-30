# Comparing `tmp/pylinweb-1.9.tar.gz` & `tmp/pylinweb-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylinweb-1.9.tar", last modified: Mon Apr 29 22:40:51 2024, max compression
+gzip compressed data, was "pylinweb-1.9.1.tar", last modified: Mon Apr 29 22:44:15 2024, max compression
```

## Comparing `pylinweb-1.9.tar` & `pylinweb-1.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 22:40:51.400781 pylinweb-1.9/
--rw-rw-rw-   0        0        0       34 2024-04-29 20:50:14.000000 pylinweb-1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2518 2024-04-29 22:40:51.398777 pylinweb-1.9/PKG-INFO
--rw-rw-rw-   0        0        0     1581 2024-04-26 00:01:05.000000 pylinweb-1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 22:40:51.363569 pylinweb-1.9/pylinweb/
--rw-rw-rw-   0        0        0       63 2024-04-29 20:52:26.000000 pylinweb-1.9/pylinweb/__init__.py
--rw-rw-rw-   0        0        0     3297 2024-04-29 20:49:24.000000 pylinweb-1.9/pylinweb/functions.py
--rw-rw-rw-   0        0        0     1544 2024-04-29 20:51:43.000000 pylinweb-1.9/pylinweb/main.py
--rw-rw-rw-   0        0        0      113 2024-04-29 22:39:55.000000 pylinweb-1.9/pylinweb/variables.py
-drwxrwxrwx   0        0        0        0 2024-04-29 22:40:51.396780 pylinweb-1.9/pylinweb.egg-info/
--rw-rw-rw-   0        0        0     2518 2024-04-29 22:40:51.000000 pylinweb-1.9/pylinweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-04-29 22:40:51.000000 pylinweb-1.9/pylinweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 22:40:51.000000 pylinweb-1.9/pylinweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-29 22:40:51.000000 pylinweb-1.9/pylinweb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      284 2024-04-29 22:40:51.000000 pylinweb-1.9/pylinweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-29 22:40:51.000000 pylinweb-1.9/pylinweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 22:40:51.400781 pylinweb-1.9/setup.cfg
--rw-rw-rw-   0        0        0     1473 2024-04-29 22:38:15.000000 pylinweb-1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 22:44:15.117095 pylinweb-1.9.1/
+-rw-rw-rw-   0        0        0       34 2024-04-29 20:50:14.000000 pylinweb-1.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2520 2024-04-29 22:44:15.115089 pylinweb-1.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1581 2024-04-26 00:01:05.000000 pylinweb-1.9.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 22:44:15.066332 pylinweb-1.9.1/pylinweb/
+-rw-rw-rw-   0        0        0       63 2024-04-29 20:52:26.000000 pylinweb-1.9.1/pylinweb/__init__.py
+-rw-rw-rw-   0        0        0     3297 2024-04-29 20:49:24.000000 pylinweb-1.9.1/pylinweb/functions.py
+-rw-rw-rw-   0        0        0     1544 2024-04-29 20:51:43.000000 pylinweb-1.9.1/pylinweb/main.py
+-rw-rw-rw-   0        0        0      115 2024-04-29 22:44:10.000000 pylinweb-1.9.1/pylinweb/variables.py
+drwxrwxrwx   0        0        0        0 2024-04-29 22:44:15.110516 pylinweb-1.9.1/pylinweb.egg-info/
+-rw-rw-rw-   0        0        0     2520 2024-04-29 22:44:14.000000 pylinweb-1.9.1/pylinweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-04-29 22:44:14.000000 pylinweb-1.9.1/pylinweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 22:44:14.000000 pylinweb-1.9.1/pylinweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-29 22:44:14.000000 pylinweb-1.9.1/pylinweb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      284 2024-04-29 22:44:14.000000 pylinweb-1.9.1/pylinweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-29 22:44:14.000000 pylinweb-1.9.1/pylinweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 22:44:15.118097 pylinweb-1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1460 2024-04-29 22:43:45.000000 pylinweb-1.9.1/setup.py
```

### Comparing `pylinweb-1.9/PKG-INFO` & `pylinweb-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pylinweb
-Version: 1.9
+Version: 1.9.1
 Summary: A simple functional test library using Python and Selenium
 Author: Linda Lopez
 Keywords: selenium,testing,web,chrome
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Requires-Dist: allure-behave==2.13.5
-Requires-Dist: allure-python-commons==2.13.4
+Requires-Dist: allure-python-commons==2.13.5
 Requires-Dist: behave==1.2.6
 Requires-Dist: behave-html-formatter==0.9.10
 Requires-Dist: behave2cucumber==1.0.3
 Requires-Dist: docxcompose==1.4.0
 Requires-Dist: docxtpl==0.16.8
 Requires-Dist: playwright==1.42.0
 Requires-Dist: psutil==5.9.2
```

### Comparing `pylinweb-1.9/README.md` & `pylinweb-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pylinweb-1.9/pylinweb/functions.py` & `pylinweb-1.9.1/pylinweb/functions.py`

 * *Files identical despite different names*

### Comparing `pylinweb-1.9/pylinweb/main.py` & `pylinweb-1.9.1/pylinweb/main.py`

 * *Files identical despite different names*

### Comparing `pylinweb-1.9/pylinweb.egg-info/PKG-INFO` & `pylinweb-1.9.1/pylinweb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pylinweb
-Version: 1.9
+Version: 1.9.1
 Summary: A simple functional test library using Python and Selenium
 Author: Linda Lopez
 Keywords: selenium,testing,web,chrome
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Requires-Dist: allure-behave==2.13.5
-Requires-Dist: allure-python-commons==2.13.4
+Requires-Dist: allure-python-commons==2.13.5
 Requires-Dist: behave==1.2.6
 Requires-Dist: behave-html-formatter==0.9.10
 Requires-Dist: behave2cucumber==1.0.3
 Requires-Dist: docxcompose==1.4.0
 Requires-Dist: docxtpl==0.16.8
 Requires-Dist: playwright==1.42.0
 Requires-Dist: psutil==5.9.2
```

### Comparing `pylinweb-1.9/setup.py` & `pylinweb-1.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     name='pylinweb',
     version= version,
     description='A simple functional test library using Python and Selenium',
     author='Linda Lopez',
     packages=find_packages(),
     include_package_data=True, #Esto hace que setuptools lea el archivo MANIFEST.in
     install_requires=[
-        "allure-behave==2.13.5", #actualizar!
-        "allure-python-commons==2.13.4",
+        "allure-behave==2.13.5",
+        "allure-python-commons==2.13.5",
         "behave==1.2.6",
         "behave-html-formatter==0.9.10",
         "behave2cucumber==1.0.3",
         "docxcompose==1.4.0",
         "docxtpl==0.16.8",
         "playwright==1.42.0",
         "psutil==5.9.2",
```

