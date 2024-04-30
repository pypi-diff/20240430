# Comparing `tmp/pybangla-0.0.1.tar.gz` & `tmp/pybangla-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybangla-0.0.1.tar", last modified: Tue Apr 30 06:50:16 2024, max compression
+gzip compressed data, was "pybangla-0.0.2.tar", last modified: Tue Apr 30 17:37:02 2024, max compression
```

## Comparing `pybangla-0.0.1.tar` & `pybangla-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 gspc      (1000) gspc      (1000)        0 2024-04-30 06:50:16.640484 pybangla-0.0.1/
--rw-rw-r--   0 gspc      (1000) gspc      (1000)        0 2024-04-29 18:00:46.000000 pybangla-0.0.1/MANIFEST.in
--rw-rw-r--   0 gspc      (1000) gspc      (1000)    13652 2024-04-30 06:50:16.640484 pybangla-0.0.1/PKG-INFO
--rw-rw-r--   0 gspc      (1000) gspc      (1000)    13218 2024-04-30 06:28:20.000000 pybangla-0.0.1/README.md
-drwxrwxr-x   0 gspc      (1000) gspc      (1000)        0 2024-04-30 06:50:16.632484 pybangla-0.0.1/pybangla/
--rw-rw-r--   0 gspc      (1000) gspc      (1000)       66 2024-04-29 18:00:46.000000 pybangla-0.0.1/pybangla/__init__.py
-drwxrwxr-x   0 gspc      (1000) gspc      (1000)        0 2024-04-30 06:50:16.636484 pybangla-0.0.1/pybangla/module/
--rw-rw-r--   0 gspc      (1000) gspc      (1000)        0 2024-04-29 18:00:46.000000 pybangla-0.0.1/pybangla/module/__init__.py
--rw-rw-r--   0 gspc      (1000) gspc      (1000)    16862 2024-04-30 04:48:35.000000 pybangla-0.0.1/pybangla/module/config.py
--rw-rw-r--   0 gspc      (1000) gspc      (1000)     9002 2024-04-30 04:31:39.000000 pybangla-0.0.1/pybangla/module/main.py
--rw-rw-r--   0 gspc      (1000) gspc      (1000)    16398 2024-04-29 18:00:46.000000 pybangla-0.0.1/pybangla/module/number_parser.py
--rw-rw-r--   0 gspc      (1000) gspc      (1000)    15187 2024-04-29 18:00:46.000000 pybangla-0.0.1/pybangla/module/parser.py
--rw-rw-r--   0 gspc      (1000) gspc      (1000)    22922 2024-04-29 18:00:46.000000 pybangla-0.0.1/pybangla/module/word_to_number.py
--rw-rw-r--   0 gspc      (1000) gspc      (1000)     8917 2024-04-30 06:18:16.000000 pybangla-0.0.1/pybangla/test.py
-drwxrwxr-x   0 gspc      (1000) gspc      (1000)        0 2024-04-30 06:50:16.636484 pybangla-0.0.1/pybangla.egg-info/
--rw-rw-r--   0 gspc      (1000) gspc      (1000)    13652 2024-04-30 06:50:16.000000 pybangla-0.0.1/pybangla.egg-info/PKG-INFO
--rw-rw-r--   0 gspc      (1000) gspc      (1000)      422 2024-04-30 06:50:16.000000 pybangla-0.0.1/pybangla.egg-info/SOURCES.txt
--rw-rw-r--   0 gspc      (1000) gspc      (1000)        1 2024-04-30 06:50:16.000000 pybangla-0.0.1/pybangla.egg-info/dependency_links.txt
--rw-rw-r--   0 gspc      (1000) gspc      (1000)       19 2024-04-30 06:50:16.000000 pybangla-0.0.1/pybangla.egg-info/requires.txt
--rw-rw-r--   0 gspc      (1000) gspc      (1000)        9 2024-04-30 06:50:16.000000 pybangla-0.0.1/pybangla.egg-info/top_level.txt
--rw-rw-r--   0 gspc      (1000) gspc      (1000)       38 2024-04-30 06:50:16.640484 pybangla-0.0.1/setup.cfg
--rw-rw-r--   0 gspc      (1000) gspc      (1000)      865 2024-04-29 18:00:46.000000 pybangla-0.0.1/setup.py
-drwxrwxr-x   0 gspc      (1000) gspc      (1000)        0 2024-04-30 06:50:16.640484 pybangla-0.0.1/tests/
--rw-rw-r--   0 gspc      (1000) gspc      (1000)     2751 2024-04-29 18:00:46.000000 pybangla-0.0.1/tests/test.py
+drwxrwxr-x   0 sayan     (1000) sayan     (1000)        0 2024-04-30 17:37:02.321241 pybangla-0.0.2/
+-rw-rw-r--   0 sayan     (1000) sayan     (1000)        0 2024-04-30 17:27:19.000000 pybangla-0.0.2/MANIFEST.in
+-rw-rw-r--   0 sayan     (1000) sayan     (1000)    13705 2024-04-30 17:37:02.321241 pybangla-0.0.2/PKG-INFO
+-rw-rw-r--   0 sayan     (1000) sayan     (1000)    13196 2024-04-30 17:31:39.000000 pybangla-0.0.2/README.md
+drwxrwxr-x   0 sayan     (1000) sayan     (1000)        0 2024-04-30 17:37:02.321241 pybangla-0.0.2/pybangla/
+-rw-rw-r--   0 sayan     (1000) sayan     (1000)       66 2024-04-30 17:27:19.000000 pybangla-0.0.2/pybangla/__init__.py
+drwxrwxr-x   0 sayan     (1000) sayan     (1000)        0 2024-04-30 17:37:02.321241 pybangla-0.0.2/pybangla/module/
+-rw-rw-r--   0 sayan     (1000) sayan     (1000)        0 2024-04-30 17:27:19.000000 pybangla-0.0.2/pybangla/module/__init__.py
+-rw-rw-r--   0 sayan     (1000) sayan     (1000)    16979 2024-04-30 17:31:06.000000 pybangla-0.0.2/pybangla/module/config.py
+-rw-rw-r--   0 sayan     (1000) sayan     (1000)     9002 2024-04-30 17:27:19.000000 pybangla-0.0.2/pybangla/module/main.py
+-rw-rw-r--   0 sayan     (1000) sayan     (1000)    16398 2024-04-30 17:27:19.000000 pybangla-0.0.2/pybangla/module/number_parser.py
+-rw-rw-r--   0 sayan     (1000) sayan     (1000)    15187 2024-04-30 17:27:19.000000 pybangla-0.0.2/pybangla/module/parser.py
+-rw-rw-r--   0 sayan     (1000) sayan     (1000)    22922 2024-04-30 17:27:19.000000 pybangla-0.0.2/pybangla/module/word_to_number.py
+-rw-rw-r--   0 sayan     (1000) sayan     (1000)     8917 2024-04-30 17:27:19.000000 pybangla-0.0.2/pybangla/test.py
+drwxrwxr-x   0 sayan     (1000) sayan     (1000)        0 2024-04-30 17:37:02.321241 pybangla-0.0.2/pybangla.egg-info/
+-rw-rw-r--   0 sayan     (1000) sayan     (1000)    13705 2024-04-30 17:37:02.000000 pybangla-0.0.2/pybangla.egg-info/PKG-INFO
+-rw-rw-r--   0 sayan     (1000) sayan     (1000)      422 2024-04-30 17:37:02.000000 pybangla-0.0.2/pybangla.egg-info/SOURCES.txt
+-rw-rw-r--   0 sayan     (1000) sayan     (1000)        1 2024-04-30 17:37:02.000000 pybangla-0.0.2/pybangla.egg-info/dependency_links.txt
+-rw-rw-r--   0 sayan     (1000) sayan     (1000)       19 2024-04-30 17:37:02.000000 pybangla-0.0.2/pybangla.egg-info/requires.txt
+-rw-rw-r--   0 sayan     (1000) sayan     (1000)        9 2024-04-30 17:37:02.000000 pybangla-0.0.2/pybangla.egg-info/top_level.txt
+-rw-rw-r--   0 sayan     (1000) sayan     (1000)       38 2024-04-30 17:37:02.321241 pybangla-0.0.2/setup.cfg
+-rw-rw-r--   0 sayan     (1000) sayan     (1000)      940 2024-04-30 17:35:35.000000 pybangla-0.0.2/setup.py
+drwxrwxr-x   0 sayan     (1000) sayan     (1000)        0 2024-04-30 17:37:02.321241 pybangla-0.0.2/tests/
+-rw-rw-r--   0 sayan     (1000) sayan     (1000)     2751 2024-04-30 17:27:19.000000 pybangla-0.0.2/tests/test.py
```

### Comparing `pybangla-0.0.1/PKG-INFO` & `pybangla-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 0.0.1
-Summary: date and number digits convert to bangla digits
+Version: 0.0.2
+Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# Project Description
 
 PYBANGLA is a python3 package for Bengala Number, DateTime and Text Normalizer. This package can be used Normalize the text number and date (ex: number to text vice versa). This framework  also can be used Django, Flask, FastAPI, and others. PYBANGLA module supported operating system Linux/Unix, Mac OS and Windows.
 Available Features
 
 Features available in PYBANGLA:
 
 1. Text Normalization
