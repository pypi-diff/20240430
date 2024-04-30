# Comparing `tmp/repo2text-0.1.0.tar.gz` & `tmp/repo2text-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo2text-0.1.0.tar", last modified: Tue Apr 30 06:15:12 2024, max compression
+gzip compressed data, was "repo2text-0.1.1.tar", last modified: Tue Apr 30 06:35:45 2024, max compression
```

## Comparing `repo2text-0.1.0.tar` & `repo2text-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 yash       (501) staff       (20)        0 2024-04-30 06:15:12.882317 repo2text-0.1.0/
--rw-r--r--   0 yash       (501) staff       (20)     1066 2024-04-30 06:14:34.000000 repo2text-0.1.0/LICENSE
--rw-r--r--   0 yash       (501) staff       (20)     1893 2024-04-30 06:15:12.882119 repo2text-0.1.0/PKG-INFO
--rw-r--r--   0 yash       (501) staff       (20)     1410 2024-04-30 06:14:34.000000 repo2text-0.1.0/README.md
-drwxr-xr-x   0 yash       (501) staff       (20)        0 2024-04-30 06:15:12.880927 repo2text-0.1.0/repo2text/
--rw-r--r--   0 yash       (501) staff       (20)        0 2024-04-30 06:14:34.000000 repo2text-0.1.0/repo2text/__init__.py
--rw-r--r--   0 yash       (501) staff       (20)     2251 2024-04-30 06:14:34.000000 repo2text-0.1.0/repo2text/repo2text.py
-drwxr-xr-x   0 yash       (501) staff       (20)        0 2024-04-30 06:15:12.881848 repo2text-0.1.0/repo2text.egg-info/
--rw-r--r--   0 yash       (501) staff       (20)     1893 2024-04-30 06:15:12.000000 repo2text-0.1.0/repo2text.egg-info/PKG-INFO
--rw-r--r--   0 yash       (501) staff       (20)      271 2024-04-30 06:15:12.000000 repo2text-0.1.0/repo2text.egg-info/SOURCES.txt
--rw-r--r--   0 yash       (501) staff       (20)        1 2024-04-30 06:15:12.000000 repo2text-0.1.0/repo2text.egg-info/dependency_links.txt
--rw-r--r--   0 yash       (501) staff       (20)       55 2024-04-30 06:15:12.000000 repo2text-0.1.0/repo2text.egg-info/entry_points.txt
--rw-r--r--   0 yash       (501) staff       (20)       17 2024-04-30 06:15:12.000000 repo2text-0.1.0/repo2text.egg-info/requires.txt
--rw-r--r--   0 yash       (501) staff       (20)       10 2024-04-30 06:15:12.000000 repo2text-0.1.0/repo2text.egg-info/top_level.txt
--rw-r--r--   0 yash       (501) staff       (20)       38 2024-04-30 06:15:12.882364 repo2text-0.1.0/setup.cfg
--rw-r--r--   0 yash       (501) staff       (20)      778 2024-04-30 06:14:34.000000 repo2text-0.1.0/setup.py
+drwxr-xr-x   0 yash       (501) staff       (20)        0 2024-04-30 06:35:45.121051 repo2text-0.1.1/
+-rw-r--r--   0 yash       (501) staff       (20)     1066 2024-04-30 06:14:34.000000 repo2text-0.1.1/LICENSE
+-rw-r--r--   0 yash       (501) staff       (20)     1893 2024-04-30 06:35:45.120850 repo2text-0.1.1/PKG-INFO
+-rw-r--r--   0 yash       (501) staff       (20)     1410 2024-04-30 06:14:34.000000 repo2text-0.1.1/README.md
+drwxr-xr-x   0 yash       (501) staff       (20)        0 2024-04-30 06:35:45.119608 repo2text-0.1.1/repo2text/
+-rw-r--r--   0 yash       (501) staff       (20)        0 2024-04-30 06:14:34.000000 repo2text-0.1.1/repo2text/__init__.py
+-rw-r--r--   0 yash       (501) staff       (20)     2242 2024-04-30 06:30:03.000000 repo2text-0.1.1/repo2text/repo2text.py
+drwxr-xr-x   0 yash       (501) staff       (20)        0 2024-04-30 06:35:45.120604 repo2text-0.1.1/repo2text.egg-info/
+-rw-r--r--   0 yash       (501) staff       (20)     1893 2024-04-30 06:35:45.000000 repo2text-0.1.1/repo2text.egg-info/PKG-INFO
+-rw-r--r--   0 yash       (501) staff       (20)      271 2024-04-30 06:35:45.000000 repo2text-0.1.1/repo2text.egg-info/SOURCES.txt
+-rw-r--r--   0 yash       (501) staff       (20)        1 2024-04-30 06:35:45.000000 repo2text-0.1.1/repo2text.egg-info/dependency_links.txt
+-rw-r--r--   0 yash       (501) staff       (20)       55 2024-04-30 06:35:45.000000 repo2text-0.1.1/repo2text.egg-info/entry_points.txt
+-rw-r--r--   0 yash       (501) staff       (20)       17 2024-04-30 06:35:45.000000 repo2text-0.1.1/repo2text.egg-info/requires.txt
+-rw-r--r--   0 yash       (501) staff       (20)       10 2024-04-30 06:35:45.000000 repo2text-0.1.1/repo2text.egg-info/top_level.txt
+-rw-r--r--   0 yash       (501) staff       (20)       38 2024-04-30 06:35:45.121102 repo2text-0.1.1/setup.cfg
+-rw-r--r--   0 yash       (501) staff       (20)      778 2024-04-30 06:34:40.000000 repo2text-0.1.1/setup.py
```

### Comparing `repo2text-0.1.0/LICENSE` & `repo2text-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `repo2text-0.1.0/PKG-INFO` & `repo2text-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo2text
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple utility to convert repository files to text including specific file extensions
 Home-page: https://github.com/YashJain14/repo2text
 Author: Yash Jain
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `repo2text-0.1.0/README.md` & `repo2text-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `repo2text-0.1.0/repo2text/repo2text.py` & `repo2text-0.1.1/repo2text/repo2text.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 def main():
     if len(sys.argv) < 2:
         print("Usage: python script.py [<extension>] <git url>")
         sys.exit(1)
     # Determine if the first argument is a URL or an extension
     if sys.argv[1].startswith('.'):
         if len(sys.argv) != 3:
-            print("Usage: python script.py [<extension>] <git url>")
+            print("Usage: repo2text <extension> <git url>")
             sys.exit(1)
         extension = sys.argv[1].strip('.').lower()
         repo_url = sys.argv[2]
     else:
         repo_url = sys.argv[1]
         extension = None
         if len(sys.argv) == 3:
```

### Comparing `repo2text-0.1.0/repo2text.egg-info/PKG-INFO` & `repo2text-0.1.1/repo2text.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo2text
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple utility to convert repository files to text including specific file extensions
 Home-page: https://github.com/YashJain14/repo2text
 Author: Yash Jain
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `repo2text-0.1.0/setup.py` & `repo2text-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='repo2text',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'repo2text=repo2text.repo2text:main',
         ],
     },
     author='Yash Jain',
```

