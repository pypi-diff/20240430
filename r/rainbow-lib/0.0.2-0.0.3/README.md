# Comparing `tmp/rainbow_lib-0.0.2.tar.gz` & `tmp/rainbow_lib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rainbow_lib-0.0.2.tar", last modified: Tue Apr 30 10:10:53 2024, max compression
+gzip compressed data, was "dist/rainbow_lib-0.0.3.tar", last modified: Tue Apr 30 10:22:18 2024, max compression
```

## Comparing `rainbow_lib-0.0.2.tar` & `rainbow_lib-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 kylinmiao  (1158) users      (100)        0 2024-04-30 10:10:53.000000 rainbow_lib-0.0.2/
-drwxrwxrwx   0 kylinmiao  (1158) users      (100)        0 2024-04-30 10:10:53.000000 rainbow_lib-0.0.2/rainbow_lib.egg-info/
--rw-rw-rw-   0 kylinmiao  (1158) users      (100)       37 2024-04-30 10:10:53.000000 rainbow_lib-0.0.2/rainbow_lib.egg-info/requires.txt
--rw-rw-rw-   0 kylinmiao  (1158) users      (100)      261 2024-04-30 10:10:53.000000 rainbow_lib-0.0.2/rainbow_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0 kylinmiao  (1158) users      (100)       12 2024-04-30 10:10:53.000000 rainbow_lib-0.0.2/rainbow_lib.egg-info/top_level.txt
--rw-rw-rw-   0 kylinmiao  (1158) users      (100)      427 2024-04-30 10:10:53.000000 rainbow_lib-0.0.2/rainbow_lib.egg-info/PKG-INFO
--rw-rw-rw-   0 kylinmiao  (1158) users      (100)       81 2024-04-30 10:10:53.000000 rainbow_lib-0.0.2/rainbow_lib.egg-info/dependency_links.txt
--rw-r--r--   0 kylinmiao  (1158) users      (100)        0 2024-04-29 12:12:00.000000 rainbow_lib-0.0.2/README.md
--rw-r--r--   0 kylinmiao  (1158) users      (100)      891 2024-04-30 10:10:51.000000 rainbow_lib-0.0.2/setup.py
-drwxrwxrwx   0 kylinmiao  (1158) users      (100)        0 2024-04-30 10:10:53.000000 rainbow_lib-0.0.2/rainbow_lib/
--rw-r--r--   0 kylinmiao  (1158) users      (100)    10672 2024-04-30 09:58:02.000000 rainbow_lib-0.0.2/rainbow_lib/wrapper.py
--rw-r--r--   0 kylinmiao  (1158) users      (100)     1273 2024-04-30 08:57:15.000000 rainbow_lib-0.0.2/rainbow_lib/client.py
--rw-r--r--   0 kylinmiao  (1158) users      (100)      123 2024-04-30 09:57:40.000000 rainbow_lib-0.0.2/rainbow_lib/__init__.py
--rw-rw-rw-   0 kylinmiao  (1158) users      (100)       38 2024-04-30 10:10:53.000000 rainbow_lib-0.0.2/setup.cfg
--rw-rw-rw-   0 kylinmiao  (1158) users      (100)      427 2024-04-30 10:10:53.000000 rainbow_lib-0.0.2/PKG-INFO
+drwxrwxrwx   0 kylinmiao  (1158) users      (100)        0 2024-04-30 10:22:18.000000 rainbow_lib-0.0.3/
+drwxrwxrwx   0 kylinmiao  (1158) users      (100)        0 2024-04-30 10:22:18.000000 rainbow_lib-0.0.3/rainbow_lib.egg-info/
+-rw-rw-rw-   0 kylinmiao  (1158) users      (100)       37 2024-04-30 10:22:18.000000 rainbow_lib-0.0.3/rainbow_lib.egg-info/requires.txt
+-rw-rw-rw-   0 kylinmiao  (1158) users      (100)      261 2024-04-30 10:22:18.000000 rainbow_lib-0.0.3/rainbow_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0 kylinmiao  (1158) users      (100)       12 2024-04-30 10:22:18.000000 rainbow_lib-0.0.3/rainbow_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 kylinmiao  (1158) users      (100)      427 2024-04-30 10:22:18.000000 rainbow_lib-0.0.3/rainbow_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0 kylinmiao  (1158) users      (100)       81 2024-04-30 10:22:18.000000 rainbow_lib-0.0.3/rainbow_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 kylinmiao  (1158) users      (100)        0 2024-04-29 12:12:00.000000 rainbow_lib-0.0.3/README.md
+-rw-r--r--   0 kylinmiao  (1158) users      (100)      886 2024-04-30 10:22:07.000000 rainbow_lib-0.0.3/setup.py
+drwxrwxrwx   0 kylinmiao  (1158) users      (100)        0 2024-04-30 10:22:18.000000 rainbow_lib-0.0.3/rainbow_lib/
+-rw-r--r--   0 kylinmiao  (1158) users      (100)    10672 2024-04-30 09:58:02.000000 rainbow_lib-0.0.3/rainbow_lib/wrapper.py
+-rw-r--r--   0 kylinmiao  (1158) users      (100)     1273 2024-04-30 08:57:15.000000 rainbow_lib-0.0.3/rainbow_lib/client.py
+-rw-r--r--   0 kylinmiao  (1158) users      (100)      123 2024-04-30 09:57:40.000000 rainbow_lib-0.0.3/rainbow_lib/__init__.py
+-rw-rw-rw-   0 kylinmiao  (1158) users      (100)       38 2024-04-30 10:22:18.000000 rainbow_lib-0.0.3/setup.cfg
+-rw-rw-rw-   0 kylinmiao  (1158) users      (100)      427 2024-04-30 10:22:18.000000 rainbow_lib-0.0.3/PKG-INFO
```

### Comparing `rainbow_lib-0.0.2/setup.py` & `rainbow_lib-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rainbow_lib',
-    version='0.0.2',
+    version='0.0.3',
     # 自动查找项目中的所有包
     packages=find_packages(exclude=['tests', 'tests.*', 'config.ini']),
     install_requires=[
-      'rainbow-cpp-sdk>=4.1.0',
+      'rainbow-cpp-sdk==4.1.0',
       'PyYAML>=6.0.1',
     ],
     dependency_links=[
         'https://mirrors.tencent.com/repository/pypi/tencent_pypi/simple/rainbow-cpp-sdk/'
     ],
     author='kylinmiao',
     author_email='kylinmiao@tencent.com',
@@ -20,9 +20,8 @@
     # url='https://github.com/kylinmiao/rainbow_lib',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
-    
 )
```

### Comparing `rainbow_lib-0.0.2/rainbow_lib/wrapper.py` & `rainbow_lib-0.0.3/rainbow_lib/wrapper.py`

 * *Files identical despite different names*

### Comparing `rainbow_lib-0.0.2/rainbow_lib/client.py` & `rainbow_lib-0.0.3/rainbow_lib/client.py`

 * *Files identical despite different names*

