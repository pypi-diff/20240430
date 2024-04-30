# Comparing `tmp/kedro-expectations-0.4.2.tar.gz` & `tmp/kedro_expectations-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-expectations-0.4.2.tar", last modified: Fri Mar  8 09:45:45 2024, max compression
+gzip compressed data, was "kedro_expectations-0.4.3.tar", last modified: Tue Apr 30 09:39:41 2024, max compression
```

## Comparing `kedro-expectations-0.4.2.tar` & `kedro_expectations-0.4.3.tar`

### file list

```diff
@@ -1,30 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:45:45.803585 kedro-expectations-0.4.2/
--rwxrwxrwx   0 root         (0) root         (0)     1070 2024-03-08 09:45:30.000000 kedro-expectations-0.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7578 2024-03-08 09:45:45.802585 kedro-expectations-0.4.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     6955 2024-03-08 09:45:30.000000 kedro-expectations-0.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:45:45.797585 kedro-expectations-0.4.2/kedro_expectations/
--rwxrwxrwx   0 root         (0) root         (0)      135 2024-03-08 09:45:30.000000 kedro-expectations-0.4.2/kedro_expectations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:45:45.800585 kedro-expectations-0.4.2/kedro_expectations/cli/
--rwxrwxrwx   0 root         (0) root         (0)       26 2024-03-08 09:45:30.000000 kedro-expectations-0.4.2/kedro_expectations/cli/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      407 2024-03-08 09:45:30.000000 kedro-expectations-0.4.2/kedro_expectations/cli/cli.py
--rwxrwxrwx   0 root         (0) root         (0)     6303 2024-03-08 09:45:30.000000 kedro-expectations-0.4.2/kedro_expectations/cli/create_suite.py
--rwxrwxrwx   0 root         (0) root         (0)     1538 2024-03-08 09:45:30.000000 kedro-expectations-0.4.2/kedro_expectations/cli/init_ge.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2024-03-08 09:45:30.000000 kedro-expectations-0.4.2/kedro_expectations/constants.py
--rwxrwxrwx   0 root         (0) root         (0)      165 2024-03-08 09:45:30.000000 kedro-expectations-0.4.2/kedro_expectations/exceptions.py
--rwxrwxrwx   0 root         (0) root         (0)    11533 2024-03-08 09:45:30.000000 kedro-expectations-0.4.2/kedro_expectations/kedro_expectations.py
--rw-rw-rw-   0 root         (0) root         (0)     3982 2024-03-08 09:45:30.000000 kedro-expectations-0.4.2/kedro_expectations/notification.py
--rwxrwxrwx   0 root         (0) root         (0)     6668 2024-03-08 09:45:30.000000 kedro-expectations-0.4.2/kedro_expectations/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:45:45.802585 kedro-expectations-0.4.2/kedro_expectations.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7578 2024-03-08 09:45:45.000000 kedro-expectations-0.4.2/kedro_expectations.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      720 2024-03-08 09:45:45.000000 kedro-expectations-0.4.2/kedro_expectations.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 09:45:45.000000 kedro-expectations-0.4.2/kedro_expectations.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-08 09:45:45.000000 kedro-expectations-0.4.2/kedro_expectations.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 09:45:45.000000 kedro-expectations-0.4.2/kedro_expectations.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       66 2024-03-08 09:45:45.000000 kedro-expectations-0.4.2/kedro_expectations.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-08 09:45:45.000000 kedro-expectations-0.4.2/kedro_expectations.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-08 09:45:45.803585 kedro-expectations-0.4.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1017 2024-03-08 09:45:30.000000 kedro-expectations-0.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:45:45.801585 kedro-expectations-0.4.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 09:45:30.000000 kedro-expectations-0.4.2/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2540 2024-03-08 09:45:30.000000 kedro-expectations-0.4.2/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2482 2024-03-08 09:45:30.000000 kedro-expectations-0.4.2/tests/test_validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:39:41.554942 kedro_expectations-0.4.3/
+-rwxrwxrwx   0 root         (0) root         (0)     1070 2024-04-30 09:39:28.000000 kedro_expectations-0.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7679 2024-04-30 09:39:41.554942 kedro_expectations-0.4.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     6955 2024-04-30 09:39:28.000000 kedro_expectations-0.4.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:39:41.551945 kedro_expectations-0.4.3/kedro_expectations/
+-rwxrwxrwx   0 root         (0) root         (0)      135 2024-04-30 09:39:28.000000 kedro_expectations-0.4.3/kedro_expectations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-04-30 09:39:28.000000 kedro_expectations-0.4.3/kedro_expectations/constants.py
+-rwxrwxrwx   0 root         (0) root         (0)      165 2024-04-30 09:39:28.000000 kedro_expectations-0.4.3/kedro_expectations/exceptions.py
+-rwxrwxrwx   0 root         (0) root         (0)    11533 2024-04-30 09:39:28.000000 kedro_expectations-0.4.3/kedro_expectations/kedro_expectations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3982 2024-04-30 09:39:28.000000 kedro_expectations-0.4.3/kedro_expectations/notification.py
+-rwxrwxrwx   0 root         (0) root         (0)     6668 2024-04-30 09:39:28.000000 kedro_expectations-0.4.3/kedro_expectations/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:39:41.553943 kedro_expectations-0.4.3/kedro_expectations.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7679 2024-04-30 09:39:41.000000 kedro_expectations-0.4.3/kedro_expectations.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      511 2024-04-30 09:39:41.000000 kedro_expectations-0.4.3/kedro_expectations.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 09:39:41.000000 kedro_expectations-0.4.3/kedro_expectations.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-30 09:39:41.000000 kedro_expectations-0.4.3/kedro_expectations.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2024-04-30 09:39:41.000000 kedro_expectations-0.4.3/kedro_expectations.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-30 09:39:41.000000 kedro_expectations-0.4.3/kedro_expectations.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      902 2024-04-30 09:39:28.000000 kedro_expectations-0.4.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 09:39:41.554942 kedro_expectations-0.4.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:39:41.553943 kedro_expectations-0.4.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2482 2024-04-30 09:39:28.000000 kedro_expectations-0.4.3/tests/test_validation.py
```

### Comparing `kedro-expectations-0.4.2/LICENSE` & `kedro_expectations-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro-expectations-0.4.2/PKG-INFO` & `kedro_expectations-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: kedro-expectations
-Version: 0.4.2
+Version: 0.4.3
 Summary: Combine Kedro data science pipelines with Great Expectations data validations.
