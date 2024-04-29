# Comparing `tmp/vapor_steam-1.5.4.tar.gz` & `tmp/vapor_steam-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vapor_steam-1.5.4.tar", max compression
+gzip compressed data, was "vapor_steam-1.5.5.tar", max compression
```

## Comparing `vapor_steam-1.5.4.tar` & `vapor_steam-1.5.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35139 2023-12-04 17:43:44.356770 vapor_steam-1.5.4/LICENSE
--rw-r--r--   0        0        0     4481 2024-02-12 17:12:51.976591 vapor_steam-1.5.4/README.md
--rw-r--r--   0        0        0     2938 2024-02-13 16:42:00.058175 vapor_steam-1.5.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-13 16:42:00.058175 vapor_steam-1.5.4/tests/__init__.py
--rw-r--r--   0        0        0     2644 2024-02-12 17:12:51.983258 vapor_steam-1.5.4/tests/test_api_interface.py
--rw-r--r--   0        0        0      790 2024-02-12 17:12:51.983258 vapor_steam-1.5.4/tests/test_arg_parsing.py
--rw-r--r--   0        0        0     3783 2024-02-13 16:07:33.920232 vapor_steam-1.5.4/tests/test_cache.py
--rw-r--r--   0        0        0     1816 2024-02-13 16:07:33.920232 vapor_steam-1.5.4/tests/test_config.py
--rw-r--r--   0        0        0      427 2024-02-12 17:12:51.983258 vapor_steam-1.5.4/tests/test_data_structures.py
--rw-r--r--   0        0        0     9180 2024-02-12 17:12:51.983258 vapor_steam-1.5.4/tests/test_ui.py
--rw-r--r--   0        0        0        0 2024-02-11 19:24:52.813973 vapor_steam-1.5.4/vapor/__init__.py
--rw-r--r--   0        0        0      189 2024-02-11 19:24:52.820640 vapor_steam-1.5.4/vapor/__main__.py
--rw-r--r--   0        0        0     6850 2024-02-12 17:12:51.986591 vapor_steam-1.5.4/vapor/api_interface.py
--rw-r--r--   0        0        0      458 2024-02-11 19:24:52.820640 vapor_steam-1.5.4/vapor/argument_handler.py
--rw-r--r--   0        0        0     5394 2024-02-13 16:07:33.920232 vapor_steam-1.5.4/vapor/cache_handler.py
--rw-r--r--   0        0        0     2336 2024-02-12 17:12:51.986591 vapor_steam-1.5.4/vapor/config_handler.py
--rw-r--r--   0        0        0     2699 2024-02-13 16:07:33.920232 vapor_steam-1.5.4/vapor/data_structures.py
--rw-r--r--   0        0        0      577 2024-02-12 17:12:51.986591 vapor_steam-1.5.4/vapor/exceptions.py
--rw-r--r--   0        0        0     6386 2024-02-12 17:12:51.989925 vapor_steam-1.5.4/vapor/main.py
--rw-r--r--   0        0        0      830 2024-02-12 17:12:51.989925 vapor_steam-1.5.4/vapor/main.tcss
--rw-r--r--   0        0        0     5796 1970-01-01 00:00:00.000000 vapor_steam-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0    35139 2023-12-04 17:43:44.356770 vapor_steam-1.5.5/LICENSE
+-rw-r--r--   0        0        0     4481 2024-02-12 17:12:51.976591 vapor_steam-1.5.5/README.md
+-rw-r--r--   0        0        0     2938 2024-04-29 23:54:44.582309 vapor_steam-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-13 16:42:00.058175 vapor_steam-1.5.5/tests/__init__.py
+-rw-r--r--   0        0        0     2644 2024-02-12 17:12:51.983258 vapor_steam-1.5.5/tests/test_api_interface.py
+-rw-r--r--   0        0        0      790 2024-02-12 17:12:51.983258 vapor_steam-1.5.5/tests/test_arg_parsing.py
+-rw-r--r--   0        0        0     3783 2024-02-13 16:07:33.920232 vapor_steam-1.5.5/tests/test_cache.py
+-rw-r--r--   0        0        0     1816 2024-02-13 16:07:33.920232 vapor_steam-1.5.5/tests/test_config.py
+-rw-r--r--   0        0        0      427 2024-02-12 17:12:51.983258 vapor_steam-1.5.5/tests/test_data_structures.py
+-rw-r--r--   0        0        0     9180 2024-02-12 17:12:51.983258 vapor_steam-1.5.5/tests/test_ui.py
+-rw-r--r--   0        0        0        0 2024-02-11 19:24:52.813973 vapor_steam-1.5.5/vapor/__init__.py
+-rw-r--r--   0        0        0      189 2024-02-11 19:24:52.820640 vapor_steam-1.5.5/vapor/__main__.py
+-rw-r--r--   0        0        0     6850 2024-03-06 03:13:47.011560 vapor_steam-1.5.5/vapor/api_interface.py
+-rw-r--r--   0        0        0      458 2024-02-11 19:24:52.820640 vapor_steam-1.5.5/vapor/argument_handler.py
+-rw-r--r--   0        0        0     5394 2024-02-13 16:07:33.920232 vapor_steam-1.5.5/vapor/cache_handler.py
+-rw-r--r--   0        0        0     2336 2024-02-12 17:12:51.986591 vapor_steam-1.5.5/vapor/config_handler.py
+-rw-r--r--   0        0        0     2699 2024-02-13 16:07:33.920232 vapor_steam-1.5.5/vapor/data_structures.py
+-rw-r--r--   0        0        0      577 2024-02-12 17:12:51.986591 vapor_steam-1.5.5/vapor/exceptions.py
+-rw-r--r--   0        0        0     6386 2024-02-12 17:12:51.989925 vapor_steam-1.5.5/vapor/main.py
+-rw-r--r--   0        0        0      844 2024-04-29 23:54:44.582309 vapor_steam-1.5.5/vapor/main.tcss
+-rw-r--r--   0        0        0     5796 1970-01-01 00:00:00.000000 vapor_steam-1.5.5/PKG-INFO
```

### Comparing `vapor_steam-1.5.4/LICENSE` & `vapor_steam-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vapor_steam-1.5.4/README.md` & `vapor_steam-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `vapor_steam-1.5.4/pyproject.toml` & `vapor_steam-1.5.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vapor-steam"
-version = "1.5.4"
+version = "1.5.5"
 description = "TUI program to check the ProtonDB compatibility of all the games of a Steam user."
 authors = ["TabulateJarl8 <tabulatejarl8@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "vapor"}]
 homepage = "https://tabulate.tech/software/vapor"
 repository = "https://github.com/TabulateJarl8/vapor"
@@ -25,25 +25,25 @@
 ]
 include = [
 	{ path = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-textual = "^0.50.1"
+textual = "^0.58.0"
 aiohttp = "^3.9.3"
 platformdirs = "^4.1.0"
 typing-extensions = "^4.9.0"
 
 [tool.poetry.scripts]
 vapor = "vapor.__main__:main"
 
 [tool.poetry.group.dev.dependencies]
-textual-dev = "^1.4.0"
-ruff = "^0.2.1"
+textual-dev = "^1.5.1"
+ruff = "^0.4.2"
 pytest = "^8.0.0"
 pytest-cov = "^4.1.0"
 pytest-asyncio = "^0.23.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `vapor_steam-1.5.4/tests/test_api_interface.py` & `vapor_steam-1.5.5/tests/test_api_interface.py`

 * *Files identical despite different names*

### Comparing `vapor_steam-1.5.4/tests/test_arg_parsing.py` & `vapor_steam-1.5.5/tests/test_arg_parsing.py`

 * *Files identical despite different names*

### Comparing `vapor_steam-1.5.4/tests/test_cache.py` & `vapor_steam-1.5.5/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `vapor_steam-1.5.4/tests/test_config.py` & `vapor_steam-1.5.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `vapor_steam-1.5.4/tests/test_ui.py` & `vapor_steam-1.5.5/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `vapor_steam-1.5.4/vapor/api_interface.py` & `vapor_steam-1.5.5/vapor/api_interface.py`

 * *Files identical despite different names*

