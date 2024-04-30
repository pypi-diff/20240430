# Comparing `tmp/appthreat_chen-2.0.8.tar.gz` & `tmp/appthreat_chen-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appthreat_chen-2.0.8.tar", max compression
+gzip compressed data, was "appthreat_chen-2.0.9.tar", max compression
```

## Comparing `appthreat_chen-2.0.8.tar` & `appthreat_chen-2.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    12015 2024-02-15 16:26:28.515828 appthreat_chen-2.0.8/LICENSE
--rw-r--r--   0        0        0     9479 2024-02-15 16:26:28.515828 appthreat_chen-2.0.8/README.md
--rw-r--r--   0        0        0       85 2024-02-15 16:26:28.515828 appthreat_chen-2.0.8/chenpy/__init__.py
--rw-r--r--   0        0        0     9509 2024-02-15 16:26:28.515828 appthreat_chen-2.0.8/chenpy/cli.py
--rw-r--r--   0        0        0    15364 2024-02-15 16:26:28.515828 appthreat_chen-2.0.8/chenpy/client.py
--rw-r--r--   0        0        0      256 2024-02-15 16:26:28.515828 appthreat_chen-2.0.8/chenpy/config.py
--rw-r--r--   0        0        0       61 2024-02-15 16:26:28.515828 appthreat_chen-2.0.8/chenpy/detectors/__init__.py
--rw-r--r--   0        0        0      999 2024-02-15 16:26:28.515828 appthreat_chen-2.0.8/chenpy/detectors/c.py
--rw-r--r--   0        0        0    15079 2024-02-15 16:26:28.515828 appthreat_chen-2.0.8/chenpy/detectors/common.py
--rw-r--r--   0        0        0     6052 2024-02-15 16:26:28.515828 appthreat_chen-2.0.8/chenpy/detectors/java.py
--rw-r--r--   0        0        0     5077 2024-02-15 16:26:28.515828 appthreat_chen-2.0.8/chenpy/detectors/js.py
--rw-r--r--   0        0        0     2311 2024-02-15 16:26:28.515828 appthreat_chen-2.0.8/chenpy/detectors/python.py
--rw-r--r--   0        0        0    13262 2024-02-15 16:26:28.515828 appthreat_chen-2.0.8/chenpy/graph.py
--rw-r--r--   0        0        0     2100 2024-02-15 16:26:28.515828 appthreat_chen-2.0.8/chenpy/logger.py
--rw-r--r--   0        0        0        0 2024-02-15 16:26:28.515828 appthreat_chen-2.0.8/chenpy/source/__init__.py
--rw-r--r--   0        0        0     4002 2024-02-15 16:26:28.515828 appthreat_chen-2.0.8/chenpy/source/ghsa.py
--rw-r--r--   0        0        0    30127 2024-02-15 16:26:28.515828 appthreat_chen-2.0.8/chenpy/utils.py
--rw-r--r--   0        0        0     6496 2024-02-15 16:26:28.515828 appthreat_chen-2.0.8/chenpy/workspace.py
--rw-r--r--   0        0        0     2612 2024-02-15 16:26:28.603828 appthreat_chen-2.0.8/pyproject.toml
--rw-r--r--   0        0        0    11057 1970-01-01 00:00:00.000000 appthreat_chen-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0    12015 2024-04-29 10:57:54.663668 appthreat_chen-2.0.9/LICENSE
+-rw-r--r--   0        0        0     9479 2024-04-29 10:57:54.663668 appthreat_chen-2.0.9/README.md
+-rw-r--r--   0        0        0       85 2024-04-29 10:57:54.663668 appthreat_chen-2.0.9/chenpy/__init__.py
+-rw-r--r--   0        0        0     9509 2024-04-29 10:57:54.663668 appthreat_chen-2.0.9/chenpy/cli.py
+-rw-r--r--   0        0        0    15364 2024-04-29 10:57:54.663668 appthreat_chen-2.0.9/chenpy/client.py
+-rw-r--r--   0        0        0      256 2024-04-29 10:57:54.663668 appthreat_chen-2.0.9/chenpy/config.py
+-rw-r--r--   0        0        0       61 2024-04-29 10:57:54.663668 appthreat_chen-2.0.9/chenpy/detectors/__init__.py
+-rw-r--r--   0        0        0      999 2024-04-29 10:57:54.663668 appthreat_chen-2.0.9/chenpy/detectors/c.py
+-rw-r--r--   0        0        0    15079 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/detectors/common.py
+-rw-r--r--   0        0        0     6052 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/detectors/java.py
+-rw-r--r--   0        0        0     5077 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/detectors/js.py
+-rw-r--r--   0        0        0     2311 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/detectors/python.py
+-rw-r--r--   0        0        0    13262 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/graph.py
+-rw-r--r--   0        0        0     2100 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/logger.py
+-rw-r--r--   0        0        0        0 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/source/__init__.py
+-rw-r--r--   0        0        0     4002 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/source/ghsa.py
+-rw-r--r--   0        0        0    30127 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/utils.py
+-rw-r--r--   0        0        0     6496 2024-04-29 10:57:54.667668 appthreat_chen-2.0.9/chenpy/workspace.py
+-rw-r--r--   0        0        0     2554 2024-04-29 10:57:54.755667 appthreat_chen-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0    11004 1970-01-01 00:00:00.000000 appthreat_chen-2.0.9/PKG-INFO
```

### Comparing `appthreat_chen-2.0.8/LICENSE` & `appthreat_chen-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.8/README.md` & `appthreat_chen-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.8/chenpy/cli.py` & `appthreat_chen-2.0.9/chenpy/cli.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.8/chenpy/client.py` & `appthreat_chen-2.0.9/chenpy/client.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.8/chenpy/detectors/c.py` & `appthreat_chen-2.0.9/chenpy/detectors/c.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.8/chenpy/detectors/common.py` & `appthreat_chen-2.0.9/chenpy/detectors/common.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.8/chenpy/detectors/java.py` & `appthreat_chen-2.0.9/chenpy/detectors/java.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.8/chenpy/detectors/js.py` & `appthreat_chen-2.0.9/chenpy/detectors/js.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.8/chenpy/detectors/python.py` & `appthreat_chen-2.0.9/chenpy/detectors/python.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.8/chenpy/graph.py` & `appthreat_chen-2.0.9/chenpy/graph.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.8/chenpy/logger.py` & `appthreat_chen-2.0.9/chenpy/logger.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.8/chenpy/source/ghsa.py` & `appthreat_chen-2.0.9/chenpy/source/ghsa.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.8/chenpy/utils.py` & `appthreat_chen-2.0.9/chenpy/utils.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.8/chenpy/workspace.py` & `appthreat_chen-2.0.9/chenpy/workspace.py`

 * *Files identical despite different names*

### Comparing `appthreat_chen-2.0.8/pyproject.toml` & `appthreat_chen-2.0.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,79 +1,78 @@
 [tool.poetry]
 name = "appthreat-chen"
