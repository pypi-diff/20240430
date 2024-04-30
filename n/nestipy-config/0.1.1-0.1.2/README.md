# Comparing `tmp/nestipy_config-0.1.1.tar.gz` & `tmp/nestipy_config-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy_config-0.1.1.tar", max compression
+gzip compressed data, was "nestipy_config-0.1.2.tar", max compression
```

## Comparing `nestipy_config-0.1.1.tar` & `nestipy_config-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy_config-0.1.1/LICENSE
--rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy_config-0.1.1/README.md
--rw-r--r--   0        0        0      435 2024-04-29 13:32:12.203446 nestipy_config-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      198 2024-04-27 18:09:34.176104 nestipy_config-0.1.1/src/nestipy_config/__init__.py
--rw-r--r--   0        0        0      686 2024-04-29 12:25:23.905614 nestipy_config-0.1.1/src/nestipy_config/config_builder.py
--rw-r--r--   0        0        0      283 2024-04-27 18:06:48.892072 nestipy_config-0.1.1/src/nestipy_config/config_module.py
--rw-r--r--   0        0        0      758 2024-04-29 11:59:37.960181 nestipy_config-0.1.1/src/nestipy_config/config_service.py
--rw-r--r--   0        0        0     2388 1970-01-01 00:00:00.000000 nestipy_config-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-03-29 11:21:44.560810 nestipy_config-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1906 2024-04-26 13:39:21.397719 nestipy_config-0.1.2/README.md
+-rw-r--r--   0        0        0      435 2024-04-30 15:17:30.582179 nestipy_config-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-27 18:09:34.176104 nestipy_config-0.1.2/src/nestipy_config/__init__.py
+-rw-r--r--   0        0        0      686 2024-04-30 15:17:39.786102 nestipy_config-0.1.2/src/nestipy_config/config_builder.py
+-rw-r--r--   0        0        0      283 2024-04-27 18:06:48.892072 nestipy_config-0.1.2/src/nestipy_config/config_module.py
+-rw-r--r--   0        0        0      758 2024-04-29 11:59:37.960181 nestipy_config-0.1.2/src/nestipy_config/config_service.py
+-rw-r--r--   0        0        0     2388 1970-01-01 00:00:00.000000 nestipy_config-0.1.2/PKG-INFO
```

### Comparing `nestipy_config-0.1.1/LICENSE` & `nestipy_config-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nestipy_config-0.1.1/README.md` & `nestipy_config-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nestipy_config-0.1.1/src/nestipy_config/config_builder.py` & `nestipy_config-0.1.2/src/nestipy_config/config_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass, field
 from typing import Callable
 
-from nestipy_dynamic_module import ConfigurableModuleBuilder, DynamicModule
+from nestipy.dynamic_module import ConfigurableModuleBuilder, DynamicModule
 
 
 @dataclass
 class ConfigOption:
     folder: str = './'
     is_global: bool = False
     ignore_env_file: bool = False
```

### Comparing `nestipy_config-0.1.1/src/nestipy_config/config_service.py` & `nestipy_config-0.1.2/src/nestipy_config/config_service.py`

 * *Files identical despite different names*

### Comparing `nestipy_config-0.1.1/PKG-INFO` & `nestipy_config-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nestipy-config
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: tsiresymila
 Author-email: tsiresymila@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: nestipy (>=0.2.9,<0.3.0)
+Requires-Dist: nestipy (>=0.3.0,<0.4.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a target="_blank"><img src="https://raw.githubusercontent.com/nestipy/nestipy/release-v1/nestipy.png" width="200" alt="Nestipy Logo" /></a></p>
 <p align="center">
     <a href="https://pypi.org/project/nestipy">
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: nestipy-config Version: 0.1.1 Summary: Author:
+Metadata-Version: 2.1 Name: nestipy-config Version: 0.1.2 Summary: Author:
 tsiresymila Author-email: tsiresymila@gmail.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: nestipy
-(>=0.2.9,<0.3.0) Requires-Dist: python-dotenv (>=1.0.1,<2.0.0) Description-
+(>=0.3.0,<0.4.0) Requires-Dist: python-dotenv (>=1.0.1,<2.0.0) Description-
 Content-Type: text/markdown
                                 [Nestipy Logo]
                           _[_V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_L_i_c_e_n_s_e_]
 ## Description
 Nestipy is a Python framework built on top of FastAPI that follows the modular
 architecture of NestJS
 Under the hood, Nestipy makes use of _F_a_s_t_A_P_I, but also provides compatibility
```

