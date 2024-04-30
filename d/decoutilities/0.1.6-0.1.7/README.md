# Comparing `tmp/decoutilities-0.1.6.tar.gz` & `tmp/decoutilities-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.1.6.tar", last modified: Mon Apr 29 10:58:47 2024, max compression
+gzip compressed data, was "decoutilities-0.1.7.tar", last modified: Mon Apr 29 13:27:31 2024, max compression
```

## Comparing `decoutilities-0.1.6.tar` & `decoutilities-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 10:58:47.155481 decoutilities-0.1.6/
--rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     3116 2024-04-29 10:58:47.138488 decoutilities-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2645 2024-04-29 10:51:04.000000 decoutilities-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 10:58:46.938480 decoutilities-0.1.6/decoutilities/
--rw-rw-rw-   0        0        0      428 2024-04-29 10:52:56.000000 decoutilities-0.1.6/decoutilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:58:47.090484 decoutilities-0.1.6/decoutilities/config/
--rw-rw-rw-   0        0        0       76 2024-04-29 10:57:10.000000 decoutilities-0.1.6/decoutilities/config/__init__.py
--rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.1.6/decoutilities/config/config.py
--rw-rw-rw-   0        0        0     4322 2024-04-26 08:53:27.000000 decoutilities-0.1.6/decoutilities/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:58:47.122482 decoutilities-0.1.6/decoutilities.egg-info/
--rw-rw-rw-   0        0        0     3116 2024-04-29 10:58:46.000000 decoutilities-0.1.6/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-04-29 10:58:46.000000 decoutilities-0.1.6/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 10:58:46.000000 decoutilities-0.1.6/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-29 10:58:46.000000 decoutilities-0.1.6/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 10:58:47.156481 decoutilities-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-04-29 10:58:03.000000 decoutilities-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 13:27:31.191102 decoutilities-0.1.7/
+-rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     4767 2024-04-29 13:27:31.174105 decoutilities-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4296 2024-04-29 13:26:01.000000 decoutilities-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 13:27:30.941102 decoutilities-0.1.7/decoutilities/
+-rw-rw-rw-   0        0        0     1104 2024-04-29 13:11:45.000000 decoutilities-0.1.7/decoutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 13:27:31.084103 decoutilities-0.1.7/decoutilities/config/
+-rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.1.7/decoutilities/config/__init__.py
+-rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.1.7/decoutilities/config/config.py
+-rw-rw-rw-   0        0        0     4322 2024-04-26 08:53:27.000000 decoutilities-0.1.7/decoutilities/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-04-29 13:27:31.138101 decoutilities-0.1.7/decoutilities/inject/
+-rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.1.7/decoutilities/inject/__init__.py
+-rw-rw-rw-   0        0        0      483 2024-04-29 13:14:09.000000 decoutilities-0.1.7/decoutilities/inject/injector.py
+drwxrwxrwx   0        0        0        0 2024-04-29 13:27:31.157102 decoutilities-0.1.7/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0     4767 2024-04-29 13:27:30.000000 decoutilities-0.1.7/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2024-04-29 13:27:30.000000 decoutilities-0.1.7/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 13:27:30.000000 decoutilities-0.1.7/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-29 13:27:30.000000 decoutilities-0.1.7/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 13:27:31.194103 decoutilities-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-04-29 13:26:18.000000 decoutilities-0.1.7/setup.py
```

### Comparing `decoutilities-0.1.6/LICENSE` & `decoutilities-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.6/decoutilities/config/config.py` & `decoutilities-0.1.7/decoutilities/config/config.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.6/decoutilities/config/configContainer.py` & `decoutilities-0.1.7/decoutilities/config/configContainer.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.6/setup.py` & `decoutilities-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='decoutilities',
-version='0.1.6',
+version='0.1.7',
 author='Hugo Torres',
 author_email='contact@redactado.es',
 description='Enhance the readability of your code with decorators and simplify the creation of configuration files.',
 packages=find_packages(include=['decoutilities', 'decoutilities.*']),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