### Comparing `vapor_steam-1.5.4/vapor/cache_handler.py` & `vapor_steam-1.5.5/vapor/cache_handler.py`

 * *Files identical despite different names*

### Comparing `vapor_steam-1.5.4/vapor/config_handler.py` & `vapor_steam-1.5.5/vapor/config_handler.py`

 * *Files identical despite different names*

### Comparing `vapor_steam-1.5.4/vapor/data_structures.py` & `vapor_steam-1.5.5/vapor/data_structures.py`

 * *Files identical despite different names*

### Comparing `vapor_steam-1.5.4/vapor/exceptions.py` & `vapor_steam-1.5.5/vapor/exceptions.py`

 * *Files identical despite different names*

### Comparing `vapor_steam-1.5.4/vapor/main.py` & `vapor_steam-1.5.5/vapor/main.py`

 * *Files identical despite different names*

### Comparing `vapor_steam-1.5.4/vapor/main.tcss` & `vapor_steam-1.5.5/vapor/main.tcss`

 * *Files 13% similar despite different names*

```diff
@@ -46,18 +46,19 @@
 }
 
 Screen {
 	align: center middle;
 }
 
 #content-container {
-	width: 50%;
+	width: 75%;
 	height: auto;
 	max-height: 100%;
 	padding: 1 2;
+	margin: 2 0;
 	background: $panel;
 	color: $text;
 	border: $secondary tall;
 }
 
 #content-container * {
 	align: center top;
```

