# Comparing `tmp/argostranslate-1.9.4.tar.gz` & `tmp/argostranslate-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argostranslate-1.9.4.tar", last modified: Mon Apr 29 17:54:08 2024, max compression
+gzip compressed data, was "argostranslate-1.9.5.tar", last modified: Tue Apr 30 11:58:47 2024, max compression
```

## Comparing `argostranslate-1.9.4.tar` & `argostranslate-1.9.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-04-29 17:54:08.991991 argostranslate-1.9.4/
--rw-rw-r--   0 pj        (1000) pj        (1000)     1085 2023-06-02 23:17:46.000000 argostranslate-1.9.4/LICENSE
--rw-rw-r--   0 pj        (1000) pj        (1000)     9840 2024-04-29 17:54:08.991991 argostranslate-1.9.4/PKG-INFO
--rw-rw-r--   0 pj        (1000) pj        (1000)     9024 2024-04-29 17:52:23.000000 argostranslate-1.9.4/README.md
-drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-04-29 17:54:08.991991 argostranslate-1.9.4/argostranslate/
--rw-rw-r--   0 pj        (1000) pj        (1000)        0 2023-06-02 23:17:46.000000 argostranslate-1.9.4/argostranslate/__init__.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     4324 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/apis.py
--rw-rw-r--   0 pj        (1000) pj        (1000)    14371 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/apply_bpe.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     4313 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/argospm.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     2147 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/cli.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     2240 2023-06-02 23:17:46.000000 argostranslate-1.9.4/argostranslate/fewshot.py
--rw-rw-r--   0 pj        (1000) pj        (1000)      298 2023-06-02 23:17:46.000000 argostranslate-1.9.4/argostranslate/models.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     2269 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/networking.py
--rw-rw-r--   0 pj        (1000) pj        (1000)    13220 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/package.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     3287 2024-04-29 17:52:19.000000 argostranslate-1.9.4/argostranslate/sbd.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     3119 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/settings.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     6544 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/tags.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     2268 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/tokenizer.py
--rw-rw-r--   0 pj        (1000) pj        (1000)    23803 2024-04-29 17:52:19.000000 argostranslate-1.9.4/argostranslate/translate.py
--rw-rw-r--   0 pj        (1000) pj        (1000)      487 2024-03-13 15:02:19.000000 argostranslate-1.9.4/argostranslate/utils.py
-drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-04-29 17:54:08.991991 argostranslate-1.9.4/argostranslate.egg-info/
--rw-r--r--   0 pj        (1000) pj        (1000)     9840 2024-04-29 17:54:08.000000 argostranslate-1.9.4/argostranslate.egg-info/PKG-INFO
--rw-rw-r--   0 pj        (1000) pj        (1000)      695 2024-04-29 17:54:08.000000 argostranslate-1.9.4/argostranslate.egg-info/SOURCES.txt
--rw-rw-r--   0 pj        (1000) pj        (1000)        1 2024-04-29 17:54:08.000000 argostranslate-1.9.4/argostranslate.egg-info/dependency_links.txt
--rw-rw-r--   0 pj        (1000) pj        (1000)       84 2024-04-29 17:54:08.000000 argostranslate-1.9.4/argostranslate.egg-info/requires.txt
--rw-rw-r--   0 pj        (1000) pj        (1000)       21 2024-04-29 17:54:08.000000 argostranslate-1.9.4/argostranslate.egg-info/top_level.txt
-drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-04-29 17:54:08.991991 argostranslate-1.9.4/bin/
--rwxrwxr-x   0 pj        (1000) pj        (1000)       69 2023-06-02 23:17:46.000000 argostranslate-1.9.4/bin/argos-translate
--rw-rw-r--   0 pj        (1000) pj        (1000)       74 2023-06-02 23:17:47.000000 argostranslate-1.9.4/bin/argospm
--rw-rw-r--   0 pj        (1000) pj        (1000)       38 2024-04-29 17:54:08.991991 argostranslate-1.9.4/setup.cfg
--rw-rw-r--   0 pj        (1000) pj        (1000)     1224 2024-04-29 17:52:38.000000 argostranslate-1.9.4/setup.py
-drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-04-29 17:54:08.991991 argostranslate-1.9.4/tests/
--rw-rw-r--   0 pj        (1000) pj        (1000)        0 2024-03-13 15:02:19.000000 argostranslate-1.9.4/tests/__init__.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     2489 2024-03-13 15:02:19.000000 argostranslate-1.9.4/tests/test_package.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     4581 2024-03-13 15:02:19.000000 argostranslate-1.9.4/tests/test_translate.py
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-04-30 11:58:47.945257 argostranslate-1.9.5/
+-rw-rw-r--   0 pj        (1000) pj        (1000)     1085 2023-06-02 23:17:46.000000 argostranslate-1.9.5/LICENSE
+-rw-rw-r--   0 pj        (1000) pj        (1000)     9840 2024-04-30 11:58:47.945257 argostranslate-1.9.5/PKG-INFO
+-rw-rw-r--   0 pj        (1000) pj        (1000)     9024 2024-04-29 17:52:23.000000 argostranslate-1.9.5/README.md
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-04-30 11:58:47.945257 argostranslate-1.9.5/argostranslate/
+-rw-rw-r--   0 pj        (1000) pj        (1000)        0 2023-06-02 23:17:46.000000 argostranslate-1.9.5/argostranslate/__init__.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     4324 2024-03-13 15:02:19.000000 argostranslate-1.9.5/argostranslate/apis.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)    14371 2024-03-13 15:02:19.000000 argostranslate-1.9.5/argostranslate/apply_bpe.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     4313 2024-03-13 15:02:19.000000 argostranslate-1.9.5/argostranslate/argospm.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     2147 2024-03-13 15:02:19.000000 argostranslate-1.9.5/argostranslate/cli.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     2240 2023-06-02 23:17:46.000000 argostranslate-1.9.5/argostranslate/fewshot.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)      298 2023-06-02 23:17:46.000000 argostranslate-1.9.5/argostranslate/models.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     2269 2024-03-13 15:02:19.000000 argostranslate-1.9.5/argostranslate/networking.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)    13220 2024-03-13 15:02:19.000000 argostranslate-1.9.5/argostranslate/package.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     3287 2024-04-29 17:52:19.000000 argostranslate-1.9.5/argostranslate/sbd.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     3119 2024-03-13 15:02:19.000000 argostranslate-1.9.5/argostranslate/settings.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     6544 2024-03-13 15:02:19.000000 argostranslate-1.9.5/argostranslate/tags.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     2268 2024-03-13 15:02:19.000000 argostranslate-1.9.5/argostranslate/tokenizer.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)    23802 2024-04-30 11:22:07.000000 argostranslate-1.9.5/argostranslate/translate.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)      487 2024-03-13 15:02:19.000000 argostranslate-1.9.5/argostranslate/utils.py
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-04-30 11:58:47.945257 argostranslate-1.9.5/argostranslate.egg-info/
+-rw-r--r--   0 pj        (1000) pj        (1000)     9840 2024-04-30 11:58:47.000000 argostranslate-1.9.5/argostranslate.egg-info/PKG-INFO
+-rw-rw-r--   0 pj        (1000) pj        (1000)      695 2024-04-30 11:58:47.000000 argostranslate-1.9.5/argostranslate.egg-info/SOURCES.txt
+-rw-rw-r--   0 pj        (1000) pj        (1000)        1 2024-04-30 11:58:47.000000 argostranslate-1.9.5/argostranslate.egg-info/dependency_links.txt
+-rw-rw-r--   0 pj        (1000) pj        (1000)       84 2024-04-30 11:58:47.000000 argostranslate-1.9.5/argostranslate.egg-info/requires.txt
+-rw-rw-r--   0 pj        (1000) pj        (1000)       21 2024-04-30 11:58:47.000000 argostranslate-1.9.5/argostranslate.egg-info/top_level.txt
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-04-30 11:58:47.945257 argostranslate-1.9.5/bin/
+-rwxrwxr-x   0 pj        (1000) pj        (1000)       69 2023-06-02 23:17:46.000000 argostranslate-1.9.5/bin/argos-translate
+-rw-rw-r--   0 pj        (1000) pj        (1000)       74 2023-06-02 23:17:47.000000 argostranslate-1.9.5/bin/argospm
+-rw-rw-r--   0 pj        (1000) pj        (1000)       38 2024-04-30 11:58:47.945257 argostranslate-1.9.5/setup.cfg
+-rw-rw-r--   0 pj        (1000) pj        (1000)     1224 2024-04-30 11:57:41.000000 argostranslate-1.9.5/setup.py
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2024-04-30 11:58:47.945257 argostranslate-1.9.5/tests/
+-rw-rw-r--   0 pj        (1000) pj        (1000)        0 2024-03-13 15:02:19.000000 argostranslate-1.9.5/tests/__init__.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     2489 2024-03-13 15:02:19.000000 argostranslate-1.9.5/tests/test_package.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     4581 2024-03-13 15:02:19.000000 argostranslate-1.9.5/tests/test_translate.py
```

### Comparing `argostranslate-1.9.4/LICENSE` & `argostranslate-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.4/PKG-INFO` & `argostranslate-1.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argostranslate
-Version: 1.9.4
+Version: 1.9.5
 Summary: Open-source neural machine translation library based on OpenNMT's CTranslate2
 Home-page: https://www.argosopentech.com
 Author: Argos Open Technologies, LLC
 Author-email: admin@argosopentech.com
 License: UNKNOWN
 Project-URL: Website, https://www.argosopentech.com
 Project-URL: Documentation, https://argos-translate.readthedocs.io/en/latest/