-Home-page: https://gitlab.com/anacision/kedro-expectations.git
-Author: anacision GmbH
-Author-email: tech@anacision.de
+Author-email: anacision GmbH <tech@anacision.de>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: kedro~=0.19
-Requires-Dist: kedro-datasets~=2.0
 Requires-Dist: great_expectations>=0.18.1
+Requires-Dist: kedro-datasets~=2.0
+Requires-Dist: kedro~=0.19
 Requires-Dist: pandas
+Provides-Extra: dev
+Requires-Dist: black>=23.0; extra == "dev"
+Requires-Dist: twine~=4.0; extra == "dev"
+Provides-Extra: test
+Requires-Dist: pytest~=7.4; extra == "test"
 
 # kedro-expectations
 A tool to better integrate Kedro and Great Expectations
 
 ## Introduction
 
 Kedro Expectations is a tool designed to make the use of Great Expectations (GX, a data validation tool) within Kedro data science pipelines easier. It is composed of a couple of commands and a hook, allowing the user to create expectation suites and run validations on the Kedro DataCatalog on-the-fly.
```

### Comparing `kedro-expectations-0.4.2/README.md` & `kedro_expectations-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `kedro-expectations-0.4.2/kedro_expectations/kedro_expectations.py` & `kedro_expectations-0.4.3/kedro_expectations/kedro_expectations.py`

 * *Files identical despite different names*

### Comparing `kedro-expectations-0.4.2/kedro_expectations/notification.py` & `kedro_expectations-0.4.3/kedro_expectations/notification.py`

 * *Files identical despite different names*

### Comparing `kedro-expectations-0.4.2/kedro_expectations/utils.py` & `kedro_expectations-0.4.3/kedro_expectations/utils.py`

 * *Files identical despite different names*

### Comparing `kedro-expectations-0.4.2/kedro_expectations.egg-info/PKG-INFO` & `kedro_expectations-0.4.3/kedro_expectations.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: kedro-expectations
-Version: 0.4.2
+Version: 0.4.3
 Summary: Combine Kedro data science pipelines with Great Expectations data validations.
-Home-page: https://gitlab.com/anacision/kedro-expectations.git
-Author: anacision GmbH
-Author-email: tech@anacision.de
+Author-email: anacision GmbH <tech@anacision.de>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: kedro~=0.19
-Requires-Dist: kedro-datasets~=2.0
 Requires-Dist: great_expectations>=0.18.1
+Requires-Dist: kedro-datasets~=2.0
+Requires-Dist: kedro~=0.19
 Requires-Dist: pandas
+Provides-Extra: dev
+Requires-Dist: black>=23.0; extra == "dev"
+Requires-Dist: twine~=4.0; extra == "dev"
+Provides-Extra: test
+Requires-Dist: pytest~=7.4; extra == "test"
 
 # kedro-expectations
 A tool to better integrate Kedro and Great Expectations
 
 ## Introduction
 
 Kedro Expectations is a tool designed to make the use of Great Expectations (GX, a data validation tool) within Kedro data science pipelines easier. It is composed of a couple of commands and a hook, allowing the user to create expectation suites and run validations on the Kedro DataCatalog on-the-fly.
```

### Comparing `kedro-expectations-0.4.2/tests/test_validation.py` & `kedro_expectations-0.4.3/tests/test_validation.py`

 * *Files identical despite different names*

