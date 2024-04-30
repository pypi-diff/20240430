# Comparing `tmp/raspberry_config_sdk-1.0.0.tar.gz` & `tmp/raspberry_config_sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspberry_config_sdk-1.0.0.tar", last modified: Tue Apr 23 00:13:54 2024, max compression
+gzip compressed data, was "raspberry_config_sdk-1.0.2.tar", last modified: Tue Apr 30 19:20:56 2024, max compression
```

## Comparing `raspberry_config_sdk-1.0.0.tar` & `raspberry_config_sdk-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:13:54.125403 raspberry_config_sdk-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-23 00:13:50.000000 raspberry_config_sdk-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-23 00:13:54.125403 raspberry_config_sdk-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-23 00:13:50.000000 raspberry_config_sdk-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-23 00:13:50.000000 raspberry_config_sdk-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:13:54.121403 raspberry_config_sdk-1.0.0/raspberry_config_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-23 00:13:50.000000 raspberry_config_sdk-1.0.0/raspberry_config_sdk/BootConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-23 00:13:50.000000 raspberry_config_sdk-1.0.0/raspberry_config_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-23 00:13:50.000000 raspberry_config_sdk-1.0.0/raspberry_config_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:13:54.125403 raspberry_config_sdk-1.0.0/raspberry_config_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-23 00:13:54.000000 raspberry_config_sdk-1.0.0/raspberry_config_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-23 00:13:54.000000 raspberry_config_sdk-1.0.0/raspberry_config_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 00:13:54.000000 raspberry_config_sdk-1.0.0/raspberry_config_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 00:13:54.000000 raspberry_config_sdk-1.0.0/raspberry_config_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 00:13:54.125403 raspberry_config_sdk-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-23 00:13:50.000000 raspberry_config_sdk-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:13:54.125403 raspberry_config_sdk-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:13:50.000000 raspberry_config_sdk-1.0.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-23 00:13:50.000000 raspberry_config_sdk-1.0.0/test/test_boot_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:20:56.709672 raspberry_config_sdk-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-30 19:20:49.000000 raspberry_config_sdk-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-30 19:20:56.709672 raspberry_config_sdk-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-30 19:20:49.000000 raspberry_config_sdk-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-30 19:20:49.000000 raspberry_config_sdk-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:20:56.709672 raspberry_config_sdk-1.0.2/raspberry_config_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-30 19:20:49.000000 raspberry_config_sdk-1.0.2/raspberry_config_sdk/BootConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-30 19:20:49.000000 raspberry_config_sdk-1.0.2/raspberry_config_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-30 19:20:49.000000 raspberry_config_sdk-1.0.2/raspberry_config_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:20:56.709672 raspberry_config_sdk-1.0.2/raspberry_config_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-30 19:20:56.000000 raspberry_config_sdk-1.0.2/raspberry_config_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-30 19:20:56.000000 raspberry_config_sdk-1.0.2/raspberry_config_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:20:56.000000 raspberry_config_sdk-1.0.2/raspberry_config_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 19:20:56.000000 raspberry_config_sdk-1.0.2/raspberry_config_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 19:20:56.000000 raspberry_config_sdk-1.0.2/raspberry_config_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:20:56.709672 raspberry_config_sdk-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-30 19:20:49.000000 raspberry_config_sdk-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:20:56.709672 raspberry_config_sdk-1.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:20:49.000000 raspberry_config_sdk-1.0.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-30 19:20:49.000000 raspberry_config_sdk-1.0.2/test/test_boot_config.py
```

### Comparing `raspberry_config_sdk-1.0.0/LICENSE` & `raspberry_config_sdk-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `raspberry_config_sdk-1.0.0/PKG-INFO` & `raspberry_config_sdk-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: raspberry-config-sdk
-Version: 1.0.0
+Version: 1.0.2
 Summary: Easily Configure your Raspberry Pi from your code
-Home-page: https://github.com/DEADSEC-SECURITY/sma-manager
+Home-page: https://github.com/DEADSEC-SECURITY/raspberry-config-sdk
 Author: DeadSec-Security
 Author-email: amng835@gmail.com
 License: MIT
 Keywords: raspberry,raspberry pi,config.txt,raspberry config,boot
-Requires-Python: >=3.8
+Requires-Python: >=3.8,==3.11.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: tqdm~=4.66.0
+Requires-Dist: bigtree~=0.17.0
 
 # Raspberry Config SDK ![Release](https://img.shields.io/github/v/release/DEADSEC-SECURITY/raspberry-config-sdk?label=Release&style=flat-square) ![Python_Version](https://img.shields.io/badge/Python-3.9%2B-blue?style=flat-square) ![License](https://img.shields.io/github/license/DEADSEC-SECURITY/raspberry-config-sdk?label=License&style=flat-square) 
 
 [![CodeQL](https://github.com/DEADSEC-SECURITY/raspberry-config-sdk/actions/workflows/codeql.yml/badge.svg)](https://github.com/DEADSEC-SECURITY/raspberry-config-sdk/actions/workflows/codeql.yml) 
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dd/raspberry-config-sdk?label=Daily%20Downloads&style=flat-square) ![PyPI - Downloads](https://img.shields.io/pypi/dw/raspberry-config-sdk?label=Weekly%20Downloads&style=flat-square) ![PyPI - Downloads](https://img.shields.io/pypi/dm/raspberry-config-sdk?label=Monthly%20Downloads&style=flat-square)
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1 Name: raspberry-config-sdk Version: 1.0.0 Summary: Easily
+Metadata-Version: 2.1 Name: raspberry-config-sdk Version: 1.0.2 Summary: Easily
 Configure your Raspberry Pi from your code Home-page: https://github.com/
-DEADSEC-SECURITY/sma-manager Author: DeadSec-Security Author-email:
+DEADSEC-SECURITY/raspberry-config-sdk Author: DeadSec-Security Author-email:
 amng835@gmail.com License: MIT Keywords: raspberry,raspberry
-pi,config.txt,raspberry config,boot Requires-Python: >=3.8 Description-Content-
-Type: text/markdown License-File: LICENSE # Raspberry Config SDK ![Release]
+pi,config.txt,raspberry config,boot Requires-Python: >=3.8,==3.11.2
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+tqdm~=4.66.0 Requires-Dist: bigtree~=0.17.0 # Raspberry Config SDK ![Release]
 (https://img.shields.io/github/v/release/DEADSEC-SECURITY/raspberry-config-
 sdk?label=Release&style=flat-square) ![Python_Version](https://img.shields.io/
 badge/Python-3.9%2B-blue?style=flat-square) ![License](https://img.shields.io/
 github/license/DEADSEC-SECURITY/raspberry-config-sdk?label=License&style=flat-
 square) [![CodeQL](https://github.com/DEADSEC-SECURITY/raspberry-config-sdk/
 actions/workflows/codeql.yml/badge.svg)](https://github.com/DEADSEC-SECURITY/
 raspberry-config-sdk/actions/workflows/codeql.yml) ![PyPI - Downloads](https://
```

