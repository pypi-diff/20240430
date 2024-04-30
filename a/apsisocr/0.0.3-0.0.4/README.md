# Comparing `tmp/apsisocr-0.0.3.tar.gz` & `tmp/apsisocr-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apsisocr-0.0.3.tar", last modified: Sun Nov  5 15:29:40 2023, max compression
+gzip compressed data, was "apsisocr-0.0.4.tar", last modified: Tue Apr 30 18:58:04 2024, max compression
```

## Comparing `apsisocr-0.0.3.tar` & `apsisocr-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2023-11-05 15:29:40.817262 apsisocr-0.0.3/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)      244 2023-11-05 15:27:50.000000 apsisocr-0.0.3/CHANGELOG.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)       25 2023-04-15 06:54:42.000000 apsisocr-0.0.3/MANIFEST.in
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     7045 2023-11-05 15:29:40.817262 apsisocr-0.0.3/PKG-INFO
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     6217 2023-10-23 03:00:38.000000 apsisocr-0.0.3/README.md
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2023-11-05 15:29:40.817262 apsisocr-0.0.3/apsisocr/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)      182 2023-11-05 15:15:02.000000 apsisocr-0.0.3/apsisocr/__init__.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     6050 2023-09-16 14:32:45.000000 apsisocr-0.0.3/apsisocr/apsisnet.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     4042 2023-11-05 15:15:48.000000 apsisocr-0.0.3/apsisocr/base.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     4206 2023-09-16 14:33:05.000000 apsisocr-0.0.3/apsisocr/densenet121bnencls.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)      891 2023-09-16 14:33:19.000000 apsisocr-0.0.3/apsisocr/modules.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     8156 2023-11-05 08:44:48.000000 apsisocr-0.0.3/apsisocr/ocr.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     8331 2023-11-05 08:44:26.000000 apsisocr-0.0.3/apsisocr/paddledbnet.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     3309 2023-09-16 14:33:43.000000 apsisocr-0.0.3/apsisocr/paddlesvtr.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     9509 2023-09-16 14:33:53.000000 apsisocr-0.0.3/apsisocr/utils.py
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2023-11-05 15:29:40.817262 apsisocr-0.0.3/apsisocr.egg-info/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     7045 2023-11-05 15:29:40.000000 apsisocr-0.0.3/apsisocr.egg-info/PKG-INFO
--rw-rw-r--   0 ansary    (1000) ansary    (1000)      500 2023-11-05 15:29:40.000000 apsisocr-0.0.3/apsisocr.egg-info/SOURCES.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)        1 2023-11-05 15:29:40.000000 apsisocr-0.0.3/apsisocr.egg-info/dependency_links.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)      106 2023-11-05 15:29:40.000000 apsisocr-0.0.3/apsisocr.egg-info/requires.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)        9 2023-11-05 15:29:40.000000 apsisocr-0.0.3/apsisocr.egg-info/top_level.txt
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2023-11-05 15:29:40.817262 apsisocr-0.0.3/deployment/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     3422 2023-11-05 15:17:51.000000 apsisocr-0.0.3/deployment/api_base.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     3414 2023-09-24 12:22:48.000000 apsisocr-0.0.3/deployment/api_ocr.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     2930 2023-09-24 12:35:48.000000 apsisocr-0.0.3/deployment/app.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)      209 2023-11-05 15:18:05.000000 apsisocr-0.0.3/deployment/config.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)       38 2023-11-05 15:29:40.817262 apsisocr-0.0.3/setup.cfg
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     1379 2023-11-05 15:27:21.000000 apsisocr-0.0.3/setup.py
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2023-11-05 15:29:40.817262 apsisocr-0.0.3/useage/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)      478 2023-09-24 12:58:26.000000 apsisocr-0.0.3/useage/setup_check.py
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-04-30 18:58:04.214517 apsisocr-0.0.4/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)      296 2024-04-30 18:30:24.000000 apsisocr-0.0.4/CHANGELOG.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)       25 2023-04-15 06:54:42.000000 apsisocr-0.0.4/MANIFEST.in
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     7098 2024-04-30 18:58:04.214517 apsisocr-0.0.4/PKG-INFO
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     6217 2023-10-23 03:00:38.000000 apsisocr-0.0.4/README.md
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-04-30 18:58:04.214517 apsisocr-0.0.4/apsisocr/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)      213 2024-04-30 18:27:35.000000 apsisocr-0.0.4/apsisocr/__init__.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     6050 2023-09-16 14:32:45.000000 apsisocr-0.0.4/apsisocr/apsisnet.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     4042 2023-11-05 15:15:48.000000 apsisocr-0.0.4/apsisocr/base.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     6987 2024-04-30 18:56:18.000000 apsisocr-0.0.4/apsisocr/bnocr.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     4206 2023-09-16 14:33:05.000000 apsisocr-0.0.4/apsisocr/densenet121bnencls.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)      891 2023-09-16 14:33:19.000000 apsisocr-0.0.4/apsisocr/modules.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     8156 2023-11-05 08:44:48.000000 apsisocr-0.0.4/apsisocr/ocr.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     8331 2023-11-05 08:44:26.000000 apsisocr-0.0.4/apsisocr/paddledbnet.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     3309 2023-09-16 14:33:43.000000 apsisocr-0.0.4/apsisocr/paddlesvtr.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     9509 2023-09-16 14:33:53.000000 apsisocr-0.0.4/apsisocr/utils.py
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-04-30 18:58:04.214517 apsisocr-0.0.4/apsisocr.egg-info/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     7098 2024-04-30 18:58:04.000000 apsisocr-0.0.4/apsisocr.egg-info/PKG-INFO
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)      518 2024-04-30 18:58:04.000000 apsisocr-0.0.4/apsisocr.egg-info/SOURCES.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)        1 2024-04-30 18:58:04.000000 apsisocr-0.0.4/apsisocr.egg-info/dependency_links.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)      106 2024-04-30 18:58:04.000000 apsisocr-0.0.4/apsisocr.egg-info/requires.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)        9 2024-04-30 18:58:04.000000 apsisocr-0.0.4/apsisocr.egg-info/top_level.txt
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-04-30 18:58:04.214517 apsisocr-0.0.4/deployment/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     3422 2023-11-05 15:17:51.000000 apsisocr-0.0.4/deployment/api_base.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     3414 2023-09-24 12:22:48.000000 apsisocr-0.0.4/deployment/api_ocr.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     2930 2023-09-24 12:35:48.000000 apsisocr-0.0.4/deployment/app.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)      209 2023-11-05 15:18:05.000000 apsisocr-0.0.4/deployment/config.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)       38 2024-04-30 18:58:04.214517 apsisocr-0.0.4/setup.cfg
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     1379 2024-04-30 18:29:53.000000 apsisocr-0.0.4/setup.py
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-04-30 18:58:04.214517 apsisocr-0.0.4/useage/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)      478 2023-09-24 12:58:26.000000 apsisocr-0.0.4/useage/setup_check.py
```

### Comparing `apsisocr-0.0.3/PKG-INFO` & `apsisocr-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apsisocr
-Version: 0.0.3
+Version: 0.0.4
 Summary: Bangla English Mixed Languge Scene / printed OCR Toolkit
 Home-page: https://github.com/mnansary/apsis-ocr/
 Author: Nazmuddoha Ansary
 Author-email: nazmuddoha.ansary@apsissolutions.com
 License: MIT
 Keywords: ocr,multilingual-ocr,scene ocr,apsisnet
 Classifier: Development Status :: 3 - Alpha
