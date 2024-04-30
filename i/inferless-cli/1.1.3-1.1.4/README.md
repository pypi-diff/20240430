# Comparing `tmp/inferless_cli-1.1.3.tar.gz` & `tmp/inferless_cli-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inferless_cli-1.1.3.tar", max compression
+gzip compressed data, was "inferless_cli-1.1.4.tar", max compression
```

## Comparing `inferless_cli-1.1.3.tar` & `inferless_cli-1.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    10052 2024-04-29 12:49:54.154706 inferless_cli-1.1.3/README.md
--rw-r--r--   0        0        0       37 2024-04-29 12:49:54.155009 inferless_cli-1.1.3/inferless_cli/__init__.py
--rw-r--r--   0        0        0       50 2024-03-13 03:52:17.953547 inferless_cli-1.1.3/inferless_cli/__main__.py
--rw-r--r--   0        0        0     7282 2024-04-29 12:49:54.155402 inferless_cli-1.1.3/inferless_cli/main.py
--rw-r--r--   0        0        0        0 2024-03-13 03:51:47.516671 inferless_cli-1.1.3/inferless_cli/prompts/__init__.py
--rw-r--r--   0        0        0    23068 2024-04-29 12:49:54.155748 inferless_cli-1.1.3/inferless_cli/prompts/deploy.py
--rw-r--r--   0        0        0     1802 2024-04-29 12:49:54.156043 inferless_cli-1.1.3/inferless_cli/prompts/export.py
--rw-r--r--   0        0        0    11391 2024-04-29 12:49:54.156678 inferless_cli-1.1.3/inferless_cli/prompts/init.py
--rw-r--r--   0        0        0     3779 2024-04-29 12:49:54.157030 inferless_cli-1.1.3/inferless_cli/prompts/log.py
--rw-r--r--   0        0        0      854 2024-03-13 03:51:54.338936 inferless_cli-1.1.3/inferless_cli/prompts/login.py
--rw-r--r--   0        0        0    15846 2024-04-29 12:49:54.157620 inferless_cli-1.1.3/inferless_cli/prompts/model.py
--rw-r--r--   0        0        0    18882 2024-04-29 12:49:54.157892 inferless_cli-1.1.3/inferless_cli/prompts/run.py
--rw-r--r--   0        0        0     5984 2024-04-29 12:49:54.158229 inferless_cli-1.1.3/inferless_cli/prompts/runtime.py
--rw-r--r--   0        0        0     2026 2024-04-29 12:49:54.158392 inferless_cli-1.1.3/inferless_cli/prompts/secret.py
--rw-r--r--   0        0        0     4231 2024-04-29 12:49:54.158770 inferless_cli-1.1.3/inferless_cli/prompts/token.py
--rw-r--r--   0        0        0    22319 2024-04-29 12:49:54.159108 inferless_cli-1.1.3/inferless_cli/prompts/volume.py
--rw-r--r--   0        0        0     1699 2024-04-29 12:49:54.159427 inferless_cli-1.1.3/inferless_cli/prompts/workspace.py
--rw-r--r--   0        0        0        0 2024-03-13 03:52:07.884835 inferless_cli-1.1.3/inferless_cli/utils/__init__.py
--rw-r--r--   0        0        0     2870 2024-04-29 12:49:54.159619 inferless_cli-1.1.3/inferless_cli/utils/api.py
--rw-r--r--   0        0        0    14752 2024-04-29 12:49:54.160026 inferless_cli-1.1.3/inferless_cli/utils/constants.py
--rw-r--r--   0        0        0     1068 2024-04-29 12:49:54.160238 inferless_cli-1.1.3/inferless_cli/utils/convertors.py
--rw-r--r--   0        0        0     7179 2024-04-29 12:49:54.160563 inferless_cli-1.1.3/inferless_cli/utils/credentials.py
--rw-r--r--   0        0        0    28795 2024-04-29 12:49:54.160943 inferless_cli-1.1.3/inferless_cli/utils/helpers.py
--rw-r--r--   0        0        0    26839 2024-04-29 12:49:54.161332 inferless_cli-1.1.3/inferless_cli/utils/services.py
--rw-r--r--   0        0        0     7065 2024-03-13 03:52:15.076191 inferless_cli-1.1.3/inferless_cli/utils/validators.py
--rw-r--r--   0        0        0      671 2024-04-29 12:49:54.162514 inferless_cli-1.1.3/pyproject.toml
--rw-r--r--   0        0        0    11065 1970-01-01 00:00:00.000000 inferless_cli-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0    10052 2024-04-29 12:49:54.154706 inferless_cli-1.1.4/README.md
+-rw-r--r--   0        0        0       37 2024-04-29 17:44:53.904701 inferless_cli-1.1.4/inferless_cli/__init__.py
+-rw-r--r--   0        0        0       50 2024-03-13 03:52:17.953547 inferless_cli-1.1.4/inferless_cli/__main__.py
+-rw-r--r--   0        0        0     7282 2024-04-29 12:49:54.155402 inferless_cli-1.1.4/inferless_cli/main.py
+-rw-r--r--   0        0        0        0 2024-03-13 03:51:47.516671 inferless_cli-1.1.4/inferless_cli/prompts/__init__.py
+-rw-r--r--   0        0        0    23068 2024-04-29 12:49:54.155748 inferless_cli-1.1.4/inferless_cli/prompts/deploy.py
+-rw-r--r--   0        0        0     1802 2024-04-29 12:49:54.156043 inferless_cli-1.1.4/inferless_cli/prompts/export.py
+-rw-r--r--   0        0        0    11391 2024-04-29 12:49:54.156678 inferless_cli-1.1.4/inferless_cli/prompts/init.py
+-rw-r--r--   0        0        0     3779 2024-04-29 12:49:54.157030 inferless_cli-1.1.4/inferless_cli/prompts/log.py
+-rw-r--r--   0        0        0      854 2024-03-13 03:51:54.338936 inferless_cli-1.1.4/inferless_cli/prompts/login.py
+-rw-r--r--   0        0        0    15846 2024-04-29 12:49:54.157620 inferless_cli-1.1.4/inferless_cli/prompts/model.py
+-rw-r--r--   0        0        0    18882 2024-04-29 12:49:54.157892 inferless_cli-1.1.4/inferless_cli/prompts/run.py
+-rw-r--r--   0        0        0     5984 2024-04-29 12:49:54.158229 inferless_cli-1.1.4/inferless_cli/prompts/runtime.py
+-rw-r--r--   0        0        0     2026 2024-04-29 12:49:54.158392 inferless_cli-1.1.4/inferless_cli/prompts/secret.py
+-rw-r--r--   0        0        0     4231 2024-04-29 12:49:54.158770 inferless_cli-1.1.4/inferless_cli/prompts/token.py
+-rw-r--r--   0        0        0    22378 2024-04-29 18:01:24.312203 inferless_cli-1.1.4/inferless_cli/prompts/volume.py
+-rw-r--r--   0        0        0     1699 2024-04-29 12:49:54.159427 inferless_cli-1.1.4/inferless_cli/prompts/workspace.py
+-rw-r--r--   0        0        0        0 2024-03-13 03:52:07.884835 inferless_cli-1.1.4/inferless_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2870 2024-04-29 12:49:54.159619 inferless_cli-1.1.4/inferless_cli/utils/api.py
+-rw-r--r--   0        0        0    14752 2024-04-29 12:49:54.160026 inferless_cli-1.1.4/inferless_cli/utils/constants.py
+-rw-r--r--   0        0        0     1068 2024-04-29 12:49:54.160238 inferless_cli-1.1.4/inferless_cli/utils/convertors.py
+-rw-r--r--   0        0        0     7179 2024-04-29 12:49:54.160563 inferless_cli-1.1.4/inferless_cli/utils/credentials.py
+-rw-r--r--   0        0        0    28795 2024-04-29 12:49:54.160943 inferless_cli-1.1.4/inferless_cli/utils/helpers.py
+-rw-r--r--   0        0        0    26839 2024-04-29 12:49:54.161332 inferless_cli-1.1.4/inferless_cli/utils/services.py
+-rw-r--r--   0        0        0     7065 2024-03-13 03:52:15.076191 inferless_cli-1.1.4/inferless_cli/utils/validators.py
+-rw-r--r--   0        0        0      671 2024-04-29 17:01:29.831621 inferless_cli-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0    11065 1970-01-01 00:00:00.000000 inferless_cli-1.1.4/PKG-INFO
```

### Comparing `inferless_cli-1.1.3/README.md` & `inferless_cli-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/inferless_cli/main.py` & `inferless_cli-1.1.4/inferless_cli/main.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/inferless_cli/prompts/deploy.py` & `inferless_cli-1.1.4/inferless_cli/prompts/deploy.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/inferless_cli/prompts/export.py` & `inferless_cli-1.1.4/inferless_cli/prompts/export.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/inferless_cli/prompts/init.py` & `inferless_cli-1.1.4/inferless_cli/prompts/init.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/inferless_cli/prompts/log.py` & `inferless_cli-1.1.4/inferless_cli/prompts/log.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/inferless_cli/prompts/login.py` & `inferless_cli-1.1.4/inferless_cli/prompts/login.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/inferless_cli/prompts/model.py` & `inferless_cli-1.1.4/inferless_cli/prompts/model.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/inferless_cli/prompts/run.py` & `inferless_cli-1.1.4/inferless_cli/prompts/run.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/inferless_cli/prompts/runtime.py` & `inferless_cli-1.1.4/inferless_cli/prompts/runtime.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/inferless_cli/prompts/secret.py` & `inferless_cli-1.1.4/inferless_cli/prompts/secret.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/inferless_cli/prompts/token.py` & `inferless_cli-1.1.4/inferless_cli/prompts/token.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/inferless_cli/prompts/volume.py` & `inferless_cli-1.1.4/inferless_cli/prompts/volume.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     get_workspaces_list,
     sync_s3_to_nfs,
     sync_s3_to_s3,
     get_volume_files,
     upload_file,
 )
 from inferless_cli.utils.validators import validate_region_types
