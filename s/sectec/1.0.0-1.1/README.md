# Comparing `tmp/sectec-1.0.0.tar.gz` & `tmp/sectec-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sectec-1.0.0.tar", last modified: Tue Apr 30 20:17:39 2024, max compression
+gzip compressed data, was "sectec-1.1.tar", last modified: Tue Apr 30 20:34:19 2024, max compression
```

## Comparing `sectec-1.0.0.tar` & `sectec-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 20:17:39.955684 sectec-1.0.0/
--rw-rw-rw-   0        0        0     1376 2024-04-30 20:17:39.952685 sectec-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-30 20:17:39.888720 sectec-1.0.0/sectec/
--rw-rw-rw-   0        0        0       80 2024-04-30 19:33:26.000000 sectec-1.0.0/sectec/__init__.py
--rw-rw-rw-   0        0        0     1546 2024-04-30 18:40:49.000000 sectec-1.0.0/sectec/main.py
-drwxrwxrwx   0        0        0        0 2024-04-30 20:17:39.945733 sectec-1.0.0/sectec.egg-info/
--rw-rw-rw-   0        0        0     1376 2024-04-30 20:17:39.000000 sectec-1.0.0/sectec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2024-04-30 20:17:39.000000 sectec-1.0.0/sectec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 20:17:39.000000 sectec-1.0.0/sectec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-04-30 20:17:39.000000 sectec-1.0.0/sectec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-30 20:17:39.000000 sectec-1.0.0/sectec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 20:17:39.955684 sectec-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      463 2024-04-30 20:17:10.000000 sectec-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 20:34:19.943045 sectec-1.1/
+-rw-rw-rw-   0        0        0     1374 2024-04-30 20:34:19.936048 sectec-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 20:34:19.839104 sectec-1.1/sectec/
+-rw-rw-rw-   0        0        0      108 2024-04-30 20:22:28.000000 sectec-1.1/sectec/__init__.py
+-rw-rw-rw-   0        0        0     1233 2024-04-30 20:19:43.000000 sectec-1.1/sectec/main.py
+drwxrwxrwx   0        0        0        0 2024-04-30 20:34:19.921057 sectec-1.1/sectec.egg-info/
+-rw-rw-rw-   0        0        0     1374 2024-04-30 20:34:19.000000 sectec-1.1/sectec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2024-04-30 20:34:19.000000 sectec-1.1/sectec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 20:34:19.000000 sectec-1.1/sectec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-04-30 20:34:19.000000 sectec-1.1/sectec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-30 20:34:19.000000 sectec-1.1/sectec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 20:34:19.944049 sectec-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      461 2024-04-30 20:21:17.000000 sectec-1.1/setup.py
```

### Comparing `sectec-1.0.0/PKG-INFO` & `sectec-1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sectec
-Version: 1.0.0
+Version: 1.1
 Summary: Easy to use Webscraper module for python
 Author: Ali Lodhi
 Author-email: alilodhibusiness@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: requests==2.31.0
 Requires-Dist: bs4==0.0.2
```

### Comparing `sectec-1.0.0/sectec.egg-info/PKG-INFO` & `sectec-1.1/sectec.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sectec
-Version: 1.0.0
+Version: 1.1
 Summary: Easy to use Webscraper module for python
 Author: Ali Lodhi
 Author-email: alilodhibusiness@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: requests==2.31.0
 Requires-Dist: bs4==0.0.2
```

