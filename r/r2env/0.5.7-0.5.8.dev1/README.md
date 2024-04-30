# Comparing `tmp/r2env-0.5.7.tar.gz` & `tmp/r2env-0.5.8.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r2env-0.5.7.tar", last modified: Fri Mar  3 20:14:02 2023, max compression
+gzip compressed data, was "r2env-0.5.8.dev1.tar", last modified: Tue Apr 30 14:55:42 2024, max compression
```

## Comparing `r2env-0.5.7.tar` & `r2env-0.5.8.dev1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 20:14:02.255144 r2env-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (122)    53248 2023-03-03 20:13:52.000000 r2env-0.5.7/.coverage
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 20:14:02.251144 r2env-0.5.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 20:14:02.251144 r2env-0.5.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2446 2023-03-03 20:13:52.000000 r2env-0.5.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2337 2023-03-03 20:13:52.000000 r2env-0.5.7/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (122)      338 2023-03-03 20:13:52.000000 r2env-0.5.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-03-03 20:14:02.000000 r2env-0.5.7/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-03-03 20:14:02.000000 r2env-0.5.7/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-03-03 20:13:52.000000 r2env-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-03-03 20:13:52.000000 r2env-0.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-03-03 20:13:52.000000 r2env-0.5.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-03-03 20:14:02.255144 r2env-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2422 2023-03-03 20:13:52.000000 r2env-0.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 20:14:02.251144 r2env-0.5.7/r2env/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-03-03 20:13:52.000000 r2env-0.5.7/r2env/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 20:14:02.251144 r2env-0.5.7/r2env/config/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-03-03 20:13:52.000000 r2env-0.5.7/r2env/config/config.json
--rw-r--r--   0 runner    (1001) docker     (122)     7327 2023-03-03 20:13:52.000000 r2env-0.5.7/r2env/core.py
--rw-r--r--   0 runner    (1001) docker     (122)      150 2023-03-03 20:13:52.000000 r2env-0.5.7/r2env/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    15681 2023-03-03 20:13:52.000000 r2env-0.5.7/r2env/package_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     4999 2023-03-03 20:13:52.000000 r2env-0.5.7/r2env/repl.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 20:14:02.251144 r2env-0.5.7/r2env/test/
--rw-r--r--   0 runner    (1001) docker     (122)    13387 2023-03-03 20:13:52.000000 r2env-0.5.7/r2env/test/test_core.py
--rw-r--r--   0 runner    (1001) docker     (122)    20215 2023-03-03 20:13:52.000000 r2env-0.5.7/r2env/test/test_package.py
--rw-r--r--   0 runner    (1001) docker     (122)     1765 2023-03-03 20:13:52.000000 r2env-0.5.7/r2env/test/test_repl.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-03 20:13:52.000000 r2env-0.5.7/r2env/test/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-03-03 20:13:52.000000 r2env-0.5.7/r2env/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-03-03 20:13:52.000000 r2env-0.5.7/r2env/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 20:14:02.251144 r2env-0.5.7/r2env.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-03-03 20:14:02.000000 r2env-0.5.7/r2env.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      740 2023-03-03 20:14:02.000000 r2env-0.5.7/r2env.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-03 20:14:02.000000 r2env-0.5.7/r2env.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-03-03 20:14:02.000000 r2env-0.5.7/r2env.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-03 20:14:02.000000 r2env-0.5.7/r2env.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-03-03 20:14:02.000000 r2env-0.5.7/r2env.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-03-03 20:14:02.000000 r2env-0.5.7/r2env.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-03-03 20:14:02.000000 r2env-0.5.7/r2env.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-03 20:14:02.251144 r2env-0.5.7/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-03-03 20:13:52.000000 r2env-0.5.7/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-03-03 20:13:52.000000 r2env-0.5.7/requirements/dist.txt
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-03-03 20:13:52.000000 r2env-0.5.7/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-03-03 20:13:52.000000 r2env-0.5.7/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      656 2023-03-03 20:13:52.000000 r2env-0.5.7/run_tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1185 2023-03-03 20:14:02.255144 r2env-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-03-03 20:13:52.000000 r2env-0.5.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-03-03 20:13:52.000000 r2env-0.5.7/tox.ini
+drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-04-30 14:55:42.833595 r2env-0.5.8.dev1/
+-rw-r--r--   0 pancake    (501) staff       (20)    53248 2022-03-17 09:47:40.000000 r2env-0.5.8.dev1/.coverage
+drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-04-30 14:55:42.828734 r2env-0.5.8.dev1/.github/
+drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-04-30 14:55:42.830770 r2env-0.5.8.dev1/.github/workflows/
+-rw-r--r--   0 pancake    (501) staff       (20)     2446 2022-03-17 09:47:40.000000 r2env-0.5.8.dev1/.github/workflows/ci.yml
+-rw-r--r--   0 pancake    (501) staff       (20)     2337 2022-03-17 09:47:40.000000 r2env-0.5.8.dev1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 pancake    (501) staff       (20)      469 2024-04-30 14:52:19.000000 r2env-0.5.8.dev1/.github/workflows/semgrep.yml
+-rw-r--r--   0 pancake    (501) staff       (20)      338 2022-03-17 09:47:40.000000 r2env-0.5.8.dev1/.pylintrc
+-rw-r--r--   0 pancake    (501) staff       (20)      451 2024-04-30 14:55:42.000000 r2env-0.5.8.dev1/AUTHORS
+-rw-r--r--   0 pancake    (501) staff       (20)     5162 2024-04-30 14:55:42.000000 r2env-0.5.8.dev1/ChangeLog
+-rw-r--r--   0 pancake    (501) staff       (20)     1073 2022-03-17 09:47:40.000000 r2env-0.5.8.dev1/LICENSE
+-rw-r--r--   0 pancake    (501) staff       (20)       22 2024-04-30 14:54:05.000000 r2env-0.5.8.dev1/MANIFEST.in
+-rw-r--r--   0 pancake    (501) staff       (20)      363 2024-04-30 14:55:37.000000 r2env-0.5.8.dev1/Makefile
+-rw-r--r--   0 pancake    (501) staff       (20)     1221 2024-04-30 14:55:42.833535 r2env-0.5.8.dev1/PKG-INFO
+-rw-r--r--   0 pancake    (501) staff       (20)     2422 2024-04-30 14:52:19.000000 r2env-0.5.8.dev1/README.md
+drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-04-30 14:55:42.831503 r2env-0.5.8.dev1/r2env/
+-rw-r--r--   0 pancake    (501) staff       (20)       24 2022-03-17 09:47:40.000000 r2env-0.5.8.dev1/r2env/__init__.py
+drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-04-30 14:55:42.832395 r2env-0.5.8.dev1/r2env/config/
+-rw-r--r--   0 pancake    (501) staff       (20)       22 2022-03-17 09:47:40.000000 r2env-0.5.8.dev1/r2env/config/config.json
+-rw-r--r--   0 pancake    (501) staff       (20)     7327 2024-04-30 14:52:19.000000 r2env-0.5.8.dev1/r2env/core.py
+-rw-r--r--   0 pancake    (501) staff       (20)      150 2022-03-17 09:47:40.000000 r2env-0.5.8.dev1/r2env/exceptions.py
+-rw-r--r--   0 pancake    (501) staff       (20)    15681 2024-04-30 14:52:19.000000 r2env-0.5.8.dev1/r2env/package_manager.py
+-rw-r--r--   0 pancake    (501) staff       (20)     4999 2024-04-30 14:52:19.000000 r2env-0.5.8.dev1/r2env/repl.py
+drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-04-30 14:55:42.832831 r2env-0.5.8.dev1/r2env/test/
+-rw-r--r--   0 pancake    (501) staff       (20)    13387 2022-07-07 08:52:40.000000 r2env-0.5.8.dev1/r2env/test/test_core.py
+-rw-r--r--   0 pancake    (501) staff       (20)    20215 2022-07-07 08:52:40.000000 r2env-0.5.8.dev1/r2env/test/test_package.py
+-rw-r--r--   0 pancake    (501) staff       (20)     1765 2022-03-17 09:47:40.000000 r2env-0.5.8.dev1/r2env/test/test_repl.py
+-rw-r--r--   0 pancake    (501) staff       (20)        0 2022-03-17 09:47:40.000000 r2env-0.5.8.dev1/r2env/test/test_tools.py
+-rw-r--r--   0 pancake    (501) staff       (20)     2860 2022-07-07 08:52:40.000000 r2env-0.5.8.dev1/r2env/tools.py
+-rw-r--r--   0 pancake    (501) staff       (20)        6 2024-04-30 14:52:19.000000 r2env-0.5.8.dev1/r2env/version.txt
+drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-04-30 14:55:42.833259 r2env-0.5.8.dev1/r2env.egg-info/
+-rw-r--r--   0 pancake    (501) staff       (20)     1221 2024-04-30 14:55:42.000000 r2env-0.5.8.dev1/r2env.egg-info/PKG-INFO
+-rw-r--r--   0 pancake    (501) staff       (20)      770 2024-04-30 14:55:42.000000 r2env-0.5.8.dev1/r2env.egg-info/SOURCES.txt
+-rw-r--r--   0 pancake    (501) staff       (20)        1 2024-04-30 14:55:42.000000 r2env-0.5.8.dev1/r2env.egg-info/dependency_links.txt
+-rw-r--r--   0 pancake    (501) staff       (20)       42 2024-04-30 14:55:42.000000 r2env-0.5.8.dev1/r2env.egg-info/entry_points.txt
+-rw-r--r--   0 pancake    (501) staff       (20)        1 2022-08-15 14:04:35.000000 r2env-0.5.8.dev1/r2env.egg-info/not-zip-safe
+-rw-r--r--   0 pancake    (501) staff       (20)       47 2024-04-30 14:55:42.000000 r2env-0.5.8.dev1/r2env.egg-info/pbr.json
+-rw-r--r--   0 pancake    (501) staff       (20)       53 2024-04-30 14:55:42.000000 r2env-0.5.8.dev1/r2env.egg-info/requires.txt
+-rw-r--r--   0 pancake    (501) staff       (20)        6 2024-04-30 14:55:42.000000 r2env-0.5.8.dev1/r2env.egg-info/top_level.txt
+drwxr-xr-x   0 pancake    (501) staff       (20)        0 2024-04-30 14:55:42.833105 r2env-0.5.8.dev1/requirements/
+-rw-r--r--   0 pancake    (501) staff       (20)       52 2024-04-30 14:52:19.000000 r2env-0.5.8.dev1/requirements/build.txt
+-rw-r--r--   0 pancake    (501) staff       (20)       37 2022-03-17 09:47:40.000000 r2env-0.5.8.dev1/requirements/dist.txt
+-rw-r--r--   0 pancake    (501) staff       (20)       81 2022-03-17 09:47:40.000000 r2env-0.5.8.dev1/requirements/test.txt
+-rw-r--r--   0 pancake    (501) staff       (20)       25 2022-03-17 09:47:40.000000 r2env-0.5.8.dev1/requirements.txt
+-rwxr-xr-x   0 pancake    (501) staff       (20)      656 2022-03-17 09:47:40.000000 r2env-0.5.8.dev1/run_tests.sh
+-rw-r--r--   0 pancake    (501) staff       (20)     1185 2024-04-30 14:55:42.833898 r2env-0.5.8.dev1/setup.cfg
+-rw-r--r--   0 pancake    (501) staff       (20)      249 2024-04-30 14:52:19.000000 r2env-0.5.8.dev1/setup.py
+-rw-r--r--   0 pancake    (501) staff       (20)     1060 2024-04-30 14:52:19.000000 r2env-0.5.8.dev1/tox.ini
```

### Comparing `r2env-0.5.7/.coverage` & `r2env-0.5.8.dev1/.coverage`

 * *Files identical despite different names*

### Comparing `r2env-0.5.7/.github/workflows/ci.yml` & `r2env-0.5.8.dev1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `r2env-0.5.7/.github/workflows/codeql-analysis.yml` & `r2env-0.5.8.dev1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `r2env-0.5.7/LICENSE` & `r2env-0.5.8.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `r2env-0.5.7/PKG-INFO` & `r2env-0.5.8.dev1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: r2env
-Version: 0.5.7
+Version: 0.5.8.dev1
 Summary: radare2 multiple version and environment installation tool
 Home-page: https://www.radare.org/
 Author: pancake
 Author-email: pancake@nopcode.org
-License: UNKNOWN
 Project-URL: Source, https://github.com/radareorg/r2env
 Project-URL: Documentation, https://github.com/radareorg/r2env
-Description: radare2 multiple version and environment installation tool
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: License :: OSI Approved
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -22,7 +19,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: dploy>=0.1.2
+Requires-Dist: colorama>=0.4.4
+Requires-Dist: wget
+Requires-Dist: requests
+Requires-Dist: GitPython
+
+radare2 multiple version and environment installation tool
```

