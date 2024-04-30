# Comparing `tmp/openseneca-0.0.1.tar.gz` & `tmp/openseneca-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openseneca-0.0.1.tar", last modified: Tue Apr 30 14:22:24 2024, max compression
+gzip compressed data, was "openseneca-0.0.2.tar", last modified: Tue Apr 30 14:39:48 2024, max compression
```

## Comparing `openseneca-0.0.1.tar` & `openseneca-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,38 @@
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:22:24.336330 openseneca-0.0.1/
--rw-r--r--   0 otto       (501) staff       (20)      161 2024-04-30 14:22:24.336119 openseneca-0.0.1/PKG-INFO
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:22:24.334447 openseneca-0.0.1/openseneca/
--rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 10:06:53.000000 openseneca-0.0.1/openseneca/__init__.py
--rw-r--r--   0 otto       (501) staff       (20)     1289 2024-04-30 14:12:45.000000 openseneca-0.0.1/openseneca/costs.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:22:24.335765 openseneca-0.0.1/openseneca/models/
--rw-r--r--   0 otto       (501) staff       (20)      612 2024-04-30 10:06:53.000000 openseneca-0.0.1/openseneca/models/__init__.py
--rw-r--r--   0 otto       (501) staff       (20)     1900 2024-04-30 10:06:53.000000 openseneca-0.0.1/openseneca/models/cohere.py
--rw-r--r--   0 otto       (501) staff       (20)      983 2024-04-30 10:06:53.000000 openseneca-0.0.1/openseneca/models/gpt3.py
--rw-r--r--   0 otto       (501) staff       (20)      974 2024-04-30 10:06:53.000000 openseneca-0.0.1/openseneca/models/gpt4.py
--rw-r--r--   0 otto       (501) staff       (20)     3134 2024-04-30 10:06:53.000000 openseneca-0.0.1/openseneca/models/llama2.py
--rw-r--r--   0 otto       (501) staff       (20)     2160 2024-04-30 10:06:53.000000 openseneca-0.0.1/openseneca/models/llama3.py
--rw-r--r--   0 otto       (501) staff       (20)     1034 2024-04-30 10:06:53.000000 openseneca-0.0.1/openseneca/models/mistral.py
--rw-r--r--   0 otto       (501) staff       (20)     4976 2024-04-30 14:11:38.000000 openseneca-0.0.1/openseneca/router.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:22:24.335925 openseneca-0.0.1/openseneca.egg-info/
--rw-r--r--   0 otto       (501) staff       (20)      161 2024-04-30 14:22:24.000000 openseneca-0.0.1/openseneca.egg-info/PKG-INFO
--rw-r--r--   0 otto       (501) staff       (20)      403 2024-04-30 14:22:24.000000 openseneca-0.0.1/openseneca.egg-info/SOURCES.txt
--rw-r--r--   0 otto       (501) staff       (20)        1 2024-04-30 14:22:24.000000 openseneca-0.0.1/openseneca.egg-info/dependency_links.txt
--rw-r--r--   0 otto       (501) staff       (20)       11 2024-04-30 14:22:24.000000 openseneca-0.0.1/openseneca.egg-info/top_level.txt
--rw-r--r--   0 otto       (501) staff       (20)       38 2024-04-30 14:22:24.336380 openseneca-0.0.1/setup.cfg
--rw-r--r--   0 otto       (501) staff       (20)      547 2024-04-30 14:20:55.000000 openseneca-0.0.1/setup.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:39:48.434568 openseneca-0.0.2/
+-rw-r--r--   0 otto       (501) staff       (20)      161 2024-04-30 14:39:48.434308 openseneca-0.0.2/PKG-INFO
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:39:48.431054 openseneca-0.0.2/openseneca/
+-rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 10:06:53.000000 openseneca-0.0.2/openseneca/__init__.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:39:48.432033 openseneca-0.0.2/openseneca/classify/
+-rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:32:02.000000 openseneca-0.0.2/openseneca/classify/__init__.py
+-rw-r--r--   0 otto       (501) staff       (20)     1967 2024-04-30 10:06:53.000000 openseneca-0.0.2/openseneca/classify/categories.py
+-rw-r--r--   0 otto       (501) staff       (20)     2950 2024-04-30 14:01:40.000000 openseneca-0.0.2/openseneca/classify/llm.py
+-rw-r--r--   0 otto       (501) staff       (20)      386 2024-04-30 10:06:53.000000 openseneca-0.0.2/openseneca/classify/static.py
+-rw-r--r--   0 otto       (501) staff       (20)     1289 2024-04-30 14:12:45.000000 openseneca-0.0.2/openseneca/costs.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:39:48.432496 openseneca-0.0.2/openseneca/interfaces/
+-rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:31:56.000000 openseneca-0.0.2/openseneca/interfaces/__init__.py
+-rw-r--r--   0 otto       (501) staff       (20)     3228 2024-04-30 14:13:35.000000 openseneca-0.0.2/openseneca/interfaces/models.py
+-rw-r--r--   0 otto       (501) staff       (20)      844 2024-04-30 10:06:53.000000 openseneca-0.0.2/openseneca/interfaces/providers.py
+-rw-r--r--   0 otto       (501) staff       (20)     1021 2024-04-30 10:06:53.000000 openseneca-0.0.2/openseneca/interfaces/response.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:39:48.433294 openseneca-0.0.2/openseneca/models/
+-rw-r--r--   0 otto       (501) staff       (20)      612 2024-04-30 10:06:53.000000 openseneca-0.0.2/openseneca/models/__init__.py
+-rw-r--r--   0 otto       (501) staff       (20)     1900 2024-04-30 10:06:53.000000 openseneca-0.0.2/openseneca/models/cohere.py
+-rw-r--r--   0 otto       (501) staff       (20)      983 2024-04-30 10:06:53.000000 openseneca-0.0.2/openseneca/models/gpt3.py
+-rw-r--r--   0 otto       (501) staff       (20)      974 2024-04-30 10:06:53.000000 openseneca-0.0.2/openseneca/models/gpt4.py
+-rw-r--r--   0 otto       (501) staff       (20)     3134 2024-04-30 10:06:53.000000 openseneca-0.0.2/openseneca/models/llama2.py
+-rw-r--r--   0 otto       (501) staff       (20)     2160 2024-04-30 10:06:53.000000 openseneca-0.0.2/openseneca/models/llama3.py
+-rw-r--r--   0 otto       (501) staff       (20)     1034 2024-04-30 10:06:53.000000 openseneca-0.0.2/openseneca/models/mistral.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:39:48.433507 openseneca-0.0.2/openseneca/providers/
+-rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:31:49.000000 openseneca-0.0.2/openseneca/providers/__init__.py
+-rw-r--r--   0 otto       (501) staff       (20)     5297 2024-04-30 10:06:53.000000 openseneca-0.0.2/openseneca/providers/azure.py
+-rw-r--r--   0 otto       (501) staff       (20)     4976 2024-04-30 14:11:38.000000 openseneca-0.0.2/openseneca/router.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:39:48.433884 openseneca-0.0.2/openseneca/utils/
+-rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:32:18.000000 openseneca-0.0.2/openseneca/utils/__init__.py
+-rw-r--r--   0 otto       (501) staff       (20)     1799 2024-04-30 10:06:53.000000 openseneca-0.0.2/openseneca/utils/inspection.py
+-rw-r--r--   0 otto       (501) staff       (20)     2715 2024-04-30 10:06:53.000000 openseneca-0.0.2/openseneca/utils/logger.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:39:48.434060 openseneca-0.0.2/openseneca.egg-info/
+-rw-r--r--   0 otto       (501) staff       (20)      161 2024-04-30 14:39:48.000000 openseneca-0.0.2/openseneca.egg-info/PKG-INFO
+-rw-r--r--   0 otto       (501) staff       (20)      811 2024-04-30 14:39:48.000000 openseneca-0.0.2/openseneca.egg-info/SOURCES.txt
+-rw-r--r--   0 otto       (501) staff       (20)        1 2024-04-30 14:39:48.000000 openseneca-0.0.2/openseneca.egg-info/dependency_links.txt
+-rw-r--r--   0 otto       (501) staff       (20)       11 2024-04-30 14:39:48.000000 openseneca-0.0.2/openseneca.egg-info/top_level.txt
+-rw-r--r--   0 otto       (501) staff       (20)       38 2024-04-30 14:39:48.434615 openseneca-0.0.2/setup.cfg
+-rw-r--r--   0 otto       (501) staff       (20)      547 2024-04-30 14:39:31.000000 openseneca-0.0.2/setup.py
```

### Comparing `openseneca-0.0.1/openseneca/costs.py` & `openseneca-0.0.2/openseneca/costs.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.1/openseneca/models/__init__.py` & `openseneca-0.0.2/openseneca/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.1/openseneca/models/cohere.py` & `openseneca-0.0.2/openseneca/models/cohere.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.1/openseneca/models/gpt3.py` & `openseneca-0.0.2/openseneca/models/gpt3.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.1/openseneca/models/gpt4.py` & `openseneca-0.0.2/openseneca/models/gpt4.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.1/openseneca/models/llama2.py` & `openseneca-0.0.2/openseneca/models/llama2.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.1/openseneca/models/llama3.py` & `openseneca-0.0.2/openseneca/models/llama3.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.1/openseneca/models/mistral.py` & `openseneca-0.0.2/openseneca/models/mistral.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.1/openseneca/router.py` & `openseneca-0.0.2/openseneca/router.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.1/setup.py` & `openseneca-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'OpenSeneca'
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
         name="openseneca",
         version=VERSION,
```

