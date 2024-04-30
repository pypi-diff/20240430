# Comparing `tmp/sigmoid_check-0.0.4.tar.gz` & `tmp/sigmoid_check-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmoid_check-0.0.4.tar", last modified: Wed Apr 24 20:26:33 2024, max compression
+gzip compressed data, was "sigmoid_check-0.0.5.tar", last modified: Tue Apr 30 12:27:42 2024, max compression
```

## Comparing `sigmoid_check-0.0.4.tar` & `sigmoid_check-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 20:26:33.163908 sigmoid_check-0.0.4/
--rw-rw-rw-   0        0        0    11538 2024-04-23 18:15:46.000000 sigmoid_check-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2756 2024-04-24 20:26:33.162901 sigmoid_check-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1881 2024-04-23 18:29:06.000000 sigmoid_check-0.0.4/README.md
--rw-rw-rw-   0        0        0       86 2024-04-24 20:26:33.169908 sigmoid_check-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1104 2024-04-24 18:55:15.000000 sigmoid_check-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 20:26:33.142791 sigmoid_check-0.0.4/sigmoid_check/
--rw-rw-rw-   0        0        0        0 2024-04-23 19:00:37.000000 sigmoid_check-0.0.4/sigmoid_check/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 20:26:33.153396 sigmoid_check-0.0.4/sigmoid_check/python_odyssey/
--rw-rw-rw-   0        0        0       84 2024-04-24 19:44:04.000000 sigmoid_check-0.0.4/sigmoid_check/python_odyssey/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 20:26:33.156397 sigmoid_check-0.0.4/sigmoid_check/python_odyssey/lesson_10/
--rw-rw-rw-   0        0        0        0 2024-04-24 19:44:19.000000 sigmoid_check-0.0.4/sigmoid_check/python_odyssey/lesson_10/__init__.py
--rw-rw-rw-   0        0        0    22558 2024-04-23 20:44:39.000000 sigmoid_check-0.0.4/sigmoid_check/python_odyssey/lesson_10/lesson_10.py
-drwxrwxrwx   0        0        0        0 2024-04-24 20:26:33.159398 sigmoid_check-0.0.4/sigmoid_check/python_odyssey/lesson_11/
--rw-rw-rw-   0        0        0        0 2024-04-24 19:44:19.000000 sigmoid_check-0.0.4/sigmoid_check/python_odyssey/lesson_11/__init__.py
--rw-rw-rw-   0        0        0    41222 2024-04-24 20:20:21.000000 sigmoid_check-0.0.4/sigmoid_check/python_odyssey/lesson_11/lesson_11.py
-drwxrwxrwx   0        0        0        0 2024-04-24 20:26:33.161395 sigmoid_check-0.0.4/sigmoid_check.egg-info/
--rw-rw-rw-   0        0        0     2756 2024-04-24 20:26:33.000000 sigmoid_check-0.0.4/sigmoid_check.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2024-04-24 20:26:33.000000 sigmoid_check-0.0.4/sigmoid_check.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 20:26:33.000000 sigmoid_check-0.0.4/sigmoid_check.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-24 20:26:33.000000 sigmoid_check-0.0.4/sigmoid_check.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 12:27:42.309676 sigmoid_check-0.0.5/
+-rw-rw-rw-   0        0        0    11538 2024-04-23 18:15:46.000000 sigmoid_check-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2756 2024-04-30 12:27:42.308674 sigmoid_check-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1881 2024-04-23 18:29:06.000000 sigmoid_check-0.0.5/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-30 12:27:42.316201 sigmoid_check-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1104 2024-04-29 12:54:57.000000 sigmoid_check-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 12:27:42.277739 sigmoid_check-0.0.5/sigmoid_check/
+-rw-rw-rw-   0        0        0        0 2024-04-23 19:00:37.000000 sigmoid_check-0.0.5/sigmoid_check/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 12:27:42.294368 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/
+-rw-rw-rw-   0        0        0       84 2024-04-24 19:44:04.000000 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 12:27:42.298630 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_10/
+-rw-rw-rw-   0        0        0        0 2024-04-24 19:44:19.000000 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_10/__init__.py
+-rw-rw-rw-   0        0        0    22558 2024-04-23 20:44:39.000000 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_10/lesson_10.py
+drwxrwxrwx   0        0        0        0 2024-04-30 12:27:42.300658 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_11/
+-rw-rw-rw-   0        0        0        0 2024-04-24 19:44:19.000000 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_11/__init__.py
+-rw-rw-rw-   0        0        0    41222 2024-04-24 20:20:21.000000 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_11/lesson_11.py
+drwxrwxrwx   0        0        0        0 2024-04-30 12:27:42.303653 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_13/
+-rw-rw-rw-   0        0        0        0 2024-04-29 12:54:48.000000 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_13/__init__.py
+-rw-rw-rw-   0        0        0    21468 2024-04-30 12:20:28.000000 sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_13/lesson_13.py
+drwxrwxrwx   0        0        0        0 2024-04-30 12:27:42.306170 sigmoid_check-0.0.5/sigmoid_check.egg-info/
+-rw-rw-rw-   0        0        0     2756 2024-04-30 12:27:42.000000 sigmoid_check-0.0.5/sigmoid_check.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      560 2024-04-30 12:27:42.000000 sigmoid_check-0.0.5/sigmoid_check.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 12:27:42.000000 sigmoid_check-0.0.5/sigmoid_check.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-30 12:27:42.000000 sigmoid_check-0.0.5/sigmoid_check.egg-info/top_level.txt
```

### Comparing `sigmoid_check-0.0.4/LICENSE` & `sigmoid_check-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmoid_check-0.0.4/PKG-INFO` & `sigmoid_check-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmoid_check
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for checking the implementation of tasks in Sigmoid Courses
 Author: SigmoidAI - Balamatiuc Eduard
 Author-email: balamatiuc2@gmail.com
 License: Apache License 2.0
 Keywords: tasks,check,sigmoid,sigmoidai,sigmoid_check
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sigmoid_check-0.0.4/README.md` & `sigmoid_check-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sigmoid_check-0.0.4/setup.py` & `sigmoid_check-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="sigmoid_check",
-    version="0.0.4",
+    version="0.0.5",
     packages=find_packages(),
     description="A package for checking the implementation of tasks in Sigmoid Courses",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="SigmoidAI - Balamatiuc Eduard",
     author_email="balamatiuc2@gmail.com",
     keywords=["tasks", "check", "sigmoid", "sigmoidai", "sigmoid_check"],
```

### Comparing `sigmoid_check-0.0.4/sigmoid_check/python_odyssey/lesson_10/lesson_10.py` & `sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_10/lesson_10.py`

 * *Files identical despite different names*

### Comparing `sigmoid_check-0.0.4/sigmoid_check/python_odyssey/lesson_11/lesson_11.py` & `sigmoid_check-0.0.5/sigmoid_check/python_odyssey/lesson_11/lesson_11.py`

 * *Files identical despite different names*

### Comparing `sigmoid_check-0.0.4/sigmoid_check.egg-info/PKG-INFO` & `sigmoid_check-0.0.5/sigmoid_check.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmoid_check
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for checking the implementation of tasks in Sigmoid Courses
 Author: SigmoidAI - Balamatiuc Eduard
 Author-email: balamatiuc2@gmail.com
 License: Apache License 2.0
 Keywords: tasks,check,sigmoid,sigmoidai,sigmoid_check
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

