# Comparing `tmp/openseneca-0.0.5.tar.gz` & `tmp/openseneca-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openseneca-0.0.5.tar", last modified: Tue Apr 30 15:13:59 2024, max compression
+gzip compressed data, was "openseneca-0.0.6.tar", last modified: Tue Apr 30 15:15:07 2024, max compression
```

## Comparing `openseneca-0.0.5.tar` & `openseneca-0.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:13:59.920845 openseneca-0.0.5/
--rw-r--r--   0 otto       (501) staff       (20)      865 2024-04-30 15:13:59.920599 openseneca-0.0.5/PKG-INFO
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:13:59.917039 openseneca-0.0.5/openseneca/
--rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 10:06:53.000000 openseneca-0.0.5/openseneca/__init__.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:13:59.918169 openseneca-0.0.5/openseneca/classify/
--rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:32:02.000000 openseneca-0.0.5/openseneca/classify/__init__.py
--rw-r--r--   0 otto       (501) staff       (20)     1967 2024-04-30 10:06:53.000000 openseneca-0.0.5/openseneca/classify/categories.py
--rw-r--r--   0 otto       (501) staff       (20)     2950 2024-04-30 14:01:40.000000 openseneca-0.0.5/openseneca/classify/llm.py
--rw-r--r--   0 otto       (501) staff       (20)      386 2024-04-30 10:06:53.000000 openseneca-0.0.5/openseneca/classify/static.py
--rw-r--r--   0 otto       (501) staff       (20)     1306 2024-04-28 17:17:13.000000 openseneca-0.0.5/openseneca/config.yml
--rw-r--r--   0 otto       (501) staff       (20)     1478 2024-04-30 14:58:39.000000 openseneca-0.0.5/openseneca/costs.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:13:59.918688 openseneca-0.0.5/openseneca/interfaces/
--rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:31:56.000000 openseneca-0.0.5/openseneca/interfaces/__init__.py
--rw-r--r--   0 otto       (501) staff       (20)     3398 2024-04-30 14:58:10.000000 openseneca-0.0.5/openseneca/interfaces/models.py
--rw-r--r--   0 otto       (501) staff       (20)      844 2024-04-30 10:06:53.000000 openseneca-0.0.5/openseneca/interfaces/providers.py
--rw-r--r--   0 otto       (501) staff       (20)     1021 2024-04-30 10:06:53.000000 openseneca-0.0.5/openseneca/interfaces/response.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:13:59.919481 openseneca-0.0.5/openseneca/models/
--rw-r--r--   0 otto       (501) staff       (20)      612 2024-04-30 10:06:53.000000 openseneca-0.0.5/openseneca/models/__init__.py
--rw-r--r--   0 otto       (501) staff       (20)     1900 2024-04-30 10:06:53.000000 openseneca-0.0.5/openseneca/models/cohere.py
--rw-r--r--   0 otto       (501) staff       (20)      983 2024-04-30 10:06:53.000000 openseneca-0.0.5/openseneca/models/gpt3.py
--rw-r--r--   0 otto       (501) staff       (20)      974 2024-04-30 10:06:53.000000 openseneca-0.0.5/openseneca/models/gpt4.py
--rw-r--r--   0 otto       (501) staff       (20)     3134 2024-04-30 10:06:53.000000 openseneca-0.0.5/openseneca/models/llama2.py
--rw-r--r--   0 otto       (501) staff       (20)     2160 2024-04-30 10:06:53.000000 openseneca-0.0.5/openseneca/models/llama3.py
--rw-r--r--   0 otto       (501) staff       (20)     1034 2024-04-30 10:06:53.000000 openseneca-0.0.5/openseneca/models/mistral.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:13:59.919685 openseneca-0.0.5/openseneca/providers/
--rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:31:49.000000 openseneca-0.0.5/openseneca/providers/__init__.py
--rw-r--r--   0 otto       (501) staff       (20)     5297 2024-04-30 10:06:53.000000 openseneca-0.0.5/openseneca/providers/azure.py
--rw-r--r--   0 otto       (501) staff       (20)   222818 2024-04-30 10:06:53.000000 openseneca-0.0.5/openseneca/router.pk
--rw-r--r--   0 otto       (501) staff       (20)     5111 2024-04-30 14:56:41.000000 openseneca-0.0.5/openseneca/router.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:13:59.920061 openseneca-0.0.5/openseneca/utils/
--rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:32:18.000000 openseneca-0.0.5/openseneca/utils/__init__.py
--rw-r--r--   0 otto       (501) staff       (20)     1799 2024-04-30 10:06:53.000000 openseneca-0.0.5/openseneca/utils/inspection.py
--rw-r--r--   0 otto       (501) staff       (20)     2715 2024-04-30 10:06:53.000000 openseneca-0.0.5/openseneca/utils/logger.py
-drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:13:59.920242 openseneca-0.0.5/openseneca.egg-info/
--rw-r--r--   0 otto       (501) staff       (20)      865 2024-04-30 15:13:59.000000 openseneca-0.0.5/openseneca.egg-info/PKG-INFO
--rw-r--r--   0 otto       (501) staff       (20)      887 2024-04-30 15:13:59.000000 openseneca-0.0.5/openseneca.egg-info/SOURCES.txt
--rw-r--r--   0 otto       (501) staff       (20)        1 2024-04-30 15:13:59.000000 openseneca-0.0.5/openseneca.egg-info/dependency_links.txt
--rw-r--r--   0 otto       (501) staff       (20)      344 2024-04-30 15:13:59.000000 openseneca-0.0.5/openseneca.egg-info/requires.txt
--rw-r--r--   0 otto       (501) staff       (20)       11 2024-04-30 15:13:59.000000 openseneca-0.0.5/openseneca.egg-info/top_level.txt
--rw-r--r--   0 otto       (501) staff       (20)       38 2024-04-30 15:13:59.920890 openseneca-0.0.5/setup.cfg
--rw-r--r--   0 otto       (501) staff       (20)      852 2024-04-30 15:13:58.000000 openseneca-0.0.5/setup.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:15:07.494617 openseneca-0.0.6/
+-rw-r--r--   0 otto       (501) staff       (20)      828 2024-04-30 15:15:07.494346 openseneca-0.0.6/PKG-INFO
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:15:07.490557 openseneca-0.0.6/openseneca/
+-rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/__init__.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:15:07.491613 openseneca-0.0.6/openseneca/classify/
+-rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:32:02.000000 openseneca-0.0.6/openseneca/classify/__init__.py
+-rw-r--r--   0 otto       (501) staff       (20)     1967 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/classify/categories.py
+-rw-r--r--   0 otto       (501) staff       (20)     2950 2024-04-30 14:01:40.000000 openseneca-0.0.6/openseneca/classify/llm.py
+-rw-r--r--   0 otto       (501) staff       (20)      386 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/classify/static.py
+-rw-r--r--   0 otto       (501) staff       (20)     1306 2024-04-28 17:17:13.000000 openseneca-0.0.6/openseneca/config.yml
+-rw-r--r--   0 otto       (501) staff       (20)     1478 2024-04-30 14:58:39.000000 openseneca-0.0.6/openseneca/costs.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:15:07.492202 openseneca-0.0.6/openseneca/interfaces/
+-rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:31:56.000000 openseneca-0.0.6/openseneca/interfaces/__init__.py
+-rw-r--r--   0 otto       (501) staff       (20)     3398 2024-04-30 14:58:10.000000 openseneca-0.0.6/openseneca/interfaces/models.py
+-rw-r--r--   0 otto       (501) staff       (20)      844 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/interfaces/providers.py
+-rw-r--r--   0 otto       (501) staff       (20)     1021 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/interfaces/response.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:15:07.493228 openseneca-0.0.6/openseneca/models/
+-rw-r--r--   0 otto       (501) staff       (20)      612 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/models/__init__.py
+-rw-r--r--   0 otto       (501) staff       (20)     1900 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/models/cohere.py
+-rw-r--r--   0 otto       (501) staff       (20)      983 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/models/gpt3.py
+-rw-r--r--   0 otto       (501) staff       (20)      974 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/models/gpt4.py
+-rw-r--r--   0 otto       (501) staff       (20)     3134 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/models/llama2.py
+-rw-r--r--   0 otto       (501) staff       (20)     2160 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/models/llama3.py
+-rw-r--r--   0 otto       (501) staff       (20)     1034 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/models/mistral.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:15:07.493442 openseneca-0.0.6/openseneca/providers/
+-rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:31:49.000000 openseneca-0.0.6/openseneca/providers/__init__.py
+-rw-r--r--   0 otto       (501) staff       (20)     5297 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/providers/azure.py
+-rw-r--r--   0 otto       (501) staff       (20)   222818 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/router.pk
+-rw-r--r--   0 otto       (501) staff       (20)     5111 2024-04-30 14:56:41.000000 openseneca-0.0.6/openseneca/router.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:15:07.493864 openseneca-0.0.6/openseneca/utils/
+-rw-r--r--   0 otto       (501) staff       (20)        0 2024-04-30 14:32:18.000000 openseneca-0.0.6/openseneca/utils/__init__.py
+-rw-r--r--   0 otto       (501) staff       (20)     1799 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/utils/inspection.py
+-rw-r--r--   0 otto       (501) staff       (20)     2715 2024-04-30 10:06:53.000000 openseneca-0.0.6/openseneca/utils/logger.py
+drwxr-xr-x   0 otto       (501) staff       (20)        0 2024-04-30 15:15:07.494036 openseneca-0.0.6/openseneca.egg-info/
+-rw-r--r--   0 otto       (501) staff       (20)      828 2024-04-30 15:15:07.000000 openseneca-0.0.6/openseneca.egg-info/PKG-INFO
+-rw-r--r--   0 otto       (501) staff       (20)      887 2024-04-30 15:15:07.000000 openseneca-0.0.6/openseneca.egg-info/SOURCES.txt
+-rw-r--r--   0 otto       (501) staff       (20)        1 2024-04-30 15:15:07.000000 openseneca-0.0.6/openseneca.egg-info/dependency_links.txt
+-rw-r--r--   0 otto       (501) staff       (20)      322 2024-04-30 15:15:07.000000 openseneca-0.0.6/openseneca.egg-info/requires.txt
+-rw-r--r--   0 otto       (501) staff       (20)       11 2024-04-30 15:15:07.000000 openseneca-0.0.6/openseneca.egg-info/top_level.txt
+-rw-r--r--   0 otto       (501) staff       (20)       38 2024-04-30 15:15:07.494660 openseneca-0.0.6/setup.cfg
+-rw-r--r--   0 otto       (501) staff       (20)      852 2024-04-30 15:15:05.000000 openseneca-0.0.6/setup.py
```

### Comparing `openseneca-0.0.5/PKG-INFO` & `openseneca-0.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openseneca
-Version: 0.0.5
+Version: 0.0.6
 Summary: OpenSeneca
 Author: Ottavio Fogliata
 Author-email: ottavio.fogliata@openseneca.ai
 Keywords: python
 Requires-Dist: fire>=0.6.0
 Requires-Dist: uvicorn[standard]>=0.29.0
 Requires-Dist: fastapi>=0.110.1
