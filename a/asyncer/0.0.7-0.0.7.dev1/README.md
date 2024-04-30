# Comparing `tmp/asyncer-0.0.7.tar.gz` & `tmp/asyncer-0.0.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncer-0.0.7.tar", last modified: Tue Apr 30 06:25:54 2024, max compression
+gzip compressed data, was "asyncer-0.0.7.dev1.tar", last modified: Tue Apr 30 01:08:38 2024, max compression
```

## Comparing `asyncer-0.0.7.tar` & `asyncer-0.0.7.dev1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1086 2024-04-30 06:25:50.283696 asyncer-0.0.7/LICENSE
--rw-r--r--   0        0        0     5297 2024-04-30 06:25:50.283696 asyncer-0.0.7/README.md
--rw-r--r--   0        0        0      347 2024-04-30 06:25:50.283696 asyncer-0.0.7/asyncer/__init__.py
--rw-r--r--   0        0        0    13107 2024-04-30 06:25:50.283696 asyncer-0.0.7/asyncer/_main.py
--rw-r--r--   0        0        0        0 2024-04-30 06:25:50.283696 asyncer-0.0.7/asyncer/py.typed
--rw-r--r--   0        0        0        0 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/tutorial/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/tutorial/asyncify/__init__.py
--rw-r--r--   0        0        0      201 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/tutorial/asyncify/tutorial001.py
--rw-r--r--   0        0        0      246 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/tutorial/asyncify/tutorial002.py
--rw-r--r--   0        0        0        0 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/tutorial/first_steps/__init__.py
--rw-r--r--   0        0        0      220 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/tutorial/first_steps/tutorial001.py
--rw-r--r--   0        0        0        0 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/tutorial/runnify/__init__.py
--rw-r--r--   0        0        0      259 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/tutorial/runnify/tutorial001.py
--rw-r--r--   0        0        0        0 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/tutorial/soonify/__init__.py
--rw-r--r--   0        0        0      279 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/tutorial/soonify/tutorial001.py
--rw-r--r--   0        0        0      406 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/tutorial/soonify/tutorial002.py
--rw-r--r--   0        0        0        0 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/tutorial/soonify_return/__init__.py
--rw-r--r--   0        0        0      611 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/tutorial/soonify_return/tutorial001.py
--rw-r--r--   0        0        0      644 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/tutorial/soonify_return/tutorial002.py
--rw-r--r--   0        0        0      728 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/tutorial/soonify_return/tutorial003.py
--rw-r--r--   0        0        0        0 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/tutorial/syncify/__init__.py
--rw-r--r--   0        0        0      385 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/tutorial/syncify/tutorial001.py
--rw-r--r--   0        0        0        0 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/tutorial/syncify_no_raise/__init__.py
--rw-r--r--   0        0        0      505 2024-04-30 06:25:50.287696 asyncer-0.0.7/docs_src/tutorial/syncify_no_raise/tutorial001.py
--rw-r--r--   0        0        0     1722 2024-04-30 06:25:50.287696 asyncer-0.0.7/pdm_build.py
--rw-r--r--   0        0        0     2451 2024-04-30 06:25:54.955714 asyncer-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      438 2024-04-30 06:25:50.287696 asyncer-0.0.7/requirements-docs.txt
--rw-r--r--   0        0        0       80 2024-04-30 06:25:50.287696 asyncer-0.0.7/requirements-tests.txt
--rw-r--r--   0        0        0       85 2024-04-30 06:25:50.287696 asyncer-0.0.7/requirements.txt
--rwxr-xr-x   0        0        0      131 2024-04-30 06:25:50.287696 asyncer-0.0.7/scripts/docs-live.sh
--rwxr-xr-x   0        0        0       96 2024-04-30 06:25:50.287696 asyncer-0.0.7/scripts/format.sh
--rwxr-xr-x   0        0        0      126 2024-04-30 06:25:50.287696 asyncer-0.0.7/scripts/lint.sh
--rwxr-xr-x   0        0        0      105 2024-04-30 06:25:50.287696 asyncer-0.0.7/scripts/test-files.sh
--rwxr-xr-x   0        0        0      127 2024-04-30 06:25:50.287696 asyncer-0.0.7/scripts/test.sh
--rw-r--r--   0        0        0        0 2024-04-30 06:25:50.287696 asyncer-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0      309 2024-04-30 06:25:50.287696 asyncer-0.0.7/tests/conftest.py
--rw-r--r--   0        0        0      100 2024-04-30 06:25:50.287696 asyncer-0.0.7/tests/test_others.py
--rw-r--r--   0        0        0     2690 2024-04-30 06:25:50.287696 asyncer-0.0.7/tests/test_syncify_no_raise.py
--rw-r--r--   0        0        0        0 2024-04-30 06:25:50.287696 asyncer-0.0.7/tests/test_tutorial/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 06:25:50.287696 asyncer-0.0.7/tests/test_tutorial/test_asyncify/__init__.py
--rw-r--r--   0        0        0      348 2024-04-30 06:25:50.287696 asyncer-0.0.7/tests/test_tutorial/test_asyncify/test_tutorial001.py
--rw-r--r--   0        0        0      348 2024-04-30 06:25:50.287696 asyncer-0.0.7/tests/test_tutorial/test_asyncify/test_tutorial002.py
--rw-r--r--   0        0        0        0 2024-04-30 06:25:50.291696 asyncer-0.0.7/tests/test_tutorial/test_first_steps/__init__.py
--rw-r--r--   0        0        0      355 2024-04-30 06:25:50.291696 asyncer-0.0.7/tests/test_tutorial/test_first_steps/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-04-30 06:25:50.291696 asyncer-0.0.7/tests/test_tutorial/test_runnify/__init__.py
--rw-r--r--   0        0        0      351 2024-04-30 06:25:50.291696 asyncer-0.0.7/tests/test_tutorial/test_runnify/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-04-30 06:25:50.291696 asyncer-0.0.7/tests/test_tutorial/test_soonify/__init__.py
--rw-r--r--   0        0        0      385 2024-04-30 06:25:50.291696 asyncer-0.0.7/tests/test_tutorial/test_soonify/test_tutorial001.py
--rw-r--r--   0        0        0      385 2024-04-30 06:25:50.291696 asyncer-0.0.7/tests/test_tutorial/test_soonify/test_tutorial002.py
--rw-r--r--   0        0        0        0 2024-04-30 06:25:50.291696 asyncer-0.0.7/tests/test_tutorial/test_soonify_return/__init__.py
--rw-r--r--   0        0        0      392 2024-04-30 06:25:50.291696 asyncer-0.0.7/tests/test_tutorial/test_soonify_return/test_tutorial001.py
--rw-r--r--   0        0        0      833 2024-04-30 06:25:50.291696 asyncer-0.0.7/tests/test_tutorial/test_soonify_return/test_tutorial002.py
--rw-r--r--   0        0        0      464 2024-04-30 06:25:50.291696 asyncer-0.0.7/tests/test_tutorial/test_soonify_return/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-04-30 06:25:50.291696 asyncer-0.0.7/tests/test_tutorial/test_syncify/__init__.py
--rw-r--r--   0        0        0      347 2024-04-30 06:25:50.291696 asyncer-0.0.7/tests/test_tutorial/test_syncify/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-04-30 06:25:50.291696 asyncer-0.0.7/tests/test_tutorial/test_syncify_no_raise/__init__.py
--rw-r--r--   0        0        0      379 2024-04-30 06:25:50.291696 asyncer-0.0.7/tests/test_tutorial/test_syncify_no_raise/test_tutorial001.py
--rw-r--r--   0        0        0     6602 1970-01-01 00:00:00.000000 asyncer-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-04-30 01:08:35.489572 asyncer-0.0.7.dev1/LICENSE
+-rw-r--r--   0        0        0     5297 2024-04-30 01:08:35.489572 asyncer-0.0.7.dev1/README.md
+-rw-r--r--   0        0        0      352 2024-04-30 01:08:35.489572 asyncer-0.0.7.dev1/asyncer/__init__.py
+-rw-r--r--   0        0        0    13107 2024-04-30 01:08:35.489572 asyncer-0.0.7.dev1/asyncer/_main.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:35.489572 asyncer-0.0.7.dev1/asyncer/py.typed
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/tutorial/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/tutorial/asyncify/__init__.py
+-rw-r--r--   0        0        0      201 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/tutorial/asyncify/tutorial001.py
+-rw-r--r--   0        0        0      246 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/tutorial/asyncify/tutorial002.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/tutorial/first_steps/__init__.py
+-rw-r--r--   0        0        0      220 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/tutorial/first_steps/tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/tutorial/runnify/__init__.py
+-rw-r--r--   0        0        0      259 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/tutorial/runnify/tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/tutorial/soonify/__init__.py
+-rw-r--r--   0        0        0      279 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/tutorial/soonify/tutorial001.py
+-rw-r--r--   0        0        0      406 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/tutorial/soonify/tutorial002.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/tutorial/soonify_return/__init__.py
+-rw-r--r--   0        0        0      611 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/tutorial/soonify_return/tutorial001.py
+-rw-r--r--   0        0        0      644 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/tutorial/soonify_return/tutorial002.py
+-rw-r--r--   0        0        0      728 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/tutorial/soonify_return/tutorial003.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/tutorial/syncify/__init__.py
+-rw-r--r--   0        0        0      385 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/tutorial/syncify/tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/tutorial/syncify_no_raise/__init__.py
+-rw-r--r--   0        0        0      505 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/docs_src/tutorial/syncify_no_raise/tutorial001.py
+-rw-r--r--   0        0        0     1722 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/pdm_build.py
+-rw-r--r--   0        0        0     2456 2024-04-30 01:08:38.189578 asyncer-0.0.7.dev1/pyproject.toml
+-rw-r--r--   0        0        0      438 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/requirements-docs.txt
+-rw-r--r--   0        0        0       80 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/requirements-tests.txt
+-rw-r--r--   0        0        0       85 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/requirements.txt
+-rwxr-xr-x   0        0        0      131 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/scripts/docs-live.sh
+-rwxr-xr-x   0        0        0       96 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/scripts/format.sh
+-rwxr-xr-x   0        0        0      126 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/scripts/lint.sh
+-rwxr-xr-x   0        0        0      105 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/scripts/test-files.sh
+-rwxr-xr-x   0        0        0      127 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/scripts/test.sh
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/__init__.py
+-rw-r--r--   0        0        0      309 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/conftest.py
+-rw-r--r--   0        0        0      100 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_others.py
+-rw-r--r--   0        0        0     2690 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_syncify_no_raise.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_tutorial/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_tutorial/test_asyncify/__init__.py
+-rw-r--r--   0        0        0      348 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_tutorial/test_asyncify/test_tutorial001.py
+-rw-r--r--   0        0        0      348 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_tutorial/test_asyncify/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_tutorial/test_first_steps/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_tutorial/test_first_steps/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_tutorial/test_runnify/__init__.py
+-rw-r--r--   0        0        0      351 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_tutorial/test_runnify/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_tutorial/test_soonify/__init__.py
+-rw-r--r--   0        0        0      385 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_tutorial/test_soonify/test_tutorial001.py
+-rw-r--r--   0        0        0      385 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_tutorial/test_soonify/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_tutorial/test_soonify_return/__init__.py
+-rw-r--r--   0        0        0      392 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_tutorial/test_soonify_return/test_tutorial001.py
+-rw-r--r--   0        0        0      833 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_tutorial/test_soonify_return/test_tutorial002.py
+-rw-r--r--   0        0        0      464 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_tutorial/test_soonify_return/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_tutorial/test_syncify/__init__.py
+-rw-r--r--   0        0        0      347 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_tutorial/test_syncify/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_tutorial/test_syncify_no_raise/__init__.py
+-rw-r--r--   0        0        0      379 2024-04-30 01:08:35.497573 asyncer-0.0.7.dev1/tests/test_tutorial/test_syncify_no_raise/test_tutorial001.py
+-rw-r--r--   0        0        0     6607 1970-01-01 00:00:00.000000 asyncer-0.0.7.dev1/PKG-INFO
```

### Comparing `asyncer-0.0.7/LICENSE` & `asyncer-0.0.7.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncer-0.0.7/README.md` & `asyncer-0.0.7.dev1/README.md`

 * *Files identical despite different names*

### Comparing `asyncer-0.0.7/asyncer/_main.py` & `asyncer-0.0.7.dev1/asyncer/_main.py`

 * *Files identical despite different names*

### Comparing `asyncer-0.0.7/docs_src/tutorial/soonify_return/tutorial001.py` & `asyncer-0.0.7.dev1/docs_src/tutorial/soonify_return/tutorial001.py`

 * *Files identical despite different names*

### Comparing `asyncer-0.0.7/docs_src/tutorial/soonify_return/tutorial002.py` & `asyncer-0.0.7.dev1/docs_src/tutorial/soonify_return/tutorial002.py`

 * *Files identical despite different names*

### Comparing `asyncer-0.0.7/docs_src/tutorial/soonify_return/tutorial003.py` & `asyncer-0.0.7.dev1/docs_src/tutorial/soonify_return/tutorial003.py`

 * *Files identical despite different names*

### Comparing `asyncer-0.0.7/pdm_build.py` & `asyncer-0.0.7.dev1/pdm_build.py`

 * *Files identical despite different names*

### Comparing `asyncer-0.0.7/pyproject.toml` & `asyncer-0.0.7.dev1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "Topic :: Internet",
     "Typing :: Typed",
 ]
 dependencies = [
     "anyio >=3.4.0,<5.0",
     "typing_extensions >=4.8.0; python_version < '3.10'",
 ]
-version = "0.0.7"
+version = "0.0.7.dev1"
 
 [project.urls]
 Homepage = "https://github.com/tiangolo/asyncer"
 Documentation = "https://asyncer.tiangolo.com"
 Repository = "https://github.com/tiangolo/asyncer"
 
 [project.optional-dependencies]
```

### Comparing `asyncer-0.0.7/tests/test_syncify_no_raise.py` & `asyncer-0.0.7.dev1/tests/test_syncify_no_raise.py`

 * *Files identical despite different names*

### Comparing `asyncer-0.0.7/tests/test_tutorial/test_soonify_return/test_tutorial002.py` & `asyncer-0.0.7.dev1/tests/test_tutorial/test_soonify_return/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `asyncer-0.0.7/PKG-INFO` & `asyncer-0.0.7.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncer
-Version: 0.0.7
+Version: 0.0.7.dev1
 Summary: Asyncer, async and await, focused on developer experience.
 Author-Email: =?utf-8?q?Sebasti=C3=A1n_Ram=C3=ADrez?= <tiangolo@gmail.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: Trio
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

