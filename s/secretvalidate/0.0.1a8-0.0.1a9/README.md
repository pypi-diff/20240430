# Comparing `tmp/secretvalidate-0.0.1a8.tar.gz` & `tmp/secretvalidate-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretvalidate-0.0.1a8.tar", last modified: Mon Apr 29 12:34:40 2024, max compression
+gzip compressed data, was "secretvalidate-0.0.1a9.tar", last modified: Mon Apr 29 12:59:12 2024, max compression
```

## Comparing `secretvalidate-0.0.1a8.tar` & `secretvalidate-0.0.1a9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 12:34:40.739029 secretvalidate-0.0.1a8/
--rw-rw-rw-   0        0        0     1092 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a8/LICENSE
--rw-rw-rw-   0        0        0      335 2024-04-29 12:34:40.734025 secretvalidate-0.0.1a8/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 12:34:40.586027 secretvalidate-0.0.1a8/cli/
--rw-rw-rw-   0        0        0        0 2024-04-25 18:40:45.000000 secretvalidate-0.0.1a8/cli/__init__.py
--rw-rw-rw-   0        0        0       52 2024-04-29 11:11:39.000000 secretvalidate-0.0.1a8/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 12:34:40.633026 secretvalidate-0.0.1a8/secretvalidate/
--rw-rw-rw-   0        0        0        0 2024-04-25 18:40:40.000000 secretvalidate-0.0.1a8/secretvalidate/__init__.py
--rw-rw-rw-   0        0        0     2181 2024-04-29 12:02:56.000000 secretvalidate-0.0.1a8/secretvalidate/validator.py
-drwxrwxrwx   0        0        0        0 2024-04-29 12:34:40.731026 secretvalidate-0.0.1a8/secretvalidate.egg-info/
--rw-rw-rw-   0        0        0      335 2024-04-29 12:34:39.000000 secretvalidate-0.0.1a8/secretvalidate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2024-04-29 12:34:40.000000 secretvalidate-0.0.1a8/secretvalidate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 12:34:39.000000 secretvalidate-0.0.1a8/secretvalidate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-29 12:34:39.000000 secretvalidate-0.0.1a8/secretvalidate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       48 2024-04-29 12:34:39.000000 secretvalidate-0.0.1a8/secretvalidate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-29 12:34:39.000000 secretvalidate-0.0.1a8/secretvalidate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 12:34:40.740023 secretvalidate-0.0.1a8/setup.cfg
--rw-rw-rw-   0        0        0      856 2024-04-29 12:34:28.000000 secretvalidate-0.0.1a8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 12:34:40.725025 secretvalidate-0.0.1a8/tests/
--rw-rw-rw-   0        0        0        0 2024-04-25 05:52:05.000000 secretvalidate-0.0.1a8/tests/test_cli.py
--rw-rw-rw-   0        0        0        0 2024-04-25 05:51:51.000000 secretvalidate-0.0.1a8/tests/test_validator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:59:12.850352 secretvalidate-0.0.1a9/
+-rw-rw-rw-   0        0        0     1092 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a9/LICENSE
+-rw-rw-rw-   0        0        0      335 2024-04-29 12:59:12.834352 secretvalidate-0.0.1a9/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-04-25 05:46:51.000000 secretvalidate-0.0.1a9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 12:59:12.635359 secretvalidate-0.0.1a9/cli/
+-rw-rw-rw-   0        0        0        0 2024-04-25 18:40:45.000000 secretvalidate-0.0.1a9/cli/__init__.py
+-rw-rw-rw-   0        0        0       52 2024-04-29 11:11:39.000000 secretvalidate-0.0.1a9/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 12:59:12.672356 secretvalidate-0.0.1a9/secretvalidate/
+-rw-rw-rw-   0        0        0        0 2024-04-25 18:40:40.000000 secretvalidate-0.0.1a9/secretvalidate/__init__.py
+-rw-rw-rw-   0        0        0     2181 2024-04-29 12:02:56.000000 secretvalidate-0.0.1a9/secretvalidate/validator.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:59:12.830352 secretvalidate-0.0.1a9/secretvalidate.egg-info/
+-rw-rw-rw-   0        0        0      335 2024-04-29 12:59:12.000000 secretvalidate-0.0.1a9/secretvalidate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2024-04-29 12:59:12.000000 secretvalidate-0.0.1a9/secretvalidate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 12:59:12.000000 secretvalidate-0.0.1a9/secretvalidate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-04-29 12:59:12.000000 secretvalidate-0.0.1a9/secretvalidate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2024-04-29 12:59:12.000000 secretvalidate-0.0.1a9/secretvalidate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-29 12:59:12.000000 secretvalidate-0.0.1a9/secretvalidate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 12:59:12.850352 secretvalidate-0.0.1a9/setup.cfg
+-rw-rw-rw-   0        0        0      855 2024-04-29 12:59:05.000000 secretvalidate-0.0.1a9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:59:12.817353 secretvalidate-0.0.1a9/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-25 05:52:05.000000 secretvalidate-0.0.1a9/tests/test_cli.py
+-rw-rw-rw-   0        0        0        0 2024-04-25 05:51:51.000000 secretvalidate-0.0.1a9/tests/test_validator.py
```

### Comparing `secretvalidate-0.0.1a8/LICENSE` & `secretvalidate-0.0.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `secretvalidate-0.0.1a8/secretvalidate/validator.py` & `secretvalidate-0.0.1a9/secretvalidate/validator.py`

 * *Files identical despite different names*

### Comparing `secretvalidate-0.0.1a8/setup.py` & `secretvalidate-0.0.1a9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 # Read requirements from requirements.txt
 with open(requirements_path, 'r') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='secretvalidate',
-    version='0.0.1a8',
+    version='0.0.1a9',
     description='A tool for validating secrets.',
     author='VigneshKna',
     author_email='Vkna@email.com',
     license='MIT',
     packages=find_packages(),
     include_package_data=True,
     package_data={
         '': ['*.txt', '../requirements.txt'],
     },
     install_requires=requirements,
     entry_points={
         'console_scripts': [
-            'secretvalidate=secretvalidate.validator:validator',
+            'secretvalidate=secretvalidate.validator:validate',
         ],
     },
 )
```

