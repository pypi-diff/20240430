# Comparing `tmp/mama-0.9.1.tar.gz` & `tmp/mama-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mama-0.9.1.tar", last modified: Mon Apr  1 21:46:03 2024, max compression
+gzip compressed data, was "mama-0.9.3.tar", last modified: Tue Apr 30 10:01:01 2024, max compression
```

## Comparing `mama-0.9.1.tar` & `mama-0.9.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-04-01 21:46:03.806270 mama-0.9.1/
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1062 2022-10-15 13:42:02.000000 mama-0.9.1/LICENSE
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-04-01 21:46:03.796270 mama-0.9.1/PKG-INFO
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11351 2024-02-02 11:55:24.000000 mama-0.9.1/README.md
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-04-01 21:46:03.796270 mama-0.9.1/mama/
--rw-r--r--   0 jorma     (1000) jorma     (1000)      141 2022-10-15 12:52:32.000000 mama-0.9.1/mama/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11805 2024-03-24 12:54:08.000000 mama-0.9.1/mama/artifactory.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    39725 2024-03-26 12:35:49.000000 mama-0.9.1/mama/build_config.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    24912 2024-03-24 13:57:15.000000 mama-0.9.1/mama/build_dependency.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    55207 2024-03-26 11:34:57.000000 mama-0.9.1/mama/build_target.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11779 2024-03-26 11:44:52.000000 mama-0.9.1/mama/cmake_configure.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    16504 2024-03-24 11:44:20.000000 mama-0.9.1/mama/dependency_chain.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5368 2022-10-14 21:28:27.000000 mama-0.9.1/mama/init_project.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12378 2024-02-20 10:18:01.000000 mama-0.9.1/mama/main.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1796 2022-10-14 21:35:20.000000 mama-0.9.1/mama/msbuild.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     9467 2024-03-24 22:10:30.000000 mama-0.9.1/mama/package.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     7757 2024-03-24 13:37:47.000000 mama-0.9.1/mama/papa_deploy.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     3778 2024-03-24 22:17:15.000000 mama-0.9.1/mama/papa_upload.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1763 2024-03-24 13:50:55.000000 mama-0.9.1/mama/parse_mamafile.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-04-01 21:46:03.796270 mama-0.9.1/mama/platforms/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2023-02-10 12:13:25.000000 mama-0.9.1/mama/platforms/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     8558 2023-08-24 17:06:29.000000 mama-0.9.1/mama/platforms/android.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5376 2023-10-05 15:21:24.000000 mama-0.9.1/mama/platforms/mips.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5644 2024-01-24 19:36:51.000000 mama-0.9.1/mama/platforms/oclea.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-04-01 21:46:03.796270 mama-0.9.1/mama/types/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2022-10-14 22:47:55.000000 mama-0.9.1/mama/types/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1051 2023-01-31 19:23:36.000000 mama-0.9.1/mama/types/artifactory_pkg.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      789 2024-03-24 13:38:20.000000 mama-0.9.1/mama/types/asset.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      830 2023-01-31 19:23:36.000000 mama-0.9.1/mama/types/dep_source.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    15161 2024-04-01 21:45:25.000000 mama-0.9.1/mama/types/git.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1065 2022-10-13 16:33:15.000000 mama-0.9.1/mama/types/local_source.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    17510 2024-03-24 21:19:55.000000 mama-0.9.1/mama/util.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-04-01 21:46:03.796270 mama-0.9.1/mama/utils/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2022-10-14 22:47:54.000000 mama-0.9.1/mama/utils/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1637 2023-10-14 09:10:27.000000 mama-0.9.1/mama/utils/gdb.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    17034 2024-03-24 13:15:53.000000 mama-0.9.1/mama/utils/gnu_project.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      923 2023-10-14 09:10:17.000000 mama-0.9.1/mama/utils/gtest.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1038 2022-10-14 18:37:11.000000 mama-0.9.1/mama/utils/nonblocking_io.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     3693 2023-10-29 14:05:32.000000 mama-0.9.1/mama/utils/run.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    10345 2024-03-26 12:29:05.000000 mama-0.9.1/mama/utils/sub_process.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1439 2023-03-06 14:41:17.000000 mama-0.9.1/mama/utils/system.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-04-01 21:46:03.796270 mama-0.9.1/mama.egg-info/
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-04-01 21:46:03.000000 mama-0.9.1/mama.egg-info/PKG-INFO
--rw-r--r--   0 jorma     (1000) jorma     (1000)      921 2024-04-01 21:46:03.000000 mama-0.9.1/mama.egg-info/SOURCES.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)        1 2024-04-01 21:46:03.000000 mama-0.9.1/mama.egg-info/dependency_links.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)       40 2024-04-01 21:46:03.000000 mama-0.9.1/mama.egg-info/entry_points.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)       76 2024-04-01 21:46:03.000000 mama-0.9.1/mama.egg-info/requires.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)        5 2024-04-01 21:46:03.000000 mama-0.9.1/mama.egg-info/top_level.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1180 2024-04-01 21:45:40.000000 mama-0.9.1/pyproject.toml
--rw-r--r--   0 jorma     (1000) jorma     (1000)       38 2024-04-01 21:46:03.806270 mama-0.9.1/setup.cfg
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-04-30 10:01:01.397396 mama-0.9.3/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1062 2024-01-20 16:30:57.000000 mama-0.9.3/LICENSE
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-04-30 10:01:01.397396 mama-0.9.3/PKG-INFO
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11351 2024-03-25 09:35:15.000000 mama-0.9.3/README.md
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-04-30 10:01:01.397396 mama-0.9.3/mama/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      141 2024-01-20 16:30:57.000000 mama-0.9.3/mama/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11805 2024-03-25 09:35:15.000000 mama-0.9.3/mama/artifactory.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    39725 2024-04-07 19:34:43.000000 mama-0.9.3/mama/build_config.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    24912 2024-03-25 09:35:15.000000 mama-0.9.3/mama/build_dependency.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    55207 2024-04-07 19:34:43.000000 mama-0.9.3/mama/build_target.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11779 2024-04-07 19:34:43.000000 mama-0.9.3/mama/cmake_configure.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    16504 2024-03-25 09:35:15.000000 mama-0.9.3/mama/dependency_chain.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5368 2024-01-20 16:30:57.000000 mama-0.9.3/mama/init_project.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12378 2024-03-25 09:35:15.000000 mama-0.9.3/mama/main.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1796 2024-01-20 16:30:57.000000 mama-0.9.3/mama/msbuild.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     9665 2024-04-30 09:54:55.000000 mama-0.9.3/mama/package.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     7757 2024-03-25 09:35:15.000000 mama-0.9.3/mama/papa_deploy.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     3778 2024-03-25 09:35:15.000000 mama-0.9.3/mama/papa_upload.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1763 2024-03-25 09:35:15.000000 mama-0.9.3/mama/parse_mamafile.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-04-30 10:01:01.397396 mama-0.9.3/mama/platforms/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2024-01-20 16:30:57.000000 mama-0.9.3/mama/platforms/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     8558 2024-01-20 16:30:57.000000 mama-0.9.3/mama/platforms/android.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5376 2024-01-20 16:30:57.000000 mama-0.9.3/mama/platforms/mips.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5644 2024-03-25 09:35:15.000000 mama-0.9.3/mama/platforms/oclea.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-04-30 10:01:01.397396 mama-0.9.3/mama/types/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2024-01-20 16:30:57.000000 mama-0.9.3/mama/types/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1051 2024-01-20 16:30:57.000000 mama-0.9.3/mama/types/artifactory_pkg.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      789 2024-01-20 16:30:57.000000 mama-0.9.3/mama/types/asset.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      830 2024-01-20 16:30:57.000000 mama-0.9.3/mama/types/dep_source.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    15161 2024-04-07 19:34:43.000000 mama-0.9.3/mama/types/git.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1065 2024-01-20 16:30:57.000000 mama-0.9.3/mama/types/local_source.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    17510 2024-03-25 09:35:15.000000 mama-0.9.3/mama/util.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-04-30 10:01:01.397396 mama-0.9.3/mama/utils/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2024-01-20 16:30:57.000000 mama-0.9.3/mama/utils/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1637 2024-01-20 16:30:57.000000 mama-0.9.3/mama/utils/gdb.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    17034 2024-03-25 09:35:15.000000 mama-0.9.3/mama/utils/gnu_project.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      923 2024-01-20 16:30:57.000000 mama-0.9.3/mama/utils/gtest.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1038 2024-01-20 16:30:57.000000 mama-0.9.3/mama/utils/nonblocking_io.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     3789 2024-04-30 09:51:39.000000 mama-0.9.3/mama/utils/run.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    10345 2024-04-07 19:34:43.000000 mama-0.9.3/mama/utils/sub_process.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1494 2024-04-30 09:53:26.000000 mama-0.9.3/mama/utils/system.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-04-30 10:01:01.397396 mama-0.9.3/mama.egg-info/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-04-30 10:01:01.000000 mama-0.9.3/mama.egg-info/PKG-INFO
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      921 2024-04-30 10:01:01.000000 mama-0.9.3/mama.egg-info/SOURCES.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        1 2024-04-30 10:01:01.000000 mama-0.9.3/mama.egg-info/dependency_links.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       40 2024-04-30 10:01:01.000000 mama-0.9.3/mama.egg-info/entry_points.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       76 2024-04-30 10:01:01.000000 mama-0.9.3/mama.egg-info/requires.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        5 2024-04-30 10:01:01.000000 mama-0.9.3/mama.egg-info/top_level.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1180 2024-04-30 09:55:32.000000 mama-0.9.3/pyproject.toml
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       38 2024-04-30 10:01:01.397396 mama-0.9.3/setup.cfg
```

### Comparing `mama-0.9.1/LICENSE` & `mama-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/PKG-INFO` & `mama-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mama
-Version: 0.9.1
+Version: 0.9.3
 Summary: A modular C++ build tool even your mama can use
 Author-email: Jorma Rebane <jorma.rebane@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/RedFox20/Mama
 Project-URL: Bug Tracker, https://github.com/RedFox20/Mama/issues
 Keywords: mama,build,mamabuild,c,c++,tool,cmake,simple,easy,package,manager,cross-platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mama-0.9.1/README.md` & `mama-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/artifactory.py` & `mama-0.9.3/mama/artifactory.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/build_config.py` & `mama-0.9.3/mama/build_config.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/build_dependency.py` & `mama-0.9.3/mama/build_dependency.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/build_target.py` & `mama-0.9.3/mama/build_target.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/cmake_configure.py` & `mama-0.9.3/mama/cmake_configure.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/dependency_chain.py` & `mama-0.9.3/mama/dependency_chain.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/init_project.py` & `mama-0.9.3/mama/init_project.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/main.py` & `mama-0.9.3/mama/main.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/msbuild.py` & `mama-0.9.3/mama/msbuild.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/package.py` & `mama-0.9.3/mama/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from typing import List, TYPE_CHECKING
 import os
