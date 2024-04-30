# Comparing `tmp/qlv-client-0.1.7.tar.gz` & `tmp/qlv-client-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlv-client-0.1.7.tar", last modified: Sat Apr 27 02:38:32 2024, max compression
+gzip compressed data, was "qlv-client-0.1.8.tar", last modified: Mon Apr 29 09:07:51 2024, max compression
```

## Comparing `qlv-client-0.1.7.tar` & `qlv-client-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 02:38:32.094154 qlv-client-0.1.7/
--rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      456 2024-04-27 02:38:32.094154 qlv-client-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 02:38:32.091175 qlv-client-0.1.7/qlv_client/
--rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.1.7/qlv_client/__init__.py
--rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.1.7/qlv_client/api.py
--rw-rw-rw-   0        0        0     1224 2024-04-17 07:59:59.000000 qlv-client-0.1.7/qlv_client/config.py
--rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.1.7/qlv_client/converter.py
--rw-rw-rw-   0        0        0     4115 2024-04-17 08:27:22.000000 qlv-client-0.1.7/qlv_client/http_client.py
--rw-rw-rw-   0        0        0     6834 2024-04-27 02:37:27.000000 qlv-client-0.1.7/qlv_client/proxy.py
--rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.1.7/qlv_client/repository.py
--rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.1.7/qlv_client/test.py
--rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.1.7/qlv_client/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-27 02:38:32.093658 qlv-client-0.1.7/qlv_client.egg-info/
--rw-rw-rw-   0        0        0      456 2024-04-27 02:38:32.000000 qlv-client-0.1.7/qlv_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2024-04-27 02:38:32.000000 qlv-client-0.1.7/qlv_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 02:38:32.000000 qlv-client-0.1.7/qlv_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-27 02:38:32.000000 qlv-client-0.1.7/qlv_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-27 02:38:32.000000 qlv-client-0.1.7/qlv_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 02:38:32.094154 qlv-client-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1066 2024-04-27 02:35:45.000000 qlv-client-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 09:07:51.821947 qlv-client-0.1.8/
+-rw-rw-rw-   0        0        0    11558 2024-04-17 06:55:59.000000 qlv-client-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      456 2024-04-29 09:07:51.821451 qlv-client-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 06:55:59.000000 qlv-client-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 09:07:51.818502 qlv-client-0.1.8/qlv_client/
+-rw-rw-rw-   0        0        0      463 2024-04-17 08:02:13.000000 qlv-client-0.1.8/qlv_client/__init__.py
+-rw-rw-rw-   0        0        0     9543 2024-04-17 08:27:22.000000 qlv-client-0.1.8/qlv_client/api.py
+-rw-rw-rw-   0        0        0     1224 2024-04-17 07:59:59.000000 qlv-client-0.1.8/qlv_client/config.py
+-rw-rw-rw-   0        0        0     1303 2024-04-17 07:30:16.000000 qlv-client-0.1.8/qlv_client/converter.py
+-rw-rw-rw-   0        0        0     4115 2024-04-29 09:06:57.000000 qlv-client-0.1.8/qlv_client/http_client.py
+-rw-rw-rw-   0        0        0     6834 2024-04-27 02:37:27.000000 qlv-client-0.1.8/qlv_client/proxy.py
+-rw-rw-rw-   0        0        0     3187 2024-04-17 08:27:22.000000 qlv-client-0.1.8/qlv_client/repository.py
+-rw-rw-rw-   0        0        0     2235 2024-04-17 08:27:22.000000 qlv-client-0.1.8/qlv_client/test.py
+-rw-rw-rw-   0        0        0     1995 2024-04-17 07:29:50.000000 qlv-client-0.1.8/qlv_client/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 09:07:51.820954 qlv-client-0.1.8/qlv_client.egg-info/
+-rw-rw-rw-   0        0        0      456 2024-04-29 09:07:51.000000 qlv-client-0.1.8/qlv_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-04-29 09:07:51.000000 qlv-client-0.1.8/qlv_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 09:07:51.000000 qlv-client-0.1.8/qlv_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-29 09:07:51.000000 qlv-client-0.1.8/qlv_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-29 09:07:51.000000 qlv-client-0.1.8/qlv_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 09:07:51.821947 qlv-client-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2024-04-29 09:06:42.000000 qlv-client-0.1.8/setup.py
```

### Comparing `qlv-client-0.1.7/LICENSE` & `qlv-client-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.7/qlv_client/api.py` & `qlv-client-0.1.8/qlv_client/api.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.7/qlv_client/config.py` & `qlv-client-0.1.8/qlv_client/config.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.7/qlv_client/converter.py` & `qlv-client-0.1.8/qlv_client/converter.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.7/qlv_client/http_client.py` & `qlv-client-0.1.8/qlv_client/http_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 import requests
 from qlv_client.utils import logger
 from qlv_client.utils import covert_dict_key_to_lower, get_html_title
 
 
 class HttpService(object):
-    __time_out = 10
+    __time_out = 30
     __domain = None
     __url = None
     __protocol = None
     __headers: dict = {
         "Content-Type": "application/json; charset=UTF-8",
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) " +
                       "Chrome/123.0.0.0 Safari/537.36"
```

### Comparing `qlv-client-0.1.7/qlv_client/proxy.py` & `qlv-client-0.1.8/qlv_client/proxy.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.7/qlv_client/repository.py` & `qlv-client-0.1.8/qlv_client/repository.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.7/qlv_client/test.py` & `qlv-client-0.1.8/qlv_client/test.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.7/qlv_client/utils.py` & `qlv-client-0.1.8/qlv_client/utils.py`

 * *Files identical despite different names*

### Comparing `qlv-client-0.1.7/setup.py` & `qlv-client-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='qlv-client',
-    version='0.1.7',
+    version='0.1.8',
     description='This is my qlv proxy qlv_client package',
     long_description='This is my qlv proxy qlv_client package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/qlvClient',
     packages=find_packages(),
     install_requires=[
```