```

### Comparing `pybangla-0.0.1/README.md` & `pybangla-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Project Description
 
 PYBANGLA is a python3 package for Bengala Number, DateTime and Text Normalizer. This package can be used Normalize the text number and date (ex: number to text vice versa). This framework  also can be used Django, Flask, FastAPI, and others. PYBANGLA module supported operating system Linux/Unix, Mac OS and Windows.
 Available Features
 
 Features available in PYBANGLA:
 
 1. Text Normalization
```

### Comparing `pybangla-0.0.1/pybangla/module/config.py` & `pybangla-0.0.2/pybangla/module/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,18 @@
     en_number_mapping = {"জিরো": "0" ,"ওয়ান": "1", "টু": "2", "থ্রি":"3", "ফোর":"4", "ফাইভ":"5", "সিক্স":"6", "সেভেন":"7", "এইট":"8", "নাইন":"9", "টেন": "10"}
 
     en_doshok_map = {
         'ইলেভেন':"11", 'টুয়েলভ':"12", 'থার্টিন':"13", 'ফোরটিন':"14", 'ফিফটিন':"15", 'সিক্সটিন':"16", 'সেভেনটিন':"17", 'এইটিন':"18", 
         'নাইনটিন':"19","টুয়েন্টি": "20", "থার্টি": "30", "ফর্টি":"40", "ফিফ্টি": "50", "সিক্সটি": "60", "সেভেন্টি":"70", "এটি": "80", "নাইনটি":"90"
         }
 