+from pathlib import Path
 
 app = typer.Typer(
     no_args_is_help=True,
 )
 
 processing = "processing..."
 desc = "[progress.description]{task.description}"
@@ -549,24 +550,22 @@
     except Exception as e:
         rich.print(e)
         raise typer.Exit(1)
 
 
 def process_file(path: str, s3_path, root_path):
     try:
-        if root_path == path:
-            temp = os.path.basename(path)
+        unix_file_path = Path(path).as_posix()
+        unix_root_path = Path(root_path).as_posix()
+
+        if unix_root_path == unix_file_path:
             save_path = s3_path
         else:
-            if os.name == "nt":
-                temp = path.split(root_path)[-1].lstrip("\\")
-            else:
-                temp = path.split(root_path)[-1].lstrip("/")
-
-            save_path = f"{s3_path}/{temp}"
+            relative_path = unix_file_path[len(unix_root_path) :].lstrip("/")
+            save_path = f"{s3_path}/{relative_path}"
 
         if save_path.startswith("/"):
             save_path = save_path[1:]
         file_size = os.path.getsize(path)
 
         if file_size > 5 * 1024**3:  # File size is more than 5GB
             with open(path, "rb") as file:
@@ -596,16 +595,17 @@
         return True
 
 
 def process_directory(executor, dir_path: str, s3_path, root_path):
     futures = []
     for root, dirs, files in os.walk(dir_path):
         for file in files:
