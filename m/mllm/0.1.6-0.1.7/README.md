# Comparing `tmp/mllm-0.1.6.tar.gz` & `tmp/mllm-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mllm-0.1.6.tar", max compression
+gzip compressed data, was "mllm-0.1.7.tar", max compression
```

## Comparing `mllm-0.1.6.tar` & `mllm-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2024-04-27 16:19:02.140835 mllm-0.1.6/LICENSE
--rw-r--r--   0        0        0     2221 2024-04-29 21:12:11.290383 mllm-0.1.6/README.md
--rw-r--r--   0        0        0      149 2024-04-29 21:17:19.261017 mllm-0.1.6/mllm/__init__.py
--rw-r--r--   0        0        0     2249 2024-04-30 02:56:14.276096 mllm-0.1.6/mllm/db/conn.py
--rw-r--r--   0        0        0      541 2024-04-27 16:19:02.141445 mllm-0.1.6/mllm/db/models.py
--rw-r--r--   0        0        0      846 2024-04-29 21:16:16.874384 mllm-0.1.6/mllm/models.py
--rw-r--r--   0        0        0     5605 2024-04-30 21:03:51.206117 mllm-0.1.6/mllm/prompt.py
--rw-r--r--   0        0        0     8299 2024-04-29 21:17:12.773037 mllm-0.1.6/mllm/router.py
--rw-r--r--   0        0        0      793 2024-04-29 21:17:15.851578 mllm-0.1.6/mllm/util.py
--rw-r--r--   0        0        0      390 2024-04-30 21:04:07.909036 mllm-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2790 1970-01-01 00:00:00.000000 mllm-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-27 16:19:02.140835 mllm-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2221 2024-04-29 21:12:11.290383 mllm-0.1.7/README.md
+-rw-r--r--   0        0        0      149 2024-04-29 21:17:19.261017 mllm-0.1.7/mllm/__init__.py
+-rw-r--r--   0        0        0     2249 2024-04-30 02:56:14.276096 mllm-0.1.7/mllm/db/conn.py
+-rw-r--r--   0        0        0      541 2024-04-27 16:19:02.141445 mllm-0.1.7/mllm/db/models.py
+-rw-r--r--   0        0        0      846 2024-04-29 21:16:16.874384 mllm-0.1.7/mllm/models.py
+-rw-r--r--   0        0        0     5605 2024-04-30 21:03:51.206117 mllm-0.1.7/mllm/prompt.py
+-rw-r--r--   0        0        0     8299 2024-04-29 21:17:12.773037 mllm-0.1.7/mllm/router.py
+-rw-r--r--   0        0        0      793 2024-04-29 21:17:15.851578 mllm-0.1.7/mllm/util.py
+-rw-r--r--   0        0        0      390 2024-04-30 21:37:42.022957 mllm-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2790 1970-01-01 00:00:00.000000 mllm-0.1.7/PKG-INFO
```

### Comparing `mllm-0.1.6/LICENSE` & `mllm-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mllm-0.1.6/README.md` & `mllm-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mllm-0.1.6/mllm/db/conn.py` & `mllm-0.1.7/mllm/db/conn.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.6/mllm/db/models.py` & `mllm-0.1.7/mllm/db/models.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.6/mllm/models.py` & `mllm-0.1.7/mllm/models.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.6/mllm/prompt.py` & `mllm-0.1.7/mllm/prompt.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.6/mllm/router.py` & `mllm-0.1.7/mllm/router.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.6/mllm/util.py` & `mllm-0.1.7/mllm/util.py`

 * *Files identical despite different names*

### Comparing `mllm-0.1.6/PKG-INFO` & `mllm-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: mllm
-Version: 0.1.6
+Version: 0.1.7
 Summary: Multimodal Large Language Models
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: litellm (>=1.35.29,<2.0.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
-Requires-Dist: threadmem (>=0.2.24,<0.3.0)
+Requires-Dist: threadmem (>=0.2.25,<0.3.0)
 Description-Content-Type: text/markdown
 
 # MLLM
 
 MultiModal Large Language Models
 
 ## Installation
```