-    fraction_int = {"ডেরশ": "150", "দেরশ": "150", "আরাইশ": "250", "আড়াইশ": "250"}
+    fraction_int = {"ডেরশ": "150", "দেড়শো":"150", "দেড়শত":"150", "দেরশ": "150", "আরাইশ": "250", "আড়াইশ": "250", "আরাইশো" : "250", "আড়াইশত": "250" }
+
+    
+
 
     function_mapping = {
                     "সাড়ে" : "equation_of_sare_and_der", "সারে": "equation_of_sare_and_der", "আড়াই": "equation_of_arai", 
                     "আরাই": "equation_of_arai", "দেড়": "equation_of_sare_and_der", "দের" : "equation_of_sare_and_der"
                     }
 
     bn_hundreds_2 = {i.replace(i[-1], "শত"): v for i, v in bn_hundreds_1.items()}
```

### Comparing `pybangla-0.0.1/pybangla/module/main.py` & `pybangla-0.0.2/pybangla/module/main.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.1/pybangla/module/number_parser.py` & `pybangla-0.0.2/pybangla/module/number_parser.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.1/pybangla/module/parser.py` & `pybangla-0.0.2/pybangla/module/parser.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.1/pybangla/module/word_to_number.py` & `pybangla-0.0.2/pybangla/module/word_to_number.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.1/pybangla/test.py` & `pybangla-0.0.2/pybangla/test.py`

 * *Files identical despite different names*

### Comparing `pybangla-0.0.1/pybangla.egg-info/PKG-INFO` & `pybangla-0.0.2/pybangla.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 0.0.1
-Summary: date and number digits convert to bangla digits
+Version: 0.0.2
+Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# Project Description
 
 PYBANGLA is a python3 package for Bengala Number, DateTime and Text Normalizer. This package can be used Normalize the text number and date (ex: number to text vice versa). This framework  also can be used Django, Flask, FastAPI, and others. PYBANGLA module supported operating system Linux/Unix, Mac OS and Windows.
 Available Features
 
 Features available in PYBANGLA:
 
 1. Text Normalization
```

### Comparing `pybangla-0.0.1/setup.py` & `pybangla-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 
 import codecs
 from setuptools import setup, find_packages
 
 setup(
     name='pybangla',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     # entry_points={
     #     'console_scripts': [
     #         'pybangla = pybangla.main:Normalizer'
     #     ]
     # },
     author='saiful',
     author_email='saifulbrur79@gmail.com',
-    description='date and number digits convert to bangla digits',
+    description='pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes',
 
     long_description=codecs.open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     
     url='https://github.com/saiful9379/pybangla',
     license='MIT',
     classifiers = [
```

### Comparing `pybangla-0.0.1/tests/test.py` & `pybangla-0.0.2/tests/test.py`

 * *Files identical despite different names*

