# Comparing `tmp/openseneca-0.0.42.tar.gz` & `tmp/openseneca-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openseneca-0.0.42.tar", last modified: Tue Apr 30 14:58:51 2024, max compression
+gzip compressed data, was "openseneca-0.0.43.tar", last modified: Tue Apr 30 14:59:49 2024, max compression
```

## Comparing `openseneca-0.0.42.tar` & `openseneca-0.0.43.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:58:51.415783 openseneca-0.0.42/
--rw-r--r--   0 otto       (501) staff       (20)      162 2024-04-30 14:58:51.415499 openseneca-0.0.42/PKG-INFO
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:58:51.412005 openseneca-0.0.42/openseneca/
--rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 10:06:53.000000 openseneca-0.0.42/openseneca/__init__.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:58:51.413067 openseneca-0.0.42/openseneca/classify/
--rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:32:02.000000 openseneca-0.0.42/openseneca/classify/__init__.py
--rw-r--r--   0 otto       (501) staff       (20)     1967 2024-04-30 10:06:53.000000 openseneca-0.0.42/openseneca/classify/categories.py
--rw-r--r--   0 otto       (501) staff       (20)     2950 2024-04-30 14:01:40.000000 openseneca-0.0.42/openseneca/classify/llm.py
--rw-r--r--   0 otto       (501) staff       (20)      386 2024-04-30 10:06:53.000000 openseneca-0.0.42/openseneca/classify/static.py
--rw-r--r--   0 otto       (501) staff       (20)     1306 2024-04-28 17:17:13.000000 openseneca-0.0.42/openseneca/config.yml
--rw-r--r--   0 otto       (501) staff       (20)     1478 2024-04-30 14:58:39.000000 openseneca-0.0.42/openseneca/costs.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:58:51.413534 openseneca-0.0.42/openseneca/interfaces/
--rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:31:56.000000 openseneca-0.0.42/openseneca/interfaces/__init__.py
--rw-r--r--   0 otto       (501) staff       (20)     3398 2024-04-30 14:58:10.000000 openseneca-0.0.42/openseneca/interfaces/models.py
--rw-r--r--   0 otto       (501) staff       (20)      844 2024-04-30 10:06:53.000000 openseneca-0.0.42/openseneca/interfaces/providers.py
--rw-r--r--   0 otto       (501) staff       (20)     1021 2024-04-30 10:06:53.000000 openseneca-0.0.42/openseneca/interfaces/response.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:58:51.414381 openseneca-0.0.42/openseneca/models/
--rw-r--r--   0 otto       (501) staff       (20)      612 2024-04-30 10:06:53.000000 openseneca-0.0.42/openseneca/models/__init__.py
--rw-r--r--   0 otto       (501) staff       (20)     1900 2024-04-30 10:06:53.000000 openseneca-0.0.42/openseneca/models/cohere.py
--rw-r--r--   0 otto       (501) staff       (20)      983 2024-04-30 10:06:53.000000 openseneca-0.0.42/openseneca/models/gpt3.py
--rw-r--r--   0 otto       (501) staff       (20)      974 2024-04-30 10:06:53.000000 openseneca-0.0.42/openseneca/models/gpt4.py
--rw-r--r--   0 otto       (501) staff       (20)     3134 2024-04-30 10:06:53.000000 openseneca-0.0.42/openseneca/models/llama2.py
--rw-r--r--   0 otto       (501) staff       (20)     2160 2024-04-30 10:06:53.000000 openseneca-0.0.42/openseneca/models/llama3.py
--rw-r--r--   0 otto       (501) staff       (20)     1034 2024-04-30 10:06:53.000000 openseneca-0.0.42/openseneca/models/mistral.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:58:51.414613 openseneca-0.0.42/openseneca/providers/
--rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:31:49.000000 openseneca-0.0.42/openseneca/providers/__init__.py
--rw-r--r--   0 otto       (501) staff       (20)     5297 2024-04-30 10:06:53.000000 openseneca-0.0.42/openseneca/providers/azure.py
--rw-r--r--   0 otto       (501) staff       (20)   222818 2024-04-30 10:06:53.000000 openseneca-0.0.42/openseneca/router.pk
--rw-r--r--   0 otto       (501) staff       (20)     5111 2024-04-30 14:56:41.000000 openseneca-0.0.42/openseneca/router.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:58:51.414984 openseneca-0.0.42/openseneca/utils/
--rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:32:18.000000 openseneca-0.0.42/openseneca/utils/__init__.py
--rw-r--r--   0 otto       (501) staff       (20)     1799 2024-04-30 10:06:53.000000 openseneca-0.0.42/openseneca/utils/inspection.py
--rw-r--r--   0 otto       (501) staff       (20)     2715 2024-04-30 10:06:53.000000 openseneca-0.0.42/openseneca/utils/logger.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:58:51.415180 openseneca-0.0.42/openseneca.egg-info/
--rw-r--r--   0 otto       (501) staff       (20)      162 2024-04-30 14:58:51.000000 openseneca-0.0.42/openseneca.egg-info/PKG-INFO
--rw-r--r--   0 otto       (501) staff       (20)      854 2024-04-30 14:58:51.000000 openseneca-0.0.42/openseneca.egg-info/SOURCES.txt
--rw-r--r--   0 otto       (501) staff       (20)        1 2024-04-30 14:58:51.000000 openseneca-0.0.42/openseneca.egg-info/dependency_links.txt
--rw-r--r--   0 otto       (501) staff       (20)       11 2024-04-30 14:58:51.000000 openseneca-0.0.42/openseneca.egg-info/top_level.txt
--rw-r--r--   0 otto       (501) staff       (20)       38 2024-04-30 14:58:51.415831 openseneca-0.0.42/setup.cfg
--rw-r--r--   0 otto       (501) staff       (20)      653 2024-04-30 14:58:50.000000 openseneca-0.0.42/setup.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:59:49.653345 openseneca-0.0.43/
+-rw-r--r--   0 otto       (501) staff       (20)      162 2024-04-30 14:59:49.653119 openseneca-0.0.43/PKG-INFO
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:59:49.648884 openseneca-0.0.43/openseneca/
+-rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 10:06:53.000000 openseneca-0.0.43/openseneca/__init__.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:59:49.649963 openseneca-0.0.43/openseneca/classify/
+-rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:32:02.000000 openseneca-0.0.43/openseneca/classify/__init__.py
+-rw-r--r--   0 otto       (501) staff       (20)     1967 2024-04-30 10:06:53.000000 openseneca-0.0.43/openseneca/classify/categories.py
+-rw-r--r--   0 otto       (501) staff       (20)     2950 2024-04-30 14:01:40.000000 openseneca-0.0.43/openseneca/classify/llm.py
+-rw-r--r--   0 otto       (501) staff       (20)      386 2024-04-30 10:06:53.000000 openseneca-0.0.43/openseneca/classify/static.py
+-rw-r--r--   0 otto       (501) staff       (20)     1306 2024-04-28 17:17:13.000000 openseneca-0.0.43/openseneca/config.yml
+-rw-r--r--   0 otto       (501) staff       (20)     1478 2024-04-30 14:58:39.000000 openseneca-0.0.43/openseneca/costs.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:59:49.650472 openseneca-0.0.43/openseneca/interfaces/
+-rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:31:56.000000 openseneca-0.0.43/openseneca/interfaces/__init__.py
+-rw-r--r--   0 otto       (501) staff       (20)     3398 2024-04-30 14:58:10.000000 openseneca-0.0.43/openseneca/interfaces/models.py
+-rw-r--r--   0 otto       (501) staff       (20)      844 2024-04-30 10:06:53.000000 openseneca-0.0.43/openseneca/interfaces/providers.py
+-rw-r--r--   0 otto       (501) staff       (20)     1021 2024-04-30 10:06:53.000000 openseneca-0.0.43/openseneca/interfaces/response.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:59:49.651703 openseneca-0.0.43/openseneca/models/
+-rw-r--r--   0 otto       (501) staff       (20)      612 2024-04-30 10:06:53.000000 openseneca-0.0.43/openseneca/models/__init__.py
+-rw-r--r--   0 otto       (501) staff       (20)     1900 2024-04-30 10:06:53.000000 openseneca-0.0.43/openseneca/models/cohere.py
+-rw-r--r--   0 otto       (501) staff       (20)      983 2024-04-30 10:06:53.000000 openseneca-0.0.43/openseneca/models/gpt3.py
+-rw-r--r--   0 otto       (501) staff       (20)      974 2024-04-30 10:06:53.000000 openseneca-0.0.43/openseneca/models/gpt4.py
+-rw-r--r--   0 otto       (501) staff       (20)     3134 2024-04-30 10:06:53.000000 openseneca-0.0.43/openseneca/models/llama2.py
+-rw-r--r--   0 otto       (501) staff       (20)     2160 2024-04-30 10:06:53.000000 openseneca-0.0.43/openseneca/models/llama3.py
+-rw-r--r--   0 otto       (501) staff       (20)     1034 2024-04-30 10:06:53.000000 openseneca-0.0.43/openseneca/models/mistral.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:59:49.651965 openseneca-0.0.43/openseneca/providers/
+-rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:31:49.000000 openseneca-0.0.43/openseneca/providers/__init__.py
+-rw-r--r--   0 otto       (501) staff       (20)     5297 2024-04-30 10:06:53.000000 openseneca-0.0.43/openseneca/providers/azure.py
+-rw-r--r--   0 otto       (501) staff       (20)   222818 2024-04-30 10:06:53.000000 openseneca-0.0.43/openseneca/router.pk
+-rw-r--r--   0 otto       (501) staff       (20)     5111 2024-04-30 14:56:41.000000 openseneca-0.0.43/openseneca/router.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:59:49.652693 openseneca-0.0.43/openseneca/utils/
+-rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:32:18.000000 openseneca-0.0.43/openseneca/utils/__init__.py
+-rw-r--r--   0 otto       (501) staff       (20)     1799 2024-04-30 10:06:53.000000 openseneca-0.0.43/openseneca/utils/inspection.py
+-rw-r--r--   0 otto       (501) staff       (20)     2715 2024-04-30 10:06:53.000000 openseneca-0.0.43/openseneca/utils/logger.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 14:59:49.652889 openseneca-0.0.43/openseneca.egg-info/
+-rw-r--r--   0 otto       (501) staff       (20)      162 2024-04-30 14:59:49.000000 openseneca-0.0.43/openseneca.egg-info/PKG-INFO
+-rw-r--r--   0 otto       (501) staff       (20)      854 2024-04-30 14:59:49.000000 openseneca-0.0.43/openseneca.egg-info/SOURCES.txt
+-rw-r--r--   0 otto       (501) staff       (20)        1 2024-04-30 14:59:49.000000 openseneca-0.0.43/openseneca.egg-info/dependency_links.txt
+-rw-r--r--   0 otto       (501) staff       (20)       11 2024-04-30 14:59:49.000000 openseneca-0.0.43/openseneca.egg-info/top_level.txt
+-rw-r--r--   0 otto       (501) staff       (20)       38 2024-04-30 14:59:49.653391 openseneca-0.0.43/setup.cfg
+-rw-r--r--   0 otto       (501) staff       (20)      653 2024-04-30 14:59:48.000000 openseneca-0.0.43/setup.py
```

### Comparing `openseneca-0.0.42/openseneca/classify/categories.py` & `openseneca-0.0.43/openseneca/classify/categories.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/openseneca/classify/llm.py` & `openseneca-0.0.43/openseneca/classify/llm.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/openseneca/config.yml` & `openseneca-0.0.43/openseneca/config.yml`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/openseneca/costs.py` & `openseneca-0.0.43/openseneca/costs.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/openseneca/interfaces/models.py` & `openseneca-0.0.43/openseneca/interfaces/models.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/openseneca/interfaces/providers.py` & `openseneca-0.0.43/openseneca/interfaces/providers.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/openseneca/interfaces/response.py` & `openseneca-0.0.43/openseneca/interfaces/response.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/openseneca/models/__init__.py` & `openseneca-0.0.43/openseneca/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/openseneca/models/cohere.py` & `openseneca-0.0.43/openseneca/models/cohere.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/openseneca/models/gpt3.py` & `openseneca-0.0.43/openseneca/models/gpt3.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/openseneca/models/gpt4.py` & `openseneca-0.0.43/openseneca/models/gpt4.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/openseneca/models/llama2.py` & `openseneca-0.0.43/openseneca/models/llama2.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/openseneca/models/llama3.py` & `openseneca-0.0.43/openseneca/models/llama3.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/openseneca/models/mistral.py` & `openseneca-0.0.43/openseneca/models/mistral.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/openseneca/providers/azure.py` & `openseneca-0.0.43/openseneca/providers/azure.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/openseneca/router.pk` & `openseneca-0.0.43/openseneca/router.pk`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/openseneca/router.py` & `openseneca-0.0.43/openseneca/router.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/openseneca/utils/inspection.py` & `openseneca-0.0.43/openseneca/utils/inspection.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/openseneca/utils/logger.py` & `openseneca-0.0.43/openseneca/utils/logger.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/openseneca.egg-info/SOURCES.txt` & `openseneca-0.0.43/openseneca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.42/setup.py` & `openseneca-0.0.43/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 # rm -rf dist/ && python setup.py sdist bdist_wheel
 # twine upload --repository openseneca dist/*
 
-VERSION = '0.0.42'
+VERSION = '0.0.43'
 DESCRIPTION = 'OpenSeneca'
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
         name="openseneca",
         version=VERSION,
```

