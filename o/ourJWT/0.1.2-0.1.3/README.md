# Comparing `tmp/ourJWT-0.1.2.tar.gz` & `tmp/ourJWT-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourJWT-0.1.2.tar", last modified: Thu Apr 18 13:09:02 2024, max compression
+gzip compressed data, was "ourJWT-0.1.3.tar", last modified: Tue Apr 30 12:59:49 2024, max compression
```

## Comparing `ourJWT-0.1.2.tar` & `ourJWT-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-18 13:09:02.197737 ourJWT-0.1.2/
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      258 2024-04-18 13:09:02.197737 ourJWT-0.1.2/PKG-INFO
-drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-18 13:09:02.197737 ourJWT-0.1.2/ourJWT/
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)     3404 2024-04-16 13:56:23.000000 ourJWT-0.1.2/ourJWT/OUR_class.py
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      374 2024-04-16 08:08:01.000000 ourJWT-0.1.2/ourJWT/OUR_exception.py
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      153 2024-04-16 08:08:01.000000 ourJWT-0.1.2/ourJWT/__init__.py
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      859 2024-04-18 13:07:16.000000 ourJWT-0.1.2/ourJWT/decorators.py
-drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-18 13:09:02.197737 ourJWT-0.1.2/ourJWT.egg-info/
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      258 2024-04-18 13:09:02.000000 ourJWT-0.1.2/ourJWT.egg-info/PKG-INFO
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      241 2024-04-18 13:09:02.000000 ourJWT-0.1.2/ourJWT.egg-info/SOURCES.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)        1 2024-04-18 13:09:02.000000 ourJWT-0.1.2/ourJWT.egg-info/dependency_links.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      134 2024-04-18 13:09:02.000000 ourJWT-0.1.2/ourJWT.egg-info/requires.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)        7 2024-04-18 13:09:02.000000 ourJWT-0.1.2/ourJWT.egg-info/top_level.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)       38 2024-04-18 13:09:02.197737 ourJWT-0.1.2/setup.cfg
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      599 2024-04-18 13:07:59.000000 ourJWT-0.1.2/setup.py
+drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-30 12:59:49.093378 ourJWT-0.1.3/
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      258 2024-04-30 12:59:49.093378 ourJWT-0.1.3/PKG-INFO
+drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-30 12:59:49.093378 ourJWT-0.1.3/ourJWT/
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)     3404 2024-04-16 13:56:23.000000 ourJWT-0.1.3/ourJWT/OUR_class.py
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      374 2024-04-16 08:08:01.000000 ourJWT-0.1.3/ourJWT/OUR_exception.py
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      153 2024-04-16 08:08:01.000000 ourJWT-0.1.3/ourJWT/__init__.py
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      859 2024-04-18 13:07:16.000000 ourJWT-0.1.3/ourJWT/decorators.py
+drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-30 12:59:49.093378 ourJWT-0.1.3/ourJWT.egg-info/
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      258 2024-04-30 12:59:49.000000 ourJWT-0.1.3/ourJWT.egg-info/PKG-INFO
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      241 2024-04-30 12:59:49.000000 ourJWT-0.1.3/ourJWT.egg-info/SOURCES.txt
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)        1 2024-04-30 12:59:49.000000 ourJWT-0.1.3/ourJWT.egg-info/dependency_links.txt
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      134 2024-04-30 12:59:49.000000 ourJWT-0.1.3/ourJWT.egg-info/requires.txt
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)        7 2024-04-30 12:59:49.000000 ourJWT-0.1.3/ourJWT.egg-info/top_level.txt
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)       38 2024-04-30 12:59:49.093378 ourJWT-0.1.3/setup.cfg
+-rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      599 2024-04-30 12:59:42.000000 ourJWT-0.1.3/setup.py
```

### Comparing `ourJWT-0.1.2/ourJWT/OUR_class.py` & `ourJWT-0.1.3/ourJWT/OUR_class.py`

 * *Files identical despite different names*

### Comparing `ourJWT-0.1.2/ourJWT/decorators.py` & `ourJWT-0.1.3/ourJWT/decorators.py`

 * *Files identical despite different names*