### Comparing `r2env-0.5.7/README.md` & `r2env-0.5.8.dev1/README.md`

 * *Files identical despite different names*

### Comparing `r2env-0.5.7/r2env/core.py` & `r2env-0.5.8.dev1/r2env/core.py`

 * *Files identical despite different names*

### Comparing `r2env-0.5.7/r2env/package_manager.py` & `r2env-0.5.8.dev1/r2env/package_manager.py`

 * *Files identical despite different names*

### Comparing `r2env-0.5.7/r2env/repl.py` & `r2env-0.5.8.dev1/r2env/repl.py`

 * *Files identical despite different names*

### Comparing `r2env-0.5.7/r2env/test/test_core.py` & `r2env-0.5.8.dev1/r2env/test/test_core.py`

 * *Files identical despite different names*

### Comparing `r2env-0.5.7/r2env/test/test_package.py` & `r2env-0.5.8.dev1/r2env/test/test_package.py`

 * *Files identical despite different names*

### Comparing `r2env-0.5.7/r2env/test/test_repl.py` & `r2env-0.5.8.dev1/r2env/test/test_repl.py`

 * *Files identical despite different names*

### Comparing `r2env-0.5.7/r2env/tools.py` & `r2env-0.5.8.dev1/r2env/tools.py`

 * *Files identical despite different names*