-            file_path = os.path.join(root, file)
-            future = executor.submit(process_file, file_path, s3_path, root_path)
+            file_path = Path(root) / file
+            unix_file_path = file_path.as_posix()
+            future = executor.submit(process_file, unix_file_path, s3_path, root_path)
             futures.append(future)
 
     return futures
 
 
 def extract_volume_info(input_string):
     # Splitting the URL by '/'
```

### Comparing `inferless_cli-1.1.3/inferless_cli/prompts/workspace.py` & `inferless_cli-1.1.4/inferless_cli/prompts/workspace.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/inferless_cli/utils/api.py` & `inferless_cli-1.1.4/inferless_cli/utils/api.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/inferless_cli/utils/constants.py` & `inferless_cli-1.1.4/inferless_cli/utils/constants.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/inferless_cli/utils/convertors.py` & `inferless_cli-1.1.4/inferless_cli/utils/convertors.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/inferless_cli/utils/credentials.py` & `inferless_cli-1.1.4/inferless_cli/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/inferless_cli/utils/helpers.py` & `inferless_cli-1.1.4/inferless_cli/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/inferless_cli/utils/services.py` & `inferless_cli-1.1.4/inferless_cli/utils/services.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/inferless_cli/utils/validators.py` & `inferless_cli-1.1.4/inferless_cli/utils/validators.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.3/pyproject.toml` & `inferless_cli-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inferless-cli"
-version = "1.1.3"
+version = "1.1.4"
 description = "Inferless - Deploy Machine Learning Models in Minutes."
 authors = ["Naveen <naveen@inferless.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 inferless = "inferless_cli.main:app"
```

### Comparing `inferless_cli-1.1.3/PKG-INFO` & `inferless_cli-1.1.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inferless-cli
-Version: 1.1.3
+Version: 1.1.4
 Summary: Inferless - Deploy Machine Learning Models in Minutes.
 Author: Naveen
 Author-email: naveen@inferless.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

