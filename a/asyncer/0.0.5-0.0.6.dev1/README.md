# Comparing `tmp/asyncer-0.0.5.tar.gz` & `tmp/asyncer-0.0.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncer-0.0.5.tar", max compression
+gzip compressed data, was "asyncer-0.0.6.dev1.tar", last modified: Mon Apr 29 21:03:07 2024, max compression
```

## Comparing `asyncer-0.0.5.tar` & `asyncer-0.0.6.dev1.tar`

### file list

```diff
@@ -1,7 +1,59 @@
--rw-r--r--   0        0        0     1086 2024-02-22 15:43:51.325307 asyncer-0.0.5/LICENSE
--rw-r--r--   0        0        0     5297 2024-02-22 15:43:51.325307 asyncer-0.0.5/README.md
--rw-r--r--   0        0        0      347 2024-02-22 15:43:51.325307 asyncer-0.0.5/asyncer/__init__.py
--rw-r--r--   0        0        0    13107 2024-02-22 15:43:51.325307 asyncer-0.0.5/asyncer/_main.py
--rw-r--r--   0        0        0        0 2024-02-22 15:43:51.325307 asyncer-0.0.5/asyncer/py.typed
--rw-r--r--   0        0        0     2568 2024-02-22 15:43:51.329307 asyncer-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     6657 1970-01-01 00:00:00.000000 asyncer-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-04-29 21:03:04.421403 asyncer-0.0.6.dev1/LICENSE
+-rw-r--r--   0        0        0     5297 2024-04-29 21:03:04.421403 asyncer-0.0.6.dev1/README.md
+-rw-r--r--   0        0        0      352 2024-04-29 21:03:04.421403 asyncer-0.0.6.dev1/asyncer/__init__.py
+-rw-r--r--   0        0        0    13107 2024-04-29 21:03:04.421403 asyncer-0.0.6.dev1/asyncer/_main.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:03:04.421403 asyncer-0.0.6.dev1/asyncer/py.typed
+-rw-r--r--   0        0        0        0 2024-04-29 21:03:04.425403 asyncer-0.0.6.dev1/docs_src/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:03:04.425403 asyncer-0.0.6.dev1/docs_src/tutorial/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:03:04.425403 asyncer-0.0.6.dev1/docs_src/tutorial/asyncify/__init__.py
+-rw-r--r--   0        0        0      201 2024-04-29 21:03:04.425403 asyncer-0.0.6.dev1/docs_src/tutorial/asyncify/tutorial001.py
+-rw-r--r--   0        0        0      246 2024-04-29 21:03:04.425403 asyncer-0.0.6.dev1/docs_src/tutorial/asyncify/tutorial002.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:03:04.425403 asyncer-0.0.6.dev1/docs_src/tutorial/first_steps/__init__.py
+-rw-r--r--   0        0        0      220 2024-04-29 21:03:04.425403 asyncer-0.0.6.dev1/docs_src/tutorial/first_steps/tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:03:04.425403 asyncer-0.0.6.dev1/docs_src/tutorial/runnify/__init__.py
+-rw-r--r--   0        0        0      259 2024-04-29 21:03:04.425403 asyncer-0.0.6.dev1/docs_src/tutorial/runnify/tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:03:04.425403 asyncer-0.0.6.dev1/docs_src/tutorial/soonify/__init__.py
+-rw-r--r--   0        0        0      279 2024-04-29 21:03:04.425403 asyncer-0.0.6.dev1/docs_src/tutorial/soonify/tutorial001.py
+-rw-r--r--   0        0        0      406 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/docs_src/tutorial/soonify/tutorial002.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/docs_src/tutorial/soonify_return/__init__.py
+-rw-r--r--   0        0        0      611 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/docs_src/tutorial/soonify_return/tutorial001.py
+-rw-r--r--   0        0        0      644 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/docs_src/tutorial/soonify_return/tutorial002.py
+-rw-r--r--   0        0        0      728 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/docs_src/tutorial/soonify_return/tutorial003.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/docs_src/tutorial/syncify/__init__.py
+-rw-r--r--   0        0        0      385 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/docs_src/tutorial/syncify/tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/docs_src/tutorial/syncify_no_raise/__init__.py
+-rw-r--r--   0        0        0      505 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/docs_src/tutorial/syncify_no_raise/tutorial001.py
+-rw-r--r--   0        0        0     2248 2024-04-29 21:03:07.201386 asyncer-0.0.6.dev1/pyproject.toml
+-rw-r--r--   0        0        0      438 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/requirements-docs.txt
+-rw-r--r--   0        0        0       80 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/requirements-tests.txt
+-rw-r--r--   0        0        0       85 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/requirements.txt
+-rwxr-xr-x   0        0        0      131 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/scripts/docs-live.sh
+-rwxr-xr-x   0        0        0       90 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/scripts/format.sh
+-rwxr-xr-x   0        0        0      120 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/scripts/lint.sh
+-rwxr-xr-x   0        0        0       62 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/scripts/publish.sh
+-rwxr-xr-x   0        0        0      105 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/scripts/test-files.sh
+-rwxr-xr-x   0        0        0      127 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/scripts/test.sh
+-rw-r--r--   0        0        0        0 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/__init__.py
+-rw-r--r--   0        0        0      309 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/conftest.py
+-rw-r--r--   0        0        0      100 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_others.py
+-rw-r--r--   0        0        0     2690 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_syncify_no_raise.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_tutorial/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_tutorial/test_asyncify/__init__.py
+-rw-r--r--   0        0        0      348 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_tutorial/test_asyncify/test_tutorial001.py
+-rw-r--r--   0        0        0      348 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_tutorial/test_asyncify/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_tutorial/test_first_steps/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_tutorial/test_first_steps/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_tutorial/test_runnify/__init__.py
+-rw-r--r--   0        0        0      351 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_tutorial/test_runnify/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_tutorial/test_soonify/__init__.py
+-rw-r--r--   0        0        0      385 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_tutorial/test_soonify/test_tutorial001.py
+-rw-r--r--   0        0        0      385 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_tutorial/test_soonify/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_tutorial/test_soonify_return/__init__.py
+-rw-r--r--   0        0        0      392 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_tutorial/test_soonify_return/test_tutorial001.py
+-rw-r--r--   0        0        0      833 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_tutorial/test_soonify_return/test_tutorial002.py
+-rw-r--r--   0        0        0      464 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_tutorial/test_soonify_return/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_tutorial/test_syncify/__init__.py
+-rw-r--r--   0        0        0      347 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_tutorial/test_syncify/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_tutorial/test_syncify_no_raise/__init__.py
+-rw-r--r--   0        0        0      379 2024-04-29 21:03:04.429403 asyncer-0.0.6.dev1/tests/test_tutorial/test_syncify_no_raise/test_tutorial001.py
+-rw-r--r--   0        0        0     6607 1970-01-01 00:00:00.000000 asyncer-0.0.6.dev1/PKG-INFO
```

### Comparing `asyncer-0.0.5/LICENSE` & `asyncer-0.0.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncer-0.0.5/README.md` & `asyncer-0.0.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `asyncer-0.0.5/asyncer/_main.py` & `asyncer-0.0.6.dev1/asyncer/_main.py`

 * *Files identical despite different names*