-from .utils.system import console
+from .utils.system import console, is_aarch64
 from .util import normalized_path, glob_with_name_match, glob_with_extensions
 from .types.asset import Asset
 
 if TYPE_CHECKING:
     from .build_target import BuildTarget
     from .build_config import BuildConfig
 
@@ -176,21 +176,24 @@
 
 def find_syslib(target: BuildTarget, name: str, apt: bool, required: bool):
     if target.ios or target.macos:
         if not name.startswith('-framework '):
             raise EnvironmentError(f'Expected "-framework name" but got "{name}"')
         return name # '-framework Foundation'
     elif target.linux:
+        compiler_dir = 'aarch64-linux-gnu' if is_aarch64 else 'x86_64-linux-gnu'
         for candidate in [
-            lambda: f'/usr/lib/x86_64-linux-gnu/{name}',
-            lambda: f'/usr/lib/x86_64-linux-gnu/lib{name}.so',
-            lambda: f'/usr/lib/x86_64-linux-gnu/lib{name}.a',
+            lambda: f'/usr/lib/{compiler_dir}/{name}',
+            lambda: f'/usr/lib/{compiler_dir}/lib{name}.so',
+            lambda: f'/usr/lib/{compiler_dir}/lib{name}.so.2',
+            lambda: f'/usr/lib/{compiler_dir}/lib{name}.a',
             lambda: f'/usr/lib/lib{name}.so',
+            lambda: f'/usr/lib/lib{name}.so.2',
             lambda: f'/usr/lib/lib{name}.a' ]:
