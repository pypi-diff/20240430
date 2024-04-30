# Comparing `tmp/loe_simp_app_fw-1.2.0.tar.gz` & `tmp/loe_simp_app_fw-1.2.1.tar.gz`

## Comparing `loe_simp_app_fw-1.2.0.tar` & `loe_simp_app_fw-1.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/config-example.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/src/loe_simp_app_fw/__init__.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/src/loe_simp_app_fw/config.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/src/loe_simp_app_fw/helper.py
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/src/loe_simp_app_fw/logger.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/tests/test_import.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/LICENSE
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.1/config-example.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.1/src/loe_simp_app_fw/__init__.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.1/src/loe_simp_app_fw/config.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.1/src/loe_simp_app_fw/helper.py
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.1/src/loe_simp_app_fw/logger.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.1/tests/test_import.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.1/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.1/PKG-INFO
```

### Comparing `loe_simp_app_fw-1.2.0/src/loe_simp_app_fw/config.py` & `loe_simp_app_fw-1.2.1/src/loe_simp_app_fw/config.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.2.0/src/loe_simp_app_fw/helper.py` & `loe_simp_app_fw-1.2.1/src/loe_simp_app_fw/helper.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.2.0/src/loe_simp_app_fw/logger.py` & `loe_simp_app_fw-1.2.1/src/loe_simp_app_fw/logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import datetime
 import tempfile
 from io import TextIOWrapper
-from typing import Optional, IO
 from .helper import create_folder_if_not_exists, ProjectRootChanged
 
 # Do not write the Log until the explicit initialization of the logger
 
 class Logger:
     # Following parameters should be set at the top-level environment of the project
     _project_root_path = ""
@@ -24,54 +23,53 @@
 
     @classmethod
     def _create_log_file(cls):
         if not os.path.isfile(cls._log_location()) and not os.path.isdir(cls._log_location()):
             with open(cls._log_location(), "w", encoding="utf-8") as f:
                 print("Create log file successfully.")
 
-    @classmethod
-    def setup(cls, log_folder_path: str, project_root_path: str = os.getcwd()):
+    def __init__(self, log_folder_path: str, project_root_path: str = os.getcwd()):
         """Init Logger
 
         Args:
             log_folder_path (str): path to log folder relative to project root path
             project_root_path (str, optional): path to project top-level directory. Defaults to os.getcwd().
                                                 The parent folder of that would be os.path.dirname(os.path.realpath(__file__)).
 
         Raises:
             ProjectRootChanged: Project root directory should not be changed once set
         """
         # Sanity check
-        if cls._project_root_path and project_root_path and not os.path.samefile(project_root_path, cls._project_root_path):
-            cls.error("One should not change project root path twice")
+        if self._project_root_path and project_root_path and not os.path.samefile(project_root_path, self._project_root_path):
+            self.error("One should not change project root path twice")
             raise ProjectRootChanged
 
         # Save input
-        cls._log_folder_path = log_folder_path
-        cls._project_root_path = project_root_path
+        type(self)._log_folder_path = log_folder_path
+        type(self)._project_root_path = project_root_path
 
         # Create log folder
-        folder_name = os.path.join(cls._project_root_path, cls._log_folder_path)
+        folder_name = os.path.join(self._project_root_path, self._log_folder_path)
         if not os.path.isfile(folder_name) and not os.path.isdir(folder_name):
             create_folder_if_not_exists(folder_name)
 
         # Create file IO handle
-        cls._log_file_handle.close()
-        cls._log_file_handle = open(cls._log_location(), "a", encoding="utf-8")
+        type(self)._log_file_handle.close()
+        type(self)._log_file_handle = open(self._log_location(), "a", encoding="utf-8")
 
         # Save previous logs
-        cls._log_file_handle.writelines(f"\n{datetime.datetime.now()} INIT Logger successful\n")
-        cls._log_file_handle.writelines("".join(cls._log_buffer))
+        type(self)._log_file_handle.writelines(f"\n{datetime.datetime.now()} INIT Logger successful\n")
+        type(self)._log_file_handle.writelines("".join(self._log_buffer))
         
         # Empty log buffer
-        cls._log_buffer = []
+        type(self)._log_buffer = []
 
         # Update flags
-        cls._isInit = True
-        print(f"Logger init process finished, Logger isInit is set to {cls._isInit}")
+        type(self)._isInit = True
+        print(f"Logger init process finished, Logger isInit is set to {self._isInit}")
 
     @classmethod
     def info(cls, msg: str) -> None:
         cls._log("INFO", msg)
 
     @classmethod
     def debug(cls, msg: str) -> None:
@@ -98,13 +96,13 @@
             cls._log_buffer.append(composed_log_entry)
             print(composed_log_entry)
         return
         
 
 def logger_showoff() -> None:
     # Demonstrate the logger
-    Logger.setup("log")
+    Logger("log")
     print(f"Today is {datetime.date.today()}")
     Logger.info("LOGGER IS DeMoInG.")
 
 if __name__ == "__main__":
     logger_showoff()
```

### Comparing `loe_simp_app_fw-1.2.0/tests/test_import.py` & `loe_simp_app_fw-1.2.1/tests/test_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from loe_simp_app_fw.logger import Logger
 
 
 Config("config.yaml", example_config_path="config-example.yaml", project_root_path=os.path.dirname(os.path.dirname(os.path.realpath(__file__))))
 
 Logger.debug("Should be in both terminal and log file (later).")
 
-Logger.setup("log", project_root_path=os.path.dirname(os.path.dirname(os.path.realpath(__file__))))
+Logger("log", project_root_path=os.path.dirname(os.path.dirname(os.path.realpath(__file__))))
 
 something = Config.config["project root path"]
 
 Logger.debug("Should be in the log file only.")
 
 Logger.debug("andsfijasndif")
 Logger.debug("andsfijasndif")
```

### Comparing `loe_simp_app_fw-1.2.0/.gitignore` & `loe_simp_app_fw-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.2.0/LICENSE` & `loe_simp_app_fw-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.2.0/README.md` & `loe_simp_app_fw-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.2.0/pyproject.toml` & `loe_simp_app_fw-1.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "loe_simp_app_fw"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="loeeeee", email="95266635+loeeeee@users.noreply.github.com" },
 ]
 description = "A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `loe_simp_app_fw-1.2.0/PKG-INFO` & `loe_simp_app_fw-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: loe_simp_app_fw
-Version: 1.2.0
+Version: 1.2.1
 Summary: A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook.
 Project-URL: Homepage, https://github.com/loeeeee/loe-simp-app-fw
 Project-URL: Issues, https://github.com/loeeeee/loe-simp-app-fw/issues
 Author-email: loeeeee <95266635+loeeeee@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

