# Comparing `tmp/stopwords_tr-1.1.4.tar.gz` & `tmp/stopwords_tr-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stopwords_tr-1.1.4.tar", last modified: Tue Apr 30 07:35:48 2024, max compression
+gzip compressed data, was "stopwords_tr-1.1.5.tar", last modified: Tue Apr 30 07:51:45 2024, max compression
```

## Comparing `stopwords_tr-1.1.4.tar` & `stopwords_tr-1.1.5.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 07:35:48.584943 stopwords_tr-1.1.4/
--rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.1.4/LICENSE
--rw-rw-rw-   0        0        0     1051 2024-04-30 07:35:48.583946 stopwords_tr-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-30 07:35:48.584943 stopwords_tr-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1296 2024-04-30 07:35:34.000000 stopwords_tr-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 07:35:48.573943 stopwords_tr-1.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-30 07:35:48.577942 stopwords_tr-1.1.4/src/stopwords_tr/
--rw-rw-rw-   0        0        0      160 2024-04-30 07:34:51.000000 stopwords_tr-1.1.4/src/stopwords_tr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 07:35:48.582942 stopwords_tr-1.1.4/src/stopwords_tr.egg-info/
--rw-rw-rw-   0        0        0     1051 2024-04-30 07:35:48.000000 stopwords_tr-1.1.4/src/stopwords_tr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-04-30 07:35:48.000000 stopwords_tr-1.1.4/src/stopwords_tr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 07:35:48.000000 stopwords_tr-1.1.4/src/stopwords_tr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-30 07:35:48.000000 stopwords_tr-1.1.4/src/stopwords_tr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 07:51:45.263182 stopwords_tr-1.1.5/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1051 2024-04-30 07:51:45.263182 stopwords_tr-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-30 07:51:45.263182 stopwords_tr-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1355 2024-04-30 07:50:32.000000 stopwords_tr-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 07:51:45.252181 stopwords_tr-1.1.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-30 07:51:45.253181 stopwords_tr-1.1.5/src/stopwords_tr/
+drwxrwxrwx   0        0        0        0 2024-04-30 07:51:45.262183 stopwords_tr-1.1.5/src/stopwords_tr/stopwords_tr.egg-info/
+-rw-rw-rw-   0        0        0     1051 2024-04-30 07:51:45.000000 stopwords_tr-1.1.5/src/stopwords_tr/stopwords_tr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-04-30 07:51:45.000000 stopwords_tr-1.1.5/src/stopwords_tr/stopwords_tr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 07:51:45.000000 stopwords_tr-1.1.5/src/stopwords_tr/stopwords_tr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 07:51:45.000000 stopwords_tr-1.1.5/src/stopwords_tr/stopwords_tr.egg-info/top_level.txt
```

### Comparing `stopwords_tr-1.1.4/LICENSE` & `stopwords_tr-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `stopwords_tr-1.1.4/PKG-INFO` & `stopwords_tr-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.1.4
+Version: 1.1.5
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp, filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stopwords_tr-1.1.4/setup.py` & `stopwords_tr-1.1.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name= 'stopwords_tr',
-    version='1.1.4',
+    version='1.1.5',
     license='MIT',
     author="Metin Oktay DENIZ",
     author_email='metinoktaydenizz@gmail.com',
     description="Stopwords filter for Turkish languages",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     url='https://github.com/metinoktayd/StopWords-Turkish-Language',
@@ -25,10 +25,11 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12'
     ],
     #py_modules=["stopwords_tr"]
-    package_dir={'':'src'},
-    packages= find_packages("src")
+    package_dir={'':'src/stopwords_tr'},
+    package_data={'src/stopwords_tr':['data/*']},
+    packages= find_packages()
 )
```

### Comparing `stopwords_tr-1.1.4/src/stopwords_tr.egg-info/PKG-INFO` & `stopwords_tr-1.1.5/src/stopwords_tr/stopwords_tr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.1.4
+Version: 1.1.5
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp, filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
```

