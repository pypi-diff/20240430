# Comparing `tmp/stopwords_tr-1.2.0.tar.gz` & `tmp/stopwords_tr-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stopwords_tr-1.2.0.tar", last modified: Tue Apr 30 09:04:25 2024, max compression
+gzip compressed data, was "stopwords_tr-1.2.1.tar", last modified: Tue Apr 30 09:12:17 2024, max compression
```

## Comparing `stopwords_tr-1.2.0.tar` & `stopwords_tr-1.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 09:04:25.853700 stopwords_tr-1.2.0/
--rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     1051 2024-04-30 09:04:25.852699 stopwords_tr-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-30 09:04:25.854699 stopwords_tr-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1297 2024-04-30 09:04:17.000000 stopwords_tr-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 09:04:25.852699 stopwords_tr-1.2.0/stopwords_tr.egg-info/
--rw-rw-rw-   0        0        0     1051 2024-04-30 09:04:25.000000 stopwords_tr-1.2.0/stopwords_tr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-04-30 09:04:25.000000 stopwords_tr-1.2.0/stopwords_tr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 09:04:25.000000 stopwords_tr-1.2.0/stopwords_tr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-30 09:04:25.000000 stopwords_tr-1.2.0/stopwords_tr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      160 2024-04-30 09:03:41.000000 stopwords_tr-1.2.0/stopwords_tr.py
+drwxrwxrwx   0        0        0        0 2024-04-30 09:12:17.191065 stopwords_tr-1.2.1/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1051 2024-04-30 09:12:17.190065 stopwords_tr-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-30 09:12:17.191065 stopwords_tr-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1297 2024-04-30 09:12:13.000000 stopwords_tr-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 09:12:17.189064 stopwords_tr-1.2.1/stopwords_tr.egg-info/
+-rw-rw-rw-   0        0        0     1051 2024-04-30 09:12:17.000000 stopwords_tr-1.2.1/stopwords_tr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2024-04-30 09:12:17.000000 stopwords_tr-1.2.1/stopwords_tr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 09:12:17.000000 stopwords_tr-1.2.1/stopwords_tr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-30 09:12:17.000000 stopwords_tr-1.2.1/stopwords_tr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      157 2024-04-30 09:11:56.000000 stopwords_tr-1.2.1/stopwords_tr.py
```

### Comparing `stopwords_tr-1.2.0/LICENSE` & `stopwords_tr-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stopwords_tr-1.2.0/PKG-INFO` & `stopwords_tr-1.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.2.0
+Version: 1.2.1
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp, filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stopwords_tr-1.2.0/setup.py` & `stopwords_tr-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name= 'stopwords_tr',
-    version='1.2.0',
+    version='1.2.1',
     license='MIT',
     author="Metin Oktay DENIZ",
     author_email='metinoktaydenizz@gmail.com',
     description="Stopwords filter for Turkish languages",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     url='https://github.com/metinoktayd/StopWords-Turkish-Language',
```

### Comparing `stopwords_tr-1.2.0/stopwords_tr.egg-info/PKG-INFO` & `stopwords_tr-1.2.1/stopwords_tr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.2.0
+Version: 1.2.1
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp, filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
```