-            if os.path.isfile(candidate()):
+            if os.path.exists(candidate()):
                 return name # example: we found `libdl.so`, so just return `dl` for the linker
         if not required: return None
         if apt: raise IOError(f'Error {target.name} failed to find REQUIRED SysLib: {name}  Try `sudo apt install {apt}`')
         raise IOError(f'Error {target.name} failed to find REQUIRED SysLib: {name}  Try installing it with apt.')
     else:
         return name # just export it. expect system linker to find it.
```

### Comparing `mama-0.9.1/mama/papa_deploy.py` & `mama-0.9.3/mama/papa_deploy.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/papa_upload.py` & `mama-0.9.3/mama/papa_upload.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/parse_mamafile.py` & `mama-0.9.3/mama/parse_mamafile.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/platforms/android.py` & `mama-0.9.3/mama/platforms/android.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/platforms/mips.py` & `mama-0.9.3/mama/platforms/mips.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/platforms/oclea.py` & `mama-0.9.3/mama/platforms/oclea.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/types/artifactory_pkg.py` & `mama-0.9.3/mama/types/artifactory_pkg.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/types/asset.py` & `mama-0.9.3/mama/types/asset.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/types/dep_source.py` & `mama-0.9.3/mama/types/dep_source.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/types/git.py` & `mama-0.9.3/mama/types/git.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/types/local_source.py` & `mama-0.9.3/mama/types/local_source.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/util.py` & `mama-0.9.3/mama/util.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/utils/gdb.py` & `mama-0.9.3/mama/utils/gdb.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/utils/gnu_project.py` & `mama-0.9.3/mama/utils/gnu_project.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/utils/gtest.py` & `mama-0.9.3/mama/utils/gtest.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/utils/nonblocking_io.py` & `mama-0.9.3/mama/utils/nonblocking_io.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/utils/run.py` & `mama-0.9.3/mama/utils/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,17 @@
         exe = shutil.which(program)
         if not exe:
             exe = f'{cwd}/{os.path.basename(program)}'
         #print(f'DEFAULT cwd={cwd} exe={exe} args={args}')
 
     cwd = normalized_path(cwd)
     exe = normalized_path(exe)
