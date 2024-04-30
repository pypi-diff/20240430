# Comparing `tmp/kairyou-1.6.0.tar.gz` & `tmp/kairyou-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kairyou-1.6.0.tar", last modified: Mon Apr 22 18:42:35 2024, max compression
+gzip compressed data, was "kairyou-1.6.1.tar", last modified: Tue Apr 30 02:50:30 2024, max compression
```

## Comparing `kairyou-1.6.0.tar` & `kairyou-1.6.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:42:35.486013 kairyou-1.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:42:35.478012 kairyou-1.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:42:35.478012 kairyou-1.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-22 18:41:46.000000 kairyou-1.6.0/.github/workflows/workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-22 18:41:46.000000 kairyou-1.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-22 18:41:46.000000 kairyou-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-04-22 18:42:35.486013 kairyou-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10292 2024-04-22 18:41:46.000000 kairyou-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:42:35.482013 kairyou-1.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-22 18:41:46.000000 kairyou-1.6.0/examples/blank_fukuin.json
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-22 18:41:46.000000 kairyou-1.6.0/examples/blank_kudasai.json
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-04-22 18:41:46.000000 kairyou-1.6.0/examples/cote_fukuin.json
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-22 18:41:46.000000 kairyou-1.6.0/examples/cote_kudasai.json
--rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-04-22 18:41:46.000000 kairyou-1.6.0/examples/demo_sample_text.txt
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-22 18:41:46.000000 kairyou-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 18:42:35.486013 kairyou-1.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:42:35.478012 kairyou-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:42:35.482013 kairyou-1.6.0/src/kairyou/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-22 18:41:46.000000 kairyou-1.6.0/src/kairyou/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-22 18:41:46.000000 kairyou-1.6.0/src/kairyou/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17100 2024-04-22 18:41:46.000000 kairyou-1.6.0/src/kairyou/indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20899 2024-04-22 18:41:46.000000 kairyou-1.6.0/src/kairyou/kairyou.py
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-04-22 18:41:46.000000 kairyou-1.6.0/src/kairyou/katakana_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-22 18:41:46.000000 kairyou-1.6.0/src/kairyou/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-04-22 18:41:46.000000 kairyou-1.6.0/src/kairyou/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-22 18:41:46.000000 kairyou-1.6.0/src/kairyou/version.py
--rw-r--r--   0 runner    (1001) docker     (127)   190296 2024-04-22 18:41:46.000000 kairyou-1.6.0/src/kairyou/words.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:42:35.486013 kairyou-1.6.0/src/kairyou.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-04-22 18:42:35.000000 kairyou-1.6.0/src/kairyou.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-22 18:42:35.000000 kairyou-1.6.0/src/kairyou.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 18:42:35.000000 kairyou-1.6.0/src/kairyou.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-22 18:42:35.000000 kairyou-1.6.0/src/kairyou.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 18:42:35.000000 kairyou-1.6.0/src/kairyou.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:42:35.486013 kairyou-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-22 18:41:46.000000 kairyou-1.6.0/tests/passing.py
--rw-r--r--   0 runner    (1001) docker     (127)    35171 2024-04-22 18:41:46.000000 kairyou-1.6.0/tests/testing_knowledge_base.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-22 18:41:46.000000 kairyou-1.6.0/tests/testing_preprocessing_text.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-22 18:41:46.000000 kairyou-1.6.0/tests/testing_replacements.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:50:30.459461 kairyou-1.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:50:30.451461 kairyou-1.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:50:30.455461 kairyou-1.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-30 02:49:46.000000 kairyou-1.6.1/.github/workflows/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-30 02:49:46.000000 kairyou-1.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-30 02:49:46.000000 kairyou-1.6.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-04-30 02:50:30.459461 kairyou-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10285 2024-04-30 02:49:46.000000 kairyou-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:50:30.455461 kairyou-1.6.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-30 02:49:46.000000 kairyou-1.6.1/examples/blank_fukuin.json
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-30 02:49:46.000000 kairyou-1.6.1/examples/blank_kudasai.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-04-30 02:49:46.000000 kairyou-1.6.1/examples/cote_fukuin.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-30 02:49:46.000000 kairyou-1.6.1/examples/cote_kudasai.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-04-30 02:49:46.000000 kairyou-1.6.1/examples/demo_sample_text.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-30 02:49:46.000000 kairyou-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 02:50:30.459461 kairyou-1.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:50:30.451461 kairyou-1.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:50:30.455461 kairyou-1.6.1/src/kairyou/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-30 02:49:46.000000 kairyou-1.6.1/src/kairyou/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-30 02:49:46.000000 kairyou-1.6.1/src/kairyou/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17100 2024-04-30 02:49:46.000000 kairyou-1.6.1/src/kairyou/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20988 2024-04-30 02:49:46.000000 kairyou-1.6.1/src/kairyou/kairyou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-04-30 02:49:46.000000 kairyou-1.6.1/src/kairyou/katakana_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-30 02:49:46.000000 kairyou-1.6.1/src/kairyou/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-04-30 02:49:46.000000 kairyou-1.6.1/src/kairyou/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-30 02:49:46.000000 kairyou-1.6.1/src/kairyou/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190296 2024-04-30 02:49:46.000000 kairyou-1.6.1/src/kairyou/words.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:50:30.459461 kairyou-1.6.1/src/kairyou.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-04-30 02:50:30.000000 kairyou-1.6.1/src/kairyou.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-30 02:50:30.000000 kairyou-1.6.1/src/kairyou.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 02:50:30.000000 kairyou-1.6.1/src/kairyou.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 02:50:30.000000 kairyou-1.6.1/src/kairyou.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 02:50:30.000000 kairyou-1.6.1/src/kairyou.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 02:50:30.459461 kairyou-1.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-30 02:49:46.000000 kairyou-1.6.1/tests/passing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35171 2024-04-30 02:49:46.000000 kairyou-1.6.1/tests/testing_knowledge_base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-30 02:49:46.000000 kairyou-1.6.1/tests/testing_preprocessing_text.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-30 02:49:46.000000 kairyou-1.6.1/tests/testing_replacements.json
```

### Comparing `kairyou-1.6.0/.github/workflows/workflow.yml` & `kairyou-1.6.1/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `kairyou-1.6.0/.gitignore` & `kairyou-1.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `kairyou-1.6.0/LICENSE.md` & `kairyou-1.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kairyou-1.6.0/PKG-INFO` & `kairyou-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: kairyou
-Version: 1.6.0
+Version: 1.6.1
 Summary: Quickly preprocesses Japanese text using NLP/NER from SpaCy for Japanese translation or other NLP tasks.