@@ -24,8 +24,7 @@
 Requires-Dist: pytest-cov
 Requires-Dist: colorlog
 Requires-Dist: pycountry
 Requires-Dist: python-dotenv
 Requires-Dist: langdetect
 Requires-Dist: pydantic
 Requires-Dist: huggingface-cli
-Requires-Dist: lfs-enable-largefiles
```

### Comparing `openseneca-0.0.5/openseneca/classify/categories.py` & `openseneca-0.0.6/openseneca/classify/categories.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/openseneca/classify/llm.py` & `openseneca-0.0.6/openseneca/classify/llm.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/openseneca/config.yml` & `openseneca-0.0.6/openseneca/config.yml`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/openseneca/costs.py` & `openseneca-0.0.6/openseneca/costs.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/openseneca/interfaces/models.py` & `openseneca-0.0.6/openseneca/interfaces/models.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/openseneca/interfaces/providers.py` & `openseneca-0.0.6/openseneca/interfaces/providers.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/openseneca/interfaces/response.py` & `openseneca-0.0.6/openseneca/interfaces/response.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/openseneca/models/__init__.py` & `openseneca-0.0.6/openseneca/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/openseneca/models/cohere.py` & `openseneca-0.0.6/openseneca/models/cohere.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/openseneca/models/gpt3.py` & `openseneca-0.0.6/openseneca/models/gpt3.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/openseneca/models/gpt4.py` & `openseneca-0.0.6/openseneca/models/gpt4.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/openseneca/models/llama2.py` & `openseneca-0.0.6/openseneca/models/llama2.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/openseneca/models/llama3.py` & `openseneca-0.0.6/openseneca/models/llama3.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/openseneca/models/mistral.py` & `openseneca-0.0.6/openseneca/models/mistral.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/openseneca/providers/azure.py` & `openseneca-0.0.6/openseneca/providers/azure.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/openseneca/router.pk` & `openseneca-0.0.6/openseneca/router.pk`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/openseneca/router.py` & `openseneca-0.0.6/openseneca/router.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/openseneca/utils/inspection.py` & `openseneca-0.0.6/openseneca/utils/inspection.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/openseneca/utils/logger.py` & `openseneca-0.0.6/openseneca/utils/logger.py`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/openseneca.egg-info/PKG-INFO` & `openseneca-0.0.6/openseneca.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openseneca
-Version: 0.0.5
+Version: 0.0.6
 Summary: OpenSeneca
 Author: Ottavio Fogliata
 Author-email: ottavio.fogliata@openseneca.ai
 Keywords: python
 Requires-Dist: fire>=0.6.0
 Requires-Dist: uvicorn[standard]>=0.29.0
 Requires-Dist: fastapi>=0.110.1
@@ -24,8 +24,7 @@
 Requires-Dist: pytest-cov
 Requires-Dist: colorlog
 Requires-Dist: pycountry
 Requires-Dist: python-dotenv
 Requires-Dist: langdetect
 Requires-Dist: pydantic
 Requires-Dist: huggingface-cli
-Requires-Dist: lfs-enable-largefiles
```

### Comparing `openseneca-0.0.5/openseneca.egg-info/SOURCES.txt` & `openseneca-0.0.6/openseneca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openseneca-0.0.5/setup.py` & `openseneca-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # test: pip install -e .
 # rm -rf dist/ && python setup.py sdist bdist_wheel
 # twine upload --repository openseneca dist/*
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'OpenSeneca'
 LONG_DESCRIPTION = ''
 
 def read_requirements():
     with open('openseneca/requirements.txt', 'r') as req:
         content = req.read()
         requirements = content.split('\n')
```

