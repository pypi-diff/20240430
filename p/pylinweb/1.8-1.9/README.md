# Comparing `tmp/pylinweb-1.8.tar.gz` & `tmp/pylinweb-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylinweb-1.8.tar", last modified: Mon Apr 29 22:04:59 2024, max compression
+gzip compressed data, was "pylinweb-1.9.tar", last modified: Mon Apr 29 22:40:51 2024, max compression
```

## Comparing `pylinweb-1.8.tar` & `pylinweb-1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 22:04:59.910918 pylinweb-1.8/
--rw-rw-rw-   0        0        0       34 2024-04-29 20:50:14.000000 pylinweb-1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2518 2024-04-29 22:04:59.909919 pylinweb-1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1581 2024-04-26 00:01:05.000000 pylinweb-1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 22:04:59.864294 pylinweb-1.8/pylinweb/
--rw-rw-rw-   0        0        0       63 2024-04-29 20:52:26.000000 pylinweb-1.8/pylinweb/__init__.py
--rw-rw-rw-   0        0        0     3297 2024-04-29 20:49:24.000000 pylinweb-1.8/pylinweb/functions.py
--rw-rw-rw-   0        0        0     1544 2024-04-29 20:51:43.000000 pylinweb-1.8/pylinweb/main.py
--rw-rw-rw-   0        0        0      113 2024-04-29 21:59:09.000000 pylinweb-1.8/pylinweb/variables.py
-drwxrwxrwx   0        0        0        0 2024-04-29 22:04:59.907928 pylinweb-1.8/pylinweb.egg-info/
--rw-rw-rw-   0        0        0     2518 2024-04-29 22:04:59.000000 pylinweb-1.8/pylinweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-04-29 22:04:59.000000 pylinweb-1.8/pylinweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 22:04:59.000000 pylinweb-1.8/pylinweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-29 22:04:59.000000 pylinweb-1.8/pylinweb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      284 2024-04-29 22:04:59.000000 pylinweb-1.8/pylinweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-29 22:04:59.000000 pylinweb-1.8/pylinweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 22:04:59.910918 pylinweb-1.8/setup.cfg
--rw-rw-rw-   0        0        0     1460 2024-04-29 21:35:21.000000 pylinweb-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 22:40:51.400781 pylinweb-1.9/
+-rw-rw-rw-   0        0        0       34 2024-04-29 20:50:14.000000 pylinweb-1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2518 2024-04-29 22:40:51.398777 pylinweb-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1581 2024-04-26 00:01:05.000000 pylinweb-1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 22:40:51.363569 pylinweb-1.9/pylinweb/
+-rw-rw-rw-   0        0        0       63 2024-04-29 20:52:26.000000 pylinweb-1.9/pylinweb/__init__.py
+-rw-rw-rw-   0        0        0     3297 2024-04-29 20:49:24.000000 pylinweb-1.9/pylinweb/functions.py
+-rw-rw-rw-   0        0        0     1544 2024-04-29 20:51:43.000000 pylinweb-1.9/pylinweb/main.py
+-rw-rw-rw-   0        0        0      113 2024-04-29 22:39:55.000000 pylinweb-1.9/pylinweb/variables.py
+drwxrwxrwx   0        0        0        0 2024-04-29 22:40:51.396780 pylinweb-1.9/pylinweb.egg-info/
+-rw-rw-rw-   0        0        0     2518 2024-04-29 22:40:51.000000 pylinweb-1.9/pylinweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-04-29 22:40:51.000000 pylinweb-1.9/pylinweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 22:40:51.000000 pylinweb-1.9/pylinweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-29 22:40:51.000000 pylinweb-1.9/pylinweb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      284 2024-04-29 22:40:51.000000 pylinweb-1.9/pylinweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-29 22:40:51.000000 pylinweb-1.9/pylinweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 22:40:51.400781 pylinweb-1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1473 2024-04-29 22:38:15.000000 pylinweb-1.9/setup.py
```

### Comparing `pylinweb-1.8/PKG-INFO` & `pylinweb-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pylinweb
-Version: 1.8
+Version: 1.9
 Summary: A simple functional test library using Python and Selenium
 Author: Linda Lopez
 Keywords: selenium,testing,web,chrome
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
-Requires-Dist: allure-behave==2.13.4
+Requires-Dist: allure-behave==2.13.5
 Requires-Dist: allure-python-commons==2.13.4
 Requires-Dist: behave==1.2.6
 Requires-Dist: behave-html-formatter==0.9.10
 Requires-Dist: behave2cucumber==1.0.3
 Requires-Dist: docxcompose==1.4.0
 Requires-Dist: docxtpl==0.16.8
 Requires-Dist: playwright==1.42.0
```

### Comparing `pylinweb-1.8/README.md` & `pylinweb-1.9/README.md`

 * *Files identical despite different names*

### Comparing `pylinweb-1.8/pylinweb/functions.py` & `pylinweb-1.9/pylinweb/functions.py`

 * *Files identical despite different names*

### Comparing `pylinweb-1.8/pylinweb/main.py` & `pylinweb-1.9/pylinweb/main.py`

 * *Files identical despite different names*

### Comparing `pylinweb-1.8/pylinweb.egg-info/PKG-INFO` & `pylinweb-1.9/pylinweb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pylinweb
-Version: 1.8
+Version: 1.9
 Summary: A simple functional test library using Python and Selenium
 Author: Linda Lopez
 Keywords: selenium,testing,web,chrome
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
-Requires-Dist: allure-behave==2.13.4
+Requires-Dist: allure-behave==2.13.5
 Requires-Dist: allure-python-commons==2.13.4
 Requires-Dist: behave==1.2.6
 Requires-Dist: behave-html-formatter==0.9.10
 Requires-Dist: behave2cucumber==1.0.3
 Requires-Dist: docxcompose==1.4.0
 Requires-Dist: docxtpl==0.16.8
 Requires-Dist: playwright==1.42.0
```

### Comparing `pylinweb-1.8/setup.py` & `pylinweb-1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     name='pylinweb',
     version= version,
     description='A simple functional test library using Python and Selenium',
     author='Linda Lopez',
     packages=find_packages(),
     include_package_data=True, #Esto hace que setuptools lea el archivo MANIFEST.in
     install_requires=[
-        "allure-behave==2.13.4",
+        "allure-behave==2.13.5", #actualizar!
         "allure-python-commons==2.13.4",
         "behave==1.2.6",
         "behave-html-formatter==0.9.10",
         "behave2cucumber==1.0.3",
         "docxcompose==1.4.0",
         "docxtpl==0.16.8",
         "playwright==1.42.0",
```