### Comparing `raspberry_config_sdk-1.0.0/README.md` & `raspberry_config_sdk-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `raspberry_config_sdk-1.0.0/raspberry_config_sdk/BootConfig.py` & `raspberry_config_sdk-1.0.2/raspberry_config_sdk/BootConfig.py`

 * *Files identical despite different names*

### Comparing `raspberry_config_sdk-1.0.0/raspberry_config_sdk.egg-info/PKG-INFO` & `raspberry_config_sdk-1.0.2/raspberry_config_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: raspberry-config-sdk
-Version: 1.0.0
+Version: 1.0.2
 Summary: Easily Configure your Raspberry Pi from your code
-Home-page: https://github.com/DEADSEC-SECURITY/sma-manager
+Home-page: https://github.com/DEADSEC-SECURITY/raspberry-config-sdk
 Author: DeadSec-Security
 Author-email: amng835@gmail.com
 License: MIT
 Keywords: raspberry,raspberry pi,config.txt,raspberry config,boot
-Requires-Python: >=3.8
+Requires-Python: >=3.8,==3.11.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: tqdm~=4.66.0
+Requires-Dist: bigtree~=0.17.0
 
 # Raspberry Config SDK ![Release](https://img.shields.io/github/v/release/DEADSEC-SECURITY/raspberry-config-sdk?label=Release&style=flat-square) ![Python_Version](https://img.shields.io/badge/Python-3.9%2B-blue?style=flat-square) ![License](https://img.shields.io/github/license/DEADSEC-SECURITY/raspberry-config-sdk?label=License&style=flat-square) 
 
 [![CodeQL](https://github.com/DEADSEC-SECURITY/raspberry-config-sdk/actions/workflows/codeql.yml/badge.svg)](https://github.com/DEADSEC-SECURITY/raspberry-config-sdk/actions/workflows/codeql.yml) 
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dd/raspberry-config-sdk?label=Daily%20Downloads&style=flat-square) ![PyPI - Downloads](https://img.shields.io/pypi/dw/raspberry-config-sdk?label=Weekly%20Downloads&style=flat-square) ![PyPI - Downloads](https://img.shields.io/pypi/dm/raspberry-config-sdk?label=Monthly%20Downloads&style=flat-square)
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1 Name: raspberry-config-sdk Version: 1.0.0 Summary: Easily
+Metadata-Version: 2.1 Name: raspberry-config-sdk Version: 1.0.2 Summary: Easily
 Configure your Raspberry Pi from your code Home-page: https://github.com/
-DEADSEC-SECURITY/sma-manager Author: DeadSec-Security Author-email:
+DEADSEC-SECURITY/raspberry-config-sdk Author: DeadSec-Security Author-email:
 amng835@gmail.com License: MIT Keywords: raspberry,raspberry
-pi,config.txt,raspberry config,boot Requires-Python: >=3.8 Description-Content-
-Type: text/markdown License-File: LICENSE # Raspberry Config SDK ![Release]
+pi,config.txt,raspberry config,boot Requires-Python: >=3.8,==3.11.2
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+tqdm~=4.66.0 Requires-Dist: bigtree~=0.17.0 # Raspberry Config SDK ![Release]
 (https://img.shields.io/github/v/release/DEADSEC-SECURITY/raspberry-config-
 sdk?label=Release&style=flat-square) ![Python_Version](https://img.shields.io/
 badge/Python-3.9%2B-blue?style=flat-square) ![License](https://img.shields.io/
 github/license/DEADSEC-SECURITY/raspberry-config-sdk?label=License&style=flat-
 square) [![CodeQL](https://github.com/DEADSEC-SECURITY/raspberry-config-sdk/
 actions/workflows/codeql.yml/badge.svg)](https://github.com/DEADSEC-SECURITY/
 raspberry-config-sdk/actions/workflows/codeql.yml) ![PyPI - Downloads](https://
```

### Comparing `raspberry_config_sdk-1.0.0/setup.py` & `raspberry_config_sdk-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 import pathlib
 
 README = (pathlib.Path(__file__).parent / "README.md").read_text(encoding="utf8")
 
 setup(
     name="raspberry-config-sdk",
     packages=find_packages(),
-    version="1.0.0",
+    version="1.0.2",
     description="Easily Configure your Raspberry Pi from your code",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DeadSec-Security",
     author_email="amng835@gmail.com",
-    url="https://github.com/DEADSEC-SECURITY/sma-manager",
+    url="https://github.com/DEADSEC-SECURITY/raspberry-config-sdk",
+    install_requires=["tqdm~=4.66.0", "bigtree~=0.17.0"],
     keywords=["raspberry", "raspberry pi", "config.txt", "raspberry config", "boot"],
     license="MIT",
-    python_requires=">=3.8",
+    python_requires=">=3.8,==3.11.2",
 )
```

