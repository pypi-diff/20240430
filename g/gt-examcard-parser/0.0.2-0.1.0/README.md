# Comparing `tmp/gt-examcard-parser-0.0.2.tar.gz` & `tmp/gt_examcard_parser-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gt-examcard-parser-0.0.2.tar", last modified: Thu Jun  2 18:17:35 2022, max compression
+gzip compressed data, was "gt_examcard_parser-0.1.0.tar", last modified: Tue Apr 30 06:51:05 2024, max compression
```

## Comparing `gt-examcard-parser-0.0.2.tar` & `gt_examcard_parser-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 18:17:35.122408 gt-examcard-parser-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-06-02 18:17:15.000000 gt-examcard-parser-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-06-02 18:17:35.122408 gt-examcard-parser-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-06-02 18:17:15.000000 gt-examcard-parser-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 18:17:35.122408 gt-examcard-parser-0.0.2/examcard/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-06-02 18:17:15.000000 gt-examcard-parser-0.0.2/examcard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5015 2022-06-02 18:17:15.000000 gt-examcard-parser-0.0.2/examcard/examcard.py
--rw-r--r--   0 runner    (1001) docker     (121)      947 2022-06-02 18:17:15.000000 gt-examcard-parser-0.0.2/examcard/sz_funcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5627 2022-06-02 18:17:15.000000 gt-examcard-parser-0.0.2/examcard/sz_sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 18:17:35.122408 gt-examcard-parser-0.0.2/gt_examcard_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-06-02 18:17:34.000000 gt-examcard-parser-0.0.2/gt_examcard_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-06-02 18:17:35.000000 gt-examcard-parser-0.0.2/gt_examcard_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-02 18:17:34.000000 gt-examcard-parser-0.0.2/gt_examcard_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-02 18:17:35.000000 gt-examcard-parser-0.0.2/gt_examcard_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-02 18:17:35.122408 gt-examcard-parser-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-06-02 18:17:15.000000 gt-examcard-parser-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 18:17:35.122408 gt-examcard-parser-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 18:17:15.000000 gt-examcard-parser-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-06-02 18:17:15.000000 gt-examcard-parser-0.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-06-02 18:17:15.000000 gt-examcard-parser-0.0.2/tests/test_examcard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:51:05.561917 gt_examcard_parser-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-30 06:51:01.000000 gt_examcard_parser-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-30 06:51:05.561917 gt_examcard_parser-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-30 06:51:01.000000 gt_examcard_parser-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:51:05.561917 gt_examcard_parser-0.1.0/examcard/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 06:51:01.000000 gt_examcard_parser-0.1.0/examcard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-30 06:51:01.000000 gt_examcard_parser-0.1.0/examcard/examcard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-30 06:51:01.000000 gt_examcard_parser-0.1.0/examcard/sz_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-04-30 06:51:01.000000 gt_examcard_parser-0.1.0/examcard/sz_sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:51:05.561917 gt_examcard_parser-0.1.0/gt_examcard_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-30 06:51:05.000000 gt_examcard_parser-0.1.0/gt_examcard_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-30 06:51:05.000000 gt_examcard_parser-0.1.0/gt_examcard_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:51:05.000000 gt_examcard_parser-0.1.0/gt_examcard_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 06:51:05.000000 gt_examcard_parser-0.1.0/gt_examcard_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 06:51:05.561917 gt_examcard_parser-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-30 06:51:01.000000 gt_examcard_parser-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:51:05.561917 gt_examcard_parser-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:51:01.000000 gt_examcard_parser-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 06:51:01.000000 gt_examcard_parser-0.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-30 06:51:01.000000 gt_examcard_parser-0.1.0/tests/test_examcard.py
```

### Comparing `gt-examcard-parser-0.0.2/LICENSE` & `gt_examcard_parser-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gt-examcard-parser-0.0.2/PKG-INFO` & `gt_examcard_parser-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gt-examcard-parser
-Version: 0.0.2
+Version: 0.1.0
 Summary: Parser for Philips ExamCards
 Home-page: https://github.com/gyrotools/gt-examcard-parser
 Author: Martin Bührer
 Author-email: info@gyrotools.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gt-examcard-parser-0.0.2/examcard/examcard.py` & `gt_examcard_parser-0.1.0/examcard/examcard.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,22 +147,25 @@
         raise RuntimeError(f'error while parsing the ExamCard: {str(e)}')
 
     exec_step = _get_nodes_by_tag(root, 'ExecutionStep')
 
     # some info for the exam card
     out['General'] = _print_tag(root, 'ExamCard')
 
-    for one_step in exec_step:
+    for i, one_step in enumerate(exec_step):
         name, param_data, data_buff, scan_proc, scan_prop, proc_conf = _get_one_exec_step(root, one_step)
         # all needed nodes are ready now
 
         # decode the dataBuffer for sequence description
         # res = seq._get_data_buffer(data_buff, seq_cnt)
         # dataBuffer info only export to pdf as it contains image
 
+        if name is None:
+            name = filename.stem if i == 0 else f'{filename.stem}_{i}'
+
         # some more info for the sequence
         out[name] = _print_info_for_node(scan_proc, root)
 
         res = _print_info_for_node(scan_prop, root)
         out[name].update(res)
 
         res = _print_info_for_node(proc_conf, root)
```

### Comparing `gt-examcard-parser-0.0.2/examcard/sz_funcs.py` & `gt_examcard_parser-0.1.0/examcard/sz_funcs.py`

 * *Files identical despite different names*

### Comparing `gt-examcard-parser-0.0.2/examcard/sz_sequence.py` & `gt_examcard_parser-0.1.0/examcard/sz_sequence.py`

 * *Files identical despite different names*

### Comparing `gt-examcard-parser-0.0.2/gt_examcard_parser.egg-info/PKG-INFO` & `gt_examcard_parser-0.1.0/gt_examcard_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gt-examcard-parser
-Version: 0.0.2
+Version: 0.1.0
 Summary: Parser for Philips ExamCards
 Home-page: https://github.com/gyrotools/gt-examcard-parser
 Author: Martin Bührer
 Author-email: info@gyrotools.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gt-examcard-parser-0.0.2/setup.py` & `gt_examcard_parser-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gt-examcard-parser",
-    version="0.0.2",
+    version="0.1.0",
     author="Martin Bührer",
     author_email="info@gyrotools.com",
     description="Parser for Philips ExamCards",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gyrotools/gt-examcard-parser",
     packages=setuptools.find_packages(),
```