-version = "2.0.8"
+version = "2.0.9"
 description = "Code Hierarchy Exploration Net (chen)"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "chenpy"}]
 homepage = "https://github.com/AppThreat/chen"
 repository = "https://github.com/AppThreat/chen"
 keywords = ["chen", "code-analysis", "static-analysis"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "Topic :: Utilities",
     "Topic :: Security",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
 ]
 exclude = ["ci", "console", "dataflowengineoss", "macros", "platform", "project", "scripts", "semanticcpg", "target", "tests", "workspace"]
 
 [tool.poetry.urls]
 "CI" = "https://github.com/AppThreat/chen/actions"
 
 [tool.poetry.scripts]
 chen = 'chenpy.cli:main'
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<3.12"
-httpx = "^0.24.1"
-websockets = "^11.0.2"
+python = ">=3.10,<3.13"
+httpx = "^0.27.0"
+websockets = "^12.0"
 uvloop = {version = "^0.17.0", markers = "sys_platform == 'linux' or sys_platform == 'darwin'", optional = true}
-orjson = "^3.9.0"
-rich = "^13.4.1"
+orjson = "^3.10.1"
+rich = "^13.7.1"
 oras = "0.1.26"
 appdirs = "^1.4.4"
-psutil = "^5.9.5"
+psutil = "^5.9.8"
 packageurl-python = "^0.11.2"