### Comparing `r2env-0.5.7/r2env.egg-info/PKG-INFO` & `r2env-0.5.8.dev1/r2env.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: r2env
-Version: 0.5.7
+Version: 0.5.8.dev1
 Summary: radare2 multiple version and environment installation tool
 Home-page: https://www.radare.org/
 Author: pancake
 Author-email: pancake@nopcode.org
-License: UNKNOWN
 Project-URL: Source, https://github.com/radareorg/r2env
 Project-URL: Documentation, https://github.com/radareorg/r2env
-Description: radare2 multiple version and environment installation tool
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: License :: OSI Approved
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -22,7 +19,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: dploy>=0.1.2
+Requires-Dist: colorama>=0.4.4
+Requires-Dist: wget
+Requires-Dist: requests
+Requires-Dist: GitPython
+
+radare2 multiple version and environment installation tool
```

### Comparing `r2env-0.5.7/r2env.egg-info/SOURCES.txt` & `r2env-0.5.8.dev1/r2env.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 requirements.txt
 run_tests.sh
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/ci.yml
 .github/workflows/codeql-analysis.yml
+.github/workflows/semgrep.yml
 r2env/__init__.py
 r2env/core.py
 r2env/exceptions.py
 r2env/package_manager.py
 r2env/repl.py
 r2env/tools.py
 r2env/version.txt
```

### Comparing `r2env-0.5.7/run_tests.sh` & `r2env-0.5.8.dev1/run_tests.sh`

 * *Files identical despite different names*

### Comparing `r2env-0.5.7/setup.cfg` & `r2env-0.5.8.dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `r2env-0.5.7/tox.ini` & `r2env-0.5.8.dev1/tox.ini`

 * *Files identical despite different names*

