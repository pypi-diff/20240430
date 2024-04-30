# Comparing `tmp/castlabs-evs-1.1.4.tar.gz` & `tmp/castlabs-evs-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "castlabs-evs-1.1.4.tar", last modified: Sat Mar 16 00:58:55 2024, max compression
+gzip compressed data, was "castlabs-evs-1.1.5.tar", last modified: Tue Apr 30 10:21:01 2024, max compression
```

## Comparing `castlabs-evs-1.1.4.tar` & `castlabs-evs-1.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 emilp      (501) staff       (20)        0 2024-03-16 00:58:55.855052 castlabs-evs-1.1.4/
-drwxr-xr-x   0 emilp      (501) staff       (20)        0 2024-03-16 00:58:55.852711 castlabs-evs-1.1.4/.build/
-drwxr-xr-x   0 emilp      (501) staff       (20)        0 2024-03-16 00:58:55.852756 castlabs-evs-1.1.4/.build/prod/
-drwxr-xr-x   0 emilp      (501) staff       (20)        0 2024-03-16 00:58:55.852803 castlabs-evs-1.1.4/.build/prod/pypi-build/
-drwxr-xr-x   0 emilp      (501) staff       (20)        0 2024-03-16 00:58:55.854796 castlabs-evs-1.1.4/.build/prod/pypi-build/castlabs_evs.egg-info/
--rw-r--r--   0 emilp      (501) staff       (20)      231 2024-03-16 00:58:55.000000 castlabs-evs-1.1.4/.build/prod/pypi-build/castlabs_evs.egg-info/SOURCES.txt
--rw-r--r--   0 emilp      (501) staff       (20)       39 2020-08-19 21:03:00.000000 castlabs-evs-1.1.4/MANIFEST.in
--rw-r--r--   0 emilp      (501) staff       (20)     4796 2024-03-16 00:58:55.854941 castlabs-evs-1.1.4/PKG-INFO
-drwxr-xr-x   0 emilp      (501) staff       (20)        0 2024-03-16 00:58:55.853865 castlabs-evs-1.1.4/evs/
--rw-r--r--   0 emilp      (501) staff       (20)     3712 2022-05-18 21:23:24.000000 castlabs-evs-1.1.4/evs/README.md
--rw-r--r--   0 emilp      (501) staff       (20)       55 2024-03-15 23:53:04.000000 castlabs-evs-1.1.4/evs/__init__.py
--rw-r--r--   0 emilp      (501) staff       (20)     8427 2022-05-18 21:23:24.000000 castlabs-evs-1.1.4/evs/account.py
--rw-r--r--   0 emilp      (501) staff       (20)     6167 2024-03-15 22:20:02.000000 castlabs-evs-1.1.4/evs/auth.py
-drwxr-xr-x   0 emilp      (501) staff       (20)        0 2024-03-16 00:58:55.854183 castlabs-evs-1.1.4/evs/cli/
--rw-r--r--   0 emilp      (501) staff       (20)        0 2020-09-01 20:40:42.000000 castlabs-evs-1.1.4/evs/cli/__init__.py
--rw-r--r--   0 emilp      (501) staff       (20)     3979 2022-05-18 21:23:24.000000 castlabs-evs-1.1.4/evs/cli/account.py
--rw-r--r--   0 emilp      (501) staff       (20)     3890 2022-05-18 21:23:24.000000 castlabs-evs-1.1.4/evs/cli/vmp.py
-drwxr-xr-x   0 emilp      (501) staff       (20)        0 2024-03-16 00:58:55.854679 castlabs-evs-1.1.4/evs/core/
--rw-r--r--   0 emilp      (501) staff       (20)        0 2020-09-01 20:40:42.000000 castlabs-evs-1.1.4/evs/core/__init__.py
--rw-r--r--   0 emilp      (501) staff       (20)      726 2020-12-09 21:06:16.000000 castlabs-evs-1.1.4/evs/core/error.py
--rw-r--r--   0 emilp      (501) staff       (20)     1592 2022-05-18 21:23:24.000000 castlabs-evs-1.1.4/evs/core/failure.py
--rw-r--r--   0 emilp      (501) staff       (20)     3845 2022-05-18 21:23:24.000000 castlabs-evs-1.1.4/evs/core/util.py
--rw-r--r--   0 emilp      (501) staff       (20)    16534 2024-03-15 23:48:33.000000 castlabs-evs-1.1.4/evs/vmp.py
--rwxr-xr-x   0 emilp      (501) staff       (20)     1689 2024-03-15 19:48:09.000000 castlabs-evs-1.1.4/evs-setup.py
--rw-r--r--   0 emilp      (501) staff       (20)       38 2024-03-16 00:58:55.855088 castlabs-evs-1.1.4/setup.cfg
--rwxr-xr-x   0 emilp      (501) staff       (20)     1689 2024-03-15 19:48:09.000000 castlabs-evs-1.1.4/setup.py
+drwxr-xr-x   0 emilp      (501) staff       (20)        0 2024-04-30 10:21:01.233352 castlabs-evs-1.1.5/
+drwxr-xr-x   0 emilp      (501) staff       (20)        0 2024-04-30 10:21:01.230904 castlabs-evs-1.1.5/.build/
+drwxr-xr-x   0 emilp      (501) staff       (20)        0 2024-04-30 10:21:01.230951 castlabs-evs-1.1.5/.build/prod/
+drwxr-xr-x   0 emilp      (501) staff       (20)        0 2024-04-30 10:21:01.231003 castlabs-evs-1.1.5/.build/prod/pypi-build/
+drwxr-xr-x   0 emilp      (501) staff       (20)        0 2024-04-30 10:21:01.233086 castlabs-evs-1.1.5/.build/prod/pypi-build/castlabs_evs.egg-info/
+-rw-r--r--   0 emilp      (501) staff       (20)      231 2024-04-30 10:21:01.000000 castlabs-evs-1.1.5/.build/prod/pypi-build/castlabs_evs.egg-info/SOURCES.txt
+-rw-r--r--   0 emilp      (501) staff       (20)       39 2020-08-19 21:03:00.000000 castlabs-evs-1.1.5/MANIFEST.in
+-rw-r--r--   0 emilp      (501) staff       (20)     4796 2024-04-30 10:21:01.233237 castlabs-evs-1.1.5/PKG-INFO
+drwxr-xr-x   0 emilp      (501) staff       (20)        0 2024-04-30 10:21:01.232063 castlabs-evs-1.1.5/evs/
+-rw-r--r--   0 emilp      (501) staff       (20)     3712 2022-05-18 21:23:24.000000 castlabs-evs-1.1.5/evs/README.md
+-rw-r--r--   0 emilp      (501) staff       (20)       55 2024-04-30 10:17:13.000000 castlabs-evs-1.1.5/evs/__init__.py
+-rw-r--r--   0 emilp      (501) staff       (20)     8427 2022-05-18 21:23:24.000000 castlabs-evs-1.1.5/evs/account.py
+-rw-r--r--   0 emilp      (501) staff       (20)     6167 2024-03-15 22:20:02.000000 castlabs-evs-1.1.5/evs/auth.py
+drwxr-xr-x   0 emilp      (501) staff       (20)        0 2024-04-30 10:21:01.232420 castlabs-evs-1.1.5/evs/cli/
+-rw-r--r--   0 emilp      (501) staff       (20)        0 2020-09-01 20:40:42.000000 castlabs-evs-1.1.5/evs/cli/__init__.py
+-rw-r--r--   0 emilp      (501) staff       (20)     3979 2022-05-18 21:23:24.000000 castlabs-evs-1.1.5/evs/cli/account.py
+-rw-r--r--   0 emilp      (501) staff       (20)     3890 2022-05-18 21:23:24.000000 castlabs-evs-1.1.5/evs/cli/vmp.py
+drwxr-xr-x   0 emilp      (501) staff       (20)        0 2024-04-30 10:21:01.232952 castlabs-evs-1.1.5/evs/core/
+-rw-r--r--   0 emilp      (501) staff       (20)        0 2020-09-01 20:40:42.000000 castlabs-evs-1.1.5/evs/core/__init__.py
+-rw-r--r--   0 emilp      (501) staff       (20)      726 2020-12-09 21:06:16.000000 castlabs-evs-1.1.5/evs/core/error.py
+-rw-r--r--   0 emilp      (501) staff       (20)     1592 2022-05-18 21:23:24.000000 castlabs-evs-1.1.5/evs/core/failure.py
+-rw-r--r--   0 emilp      (501) staff       (20)     3930 2024-04-30 09:36:09.000000 castlabs-evs-1.1.5/evs/core/util.py
+-rw-r--r--   0 emilp      (501) staff       (20)    16534 2024-03-15 23:48:33.000000 castlabs-evs-1.1.5/evs/vmp.py
+-rwxr-xr-x   0 emilp      (501) staff       (20)     1689 2024-03-15 19:48:09.000000 castlabs-evs-1.1.5/evs-setup.py
+-rw-r--r--   0 emilp      (501) staff       (20)       38 2024-04-30 10:21:01.233388 castlabs-evs-1.1.5/setup.cfg
+-rwxr-xr-x   0 emilp      (501) staff       (20)     1689 2024-03-15 19:48:09.000000 castlabs-evs-1.1.5/setup.py
```

### Comparing `castlabs-evs-1.1.4/PKG-INFO` & `castlabs-evs-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: castlabs-evs
-Version: 1.1.4
+Version: 1.1.5
 Summary: A client for EVS, Widevine/VMP signing service
 Home-page: https://github.com/castlabs/electron-releases/wiki/EVS
 Author: Emil Pettersson
 Author-email: emil.pettersson@castlabs.com
 License: APACHE 2.0
 Keywords: castlabs evs 3pl widevine vmp drm electron wvvmp ecs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `castlabs-evs-1.1.4/evs/README.md` & `castlabs-evs-1.1.5/evs/README.md`

 * *Files identical despite different names*