```

### Comparing `argostranslate-1.9.4/README.md` & `argostranslate-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.4/argostranslate/apis.py` & `argostranslate-1.9.5/argostranslate/apis.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.4/argostranslate/apply_bpe.py` & `argostranslate-1.9.5/argostranslate/apply_bpe.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.4/argostranslate/argospm.py` & `argostranslate-1.9.5/argostranslate/argospm.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.4/argostranslate/cli.py` & `argostranslate-1.9.5/argostranslate/cli.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.4/argostranslate/fewshot.py` & `argostranslate-1.9.5/argostranslate/fewshot.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.4/argostranslate/networking.py` & `argostranslate-1.9.5/argostranslate/networking.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.4/argostranslate/package.py` & `argostranslate-1.9.5/argostranslate/package.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.4/argostranslate/sbd.py` & `argostranslate-1.9.5/argostranslate/sbd.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.4/argostranslate/settings.py` & `argostranslate-1.9.5/argostranslate/settings.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.4/argostranslate/tags.py` & `argostranslate-1.9.5/argostranslate/tags.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.4/argostranslate/tokenizer.py` & `argostranslate-1.9.5/argostranslate/tokenizer.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.4/argostranslate/translate.py` & `argostranslate-1.9.5/argostranslate/translate.py`

 * *Files 1% similar despite different names*

```diff
@@ -475,16 +475,16 @@
 
     # Build hypotheses
     value_hypotheses = []
     for i in range(num_hypotheses):
         translated_tokens = []
         cumulative_score = 0
         for translated_batch in translated_batches:
