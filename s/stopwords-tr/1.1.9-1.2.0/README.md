# Comparing `tmp/stopwords_tr-1.1.9.tar.gz` & `tmp/stopwords_tr-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stopwords_tr-1.1.9.tar", last modified: Tue Apr 30 08:15:38 2024, max compression
+gzip compressed data, was "stopwords_tr-1.2.0.tar", last modified: Tue Apr 30 09:04:25 2024, max compression
```

## Comparing `stopwords_tr-1.1.9.tar` & `stopwords_tr-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 08:15:38.529202 stopwords_tr-1.1.9/
--rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.1.9/LICENSE
--rw-rw-rw-   0        0        0     1051 2024-04-30 08:15:38.528201 stopwords_tr-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.1.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-30 08:15:38.529202 stopwords_tr-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1296 2024-04-30 08:15:29.000000 stopwords_tr-1.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:15:38.520201 stopwords_tr-1.1.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-30 08:15:38.522202 stopwords_tr-1.1.9/src/stopwords_tr/
--rw-rw-rw-   0        0        0      165 2024-04-30 07:48:28.000000 stopwords_tr-1.1.9/src/stopwords_tr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:15:38.528201 stopwords_tr-1.1.9/src/stopwords_tr.egg-info/
--rw-rw-rw-   0        0        0     1051 2024-04-30 08:15:38.000000 stopwords_tr-1.1.9/src/stopwords_tr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-04-30 08:15:38.000000 stopwords_tr-1.1.9/src/stopwords_tr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 08:15:38.000000 stopwords_tr-1.1.9/src/stopwords_tr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-30 08:15:38.000000 stopwords_tr-1.1.9/src/stopwords_tr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 09:04:25.853700 stopwords_tr-1.2.0/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1051 2024-04-30 09:04:25.852699 stopwords_tr-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-30 09:04:25.854699 stopwords_tr-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1297 2024-04-30 09:04:17.000000 stopwords_tr-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 09:04:25.852699 stopwords_tr-1.2.0/stopwords_tr.egg-info/
+-rw-rw-rw-   0        0        0     1051 2024-04-30 09:04:25.000000 stopwords_tr-1.2.0/stopwords_tr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2024-04-30 09:04:25.000000 stopwords_tr-1.2.0/stopwords_tr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 09:04:25.000000 stopwords_tr-1.2.0/stopwords_tr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-30 09:04:25.000000 stopwords_tr-1.2.0/stopwords_tr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      160 2024-04-30 09:03:41.000000 stopwords_tr-1.2.0/stopwords_tr.py
```

### Comparing `stopwords_tr-1.1.9/LICENSE` & `stopwords_tr-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stopwords_tr-1.1.9/PKG-INFO` & `stopwords_tr-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.1.9
+Version: 1.2.0
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp, filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stopwords_tr-1.1.9/setup.py` & `stopwords_tr-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name= 'stopwords_tr',
-    version='1.1.9',
+    version='1.2.0',
     license='MIT',
     author="Metin Oktay DENIZ",
     author_email='metinoktaydenizz@gmail.com',
     description="Stopwords filter for Turkish languages",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     url='https://github.com/metinoktayd/StopWords-Turkish-Language',
@@ -24,11 +24,11 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12'
     ],
-    #py_modules=["stopwords_tr"]
-    package_dir={'':'src'},
-    packages= find_packages('src')
+    py_modules=["stopwords_tr"]
+    #package_dir={'':'src'},
+    #packages= find_packages('src')
 )
```

### Comparing `stopwords_tr-1.1.9/src/stopwords_tr.egg-info/PKG-INFO` & `stopwords_tr-1.2.0/stopwords_tr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.1.9
+Version: 1.2.0
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp, filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
```

