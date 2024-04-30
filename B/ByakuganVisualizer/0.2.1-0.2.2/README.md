# Comparing `tmp/ByakuganVisualizer-0.2.1.tar.gz` & `tmp/ByakuganVisualizer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ByakuganVisualizer-0.2.1.tar", last modified: Wed Apr  3 21:29:55 2024, max compression
+gzip compressed data, was "ByakuganVisualizer-0.2.2.tar", last modified: Tue Apr 30 09:52:41 2024, max compression
```

## Comparing `ByakuganVisualizer-0.2.1.tar` & `ByakuganVisualizer-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:29:55.476952 ByakuganVisualizer-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-03 21:29:55.476952 ByakuganVisualizer-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-03 21:29:47.000000 ByakuganVisualizer-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-03 21:29:55.476952 ByakuganVisualizer-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-03 21:29:47.000000 ByakuganVisualizer-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:29:55.472952 ByakuganVisualizer-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:29:55.476952 ByakuganVisualizer-0.2.1/src/ByakuganVisualizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-03 21:29:55.000000 ByakuganVisualizer-0.2.1/src/ByakuganVisualizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-03 21:29:55.000000 ByakuganVisualizer-0.2.1/src/ByakuganVisualizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:29:55.000000 ByakuganVisualizer-0.2.1/src/ByakuganVisualizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 21:29:55.000000 ByakuganVisualizer-0.2.1/src/ByakuganVisualizer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:29:55.000000 ByakuganVisualizer-0.2.1/src/ByakuganVisualizer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 21:29:55.000000 ByakuganVisualizer-0.2.1/src/ByakuganVisualizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 21:29:55.000000 ByakuganVisualizer-0.2.1/src/ByakuganVisualizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:29:55.476952 ByakuganVisualizer-0.2.1/src/byakuganvisualizer/
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-03 21:29:47.000000 ByakuganVisualizer-0.2.1/src/byakuganvisualizer/Byakugan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-03 21:29:47.000000 ByakuganVisualizer-0.2.1/src/byakuganvisualizer/ImageFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-03 21:29:47.000000 ByakuganVisualizer-0.2.1/src/byakuganvisualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-03 21:29:47.000000 ByakuganVisualizer-0.2.1/src/byakuganvisualizer/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:52:41.489042 ByakuganVisualizer-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-04-30 09:52:41.489042 ByakuganVisualizer-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-30 09:52:31.000000 ByakuganVisualizer-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-30 09:52:41.489042 ByakuganVisualizer-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-30 09:52:31.000000 ByakuganVisualizer-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:52:41.485042 ByakuganVisualizer-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:52:41.485042 ByakuganVisualizer-0.2.2/src/ByakuganVisualizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-04-30 09:52:41.000000 ByakuganVisualizer-0.2.2/src/ByakuganVisualizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-30 09:52:41.000000 ByakuganVisualizer-0.2.2/src/ByakuganVisualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:52:41.000000 ByakuganVisualizer-0.2.2/src/ByakuganVisualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-30 09:52:41.000000 ByakuganVisualizer-0.2.2/src/ByakuganVisualizer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:52:41.000000 ByakuganVisualizer-0.2.2/src/ByakuganVisualizer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-30 09:52:41.000000 ByakuganVisualizer-0.2.2/src/ByakuganVisualizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-30 09:52:41.000000 ByakuganVisualizer-0.2.2/src/ByakuganVisualizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:52:41.485042 ByakuganVisualizer-0.2.2/src/byakuganvisualizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-30 09:52:31.000000 ByakuganVisualizer-0.2.2/src/byakuganvisualizer/Byakugan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-30 09:52:31.000000 ByakuganVisualizer-0.2.2/src/byakuganvisualizer/ImageFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-30 09:52:31.000000 ByakuganVisualizer-0.2.2/src/byakuganvisualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-30 09:52:31.000000 ByakuganVisualizer-0.2.2/src/byakuganvisualizer/main.py
```

### Comparing `ByakuganVisualizer-0.2.1/PKG-INFO` & `ByakuganVisualizer-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ByakuganVisualizer
-Version: 0.2.1
+Version: 0.2.2
 Summary: The ByakuganVisualizer repository hosts a Python tool designed to compare images and highlight their differences. It simplifies the process of identifying disparities between images, making it ideal for tasks like testing and quality assurance. Additionally, it offers options for customization, which can be helpful for color-blind users.
-Home-page: https://github.com/pyscaffold/pyscaffold/
+Home-page: https://github.com/HokageM/ByakuganVisualizer
 Author: HokageM
 Author-email: m.trzaska663@gmail.com
 License: MIT
-Project-URL: Documentation, https://pyscaffold.org/
+Project-URL: README, https://github.com/HokageM/ByakuganVisualizer/blob/main/README.md
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 
 # ByakuganVisualizer
```

### Comparing `ByakuganVisualizer-0.2.1/README.md` & `ByakuganVisualizer-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ByakuganVisualizer-0.2.1/setup.py` & `ByakuganVisualizer-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 if __name__ == "__main__":
     try:
         setup(description="The ByakuganVisualizer repository hosts a Python tool designed to compare images and "
                           "highlight their differences. It simplifies the process of identifying disparities between "
                           "images, making it ideal for tasks like testing and quality assurance. Additionally, it "
                           "offers options for customization, which can be helpful for color-blind users.",
               long_description_content_type="text/markdown",
-              version="0.2.1"
+              version="0.2.2"
               )
     except:  # noqa
         print(
             "\n\nAn error occurred while building the project, "
             "please ensure you have the most updated version of setuptools, "
             "setuptools_scm and wheel with:\n"
             "   pip install -U setup tools setuptools_scm wheel\n\n"
```

### Comparing `ByakuganVisualizer-0.2.1/src/ByakuganVisualizer.egg-info/PKG-INFO` & `ByakuganVisualizer-0.2.2/src/ByakuganVisualizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ByakuganVisualizer
-Version: 0.2.1
+Version: 0.2.2
 Summary: The ByakuganVisualizer repository hosts a Python tool designed to compare images and highlight their differences. It simplifies the process of identifying disparities between images, making it ideal for tasks like testing and quality assurance. Additionally, it offers options for customization, which can be helpful for color-blind users.
-Home-page: https://github.com/pyscaffold/pyscaffold/
+Home-page: https://github.com/HokageM/ByakuganVisualizer
 Author: HokageM
 Author-email: m.trzaska663@gmail.com
 License: MIT
-Project-URL: Documentation, https://pyscaffold.org/
+Project-URL: README, https://github.com/HokageM/ByakuganVisualizer/blob/main/README.md
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 
 # ByakuganVisualizer
```

### Comparing `ByakuganVisualizer-0.2.1/src/byakuganvisualizer/Byakugan.py` & `ByakuganVisualizer-0.2.2/src/byakuganvisualizer/Byakugan.py`

 * *Files identical despite different names*

### Comparing `ByakuganVisualizer-0.2.1/src/byakuganvisualizer/ImageFilter.py` & `ByakuganVisualizer-0.2.2/src/byakuganvisualizer/ImageFilter.py`

 * *Files identical despite different names*

### Comparing `ByakuganVisualizer-0.2.1/src/byakuganvisualizer/__init__.py` & `ByakuganVisualizer-0.2.2/src/byakuganvisualizer/__init__.py`

 * *Files identical despite different names*

### Comparing `ByakuganVisualizer-0.2.1/src/byakuganvisualizer/main.py` & `ByakuganVisualizer-0.2.2/src/byakuganvisualizer/main.py`

 * *Files identical despite different names*