-gitpython = "^3.1.37"
+gitpython = "^3.1.43"
 
 
 [tool.poetry.extras]
 science = ["uvloop", "networkx", "torch-geometric", "torch", "torchtext"]
 database = ["networkx"]
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.3.1"
-black = "^23.3.0"
-flake8 = "^6.0.0"
-pytest-cov = "^4.1.0"
-pyinstaller = "^5.10.1"
+pytest = "^8.1.1"
+black = "^24.4.1"
+flake8 = "^7.0.0"
+pytest-cov = "^5.0.0"
+pyinstaller = "^6.6.0"
 pdoc3 = "^0.10.0"
 
 [tool.poetry.group.science]
 optional = true
 
 [tool.poetry.group.database]
 optional = true
 
 [tool.poetry.group.science.dependencies]
-networkx = {extras = ["default", "extra"], version = "^3.1"}
-torch-geometric = {version = "^2.4.0"}
-torch = {version = "^2.1.0+cpu", source = "torch"}
-torchtext = {version = "^0.16.0+cpu", markers = "sys_platform == 'linux' or sys_platform == 'darwin'", source = "torch"}
-nbconvert = "^7.9.2"
-jupyter-core = "^5.4.0"
-jupyter-client = "^8.4.0"
-notebook = "^7.0.5"
+networkx = {extras = ["default", "extra"], version = "^3.3"}
+torch-geometric = "^2.5.3"
+torch = {version = "^2.3.0+cpu", source = "torch"}
+torchtext = {version = "^0.18.0+cpu", markers = "sys_platform == 'linux' or sys_platform == 'darwin'", source = "torch"}
+nbconvert = "^7.16.3"
+jupyter-core = "^5.7.2"
+jupyter-client = "^8.6.1"
+notebook = "^7.1.3"
 
 [tool.poetry.group.database.dependencies]
 networkx = {extras = ["default", "extra"], version = "^3.1"}
 
 [[tool.poetry.source]]
 name = "pyg"
 url = "https://data.pyg.org/whl/torch-2.1.0+cpu.html"
```

### Comparing `appthreat_chen-2.0.8/PKG-INFO` & `appthreat_chen-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 Metadata-Version: 2.1
 Name: appthreat-chen
-Version: 2.0.8
+Version: 2.0.9
 Summary: Code Hierarchy Exploration Net (chen)
 Home-page: https://github.com/AppThreat/chen
 License: Apache-2.0
 Keywords: chen,code-analysis,static-analysis
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
-Requires-Python: >=3.8.1,<3.12
+Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Provides-Extra: database
 Provides-Extra: science
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
-Requires-Dist: gitpython (>=3.1.37,<4.0.0)
-Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: gitpython (>=3.1.43,<4.0.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: oras (==0.1.26)
-Requires-Dist: orjson (>=3.9.0,<4.0.0)
+Requires-Dist: orjson (>=3.10.1,<4.0.0)
 Requires-Dist: packageurl-python (>=0.11.2,<0.12.0)
-Requires-Dist: psutil (>=5.9.5,<6.0.0)
-Requires-Dist: rich (>=13.4.1,<14.0.0)
+Requires-Dist: psutil (>=5.9.8,<6.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0) ; (sys_platform == "linux" or sys_platform == "darwin") and (extra == "science")
-Requires-Dist: websockets (>=11.0.2,<12.0.0)
+Requires-Dist: websockets (>=12.0,<13.0)
 Project-URL: CI, https://github.com/AppThreat/chen/actions
 Project-URL: Repository, https://github.com/AppThreat/chen
 Description-Content-Type: text/markdown
 
 # chen
 
 Code Hierarchy Exploration Net (chen) is an advanced exploration toolkit for your application source code and its dependency hierarchy. This repo contains the source code for chen library and an advanced REPL console called chennai (chen not AI).
```

