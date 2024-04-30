# Comparing `tmp/cltrier_nlp-0.1.0.tar.gz` & `tmp/cltrier_nlp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cltrier_nlp-0.1.0.tar", max compression
+gzip compressed data, was "cltrier_nlp-0.1.1.tar", max compression
```

## Comparing `cltrier_nlp-0.1.0.tar` & `cltrier_nlp-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      538 2024-04-26 13:20:55.163189 cltrier_nlp-0.1.0/README.md
--rw-r--r--   0        0        0       47 2024-04-30 09:04:48.839522 cltrier_nlp-0.1.0/cltrier_nlp/__init__.py
--rw-r--r--   0        0        0       88 2024-04-26 13:12:47.738698 cltrier_nlp-0.1.0/cltrier_nlp/__main__.py
--rw-r--r--   0        0        0     1920 2024-04-26 13:08:04.208772 cltrier_nlp-0.1.0/cltrier_nlp/corpus/__init__.py
--rw-r--r--   0        0        0      630 2024-04-26 13:06:28.069980 cltrier_nlp-0.1.0/cltrier_nlp/corpus/sentence.py
--rw-r--r--   0        0        0      633 2024-04-26 12:34:22.552840 cltrier_nlp-0.1.0/cltrier_nlp/corpus/util.py
--rw-r--r--   0        0        0      618 2024-04-30 09:02:26.554084 cltrier_nlp-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1243 1970-01-01 00:00:00.000000 cltrier_nlp-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      538 2024-04-26 13:20:55.163189 cltrier_nlp-0.1.1/README.md
+-rw-r--r--   0        0        0       47 2024-04-30 09:04:48.839522 cltrier_nlp-0.1.1/cltrier_nlp/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-26 13:12:47.738698 cltrier_nlp-0.1.1/cltrier_nlp/__main__.py
+-rw-r--r--   0        0        0     1920 2024-04-26 13:08:04.208772 cltrier_nlp-0.1.1/cltrier_nlp/corpus/__init__.py
+-rw-r--r--   0        0        0      630 2024-04-26 13:06:28.069980 cltrier_nlp-0.1.1/cltrier_nlp/corpus/sentence.py
+-rw-r--r--   0        0        0      633 2024-04-26 12:34:22.552840 cltrier_nlp-0.1.1/cltrier_nlp/corpus/util.py
+-rw-r--r--   0        0        0      623 2024-04-30 09:25:14.068101 cltrier_nlp-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1253 1970-01-01 00:00:00.000000 cltrier_nlp-0.1.1/PKG-INFO
```

### Comparing `cltrier_nlp-0.1.0/README.md` & `cltrier_nlp-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.0/cltrier_nlp/corpus/__init__.py` & `cltrier_nlp-0.1.1/cltrier_nlp/corpus/__init__.py`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.0/cltrier_nlp/corpus/sentence.py` & `cltrier_nlp-0.1.1/cltrier_nlp/corpus/sentence.py`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.0/cltrier_nlp/corpus/util.py` & `cltrier_nlp-0.1.1/cltrier_nlp/corpus/util.py`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.0/pyproject.toml` & `cltrier_nlp-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cltrier_nlp"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Simon Münker <muenker@uni-trier.de>"]
 readme = "README.md"
 license = "Apache-2.0"
-repository = "https://github.com/python-poetry/poetry"
+repository = "https://github.com/simon-muenker/cltrier_nlp"
 packages = [{include = "cltrier_nlp"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 nltk = "^3.8.1"
 pydantic = "^2.7.1"
 langdetect = "^1.0.9"
```

### Comparing `cltrier_nlp-0.1.0/PKG-INFO` & `cltrier_nlp-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cltrier_nlp
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
-Home-page: https://github.com/python-poetry/poetry
+Home-page: https://github.com/simon-muenker/cltrier_nlp
 License: Apache-2.0
 Author: Simon Münker
 Author-email: muenker@uni-trier.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: langcodes (>=3.4.0,<4.0.0)
 Requires-Dist: langdetect (>=1.0.9,<2.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
-Project-URL: Repository, https://github.com/python-poetry/poetry
+Project-URL: Repository, https://github.com/simon-muenker/cltrier_nlp
 Description-Content-Type: text/markdown
 
 # Project Repository: NLP Course (M.Sc. NLP, University Trier)
 
 ## Usage
 
 ### Install
```

