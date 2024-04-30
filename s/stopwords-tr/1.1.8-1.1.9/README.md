# Comparing `tmp/stopwords_tr-1.1.8.tar.gz` & `tmp/stopwords_tr-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stopwords_tr-1.1.8.tar", last modified: Tue Apr 30 08:09:29 2024, max compression
+gzip compressed data, was "stopwords_tr-1.1.9.tar", last modified: Tue Apr 30 08:15:38 2024, max compression
```

## Comparing `stopwords_tr-1.1.8.tar` & `stopwords_tr-1.1.9.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 08:09:29.254537 stopwords_tr-1.1.8/
--rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.1.8/LICENSE
--rw-rw-rw-   0        0        0     1051 2024-04-30 08:09:29.253537 stopwords_tr-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.1.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-30 08:09:29.254537 stopwords_tr-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1305 2024-04-30 08:09:22.000000 stopwords_tr-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:09:29.245538 stopwords_tr-1.1.8/src/
-drwxrwxrwx   0        0        0        0 2024-04-30 08:09:29.252537 stopwords_tr-1.1.8/src/stopwords_tr.egg-info/
--rw-rw-rw-   0        0        0     1051 2024-04-30 08:09:29.000000 stopwords_tr-1.1.8/src/stopwords_tr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-04-30 08:09:29.000000 stopwords_tr-1.1.8/src/stopwords_tr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 08:09:29.000000 stopwords_tr-1.1.8/src/stopwords_tr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 08:09:29.000000 stopwords_tr-1.1.8/src/stopwords_tr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 08:15:38.529202 stopwords_tr-1.1.9/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0     1051 2024-04-30 08:15:38.528201 stopwords_tr-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-30 08:15:38.529202 stopwords_tr-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1296 2024-04-30 08:15:29.000000 stopwords_tr-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:15:38.520201 stopwords_tr-1.1.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-30 08:15:38.522202 stopwords_tr-1.1.9/src/stopwords_tr/
+-rw-rw-rw-   0        0        0      165 2024-04-30 07:48:28.000000 stopwords_tr-1.1.9/src/stopwords_tr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:15:38.528201 stopwords_tr-1.1.9/src/stopwords_tr.egg-info/
+-rw-rw-rw-   0        0        0     1051 2024-04-30 08:15:38.000000 stopwords_tr-1.1.9/src/stopwords_tr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-04-30 08:15:38.000000 stopwords_tr-1.1.9/src/stopwords_tr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 08:15:38.000000 stopwords_tr-1.1.9/src/stopwords_tr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-30 08:15:38.000000 stopwords_tr-1.1.9/src/stopwords_tr.egg-info/top_level.txt
```

### Comparing `stopwords_tr-1.1.8/LICENSE` & `stopwords_tr-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stopwords_tr-1.1.8/PKG-INFO` & `stopwords_tr-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.1.8
+Version: 1.1.9
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp, filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stopwords_tr-1.1.8/setup.py` & `stopwords_tr-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name= 'stopwords_tr',
-    version='1.1.8',
+    version='1.1.9',
     license='MIT',
     author="Metin Oktay DENIZ",
     author_email='metinoktaydenizz@gmail.com',
     description="Stopwords filter for Turkish languages",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     url='https://github.com/metinoktayd/StopWords-Turkish-Language',
@@ -26,9 +26,9 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12'
     ],
     #py_modules=["stopwords_tr"]
     package_dir={'':'src'},
-    packages= find_packages('stopwords_tr')
+    packages= find_packages('src')
 )
```

### Comparing `stopwords_tr-1.1.8/src/stopwords_tr.egg-info/PKG-INFO` & `stopwords_tr-1.1.9/src/stopwords_tr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.1.8
+Version: 1.1.9
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp, filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
```