### Comparing `castlabs-evs-1.1.4/evs/account.py` & `castlabs-evs-1.1.5/evs/account.py`

 * *Files identical despite different names*

### Comparing `castlabs-evs-1.1.4/evs/auth.py` & `castlabs-evs-1.1.5/evs/auth.py`

 * *Files identical despite different names*

### Comparing `castlabs-evs-1.1.4/evs/cli/account.py` & `castlabs-evs-1.1.5/evs/cli/account.py`

 * *Files identical despite different names*

### Comparing `castlabs-evs-1.1.4/evs/cli/vmp.py` & `castlabs-evs-1.1.5/evs/cli/vmp.py`

 * *Files identical despite different names*

### Comparing `castlabs-evs-1.1.4/evs/core/error.py` & `castlabs-evs-1.1.5/evs/core/error.py`

 * *Files identical despite different names*

### Comparing `castlabs-evs-1.1.4/evs/core/failure.py` & `castlabs-evs-1.1.5/evs/core/failure.py`

 * *Files identical despite different names*

### Comparing `castlabs-evs-1.1.4/evs/core/util.py` & `castlabs-evs-1.1.5/evs/core/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     o = int.from_bytes(h[60:64], byteorder='little')
     if o < len(h):
       s = h[o:o + 6]
       if s == b'\x50\x45\x00\x00\x64\x86':
         return ('pe', 'win32', 'x64')
       elif s == b'\x50\x45\x00\x00\x4c\x01':
         return ('pe', 'win32', 'ia32')
+      elif s == b'\x50\x45\x00\x00\x64\xaa':
+        return ('pe', 'win32', 'arm64')
   raise UnsupportedError('Binary type or archtecture not supported')
 
 ################################################################################
 
 DEFAULT_HASH_BLOCK = 2 * 1024 * 1024
 
 ################################################################################
```

### Comparing `castlabs-evs-1.1.4/evs/vmp.py` & `castlabs-evs-1.1.5/evs/vmp.py`

 * *Files identical despite different names*

### Comparing `castlabs-evs-1.1.4/evs-setup.py` & `castlabs-evs-1.1.5/evs-setup.py`

 * *Files identical despite different names*

### Comparing `castlabs-evs-1.1.4/setup.py` & `castlabs-evs-1.1.5/setup.py`

 * *Files identical despite different names*

