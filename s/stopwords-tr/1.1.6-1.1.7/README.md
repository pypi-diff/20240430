# Comparing `tmp/stopwords_tr-1.1.6.tar.gz` & `tmp/stopwords_tr-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stopwords_tr-1.1.6.tar", last modified: Tue Apr 30 08:03:54 2024, max compression
+gzip compressed data, was "stopwords_tr-1.1.7.tar", last modified: Tue Apr 30 08:06:20 2024, max compression
```

## Comparing `stopwords_tr-1.1.6.tar` & `stopwords_tr-1.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 08:03:54.838303 stopwords_tr-1.1.6/
--rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.1.6/LICENSE
--rw-rw-rw-   0        0        0     1051 2024-04-30 08:03:54.837303 stopwords_tr-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.1.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-30 08:03:54.838303 stopwords_tr-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1329 2024-04-30 08:03:35.000000 stopwords_tr-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:03:54.828303 stopwords_tr-1.1.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-30 08:03:54.836302 stopwords_tr-1.1.6/src/stopwords_tr.egg-info/
--rw-rw-rw-   0        0        0     1051 2024-04-30 08:03:54.000000 stopwords_tr-1.1.6/src/stopwords_tr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-04-30 08:03:54.000000 stopwords_tr-1.1.6/src/stopwords_tr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 08:03:54.000000 stopwords_tr-1.1.6/src/stopwords_tr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 08:03:54.000000 stopwords_tr-1.1.6/src/stopwords_tr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 08:06:20.596233 stopwords_tr-1.1.7/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0     1051 2024-04-30 08:06:20.595233 stopwords_tr-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-30 08:06:20.596233 stopwords_tr-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1291 2024-04-30 08:06:06.000000 stopwords_tr-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:06:20.587232 stopwords_tr-1.1.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-30 08:06:20.594231 stopwords_tr-1.1.7/src/stopwords_tr.egg-info/
+-rw-rw-rw-   0        0        0     1051 2024-04-30 08:06:20.000000 stopwords_tr-1.1.7/src/stopwords_tr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2024-04-30 08:06:20.000000 stopwords_tr-1.1.7/src/stopwords_tr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 08:06:20.000000 stopwords_tr-1.1.7/src/stopwords_tr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 08:06:20.000000 stopwords_tr-1.1.7/src/stopwords_tr.egg-info/top_level.txt
```

### Comparing `stopwords_tr-1.1.6/LICENSE` & `stopwords_tr-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stopwords_tr-1.1.6/PKG-INFO` & `stopwords_tr-1.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.1.6
+Version: 1.1.7
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp, filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stopwords_tr-1.1.6/setup.py` & `stopwords_tr-1.1.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name= 'stopwords_tr',
-    version='1.1.6',
+    version='1.1.7',
     license='MIT',
     author="Metin Oktay DENIZ",
     author_email='metinoktaydenizz@gmail.com',
     description="Stopwords filter for Turkish languages",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     url='https://github.com/metinoktayd/StopWords-Turkish-Language',
@@ -26,10 +26,9 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12'
     ],
     #py_modules=["stopwords_tr"]
     package_dir={'':'src'},
-    package_data={'src':['data/*']},
     packages= find_packages()
 )
```

### Comparing `stopwords_tr-1.1.6/src/stopwords_tr.egg-info/PKG-INFO` & `stopwords_tr-1.1.7/src/stopwords_tr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.1.6
+Version: 1.1.7
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp, filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
```

