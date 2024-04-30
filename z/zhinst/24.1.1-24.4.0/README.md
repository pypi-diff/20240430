# Comparing `tmp/zhinst-24.1.1.tar.gz` & `tmp/zhinst-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhinst-24.1.1.tar", last modified: Thu Feb 29 18:51:53 2024, max compression
+gzip compressed data, was "zhinst-24.4.0.tar", last modified: Tue Apr 30 13:20:04 2024, max compression
```

## Comparing `zhinst-24.1.1.tar` & `zhinst-24.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:51:53.205179 zhinst-24.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:51:53.201179 zhinst-24.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:51:53.201179 zhinst-24.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-02-29 18:51:42.000000 zhinst-24.1.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-29 18:51:42.000000 zhinst-24.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-02-29 18:51:42.000000 zhinst-24.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-02-29 18:51:53.205179 zhinst-24.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-02-29 18:51:42.000000 zhinst-24.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:51:53.201179 zhinst-24.1.1/build_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-02-29 18:51:42.000000 zhinst-24.1.1/build_tools/test_wheels.sh
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-29 18:51:42.000000 zhinst-24.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-29 18:51:53.205179 zhinst-24.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)  1214826 2024-02-29 18:51:42.000000 zhinst-24.1.1/thumbnail.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 18:51:53.205179 zhinst-24.1.1/zhinst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-02-29 18:51:53.000000 zhinst-24.1.1/zhinst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-02-29 18:51:53.000000 zhinst-24.1.1/zhinst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 18:51:53.000000 zhinst-24.1.1/zhinst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-29 18:51:53.000000 zhinst-24.1.1/zhinst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-29 18:51:53.000000 zhinst-24.1.1/zhinst.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:04.389036 zhinst-24.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:04.385035 zhinst-24.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:04.389036 zhinst-24.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-30 13:19:57.000000 zhinst-24.4.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-30 13:19:57.000000 zhinst-24.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-30 13:19:57.000000 zhinst-24.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-30 13:20:04.389036 zhinst-24.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-30 13:19:57.000000 zhinst-24.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:04.389036 zhinst-24.4.0/build_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-30 13:19:57.000000 zhinst-24.4.0/build_tools/test_wheels.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-30 13:19:57.000000 zhinst-24.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-30 13:20:04.393036 zhinst-24.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)  1214826 2024-04-30 13:19:57.000000 zhinst-24.4.0/thumbnail.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:04.389036 zhinst-24.4.0/zhinst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-30 13:20:04.000000 zhinst-24.4.0/zhinst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-30 13:20:04.000000 zhinst-24.4.0/zhinst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:20:04.000000 zhinst-24.4.0/zhinst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-30 13:20:04.000000 zhinst-24.4.0/zhinst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 13:20:04.000000 zhinst-24.4.0/zhinst.egg-info/top_level.txt
```

### Comparing `zhinst-24.1.1/.github/workflows/publish.yml` & `zhinst-24.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `zhinst-24.1.1/LICENSE` & `zhinst-24.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zhinst-24.1.1/PKG-INFO` & `zhinst-24.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhinst
-Version: 24.1.1
+Version: 24.4.0
 Summary: Zurich Instruments Python API
 Author: Zurich Instrument
 Author-email: info@zhinst.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -14,16 +14,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: zhinst.core==24.1.55273
-Requires-Dist: zhinst.utils==0.4.0
+Requires-Dist: zhinst.core==24.4.57831
+Requires-Dist: zhinst.utils==0.4.1
 Requires-Dist: zhinst.toolkit==0.6.3
 
 # Zurich Instruments LabOne Packages
 
 ![](https://github.com/zhinst/zhinst-meta/blob/main/thumbnail.jpg)
 
 The `zhinst` package is purely a metapackage that installs the whole Python API
```

### Comparing `zhinst-24.1.1/README.md` & `zhinst-24.4.0/README.md`

 * *Files identical despite different names*

### Comparing `zhinst-24.1.1/setup.cfg` & `zhinst-24.4.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 	Topic :: Scientific/Engineering
 	Intended Audience :: Science/Research
 
 [options]
 python_requires = >=3.7
 use_scm_version = True
 install_requires = 
-	zhinst.core == 24.1.55273
-	zhinst.utils == 0.4.0
+	zhinst.core == 24.4.57831
+	zhinst.utils == 0.4.1
 	zhinst.toolkit == 0.6.3
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `zhinst-24.1.1/thumbnail.jpg` & `zhinst-24.4.0/thumbnail.jpg`

 * *Files identical despite different names*

### Comparing `zhinst-24.1.1/zhinst.egg-info/PKG-INFO` & `zhinst-24.4.0/zhinst.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhinst
-Version: 24.1.1
+Version: 24.4.0
 Summary: Zurich Instruments Python API
 Author: Zurich Instrument
 Author-email: info@zhinst.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -14,16 +14,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: zhinst.core==24.1.55273
-Requires-Dist: zhinst.utils==0.4.0
+Requires-Dist: zhinst.core==24.4.57831
+Requires-Dist: zhinst.utils==0.4.1
 Requires-Dist: zhinst.toolkit==0.6.3
 
 # Zurich Instruments LabOne Packages
 
 ![](https://github.com/zhinst/zhinst-meta/blob/main/thumbnail.jpg)
 
 The `zhinst` package is purely a metapackage that installs the whole Python API
```

