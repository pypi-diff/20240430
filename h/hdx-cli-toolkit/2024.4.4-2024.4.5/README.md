# Comparing `tmp/hdx_cli_toolkit-2024.4.4.tar.gz` & `tmp/hdx_cli_toolkit-2024.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdx_cli_toolkit-2024.4.4.tar", last modified: Mon Apr 29 07:42:06 2024, max compression
+gzip compressed data, was "hdx_cli_toolkit-2024.4.5.tar", last modified: Tue Apr 30 07:39:59 2024, max compression
```

## Comparing `hdx_cli_toolkit-2024.4.4.tar` & `hdx_cli_toolkit-2024.4.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:42:06.169075 hdx_cli_toolkit-2024.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-29 07:42:06.169075 hdx_cli_toolkit-2024.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 07:42:06.169075 hdx_cli_toolkit-2024.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:42:06.165075 hdx_cli_toolkit-2024.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:42:06.165075 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit/hdx_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    10036 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:42:06.169075 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-29 07:42:06.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-29 07:42:06.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:42:06.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-29 07:42:06.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-29 07:42:06.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 07:42:06.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:42:06.169075 hdx_cli_toolkit-2024.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/tests/test_cli_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/tests/test_hdx_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     7066 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/tests/test_hdx_utilities_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:39:59.341190 hdx_cli_toolkit-2024.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-30 07:39:40.000000 hdx_cli_toolkit-2024.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-30 07:39:59.341190 hdx_cli_toolkit-2024.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-30 07:39:40.000000 hdx_cli_toolkit-2024.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-30 07:39:40.000000 hdx_cli_toolkit-2024.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 07:39:59.341190 hdx_cli_toolkit-2024.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-30 07:39:40.000000 hdx_cli_toolkit-2024.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:39:59.337190 hdx_cli_toolkit-2024.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:39:59.337190 hdx_cli_toolkit-2024.4.5/src/hdx_cli_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:39:40.000000 hdx_cli_toolkit-2024.4.5/src/hdx_cli_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-30 07:39:40.000000 hdx_cli_toolkit-2024.4.5/src/hdx_cli_toolkit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20200 2024-04-30 07:39:40.000000 hdx_cli_toolkit-2024.4.5/src/hdx_cli_toolkit/hdx_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10036 2024-04-30 07:39:40.000000 hdx_cli_toolkit-2024.4.5/src/hdx_cli_toolkit/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:39:59.341190 hdx_cli_toolkit-2024.4.5/src/hdx_cli_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-30 07:39:59.000000 hdx_cli_toolkit-2024.4.5/src/hdx_cli_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-30 07:39:59.000000 hdx_cli_toolkit-2024.4.5/src/hdx_cli_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 07:39:59.000000 hdx_cli_toolkit-2024.4.5/src/hdx_cli_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-30 07:39:59.000000 hdx_cli_toolkit-2024.4.5/src/hdx_cli_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-30 07:39:59.000000 hdx_cli_toolkit-2024.4.5/src/hdx_cli_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 07:39:59.000000 hdx_cli_toolkit-2024.4.5/src/hdx_cli_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:39:59.341190 hdx_cli_toolkit-2024.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-30 07:39:40.000000 hdx_cli_toolkit-2024.4.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-30 07:39:40.000000 hdx_cli_toolkit-2024.4.5/tests/test_cli_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-30 07:39:40.000000 hdx_cli_toolkit-2024.4.5/tests/test_hdx_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-04-30 07:39:40.000000 hdx_cli_toolkit-2024.4.5/tests/test_hdx_utilities_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-30 07:39:40.000000 hdx_cli_toolkit-2024.4.5/tests/test_utilities.py
```

### Comparing `hdx_cli_toolkit-2024.4.4/LICENSE` & `hdx_cli_toolkit-2024.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.4/PKG-INFO` & `hdx_cli_toolkit-2024.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx_cli_toolkit
-Version: 2024.4.4
+Version: 2024.4.5
 Summary: HDX CLI tool kit for commandline interaction with HDX
 Author: Ian Hopkinson
 Author-email: ian.hopkinson@un.org
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Ian Hopkinson
```

### Comparing `hdx_cli_toolkit-2024.4.4/README.md` & `hdx_cli_toolkit-2024.4.5/README.md`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.4/pyproject.toml` & `hdx_cli_toolkit-2024.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hdx_cli_toolkit"
-version = "2024.4.4"
+version = "2024.4.5"
 description = "HDX CLI tool kit for commandline interaction with HDX"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 requires-python = ">=3.11"
 authors = [
   {email = "ian.hopkinson@un.org"},
   {name = "Ian Hopkinson"}
```

