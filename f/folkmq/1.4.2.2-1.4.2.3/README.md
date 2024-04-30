# Comparing `tmp/folkmq-1.4.2.2.tar.gz` & `tmp/folkmq-1.4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folkmq-1.4.2.2.tar", last modified: Mon Apr 29 13:09:00 2024, max compression
+gzip compressed data, was "folkmq-1.4.2.3.tar", last modified: Mon Apr 29 13:40:52 2024, max compression
```

## Comparing `folkmq-1.4.2.2.tar` & `folkmq-1.4.2.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:09:00.342507 folkmq-1.4.2.2/
--rw-r--r--   0 noear      (501) staff       (20)      592 2024-04-29 13:09:00.342098 folkmq-1.4.2.2/PKG-INFO
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:09:00.329183 folkmq-1.4.2.2/folkmq/
--rw-r--r--   0 noear      (501) staff       (20)      504 2024-04-29 12:16:07.000000 folkmq-1.4.2.2/folkmq/FolkMQ.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 09:58:52.000000 folkmq-1.4.2.2/folkmq/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:09:00.336678 folkmq-1.4.2.2/folkmq/client/
--rw-r--r--   0 noear      (501) staff       (20)      163 2024-04-18 13:21:26.000000 folkmq-1.4.2.2/folkmq/client/MqAlarm.py
--rw-r--r--   0 noear      (501) staff       (20)     3746 2024-04-28 14:38:17.000000 folkmq-1.4.2.2/folkmq/client/MqClient.py
--rw-r--r--   0 noear      (501) staff       (20)    13507 2024-04-28 14:39:16.000000 folkmq-1.4.2.2/folkmq/client/MqClientDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     5518 2024-04-29 00:27:34.000000 folkmq-1.4.2.2/folkmq/client/MqClientListener.py
--rw-r--r--   0 noear      (501) staff       (20)     3807 2024-04-28 14:43:14.000000 folkmq-1.4.2.2/folkmq/client/MqMessage.py
--rw-r--r--   0 noear      (501) staff       (20)     3386 2024-04-28 14:55:57.000000 folkmq-1.4.2.2/folkmq/client/MqMessageReceived.py
--rw-r--r--   0 noear      (501) staff       (20)     1091 2024-04-23 13:26:37.000000 folkmq-1.4.2.2/folkmq/client/MqRouter.py
--rw-r--r--   0 noear      (501) staff       (20)      883 2024-04-23 13:35:12.000000 folkmq-1.4.2.2/folkmq/client/MqSubscription.py
--rw-r--r--   0 noear      (501) staff       (20)     1071 2024-04-28 14:37:03.000000 folkmq-1.4.2.2/folkmq/client/MqTransaction.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 09:59:09.000000 folkmq-1.4.2.2/folkmq/client/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:09:00.340755 folkmq-1.4.2.2/folkmq/common/
--rw-r--r--   0 noear      (501) staff       (20)      315 2024-04-18 12:44:59.000000 folkmq-1.4.2.2/folkmq/common/MqApis.py
--rw-r--r--   0 noear      (501) staff       (20)     1054 2024-04-28 12:22:21.000000 folkmq-1.4.2.2/folkmq/common/MqAssert.py
--rw-r--r--   0 noear      (501) staff       (20)     2372 2024-04-18 12:55:36.000000 folkmq-1.4.2.2/folkmq/common/MqConstants.py
--rw-r--r--   0 noear      (501) staff       (20)     2510 2024-04-28 14:52:59.000000 folkmq-1.4.2.2/folkmq/common/MqMetasResolver.py
--rw-r--r--   0 noear      (501) staff       (20)     4772 2024-04-28 14:52:31.000000 folkmq-1.4.2.2/folkmq/common/MqMetasResolverV1.py
--rw-r--r--   0 noear      (501) staff       (20)     4985 2024-04-28 14:52:42.000000 folkmq-1.4.2.2/folkmq/common/MqMetasResolverV2.py
--rw-r--r--   0 noear      (501) staff       (20)      773 2024-04-18 13:07:55.000000 folkmq-1.4.2.2/folkmq/common/MqMetasV1.py
--rw-r--r--   0 noear      (501) staff       (20)      999 2024-04-18 13:09:13.000000 folkmq-1.4.2.2/folkmq/common/MqMetasV2.py
--rw-r--r--   0 noear      (501) staff       (20)      419 2024-04-28 14:12:52.000000 folkmq-1.4.2.2/folkmq/common/MqTopicHelper.py
--rw-r--r--   0 noear      (501) staff       (20)     1178 2024-04-28 14:41:42.000000 folkmq-1.4.2.2/folkmq/common/MqUtils.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 09:59:18.000000 folkmq-1.4.2.2/folkmq/common/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:09:00.341308 folkmq-1.4.2.2/folkmq/exception/
--rw-r--r--   0 noear      (501) staff       (20)      185 2024-04-18 10:00:43.000000 folkmq-1.4.2.2/folkmq/exception/FolkmqException.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 09:59:34.000000 folkmq-1.4.2.2/folkmq/exception/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:09:00.341606 folkmq-1.4.2.2/folkmq.egg-info/
--rw-r--r--   0 noear      (501) staff       (20)      592 2024-04-29 13:09:00.000000 folkmq-1.4.2.2/folkmq.egg-info/PKG-INFO
--rw-r--r--   0 noear      (501) staff       (20)      896 2024-04-29 13:09:00.000000 folkmq-1.4.2.2/folkmq.egg-info/SOURCES.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-29 13:09:00.000000 folkmq-1.4.2.2/folkmq.egg-info/dependency_links.txt
--rw-r--r--   0 noear      (501) staff       (20)       50 2024-04-29 13:09:00.000000 folkmq-1.4.2.2/folkmq.egg-info/requires.txt
--rw-r--r--   0 noear      (501) staff       (20)        7 2024-04-29 13:09:00.000000 folkmq-1.4.2.2/folkmq.egg-info/top_level.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-29 12:33:08.000000 folkmq-1.4.2.2/folkmq.egg-info/zip-safe
--rw-r--r--   0 noear      (501) staff       (20)       38 2024-04-29 13:09:00.342596 folkmq-1.4.2.2/setup.cfg
--rw-r--r--   0 noear      (501) staff       (20)      915 2024-04-29 13:08:51.000000 folkmq-1.4.2.2/setup.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:40:52.588497 folkmq-1.4.2.3/
+-rw-r--r--   0 noear      (501) staff       (20)      592 2024-04-29 13:40:52.588006 folkmq-1.4.2.3/PKG-INFO
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:40:52.575811 folkmq-1.4.2.3/folkmq/
+-rw-r--r--   0 noear      (501) staff       (20)      504 2024-04-29 12:16:07.000000 folkmq-1.4.2.3/folkmq/FolkMQ.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 09:58:52.000000 folkmq-1.4.2.3/folkmq/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:40:52.583771 folkmq-1.4.2.3/folkmq/client/
+-rw-r--r--   0 noear      (501) staff       (20)      163 2024-04-18 13:21:26.000000 folkmq-1.4.2.3/folkmq/client/MqAlarm.py
+-rw-r--r--   0 noear      (501) staff       (20)     3746 2024-04-28 14:38:17.000000 folkmq-1.4.2.3/folkmq/client/MqClient.py
+-rw-r--r--   0 noear      (501) staff       (20)    13507 2024-04-28 14:39:16.000000 folkmq-1.4.2.3/folkmq/client/MqClientDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     5518 2024-04-29 00:27:34.000000 folkmq-1.4.2.3/folkmq/client/MqClientListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     3807 2024-04-28 14:43:14.000000 folkmq-1.4.2.3/folkmq/client/MqMessage.py
+-rw-r--r--   0 noear      (501) staff       (20)     3386 2024-04-28 14:55:57.000000 folkmq-1.4.2.3/folkmq/client/MqMessageReceived.py
+-rw-r--r--   0 noear      (501) staff       (20)     1091 2024-04-23 13:26:37.000000 folkmq-1.4.2.3/folkmq/client/MqRouter.py
+-rw-r--r--   0 noear      (501) staff       (20)      883 2024-04-23 13:35:12.000000 folkmq-1.4.2.3/folkmq/client/MqSubscription.py
+-rw-r--r--   0 noear      (501) staff       (20)     1071 2024-04-28 14:37:03.000000 folkmq-1.4.2.3/folkmq/client/MqTransaction.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 09:59:09.000000 folkmq-1.4.2.3/folkmq/client/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:40:52.586816 folkmq-1.4.2.3/folkmq/common/
+-rw-r--r--   0 noear      (501) staff       (20)      315 2024-04-18 12:44:59.000000 folkmq-1.4.2.3/folkmq/common/MqApis.py
+-rw-r--r--   0 noear      (501) staff       (20)     1054 2024-04-28 12:22:21.000000 folkmq-1.4.2.3/folkmq/common/MqAssert.py
+-rw-r--r--   0 noear      (501) staff       (20)     2372 2024-04-18 12:55:36.000000 folkmq-1.4.2.3/folkmq/common/MqConstants.py
+-rw-r--r--   0 noear      (501) staff       (20)     2510 2024-04-28 14:52:59.000000 folkmq-1.4.2.3/folkmq/common/MqMetasResolver.py
+-rw-r--r--   0 noear      (501) staff       (20)     4772 2024-04-28 14:52:31.000000 folkmq-1.4.2.3/folkmq/common/MqMetasResolverV1.py
+-rw-r--r--   0 noear      (501) staff       (20)     4985 2024-04-28 14:52:42.000000 folkmq-1.4.2.3/folkmq/common/MqMetasResolverV2.py
+-rw-r--r--   0 noear      (501) staff       (20)      773 2024-04-18 13:07:55.000000 folkmq-1.4.2.3/folkmq/common/MqMetasV1.py
+-rw-r--r--   0 noear      (501) staff       (20)      999 2024-04-18 13:09:13.000000 folkmq-1.4.2.3/folkmq/common/MqMetasV2.py
+-rw-r--r--   0 noear      (501) staff       (20)      419 2024-04-28 14:12:52.000000 folkmq-1.4.2.3/folkmq/common/MqTopicHelper.py
+-rw-r--r--   0 noear      (501) staff       (20)     1178 2024-04-28 14:41:42.000000 folkmq-1.4.2.3/folkmq/common/MqUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 09:59:18.000000 folkmq-1.4.2.3/folkmq/common/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:40:52.587249 folkmq-1.4.2.3/folkmq/exception/
+-rw-r--r--   0 noear      (501) staff       (20)      185 2024-04-18 10:00:43.000000 folkmq-1.4.2.3/folkmq/exception/FolkmqException.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 09:59:34.000000 folkmq-1.4.2.3/folkmq/exception/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:40:52.587547 folkmq-1.4.2.3/folkmq.egg-info/
+-rw-r--r--   0 noear      (501) staff       (20)      592 2024-04-29 13:40:52.000000 folkmq-1.4.2.3/folkmq.egg-info/PKG-INFO
+-rw-r--r--   0 noear      (501) staff       (20)      896 2024-04-29 13:40:52.000000 folkmq-1.4.2.3/folkmq.egg-info/SOURCES.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-29 13:40:52.000000 folkmq-1.4.2.3/folkmq.egg-info/dependency_links.txt
+-rw-r--r--   0 noear      (501) staff       (20)       50 2024-04-29 13:40:52.000000 folkmq-1.4.2.3/folkmq.egg-info/requires.txt
+-rw-r--r--   0 noear      (501) staff       (20)        7 2024-04-29 13:40:52.000000 folkmq-1.4.2.3/folkmq.egg-info/top_level.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-29 12:33:08.000000 folkmq-1.4.2.3/folkmq.egg-info/zip-safe
+-rw-r--r--   0 noear      (501) staff       (20)       38 2024-04-29 13:40:52.588603 folkmq-1.4.2.3/setup.cfg
+-rw-r--r--   0 noear      (501) staff       (20)      915 2024-04-29 13:40:36.000000 folkmq-1.4.2.3/setup.py
```

### Comparing `folkmq-1.4.2.2/PKG-INFO` & `folkmq-1.4.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: folkmq
-Version: 1.4.2.2
+Version: 1.4.2.3
 Summary: @noear/folkmq python project
 Home-page: https://folkmq.noear.org/
 Author: noear
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.10
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: websockets>=12.0
-Requires-Dist: socket.d>=2.4.14.1
+Requires-Dist: socket.d>=2.4.14.2
```

### Comparing `folkmq-1.4.2.2/folkmq/client/MqClient.py` & `folkmq-1.4.2.3/folkmq/client/MqClient.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.2.2/folkmq/client/MqClientDefault.py` & `folkmq-1.4.2.3/folkmq/client/MqClientDefault.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.2.2/folkmq/client/MqClientListener.py` & `folkmq-1.4.2.3/folkmq/client/MqClientListener.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.2.2/folkmq/client/MqMessage.py` & `folkmq-1.4.2.3/folkmq/client/MqMessage.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.2.2/folkmq/client/MqMessageReceived.py` & `folkmq-1.4.2.3/folkmq/client/MqMessageReceived.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.2.2/folkmq/client/MqRouter.py` & `folkmq-1.4.2.3/folkmq/client/MqRouter.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.2.2/folkmq/client/MqSubscription.py` & `folkmq-1.4.2.3/folkmq/client/MqSubscription.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.2.2/folkmq/client/MqTransaction.py` & `folkmq-1.4.2.3/folkmq/client/MqTransaction.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.2.2/folkmq/common/MqAssert.py` & `folkmq-1.4.2.3/folkmq/common/MqAssert.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.2.2/folkmq/common/MqConstants.py` & `folkmq-1.4.2.3/folkmq/common/MqConstants.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.2.2/folkmq/common/MqMetasResolver.py` & `folkmq-1.4.2.3/folkmq/common/MqMetasResolver.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.2.2/folkmq/common/MqMetasResolverV1.py` & `folkmq-1.4.2.3/folkmq/common/MqMetasResolverV1.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.2.2/folkmq/common/MqMetasResolverV2.py` & `folkmq-1.4.2.3/folkmq/common/MqMetasResolverV2.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.2.2/folkmq/common/MqMetasV1.py` & `folkmq-1.4.2.3/folkmq/common/MqMetasV1.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.2.2/folkmq/common/MqMetasV2.py` & `folkmq-1.4.2.3/folkmq/common/MqMetasV2.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.2.2/folkmq/common/MqUtils.py` & `folkmq-1.4.2.3/folkmq/common/MqUtils.py`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.2.2/folkmq.egg-info/PKG-INFO` & `folkmq-1.4.2.3/folkmq.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: folkmq
-Version: 1.4.2.2
+Version: 1.4.2.3
 Summary: @noear/folkmq python project
 Home-page: https://folkmq.noear.org/
 Author: noear
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.10
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: websockets>=12.0
-Requires-Dist: socket.d>=2.4.14.1
+Requires-Dist: socket.d>=2.4.14.2
```

### Comparing `folkmq-1.4.2.2/folkmq.egg-info/SOURCES.txt` & `folkmq-1.4.2.3/folkmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `folkmq-1.4.2.2/setup.py` & `folkmq-1.4.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*_
 from setuptools import setup,find_packages
 
 setup(
     name='folkmq',
-    version='1.4.2.2',
+    version='1.4.2.3',
     description='@noear/folkmq python project',
     author='noear',
     url='https://folkmq.noear.org/',
     packages=find_packages(exclude=['*folkmq-test*']),   # 包内不需要引用的文件夹
     install_requires=[                          # 依赖包
         'loguru>=0.7.2',
         'websockets>=12.0',
-        'socket.d>=2.4.14.1'
+        'socket.d>=2.4.14.2'
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
```