+    if ' ' in exe:
+        exe = '"' + exe + '"'
+    #print(f'CWD={cwd} EXE={exe} ARGS={args}')
     return cwd, exe, args
 
 
 def run_in_working_dir(target: BuildTarget, working_dir: str, command: str, exit_on_fail=True, env=None):
     cwd, exe, args = get_cwd_exe_args(target, command, cwd=working_dir)
     execute_echo(cwd=cwd, cmd=f'{exe} {args}', exit_on_fail=exit_on_fail, env=env)
```

### Comparing `mama-0.9.1/mama/utils/sub_process.py` & `mama-0.9.3/mama/utils/sub_process.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/mama/utils/system.py` & `mama-0.9.3/mama/utils/system.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import sys, subprocess
+import sys, subprocess, platform
 from termcolor import colored
 
 is_windows = sys.platform == 'win32'
 is_linux   = sys.platform.startswith('linux')
 is_macos   = sys.platform == 'darwin'
 if not (is_windows or is_linux or is_macos):
     raise RuntimeError(f'MamaBuild unsupported platform {sys.platform}')
 
+is_aarch64 = platform.machine() == 'aarch64'
 
 def _is_system_64_bit():
     if sys.platform == 'win32':
         output = subprocess.check_output(['wmic', 'os', 'get', 'OSArchitecture'])
         if '64-bit' in str(output):
             return True
     else:
```

### Comparing `mama-0.9.1/mama.egg-info/PKG-INFO` & `mama-0.9.3/mama.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mama
-Version: 0.9.1
+Version: 0.9.3
 Summary: A modular C++ build tool even your mama can use
 Author-email: Jorma Rebane <jorma.rebane@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/RedFox20/Mama
 Project-URL: Bug Tracker, https://github.com/RedFox20/Mama/issues
 Keywords: mama,build,mamabuild,c,c++,tool,cmake,simple,easy,package,manager,cross-platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mama-0.9.1/mama.egg-info/SOURCES.txt` & `mama-0.9.3/mama.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mama-0.9.1/pyproject.toml` & `mama-0.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mama"
-version = "0.9.1"
+version = "0.9.3"
 description = "A modular C++ build tool even your mama can use"
 license = { text = "MIT" }
 authors = [
     { name="Jorma Rebane", email="jorma.rebane@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.6"
```