### Comparing `vapor_steam-1.5.4/PKG-INFO` & `vapor_steam-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vapor-steam
-Version: 1.5.4
+Version: 1.5.5
 Summary: TUI program to check the ProtonDB compatibility of all the games of a Steam user.
 Home-page: https://tabulate.tech/software/vapor
 License: GPLv3
 Keywords: steam,protondb,compatibility,textual,tui
 Author: TabulateJarl8
 Author-email: tabulatejarl8@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: platformdirs (>=4.1.0,<5.0.0)
-Requires-Dist: textual (>=0.50.1,<0.51.0)
+Requires-Dist: textual (>=0.58.0,<0.59.0)
 Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Project-URL: Repository, https://github.com/TabulateJarl8/vapor
 Description-Content-Type: text/markdown
 
 # Vapor: Steam Proton Compatibility Checker
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: vapor-steam Version: 1.5.4 Summary: TUI program to
+Metadata-Version: 2.1 Name: vapor-steam Version: 1.5.5 Summary: TUI program to
 check the ProtonDB compatibility of all the games of a Steam user. Home-page:
 https://tabulate.tech/software/vapor License: GPLv3 Keywords:
 steam,protondb,compatibility,textual,tui Author: TabulateJarl8 Author-email:
 tabulatejarl8@gmail.com Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Intended Audience :: End Users/Desktop Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: License :: Other/Proprietary
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Typing :: Typed Requires-Dist: aiohttp
 (>=3.9.3,<4.0.0) Requires-Dist: platformdirs (>=4.1.0,<5.0.0) Requires-Dist:
-textual (>=0.50.1,<0.51.0) Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
+textual (>=0.58.0,<0.59.0) Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Project-URL: Repository, https://github.com/TabulateJarl8/vapor Description-
 Content-Type: text/markdown # Vapor: Steam Proton Compatibility Checker
  _[_P_y_P_I_]_[_A_U_R_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]_[_L_i_c_e_n_s_e_]_[_M_a_i_n_t_e_n_a_n_c_e_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_][Coverage]
                               _[_G_i_t_H_u_b_ _f_o_l_l_o_w_e_r_s_]
                                  _[_K_o_f_i_ _B_a_d_g_e_]
 Vapor is a Python package built on [Textual](https://github.com/textualize/
 textual/) which offers a simple Terminal User Interface for checking ProtonDB
```

