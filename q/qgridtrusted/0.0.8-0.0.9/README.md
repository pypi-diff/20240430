# Comparing `tmp/qgridtrusted-0.0.8.tar.gz` & `tmp/qgridtrusted-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgridtrusted-0.0.8.tar", last modified: Sat Mar  2 17:07:40 2024, max compression
+gzip compressed data, was "qgridtrusted-0.0.9.tar", last modified: Thu Apr  4 05:22:36 2024, max compression
```

## Comparing `qgridtrusted-0.0.8.tar` & `qgridtrusted-0.0.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/
--rw-r--r--   0 root         (0) root         (0)    11347 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)    15046 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      965 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)    16653 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/jupyter/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/jupyter/nbconfig/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/jupyter/nbconfig/notebook.d/
--rw-r--r--   0 root         (0) root         (0)       59 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/jupyter/nbconfig/notebook.d/qgrid.json
--rw-r--r--   0 root         (0) root         (0)     1276 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/
--rw-r--r--   0 root         (0) root         (0)      574 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/__init__.py
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/_version.py
--rw-r--r--   0 root         (0) root         (0)    71363 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/grid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/
--rw-r--r--   0 root         (0) root         (0)      851 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/097df1053ff3246e2f1af9d5a858ac6c.gif
--rw-r--r--   0 root         (0) root         (0)     7142 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/16fec672acf4e60b212d6f213cfea45d.png
--rw-r--r--   0 root         (0) root         (0)       80 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/177e96f6b132ebf8fe08.gif
--rw-r--r--   0 root         (0) root         (0)     4670 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/2487f1f6cffd2524ad3c4b8626540a04.png
--rw-r--r--   0 root         (0) root         (0)       80 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/255ce53c58b905a5f2c3.gif
--rw-r--r--   0 root         (0) root         (0)       80 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/33d6b476767f0c2f035c.png
--rw-r--r--   0 root         (0) root         (0)       80 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/4ce09a41e666341f128d.png
--rw-r--r--   0 root         (0) root         (0)       80 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/63f6e1e148d7ef23e4dc.gif
--rw-r--r--   0 root         (0) root         (0)       80 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/720ec1bdffac972ae44e.gif
--rw-r--r--   0 root         (0) root         (0)      830 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/7e2ccbc3b7b736251403b238014dcacc.gif
--rw-r--r--   0 root         (0) root         (0)      836 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/86586a919bd10f4cedba392f64336a54.gif
--rw-r--r--   0 root         (0) root         (0)      833 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/8fcbe60e4efd8e2d1742bba8486994e1.gif
--rw-r--r--   0 root         (0) root         (0)       80 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/94bfb80995aa47cff3b0.png
--rw-r--r--   0 root         (0) root         (0)      846 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/9a52a923ceb5983fa0943c1e24d6d35b.gif
--rw-r--r--   0 root         (0) root         (0)       80 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/a2b8bfe53991521d8b1d.gif
--rw-r--r--   0 root         (0) root         (0)     4670 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/ae9b3e279d547e10151b58ff7547829e.png
--rw-r--r--   0 root         (0) root         (0)     7163 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/af253b1b82b79498bcedad50d30d155b.png
--rw-r--r--   0 root         (0) root         (0)       80 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/b2f8593cd54a831dd97a.png
--rw-r--r--   0 root         (0) root         (0)       80 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/b2fd4844280a4a216e7d.png
--rw-r--r--   0 root         (0) root         (0)       80 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/d5ce50f40bd2a5707619.gif
--rw-r--r--   0 root         (0) root         (0)     7126 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/e30ce9397cddc63d3f1827d1d7153edf.png
--rw-r--r--   0 root         (0) root         (0)      823 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/e38f33bbf55d6e20d21c4a10b9912668.gif
--rw-r--r--   0 root         (0) root         (0)       80 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/e47aff57d59b6c120c5c.png
--rw-r--r--   0 root         (0) root         (0)     6539 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/e716c93fb8aa23c1e10b5185a8191dbf.png
--rw-r--r--   0 root         (0) root         (0)      306 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/extension.js
--rw-r--r--   0 root         (0) root         (0)   925575 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/index.js
--rw-r--r--   0 root         (0) root         (0)     2152 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/index.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)  2728248 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgrid/static/index.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgridtrusted.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15046 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgridtrusted.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1484 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgridtrusted.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgridtrusted.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgridtrusted.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/qgridtrusted.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1562 2024-03-02 17:07:40.000000 qgridtrusted-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)    11347 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15046 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      965 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)    16653 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/jupyter/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/jupyter/nbconfig/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/jupyter/nbconfig/notebook.d/
+-rw-r--r--   0 root         (0) root         (0)       59 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/jupyter/nbconfig/notebook.d/qgrid.json
+-rw-r--r--   0 root         (0) root         (0)     1276 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/
+-rw-r--r--   0 root         (0) root         (0)      574 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/_version.py
+-rw-r--r--   0 root         (0) root         (0)    71363 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/grid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/
+-rw-r--r--   0 root         (0) root         (0)      851 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/097df1053ff3246e2f1af9d5a858ac6c.gif
+-rw-r--r--   0 root         (0) root         (0)     7142 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/16fec672acf4e60b212d6f213cfea45d.png
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/177e96f6b132ebf8fe08.gif
+-rw-r--r--   0 root         (0) root         (0)     4670 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/2487f1f6cffd2524ad3c4b8626540a04.png
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/255ce53c58b905a5f2c3.gif
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/33d6b476767f0c2f035c.png
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/4ce09a41e666341f128d.png
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/63f6e1e148d7ef23e4dc.gif
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/720ec1bdffac972ae44e.gif
+-rw-r--r--   0 root         (0) root         (0)      830 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/7e2ccbc3b7b736251403b238014dcacc.gif
+-rw-r--r--   0 root         (0) root         (0)      836 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/86586a919bd10f4cedba392f64336a54.gif
+-rw-r--r--   0 root         (0) root         (0)      833 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/8fcbe60e4efd8e2d1742bba8486994e1.gif
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/94bfb80995aa47cff3b0.png
+-rw-r--r--   0 root         (0) root         (0)      846 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/9a52a923ceb5983fa0943c1e24d6d35b.gif
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/a2b8bfe53991521d8b1d.gif
+-rw-r--r--   0 root         (0) root         (0)     4670 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/ae9b3e279d547e10151b58ff7547829e.png
+-rw-r--r--   0 root         (0) root         (0)     7163 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/af253b1b82b79498bcedad50d30d155b.png
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/b2f8593cd54a831dd97a.png
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/b2fd4844280a4a216e7d.png
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/d5ce50f40bd2a5707619.gif
+-rw-r--r--   0 root         (0) root         (0)     7126 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/e30ce9397cddc63d3f1827d1d7153edf.png
+-rw-r--r--   0 root         (0) root         (0)      823 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/e38f33bbf55d6e20d21c4a10b9912668.gif
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/e47aff57d59b6c120c5c.png
+-rw-r--r--   0 root         (0) root         (0)     6539 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/e716c93fb8aa23c1e10b5185a8191dbf.png
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/extension.js
+-rw-r--r--   0 root         (0) root         (0)   925575 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/index.js
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/index.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)  2728248 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgrid/static/index.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgridtrusted.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15046 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgridtrusted.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1484 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgridtrusted.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgridtrusted.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgridtrusted.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/qgridtrusted.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1562 2024-04-04 05:22:36.000000 qgridtrusted-0.0.9/setup.py
```

### Comparing `qgridtrusted-0.0.8/LICENSE` & `qgridtrusted-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/PKG-INFO` & `qgridtrusted-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgridtrusted
-Version: 0.0.8
+Version: 0.0.9
 Summary: A fork of qgrid using trusted publishing.
 Author-email: Keith Maxwell <keith.maxwell@gmail.com>, "Quantopian Inc." <opensource@quantopian.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `qgridtrusted-0.0.8/README.md` & `qgridtrusted-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/README.rst` & `qgridtrusted-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/pyproject.toml` & `qgridtrusted-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/qgrid/__init__.py` & `qgridtrusted-0.0.9/qgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/qgrid/grid.py` & `qgridtrusted-0.0.9/qgrid/grid.py`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/qgrid/static/097df1053ff3246e2f1af9d5a858ac6c.gif` & `qgridtrusted-0.0.9/qgrid/static/097df1053ff3246e2f1af9d5a858ac6c.gif`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/qgrid/static/16fec672acf4e60b212d6f213cfea45d.png` & `qgridtrusted-0.0.9/qgrid/static/16fec672acf4e60b212d6f213cfea45d.png`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/qgrid/static/2487f1f6cffd2524ad3c4b8626540a04.png` & `qgridtrusted-0.0.9/qgrid/static/2487f1f6cffd2524ad3c4b8626540a04.png`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/qgrid/static/7e2ccbc3b7b736251403b238014dcacc.gif` & `qgridtrusted-0.0.9/qgrid/static/7e2ccbc3b7b736251403b238014dcacc.gif`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/qgrid/static/86586a919bd10f4cedba392f64336a54.gif` & `qgridtrusted-0.0.9/qgrid/static/86586a919bd10f4cedba392f64336a54.gif`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/qgrid/static/8fcbe60e4efd8e2d1742bba8486994e1.gif` & `qgridtrusted-0.0.9/qgrid/static/8fcbe60e4efd8e2d1742bba8486994e1.gif`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/qgrid/static/9a52a923ceb5983fa0943c1e24d6d35b.gif` & `qgridtrusted-0.0.9/qgrid/static/9a52a923ceb5983fa0943c1e24d6d35b.gif`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/qgrid/static/ae9b3e279d547e10151b58ff7547829e.png` & `qgridtrusted-0.0.9/qgrid/static/ae9b3e279d547e10151b58ff7547829e.png`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/qgrid/static/af253b1b82b79498bcedad50d30d155b.png` & `qgridtrusted-0.0.9/qgrid/static/af253b1b82b79498bcedad50d30d155b.png`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/qgrid/static/e30ce9397cddc63d3f1827d1d7153edf.png` & `qgridtrusted-0.0.9/qgrid/static/e30ce9397cddc63d3f1827d1d7153edf.png`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/qgrid/static/e38f33bbf55d6e20d21c4a10b9912668.gif` & `qgridtrusted-0.0.9/qgrid/static/e38f33bbf55d6e20d21c4a10b9912668.gif`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/qgrid/static/e716c93fb8aa23c1e10b5185a8191dbf.png` & `qgridtrusted-0.0.9/qgrid/static/e716c93fb8aa23c1e10b5185a8191dbf.png`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/qgrid/static/index.js` & `qgridtrusted-0.0.9/qgrid/static/index.js`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/qgrid/static/index.js.LICENSE.txt` & `qgridtrusted-0.0.9/qgrid/static/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/qgrid/static/index.js.map` & `qgridtrusted-0.0.9/qgrid/static/index.js.map`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/qgridtrusted.egg-info/PKG-INFO` & `qgridtrusted-0.0.9/qgridtrusted.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgridtrusted
-Version: 0.0.8
+Version: 0.0.9
 Summary: A fork of qgrid using trusted publishing.
 Author-email: Keith Maxwell <keith.maxwell@gmail.com>, "Quantopian Inc." <opensource@quantopian.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `qgridtrusted-0.0.8/qgridtrusted.egg-info/SOURCES.txt` & `qgridtrusted-0.0.9/qgridtrusted.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qgridtrusted-0.0.8/setup.py` & `qgridtrusted-0.0.9/setup.py`

 * *Files identical despite different names*