-Author-email: Bikatr7 <Tetralon07@gmail.com>
+Author-email: Bikatr7 <Bikatr7@proton.me>
 Project-URL: Homepage, https://github.com/Bikatr7/Kairyou
 Project-URL: Issues, https://github.com/Bikatr7/Kairyou/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
@@ -194,15 +194,15 @@
 
 For a thorough explanation of the conditions and how they may apply to your use of the project, please review the full license text. This comprehensive documentation will offer guidance on your rights and obligations when utilizing LGPLv2.1 licensed software.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **Contact**<a name="contact"></a>
 
-If you have any questions or suggestions, feel free to reach out to me at [Tetralon07@gmail.com](mailto:Tetralon07@gmail.com).
+If you have any questions or suggestions, feel free to reach out to me at [Bikatr7@proton.me](mailto:Bikatr7@proton.me)
 
 Also feel free to check out the [GitHub repository](https://github.com/Bikatr7/Kairyou) for this project.
 
 Or the issue tracker [here](https://github.com/Bikatr7/Kairyou/issues).
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
```

### Comparing `kairyou-1.6.0/README.md` & `kairyou-1.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 
 For a thorough explanation of the conditions and how they may apply to your use of the project, please review the full license text. This comprehensive documentation will offer guidance on your rights and obligations when utilizing LGPLv2.1 licensed software.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **Contact**<a name="contact"></a>
 
-If you have any questions or suggestions, feel free to reach out to me at [Tetralon07@gmail.com](mailto:Tetralon07@gmail.com).
+If you have any questions or suggestions, feel free to reach out to me at [Bikatr7@proton.me](mailto:Bikatr7@proton.me)
 
 Also feel free to check out the [GitHub repository](https://github.com/Bikatr7/Kairyou) for this project.
 
 Or the issue tracker [here](https://github.com/Bikatr7/Kairyou/issues).
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
```

### Comparing `kairyou-1.6.0/examples/cote_fukuin.json` & `kairyou-1.6.1/examples/cote_fukuin.json`

 * *Files identical despite different names*

### Comparing `kairyou-1.6.0/examples/cote_kudasai.json` & `kairyou-1.6.1/examples/cote_kudasai.json`

 * *Files identical despite different names*

### Comparing `kairyou-1.6.0/examples/demo_sample_text.txt` & `kairyou-1.6.1/examples/demo_sample_text.txt`

 * *Files identical despite different names*

### Comparing `kairyou-1.6.0/pyproject.toml` & `kairyou-1.6.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 [project]
 dependencies = [
     "spacy>=3.7.0,<3.8.0"
 ]
 
 name = "kairyou"
-version = "v1.6.0"
+version = "v1.6.1"
 authors = [
-  { name="Bikatr7", email="Tetralon07@gmail.com" },
+  { name="Bikatr7", email="Bikatr7@proton.me" },
 ]
 description = "Quickly preprocesses Japanese text using NLP/NER from SpaCy for Japanese translation or other NLP tasks."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
```

### Comparing `kairyou-1.6.0/src/kairyou/exceptions.py` & `kairyou-1.6.1/src/kairyou/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,16 +6,36 @@
 
 class KairyouException(Exception):
 
     """
     
     Base exception class for Kairyou.
     
+
+    """
+
+##-------------------start-of-SpacyModelNotFound---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+
+class SpacyModelNotFound(KairyouException):
+
     """
 
+    Exception raised when the spacy model is not found.
+
+    """
+
+##-------------------start-of-__init__()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+    def __init__(self):
+                
+        message = f"Spacy model ja_core_news_lg not found. Please download the model using the following command: python -m spacy download ja_core_news_lg\n"
+        
+        super().__init__(message)
+
 ##-------------------start-of-InvalidReplacementJsonName---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 class InvalidReplacementJsonName(KairyouException):
 
     """
 
     Exception raised when the replacement json file is invalid.
```

### Comparing `kairyou-1.6.0/src/kairyou/indexer.py` & `kairyou-1.6.1/src/kairyou/indexer.py`

 * *Files identical despite different names*

### Comparing `kairyou-1.6.0/src/kairyou/kairyou.py` & `kairyou-1.6.1/src/kairyou/kairyou.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ## third-party libraries
 import spacy
 
 ## custom modules
 from .katakana_util import KatakanaUtil
 from .util import _validate_replacement_json, _get_elapsed_time, Name, ReplacementType, _kudasai_blank_json, _fukuin_blank_json, _kudasai_replacement_rules
-from .exceptions import  InvalidReplacementJsonName, InvalidReplacementJsonPath, InvalidPreprocessingText
+from .exceptions import  InvalidReplacementJsonName, InvalidReplacementJsonPath, InvalidPreprocessingText, SpacyModelNotFound
 
 # -------------------start-of-Kairyou---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 
 class Kairyou:
 
     """
@@ -50,15 +50,19 @@
     _json_type:typing.Literal["kudasai", "fukuin"] = "kudasai"
 
     _replacement_rules:typing.List = _kudasai_replacement_rules
 
     #----------------------------/
 
     ## The spacy NER model used for enhanced replacement checking.
-    _ner = spacy.load("ja_core_news_lg")
+    try:
+        _ner = spacy.load("ja_core_news_lg")
+
+    except Exception:
+        raise SpacyModelNotFound
     
 ##-------------------start-of-_reset_globals()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def _reset_globals() -> None:
 
         """
```

### Comparing `kairyou-1.6.0/src/kairyou/katakana_util.py` & `kairyou-1.6.1/src/kairyou/katakana_util.py`

 * *Files identical despite different names*

### Comparing `kairyou-1.6.0/src/kairyou/util.py` & `kairyou-1.6.1/src/kairyou/util.py`

 * *Files identical despite different names*

### Comparing `kairyou-1.6.0/src/kairyou/words.py` & `kairyou-1.6.1/src/kairyou/words.py`

 * *Files identical despite different names*

### Comparing `kairyou-1.6.0/src/kairyou.egg-info/PKG-INFO` & `kairyou-1.6.1/src/kairyou.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: kairyou
-Version: 1.6.0
+Version: 1.6.1
 Summary: Quickly preprocesses Japanese text using NLP/NER from SpaCy for Japanese translation or other NLP tasks.
-Author-email: Bikatr7 <Tetralon07@gmail.com>
+Author-email: Bikatr7 <Bikatr7@proton.me>
 Project-URL: Homepage, https://github.com/Bikatr7/Kairyou
 Project-URL: Issues, https://github.com/Bikatr7/Kairyou/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
@@ -194,15 +194,15 @@
 
 For a thorough explanation of the conditions and how they may apply to your use of the project, please review the full license text. This comprehensive documentation will offer guidance on your rights and obligations when utilizing LGPLv2.1 licensed software.
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
 
 **Contact**<a name="contact"></a>
 
-If you have any questions or suggestions, feel free to reach out to me at [Tetralon07@gmail.com](mailto:Tetralon07@gmail.com).
+If you have any questions or suggestions, feel free to reach out to me at [Bikatr7@proton.me](mailto:Bikatr7@proton.me)
 
 Also feel free to check out the [GitHub repository](https://github.com/Bikatr7/Kairyou) for this project.
 
 Or the issue tracker [here](https://github.com/Bikatr7/Kairyou/issues).
 
 ---------------------------------------------------------------------------------------------------------------------------------------------------
```

### Comparing `kairyou-1.6.0/src/kairyou.egg-info/SOURCES.txt` & `kairyou-1.6.1/src/kairyou.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kairyou-1.6.0/tests/passing.py` & `kairyou-1.6.1/tests/passing.py`

 * *Files identical despite different names*

### Comparing `kairyou-1.6.0/tests/testing_knowledge_base.txt` & `kairyou-1.6.1/tests/testing_knowledge_base.txt`

 * *Files identical despite different names*

### Comparing `kairyou-1.6.0/tests/testing_preprocessing_text.txt` & `kairyou-1.6.1/tests/testing_preprocessing_text.txt`

 * *Files identical despite different names*

### Comparing `kairyou-1.6.0/tests/testing_replacements.json` & `kairyou-1.6.1/tests/testing_replacements.json`

 * *Files identical despite different names*