### Comparing `hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit/cli.py` & `hdx_cli_toolkit-2024.4.5/src/hdx_cli_toolkit/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,14 +188,16 @@
         )
 
         if len(filtered_datasets) == 0:
             print("Specified filter returns no datasets", flush=True)
             return
 
         print(f"Updating key '{key}' with value '{value}'")
+        conversion_func = None
+        type_name = ""
         for filtered_dataset in filtered_datasets:
             try:
                 conversion_func, type_name = make_conversion_func(filtered_dataset[key])
             except KeyError:
                 continue
 
         if conversion_func is None:
```

### Comparing `hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit/hdx_utilities.py` & `hdx_cli_toolkit-2024.4.5/src/hdx_cli_toolkit/hdx_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import os
 import time
 import traceback
 import urllib3
 
 from pathlib import Path
 
+import ckanapi
 import click
 import urllib3.util
 import yaml
 
 from hdx.api.configuration import Configuration, ConfigurationError
 from hdx.data.organization import Organization
 from hdx.data.resource_view import ResourceView
@@ -35,39 +36,39 @@
 
 
 def hdx_error_handler(f):
     @functools.wraps(f)
     def inner(*args, **kwargs):
         try:
             return f(*args, **kwargs)
-        except HDXError:
-            message = parse_hdxerror_traceback(traceback.format_exc())
-            if message == "unknown":
+        except (HDXError, ckanapi.errors.ValidationError):
+            traceback_message = traceback.format_exc()
+            message = parse_hdxerror_traceback(traceback_message)
+            if message != "unknown":
                 click.secho(
                     f"Could not perform operation on HDX because of an `{message}`",
                     fg="red",
                     color=True,
                 )
             else:
-                print(traceback.format_exc)
+                print(traceback_message, flush=True)
 
     return inner
 
 
 def parse_hdxerror_traceback(traceback_message: str):
     message = "unknown"
-    if "Authorization Error" in traceback.format_exc():
+    if "Authorization Error" in traceback_message:
         message = "Authorization Error"
-    elif (
-        "{'extras': [{}, {'key': ['There is a schema field with the same name']}]"
-        in traceback.format_exc()
-    ):
+    elif "extras" in traceback_message:
         message = "Extras Key Error"
-    elif "KeyError: 'resources'" in traceback.format_exc():
+    elif "KeyError: 'resources'" in traceback_message:
         message = "No Resources Error"