-            translated_tokens += translated_batch[i]["tokens"]
-            cumulative_score += translated_batch[i]["score"]
+            translated_tokens += translated_batch.hypotheses[i]
+            cumulative_score += translated_batch.scores[i]
         
         value = pkg.tokenizer.decode(translated_tokens)
         
         if pkg.target_prefix != "" and value.startswith(pkg.target_prefix):
             # Remove target prefix
             value = value[len(pkg.target_prefix):]
```

### Comparing `argostranslate-1.9.4/argostranslate.egg-info/PKG-INFO` & `argostranslate-1.9.5/argostranslate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argostranslate
-Version: 1.9.4
+Version: 1.9.5
 Summary: Open-source neural machine translation library based on OpenNMT's CTranslate2
 Home-page: https://www.argosopentech.com
 Author: Argos Open Technologies, LLC
 Author-email: admin@argosopentech.com
 License: UNKNOWN
 Project-URL: Website, https://www.argosopentech.com
 Project-URL: Documentation, https://argos-translate.readthedocs.io/en/latest/
```

### Comparing `argostranslate-1.9.4/argostranslate.egg-info/SOURCES.txt` & `argostranslate-1.9.5/argostranslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.4/setup.py` & `argostranslate-1.9.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     required_packages = f.read().splitlines()
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="argostranslate",
-    version="1.9.4",
+    version="1.9.5",
     description="Open-source neural machine translation library based on OpenNMT's CTranslate2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Argos Open Technologies, LLC",
     author_email="admin@argosopentech.com",
     url="https://www.argosopentech.com",
     project_urls={
```

### Comparing `argostranslate-1.9.4/tests/test_package.py` & `argostranslate-1.9.5/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `argostranslate-1.9.4/tests/test_translate.py` & `argostranslate-1.9.5/tests/test_translate.py`

 * *Files identical despite different names*

