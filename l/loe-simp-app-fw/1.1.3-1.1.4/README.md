# Comparing `tmp/loe_simp_app_fw-1.1.3.tar.gz` & `tmp/loe_simp_app_fw-1.1.4.tar.gz`

## Comparing `loe_simp_app_fw-1.1.3.tar` & `loe_simp_app_fw-1.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/config-example.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/src/loe_simp_app_fw/__init__.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/src/loe_simp_app_fw/config.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/src/loe_simp_app_fw/helper.py
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/src/loe_simp_app_fw/logger.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/tests/test_import.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/LICENSE
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/config-example.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/src/loe_simp_app_fw/__init__.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/src/loe_simp_app_fw/config.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/src/loe_simp_app_fw/helper.py
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/src/loe_simp_app_fw/logger.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/tests/test_import.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/LICENSE
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/PKG-INFO
```

### Comparing `loe_simp_app_fw-1.1.3/src/loe_simp_app_fw/config.py` & `loe_simp_app_fw-1.1.4/src/loe_simp_app_fw/config.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.3/src/loe_simp_app_fw/helper.py` & `loe_simp_app_fw-1.1.4/src/loe_simp_app_fw/helper.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.3/src/loe_simp_app_fw/logger.py` & `loe_simp_app_fw-1.1.4/src/loe_simp_app_fw/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import os
 import datetime
+import tempfile
 from io import TextIOWrapper
 from typing import Optional, IO
 from .helper import create_folder_if_not_exists, ProjectRootChanged
 
 # Do not write the Log until the explicit initialization of the logger
 
 class Logger:
     # Following parameters should be set at the top-level environment of the project
     _project_root_path = ""
     _log_folder_path = "" # The path of _example_config_path relative to _project_root_path
     
     # Internal variable
     _log_buffer = []
     _isInit = False
-    _log_file_handle: Optional[IO] = None
+    _log_file_handle: IO = tempfile.TemporaryFile()
     
     @classmethod
     def _log_location(cls):
         file_name = f"{datetime.date.today()}.log"
         return os.path.join(cls._project_root_path, cls._log_folder_path, file_name)
 
     @classmethod
@@ -49,14 +50,15 @@
 
         # Create log folder
         folder_name = os.path.join(self._project_root_path, self._log_folder_path)
         if not os.path.isfile(folder_name) and not os.path.isdir(folder_name):
             create_folder_if_not_exists(folder_name)
 
         # Create file IO handle
+        self._log_file_handle.close()
         self._log_file_handle = open(self._log_location(), "a", encoding="utf-8")
 
         # Save previous logs
         self._log_file_handle.writelines(f"\n{datetime.datetime.now()} INIT Logger successful\n")
         self._log_file_handle.writelines("".join(self._log_buffer))
         
         # Empty log buffer
@@ -82,21 +84,21 @@
     def error(cls, msg :str) -> None:
         cls._log("ERROR", msg)
 
     @classmethod
     def _log(cls, level: str, msg: str) -> None:
         # Compose log
         composed_log_entry = f"{datetime.datetime.now()} {level.upper()}: {msg}\n"
-        if cls._isInit and isinstance(cls._log_file_handle, TextIOWrapper): 
+        if cls._isInit: 
             # The file handler is only to make static checker happy
             # Write to file
             try:
                 cls._log_file_handle.writelines(composed_log_entry)
             except FileNotFoundError:
-                cls._create_log_file()
+                cls._create_log_file()                
         else:
             # Write to buffer, not file
             cls._log_buffer.append(composed_log_entry)
             print(composed_log_entry)
         return
```

### Comparing `loe_simp_app_fw-1.1.3/tests/test_import.py` & `loe_simp_app_fw-1.1.4/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.3/.gitignore` & `loe_simp_app_fw-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.3/LICENSE` & `loe_simp_app_fw-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.3/README.md` & `loe_simp_app_fw-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.3/pyproject.toml` & `loe_simp_app_fw-1.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "loe_simp_app_fw"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="loeeeee", email="95266635+loeeeee@users.noreply.github.com" },
 ]
 description = "A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `loe_simp_app_fw-1.1.3/PKG-INFO` & `loe_simp_app_fw-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: loe_simp_app_fw
-Version: 1.1.3
+Version: 1.1.4
 Summary: A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook.
 Project-URL: Homepage, https://github.com/loeeeee/loe-simp-app-fw
 Project-URL: Issues, https://github.com/loeeeee/loe-simp-app-fw/issues
 Author-email: loeeeee <95266635+loeeeee@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