### Comparing `asyncer-0.0.5/PKG-INFO` & `asyncer-0.0.6.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 Metadata-Version: 2.1
 Name: asyncer
-Version: 0.0.5
+Version: 0.0.6.dev1
 Summary: Asyncer, async and await, focused on developer experience.
-Home-page: https://github.com/tiangolo/asyncer
-License: MIT
-Author: Sebastián Ramírez
-Author-email: tiangolo@gmail.com
-Requires-Python: >=3.8,<4.0
+Author-Email: =?utf-8?q?Sebasti=C3=A1n_Ram=C3=ADrez?= <tiangolo@gmail.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: Trio
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet
 Classifier: Typing :: Typed
-Requires-Dist: anyio (>=3.4.0,<5.0)
-Requires-Dist: typing_extensions (>=4.8.0,<5.0.0) ; python_version < "3.10"
+Project-URL: Homepage, https://github.com/tiangolo/asyncer
 Project-URL: Documentation, https://asyncer.tiangolo.com
 Project-URL: Repository, https://github.com/tiangolo/asyncer
+Requires-Python: >=3.8
+Requires-Dist: anyio<5.0,>=3.4.0
+Requires-Dist: typing_extensions>=4.8.0; python_version < "3.10"
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://asyncer.tiangolo.com"><img src="https://asyncer.tiangolo.com/img/logo-margin/logo-margin-vector.svg" alt="Asyncer"></a>
 </p>
 <p align="center">
     <em>Asyncer, async and await, focused on developer experience.</em>
@@ -152,8 +149,7 @@
 <img class="shadow" src="https://asyncer.tiangolo.com/img/tutorial/soonify/image02.png">
 
 * Support for tools like **mypy**, that can help you verify that your **code is correct**, and prevent many bugs.
 
 ## License
 
 This project is licensed under the terms of the [MIT license](https://github.com/tiangolo/asyncer/blob/main/LICENSE).
-
```