+    elif "{'dataset_date': ['Invalid old HDX date" in traceback_message:
+        message = "Invalid Dataset Date Error"
 
     return message
 
 
 @hdx_error_handler
 def get_filtered_datasets(
     organization: str = "",
@@ -187,15 +188,15 @@
     status = write_dictionary(output_path, output_rows, append=False)
     print(status, flush=True)
 
     print(f"Changed {n_changed} values", flush=True)
     print(f"{n_failures} failures as evidenced by HDXError", flush=True)
 
 
-@hdx_error_handler
+# This function does its own error handling for hdx, so no @hdx_error_handler
 def update_values_in_hdx(
     filtered_datasets: list[Dataset], key, value, conversion_func, hdx_site: str = "stage"
 ):
     n_changed = 0
     n_failures = 0
     row_template = {
         "dataset_name": None,
@@ -215,17 +216,15 @@
         dataset[key] = new_value
 
         row = row_template.copy()
         row["dataset_name"] = dataset["name"]
         row["old_value"] = old_value
         row["new_value"] = new_value
 
-        if old_value != str(dataset[key]):
-            n_changed += 1
-        else:
+        if old_value == str(dataset[key]):
             message = "No update required"
             print(
                 f"{dataset['name']:<70.70}{old_value:<20.20}{str(dataset[key]):<20.20} "
                 f"{message:<25.25}",
                 flush=True,
             )
             row["message"] = message
@@ -246,15 +245,16 @@
             print(
                 f"{dataset['name']:<70.70}{old_value:<20.20}{str(dataset[key]):<20.20} "
                 f"{message}",
                 flush=True,
             )
             row["message"] = message
             output_rows.append(row)
-        except (HDXError, KeyError):
+            n_changed += 1
+        except (HDXError, KeyError, ckanapi.errors.ValidationError):
             traceback_message = parse_hdxerror_traceback(traceback.format_exc())
             message = f"Could not update {dataset['name']} on '{hdx_site}' - {traceback_message}"
             n_failures += 1
 
             print(
                 f"{dataset['name']:<70.70}{old_value:<20.20}{old_value:<20.20} {message}",
                 flush=True,
```

### Comparing `hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit/utilities.py` & `hdx_cli_toolkit-2024.4.5/src/hdx_cli_toolkit/utilities.py`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit.egg-info/PKG-INFO` & `hdx_cli_toolkit-2024.4.5/src/hdx_cli_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx_cli_toolkit
-Version: 2024.4.4
+Version: 2024.4.5
 Summary: HDX CLI tool kit for commandline interaction with HDX
 Author: Ian Hopkinson
 Author-email: ian.hopkinson@un.org
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Ian Hopkinson
```

### Comparing `hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit.egg-info/SOURCES.txt` & `hdx_cli_toolkit-2024.4.5/src/hdx_cli_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.4/tests/test_cli.py` & `hdx_cli_toolkit-2024.4.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.4/tests/test_cli_integration.py` & `hdx_cli_toolkit-2024.4.5/tests/test_cli_integration.py`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.4/tests/test_hdx_utilities.py` & `hdx_cli_toolkit-2024.4.5/tests/test_hdx_utilities.py`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.4/tests/test_hdx_utilities_integration.py` & `hdx_cli_toolkit-2024.4.5/tests/test_hdx_utilities_integration.py`

 * *Files 16% similar despite different names*

```diff
@@ -211,7 +211,31 @@
 
 
 def test_update_values_in_hdx_from_file():
     update_file_path = os.path.join(os.path.dirname(__file__), "fixtures", "update-from-file.csv")
     update_values_in_hdx_from_file(HDX_SITE, update_file_path)
     dataset = Dataset.read_from_hdx(DATASET_NAME)
     assert dataset["caveats"] == "Second value from_file"
+
+    redo_file_path = os.path.join(
+        os.path.dirname(__file__), "fixtures", "update-from-file-redo.csv"
+    )
+    assert os.path.exists(redo_file_path)
+    if os.path.exists(redo_file_path):
+        os.remove(redo_file_path)
+
+
+def test_error_handling(capfd):
+    dataset = Dataset.read_from_hdx(DATASET_NAME)
+    key = "extras"
+    value = "Extras key is illegal"
+    conversion_func, _ = make_conversion_func(value)
+    n_changed, n_failures, output_rows = update_values_in_hdx(
+        [dataset], key, value, conversion_func, hdx_site=HDX_SITE
+    )
+
+    assert n_changed == 0
+    assert n_failures == 1
+    assert len(output_rows) == 1
+    output, _ = capfd.readouterr()
+
+    assert "Could not update hdx_cli_toolkit_test on 'stage' - Extras Key Error" in output
```

### Comparing `hdx_cli_toolkit-2024.4.4/tests/test_utilities.py` & `hdx_cli_toolkit-2024.4.5/tests/test_utilities.py`

 * *Files identical despite different names*

