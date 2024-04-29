# Comparing `tmp/dkist_service_configuration-2.0.0rc1.tar.gz` & `tmp/dkist_service_configuration-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_service_configuration-2.0.0rc1.tar", last modified: Mon Apr 29 20:25:42 2024, max compression
+gzip compressed data, was "dkist_service_configuration-2.0.0rc2.tar", last modified: Mon Apr 29 22:52:25 2024, max compression
```

## Comparing `dkist_service_configuration-2.0.0rc1.tar` & `dkist_service_configuration-2.0.0rc2.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 20:25:42.055435 dkist_service_configuration-2.0.0rc1/
--rw-rw-rw-   0 root         (0) root         (0)     1757 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1063 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1934 2024-04-29 20:25:42.055435 dkist_service_configuration-2.0.0rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1282 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1394 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 20:25:42.055435 dkist_service_configuration-2.0.0rc1/dkist_service_configuration/
--rw-rw-rw-   0 root         (0) root         (0)      145 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1688 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     1987 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration/settings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 20:25:42.055435 dkist_service_configuration-2.0.0rc1/dkist_service_configuration/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      279 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration/tests/test_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     1701 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration/tests/test_settings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 20:25:42.055435 dkist_service_configuration-2.0.0rc1/dkist_service_configuration.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1934 2024-04-29 20:25:42.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      631 2024-04-29 20:25:42.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-29 20:25:42.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-29 20:25:42.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-04-29 20:25:42.000000 dkist_service_configuration-2.0.0rc1/dkist_service_configuration.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1026 2024-04-29 20:25:42.055435 dkist_service_configuration-2.0.0rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       83 2024-04-29 20:25:26.000000 dkist_service_configuration-2.0.0rc1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 22:52:25.618972 dkist_service_configuration-2.0.0rc2/
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      482 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2127 2024-04-29 22:52:25.618972 dkist_service_configuration-2.0.0rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 22:52:25.618972 dkist_service_configuration-2.0.0rc2/dkist_service_configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      145 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-04-29 22:52:25.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1688 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration/settings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 22:52:25.618972 dkist_service_configuration-2.0.0rc2/dkist_service_configuration/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration/tests/test_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     1701 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration/tests/test_settings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 22:52:25.618972 dkist_service_configuration-2.0.0rc2/dkist_service_configuration.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2127 2024-04-29 22:52:25.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      763 2024-04-29 22:52:25.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-29 22:52:25.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-29 22:52:25.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-04-29 22:52:25.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-29 22:52:25.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 22:52:25.618972 dkist_service_configuration-2.0.0rc2/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/licenses/license.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2184 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-29 22:52:25.618972 dkist_service_configuration-2.0.0rc2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/tox.ini
```

### Comparing `dkist_service_configuration-2.0.0rc1/.gitignore` & `dkist_service_configuration-2.0.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.0rc1/.pre-commit-config.yaml` & `dkist_service_configuration-2.0.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.0rc1/LICENSE` & `dkist_service_configuration-2.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.0rc1/PKG-INFO` & `dkist_service_configuration-2.0.0rc2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: dkist-service-configuration
-Version: 2.0.0rc1
-Summary: Configuration support for DKIST services
-Home-page: https://bitbucket.org/dkistdc/dkist_service_configuration/src/master/
-Author: NSO / AURA
-Author-email: "dkistdc@nso.edu"
-License: MIT
-Classifier: Programming Language :: Python
+Version: 2.0.0rc2
+Summary: Library for retrieving configurations for DKIST services
+Author-email: NSO / AURA <dkistdc@nso.edu>
+License: BSD 3-Clause
+Project-URL: repository, https://bitbucket.org/dkistdc/dkist_service_configuration
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.11
+Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: loguru
-Requires-Dist: pydantic-settings
+Requires-Dist: loguru>0.7.0
+Requires-Dist: pydantic-settings>2.0
 Requires-Dist: pydantic[dotenv]>2.0
 Provides-Extra: test
+Requires-Dist: tox>=4; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: Pygments; extra == "test"
+Requires-Dist: PyPDF4; extra == "test"
 
 dkist-service-configuration
 ===========================
 
 A configuration for the `loguru <https://github.com/Delgan/loguru>`_ logger and base configuration object using `pydantic <https://docs.pydantic.dev/1.10/usage/settings/>`_ base settings.
 
 It is important that it be the first import to run so the standard logging basicConfig method has an effect.
```

### Comparing `dkist_service_configuration-2.0.0rc1/README.rst` & `dkist_service_configuration-2.0.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.0rc1/dkist_service_configuration/logging.py` & `dkist_service_configuration-2.0.0rc2/dkist_service_configuration/logging.py`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.0rc1/dkist_service_configuration/settings.py` & `dkist_service_configuration-2.0.0rc2/dkist_service_configuration/settings.py`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.0rc1/dkist_service_configuration/tests/test_settings.py` & `dkist_service_configuration-2.0.0rc2/dkist_service_configuration/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.0rc1/dkist_service_configuration.egg-info/PKG-INFO` & `dkist_service_configuration-2.0.0rc2/dkist_service_configuration.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: dkist-service-configuration
-Version: 2.0.0rc1
-Summary: Configuration support for DKIST services
-Home-page: https://bitbucket.org/dkistdc/dkist_service_configuration/src/master/
-Author: NSO / AURA
-Author-email: "dkistdc@nso.edu"
-License: MIT
-Classifier: Programming Language :: Python
+Version: 2.0.0rc2
+Summary: Library for retrieving configurations for DKIST services
+Author-email: NSO / AURA <dkistdc@nso.edu>
+License: BSD 3-Clause
+Project-URL: repository, https://bitbucket.org/dkistdc/dkist_service_configuration
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.11
+Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: loguru
-Requires-Dist: pydantic-settings
+Requires-Dist: loguru>0.7.0
+Requires-Dist: pydantic-settings>2.0
 Requires-Dist: pydantic[dotenv]>2.0
 Provides-Extra: test
+Requires-Dist: tox>=4; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: Pygments; extra == "test"
+Requires-Dist: PyPDF4; extra == "test"
 
 dkist-service-configuration
 ===========================
 
 A configuration for the `loguru <https://github.com/Delgan/loguru>`_ logger and base configuration object using `pydantic <https://docs.pydantic.dev/1.10/usage/settings/>`_ base settings.
 
 It is important that it be the first import to run so the standard logging basicConfig method has an effect.
```

### Comparing `dkist_service_configuration-2.0.0rc1/dkist_service_configuration.egg-info/SOURCES.txt` & `dkist_service_configuration-2.0.0rc2/dkist_service_configuration.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
+MANIFEST.in
 README.rst
 bitbucket-pipelines.yml
 pyproject.toml
-setup.cfg
-setup.py
+tox.ini
 dkist_service_configuration/__init__.py
+dkist_service_configuration/_version.py
 dkist_service_configuration/logging.py
 dkist_service_configuration/settings.py
 dkist_service_configuration.egg-info/PKG-INFO
 dkist_service_configuration.egg-info/SOURCES.txt
 dkist_service_configuration.egg-info/dependency_links.txt
+dkist_service_configuration.egg-info/not-zip-safe
 dkist_service_configuration.egg-info/requires.txt
 dkist_service_configuration.egg-info/top_level.txt
 dkist_service_configuration/tests/__init__.py
 dkist_service_configuration/tests/test_logging.py
-dkist_service_configuration/tests/test_settings.py
+dkist_service_configuration/tests/test_settings.py
+licenses/README.rst
+licenses/license.rst
```

