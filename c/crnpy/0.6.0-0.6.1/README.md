# Comparing `tmp/crnpy-0.6.0.tar.gz` & `tmp/crnpy-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crnpy-0.6.0.tar", last modified: Wed Apr 24 02:02:23 2024, max compression
+gzip compressed data, was "crnpy-0.6.1.tar", last modified: Tue Apr 30 04:24:53 2024, max compression
```

## Comparing `crnpy-0.6.0.tar` & `crnpy-0.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:02:23.204850 crnpy-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-24 02:02:13.000000 crnpy-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-04-24 02:02:23.204850 crnpy-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-24 02:02:13.000000 crnpy-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:02:23.204850 crnpy-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-24 02:02:13.000000 crnpy-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:02:23.200850 crnpy-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:02:23.200850 crnpy-0.6.0/src/crnpy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-24 02:02:13.000000 crnpy-0.6.0/src/crnpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68437 2024-04-24 02:02:13.000000 crnpy-0.6.0/src/crnpy/crnpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-04-24 02:02:13.000000 crnpy-0.6.0/src/crnpy/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:02:23.204850 crnpy-0.6.0/src/crnpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-04-24 02:02:23.000000 crnpy-0.6.0/src/crnpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-24 02:02:23.000000 crnpy-0.6.0/src/crnpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:02:23.000000 crnpy-0.6.0/src/crnpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 02:02:23.000000 crnpy-0.6.0/src/crnpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 02:02:23.000000 crnpy-0.6.0/src/crnpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:24:53.256915 crnpy-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-30 04:24:49.000000 crnpy-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-30 04:24:53.256915 crnpy-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-30 04:24:49.000000 crnpy-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 04:24:53.256915 crnpy-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-30 04:24:49.000000 crnpy-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:24:53.252915 crnpy-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:24:53.256915 crnpy-0.6.1/src/crnpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-30 04:24:49.000000 crnpy-0.6.1/src/crnpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68437 2024-04-30 04:24:49.000000 crnpy-0.6.1/src/crnpy/crnpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-04-30 04:24:49.000000 crnpy-0.6.1/src/crnpy/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 04:24:53.256915 crnpy-0.6.1/src/crnpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-30 04:24:53.000000 crnpy-0.6.1/src/crnpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-30 04:24:53.000000 crnpy-0.6.1/src/crnpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 04:24:53.000000 crnpy-0.6.1/src/crnpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 04:24:53.000000 crnpy-0.6.1/src/crnpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-30 04:24:53.000000 crnpy-0.6.1/src/crnpy.egg-info/top_level.txt
```

### Comparing `crnpy-0.6.0/LICENSE` & `crnpy-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crnpy-0.6.0/PKG-INFO` & `crnpy-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crnpy
-Version: 0.6.0
+Version: 0.6.1
 Summary: A Python package for the estimation and processing of soil moisture data from cosmic-ray neutron counts.
 Home-page: https://soilwater.github.io/crnpy/
 Author: Joaquin Peraza, Andres Patrignani
 Author-email: jperaza@ksu.edu, andrespatrignani@ksu.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -14,15 +14,15 @@
 Requires-Dist: requests
 Requires-Dist: utm
 
 [![GitHub Workflow Status (building)](https://img.shields.io/github/actions/workflow/status/soilwater/crnpy/python-package.yml)](https://github.com/soilwater/crnpy/actions/workflows/python-package.yml)
 [![GitHub Workflow Status (publish)](https://img.shields.io/github/actions/workflow/status/soilwater/crnpy/python-publish.yml?label=publish)](https://github.com/soilwater/crnpy/actions/workflows/python-publish.yml)
 [![PyPI - Status](https://img.shields.io/pypi/v/crnpy)](https://pypi.org/project/crnpy/)
 [![GitHub commits since latest release (by SemVer including pre-releases)](https://img.shields.io/github/commits-since/soilwater/crnpy/latest/main)](https://github.com/soilwater/crnpy)
-![JOSS submission status](https://joss.theoj.org/papers/e65c1bb5fee58c39289efc4547d1fd10/status.svg)
+[![JOSS submission status](https://joss.theoj.org/papers/e65c1bb5fee58c39289efc4547d1fd10/status.svg)](https://joss.theoj.org/papers/e65c1bb5fee58c39289efc4547d1fd10)
 
 # Cosmic-Ray Neutron Python (CRNPy) Library
 
 <img src="https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/logo/crnpy-logo.png" alt="CRNPY logo" width="250"/>
 
 ## Overview
 Welcome to the homepage of the CRNPy (Cosmic-Ray Neutron Python) library, an open-source Python library designed for the processing and conversion of raw neutron counts from cosmic-ray neutron probes (CRNP) into soil moisture data.
```

### Comparing `crnpy-0.6.0/README.md` & `crnpy-0.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![GitHub Workflow Status (building)](https://img.shields.io/github/actions/workflow/status/soilwater/crnpy/python-package.yml)](https://github.com/soilwater/crnpy/actions/workflows/python-package.yml)
 [![GitHub Workflow Status (publish)](https://img.shields.io/github/actions/workflow/status/soilwater/crnpy/python-publish.yml?label=publish)](https://github.com/soilwater/crnpy/actions/workflows/python-publish.yml)
 [![PyPI - Status](https://img.shields.io/pypi/v/crnpy)](https://pypi.org/project/crnpy/)
 [![GitHub commits since latest release (by SemVer including pre-releases)](https://img.shields.io/github/commits-since/soilwater/crnpy/latest/main)](https://github.com/soilwater/crnpy)
-![JOSS submission status](https://joss.theoj.org/papers/e65c1bb5fee58c39289efc4547d1fd10/status.svg)
+[![JOSS submission status](https://joss.theoj.org/papers/e65c1bb5fee58c39289efc4547d1fd10/status.svg)](https://joss.theoj.org/papers/e65c1bb5fee58c39289efc4547d1fd10)
 
 # Cosmic-Ray Neutron Python (CRNPy) Library
 
 <img src="https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/logo/crnpy-logo.png" alt="CRNPY logo" width="250"/>
 
 ## Overview
 Welcome to the homepage of the CRNPy (Cosmic-Ray Neutron Python) library, an open-source Python library designed for the processing and conversion of raw neutron counts from cosmic-ray neutron probes (CRNP) into soil moisture data.
```

### Comparing `crnpy-0.6.0/setup.py` & `crnpy-0.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # contents of setup.py
 import setuptools
 
 setuptools.setup(
     name="crnpy",
-    version="0.6.0",
+    version="0.6.1",
     packages=['crnpy'],
     package_dir = {"": "src"},
     description="A Python package for the estimation and processing of soil moisture data from cosmic-ray neutron counts.",
     include_package_data=True,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://soilwater.github.io/crnpy/",
@@ -18,8 +18,8 @@
     install_requires=[
         "numpy",
         "pandas",
         "scipy",
         "requests",
         "utm"
     ],
-)
+)
```

### Comparing `crnpy-0.6.0/src/crnpy/__init__.py` & `crnpy-0.6.1/src/crnpy/__init__.py`

 * *Files identical despite different names*

### Comparing `crnpy-0.6.0/src/crnpy/crnpy.py` & `crnpy-0.6.1/src/crnpy/crnpy.py`

 * *Files identical despite different names*

### Comparing `crnpy-0.6.0/src/crnpy/data.py` & `crnpy-0.6.1/src/crnpy/data.py`

 * *Files identical despite different names*

### Comparing `crnpy-0.6.0/src/crnpy.egg-info/PKG-INFO` & `crnpy-0.6.1/src/crnpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crnpy
-Version: 0.6.0
+Version: 0.6.1
 Summary: A Python package for the estimation and processing of soil moisture data from cosmic-ray neutron counts.
 Home-page: https://soilwater.github.io/crnpy/
 Author: Joaquin Peraza, Andres Patrignani
 Author-email: jperaza@ksu.edu, andrespatrignani@ksu.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -14,15 +14,15 @@
 Requires-Dist: requests
 Requires-Dist: utm
 
 [![GitHub Workflow Status (building)](https://img.shields.io/github/actions/workflow/status/soilwater/crnpy/python-package.yml)](https://github.com/soilwater/crnpy/actions/workflows/python-package.yml)
 [![GitHub Workflow Status (publish)](https://img.shields.io/github/actions/workflow/status/soilwater/crnpy/python-publish.yml?label=publish)](https://github.com/soilwater/crnpy/actions/workflows/python-publish.yml)
 [![PyPI - Status](https://img.shields.io/pypi/v/crnpy)](https://pypi.org/project/crnpy/)
 [![GitHub commits since latest release (by SemVer including pre-releases)](https://img.shields.io/github/commits-since/soilwater/crnpy/latest/main)](https://github.com/soilwater/crnpy)
-![JOSS submission status](https://joss.theoj.org/papers/e65c1bb5fee58c39289efc4547d1fd10/status.svg)
+[![JOSS submission status](https://joss.theoj.org/papers/e65c1bb5fee58c39289efc4547d1fd10/status.svg)](https://joss.theoj.org/papers/e65c1bb5fee58c39289efc4547d1fd10)
 
 # Cosmic-Ray Neutron Python (CRNPy) Library
 
 <img src="https://raw.githubusercontent.com/soilwater/crnpy/main/docs/img/logo/crnpy-logo.png" alt="CRNPY logo" width="250"/>
 
 ## Overview
 Welcome to the homepage of the CRNPy (Cosmic-Ray Neutron Python) library, an open-source Python library designed for the processing and conversion of raw neutron counts from cosmic-ray neutron probes (CRNP) into soil moisture data.
```

