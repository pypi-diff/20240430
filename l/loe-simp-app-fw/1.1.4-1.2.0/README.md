# Comparing `tmp/loe_simp_app_fw-1.1.4.tar.gz` & `tmp/loe_simp_app_fw-1.2.0.tar.gz`

## Comparing `loe_simp_app_fw-1.1.4.tar` & `loe_simp_app_fw-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/config-example.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/src/loe_simp_app_fw/__init__.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/src/loe_simp_app_fw/config.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/src/loe_simp_app_fw/helper.py
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/src/loe_simp_app_fw/logger.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/tests/test_import.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/LICENSE
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/config-example.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/src/loe_simp_app_fw/__init__.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/src/loe_simp_app_fw/config.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/src/loe_simp_app_fw/helper.py
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/src/loe_simp_app_fw/logger.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/tests/test_import.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.2.0/PKG-INFO
```

### Comparing `loe_simp_app_fw-1.1.4/src/loe_simp_app_fw/config.py` & `loe_simp_app_fw-1.2.0/src/loe_simp_app_fw/config.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.4/src/loe_simp_app_fw/helper.py` & `loe_simp_app_fw-1.2.0/src/loe_simp_app_fw/helper.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.4/src/loe_simp_app_fw/logger.py` & `loe_simp_app_fw-1.2.0/src/loe_simp_app_fw/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,66 +11,67 @@
     # Following parameters should be set at the top-level environment of the project
     _project_root_path = ""
     _log_folder_path = "" # The path of _example_config_path relative to _project_root_path
     
     # Internal variable
     _log_buffer = []
     _isInit = False
-    _log_file_handle: IO = tempfile.TemporaryFile()
+    _log_file_handle: TextIOWrapper = tempfile.TemporaryFile("w")
     
     @classmethod
     def _log_location(cls):
         file_name = f"{datetime.date.today()}.log"
         return os.path.join(cls._project_root_path, cls._log_folder_path, file_name)
 
     @classmethod
     def _create_log_file(cls):
         if not os.path.isfile(cls._log_location()) and not os.path.isdir(cls._log_location()):
             with open(cls._log_location(), "w", encoding="utf-8") as f:
                 print("Create log file successfully.")
 
-    def __init__(self, log_folder_path: str, project_root_path: str = os.getcwd()):
+    @classmethod
+    def setup(cls, log_folder_path: str, project_root_path: str = os.getcwd()):
         """Init Logger
 
         Args:
             log_folder_path (str): path to log folder relative to project root path
             project_root_path (str, optional): path to project top-level directory. Defaults to os.getcwd().
                                                 The parent folder of that would be os.path.dirname(os.path.realpath(__file__)).
 
         Raises:
             ProjectRootChanged: Project root directory should not be changed once set
         """
         # Sanity check
-        if self._project_root_path and project_root_path and not os.path.samefile(project_root_path, self._project_root_path):
-            self.error("One should not change project root path twice")
+        if cls._project_root_path and project_root_path and not os.path.samefile(project_root_path, cls._project_root_path):
+            cls.error("One should not change project root path twice")
             raise ProjectRootChanged
 
         # Save input
-        self._log_folder_path = log_folder_path
-        self._project_root_path = project_root_path
+        cls._log_folder_path = log_folder_path
+        cls._project_root_path = project_root_path
 
         # Create log folder
-        folder_name = os.path.join(self._project_root_path, self._log_folder_path)
+        folder_name = os.path.join(cls._project_root_path, cls._log_folder_path)
         if not os.path.isfile(folder_name) and not os.path.isdir(folder_name):
             create_folder_if_not_exists(folder_name)
 
         # Create file IO handle
-        self._log_file_handle.close()
-        self._log_file_handle = open(self._log_location(), "a", encoding="utf-8")
+        cls._log_file_handle.close()
+        cls._log_file_handle = open(cls._log_location(), "a", encoding="utf-8")
 
         # Save previous logs
-        self._log_file_handle.writelines(f"\n{datetime.datetime.now()} INIT Logger successful\n")
-        self._log_file_handle.writelines("".join(self._log_buffer))
+        cls._log_file_handle.writelines(f"\n{datetime.datetime.now()} INIT Logger successful\n")
+        cls._log_file_handle.writelines("".join(cls._log_buffer))
         
         # Empty log buffer
-        self._log_buffer = []
+        cls._log_buffer = []
 
         # Update flags
-        self._isInit = True
-        print(f"Logger init process finished, Logger isInit is set to {self._isInit}")
+        cls._isInit = True
+        print(f"Logger init process finished, Logger isInit is set to {cls._isInit}")
 
     @classmethod
     def info(cls, msg: str) -> None:
         cls._log("INFO", msg)
 
     @classmethod
     def debug(cls, msg: str) -> None:
@@ -84,29 +85,26 @@
     def error(cls, msg :str) -> None:
         cls._log("ERROR", msg)
 
     @classmethod
     def _log(cls, level: str, msg: str) -> None:
         # Compose log
         composed_log_entry = f"{datetime.datetime.now()} {level.upper()}: {msg}\n"
-        if cls._isInit: 
+        if cls._isInit:
             # The file handler is only to make static checker happy
             # Write to file
-            try:
-                cls._log_file_handle.writelines(composed_log_entry)
-            except FileNotFoundError:
-                cls._create_log_file()                
+            cls._log_file_handle.writelines(composed_log_entry)
         else:
             # Write to buffer, not file
             cls._log_buffer.append(composed_log_entry)
             print(composed_log_entry)
         return
         
 
 def logger_showoff() -> None:
     # Demonstrate the logger
-    Logger("log")
+    Logger.setup("log")
     print(f"Today is {datetime.date.today()}")
     Logger.info("LOGGER IS DeMoInG.")
 
 if __name__ == "__main__":
     logger_showoff()
```

### Comparing `loe_simp_app_fw-1.1.4/.gitignore` & `loe_simp_app_fw-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.4/LICENSE` & `loe_simp_app_fw-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.4/README.md` & `loe_simp_app_fw-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.4/PKG-INFO` & `loe_simp_app_fw-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: loe_simp_app_fw
-Version: 1.1.4
+Version: 1.2.0
 Summary: A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook.
 Project-URL: Homepage, https://github.com/loeeeee/loe-simp-app-fw
 Project-URL: Issues, https://github.com/loeeeee/loe-simp-app-fw/issues
 Author-email: loeeeee <95266635+loeeeee@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