@@ -278,7 +278,11 @@
 0.0.2 (24/09/2023)
 -------------------
 - added liscencing
 
 0.0.3 (05/11/2023)
 -------------------
 - added base application without line and word number
+
+0.0.4 (01/05/2024)
+-------------------
+- apsisbnocr
```

### Comparing `apsisocr-0.0.3/README.md` & `apsisocr-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `apsisocr-0.0.3/apsisocr/apsisnet.py` & `apsisocr-0.0.4/apsisocr/apsisnet.py`

 * *Files identical despite different names*

### Comparing `apsisocr-0.0.3/apsisocr/base.py` & `apsisocr-0.0.4/apsisocr/base.py`

 * *Files identical despite different names*

### Comparing `apsisocr-0.0.3/apsisocr/densenet121bnencls.py` & `apsisocr-0.0.4/apsisocr/densenet121bnencls.py`

 * *Files identical despite different names*

### Comparing `apsisocr-0.0.3/apsisocr/modules.py` & `apsisocr-0.0.4/apsisocr/modules.py`

 * *Files identical despite different names*

### Comparing `apsisocr-0.0.3/apsisocr/ocr.py` & `apsisocr-0.0.4/apsisocr/ocr.py`

 * *Files identical despite different names*

### Comparing `apsisocr-0.0.3/apsisocr/paddledbnet.py` & `apsisocr-0.0.4/apsisocr/paddledbnet.py`

 * *Files identical despite different names*

### Comparing `apsisocr-0.0.3/apsisocr/paddlesvtr.py` & `apsisocr-0.0.4/apsisocr/paddlesvtr.py`

 * *Files identical despite different names*

### Comparing `apsisocr-0.0.3/apsisocr/utils.py` & `apsisocr-0.0.4/apsisocr/utils.py`

 * *Files identical despite different names*

### Comparing `apsisocr-0.0.3/apsisocr.egg-info/PKG-INFO` & `apsisocr-0.0.4/apsisocr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apsisocr
-Version: 0.0.3
+Version: 0.0.4
 Summary: Bangla English Mixed Languge Scene / printed OCR Toolkit
 Home-page: https://github.com/mnansary/apsis-ocr/
 Author: Nazmuddoha Ansary
 Author-email: nazmuddoha.ansary@apsissolutions.com
 License: MIT
 Keywords: ocr,multilingual-ocr,scene ocr,apsisnet
 Classifier: Development Status :: 3 - Alpha
@@ -278,7 +278,11 @@
 0.0.2 (24/09/2023)
 -------------------
 - added liscencing
 
 0.0.3 (05/11/2023)
 -------------------
 - added base application without line and word number
+
+0.0.4 (01/05/2024)
+-------------------
+- apsisbnocr
```

### Comparing `apsisocr-0.0.3/deployment/api_base.py` & `apsisocr-0.0.4/deployment/api_base.py`

 * *Files identical despite different names*

### Comparing `apsisocr-0.0.3/deployment/api_ocr.py` & `apsisocr-0.0.4/deployment/api_ocr.py`

 * *Files identical despite different names*

### Comparing `apsisocr-0.0.3/deployment/app.py` & `apsisocr-0.0.4/deployment/app.py`

 * *Files identical despite different names*

### Comparing `apsisocr-0.0.3/setup.py` & `apsisocr-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   'Operating System :: POSIX :: Linux',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='apsisocr',
-  version='0.0.3',
+  version='0.0.4',
   description='Bangla English Mixed Languge Scene / printed OCR Toolkit',
   long_description=open('README.md',encoding='utf-8').read() + '\n\n' + open('CHANGELOG.txt',encoding='utf-8').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/mnansary/apsis-ocr/',  
   author='Nazmuddoha Ansary',
   author_email='nazmuddoha.ansary@apsissolutions.com',
   license='MIT',
```

