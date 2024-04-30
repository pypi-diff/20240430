# Comparing `tmp/zpodcli-0.5.0.tar.gz` & `tmp/zpodcli-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpodcli-0.5.0.tar", max compression
+gzip compressed data, was "zpodcli-0.6.0.tar", max compression
```

## Comparing `zpodcli-0.5.0.tar` & `zpodcli-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0      519 2024-03-13 08:43:24.396297 zpodcli-0.5.0/README.md
--rw-r--r--   0        0        0      613 2024-03-26 15:19:21.072381 zpodcli-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-03-26 15:19:02.734847 zpodcli-0.5.0/src/zpodcli/__init__.py
--rw-r--r--   0        0        0     4595 2024-03-25 18:36:05.584858 zpodcli-0.5.0/src/zpodcli/cmd/component_cli.py
--rw-r--r--   0        0        0     1408 2024-03-25 18:36:05.584858 zpodcli-0.5.0/src/zpodcli/cmd/endpoint_cli.py
--rw-r--r--   0        0        0     5197 2024-03-25 18:36:05.588859 zpodcli-0.5.0/src/zpodcli/cmd/endpoint_permission_cli.py
--rw-r--r--   0        0        0     2548 2024-03-25 18:36:05.588859 zpodcli-0.5.0/src/zpodcli/cmd/enet_cli.py
--rw-r--r--   0        0        0     5367 2024-03-25 18:36:05.588859 zpodcli-0.5.0/src/zpodcli/cmd/factory_cli.py
--rw-r--r--   0        0        0     5160 2024-03-25 18:36:05.588859 zpodcli-0.5.0/src/zpodcli/cmd/library_cli.py
--rw-r--r--   0        0        0     3272 2024-03-25 18:36:05.588859 zpodcli-0.5.0/src/zpodcli/cmd/permission_group_cli.py
--rw-r--r--   0        0        0     1960 2024-03-25 18:36:05.588859 zpodcli-0.5.0/src/zpodcli/cmd/permission_group_user_cli.py
--rw-r--r--   0        0        0     7434 2024-03-25 18:36:05.588859 zpodcli-0.5.0/src/zpodcli/cmd/profile_cli.py
--rw-r--r--   0        0        0     2128 2024-03-25 18:36:05.588859 zpodcli-0.5.0/src/zpodcli/cmd/setting_cli.py
--rw-r--r--   0        0        0     5447 2024-03-25 18:36:05.588859 zpodcli-0.5.0/src/zpodcli/cmd/user_cli.py
--rw-r--r--   0        0        0     5243 2024-03-21 09:35:36.945672 zpodcli-0.5.0/src/zpodcli/cmd/zpod_cli.py
--rw-r--r--   0        0        0     5418 2024-03-21 09:35:36.945672 zpodcli-0.5.0/src/zpodcli/cmd/zpod_component_cli.py
--rw-r--r--   0        0        0     5611 2024-03-21 09:35:36.945672 zpodcli-0.5.0/src/zpodcli/cmd/zpod_permission_cli.py
--rw-r--r--   0        0        0     2409 2024-03-16 19:57:43.866064 zpodcli-0.5.0/src/zpodcli/lib/factory_config.py
--rw-r--r--   0        0        0       40 2024-03-12 19:46:50.044513 zpodcli-0.5.0/src/zpodcli/lib/global_flags.py
--rw-r--r--   0        0        0      547 2024-02-05 12:29:58.596820 zpodcli-0.5.0/src/zpodcli/lib/utils.py
--rw-r--r--   0        0        0     2696 2024-03-21 09:35:36.945672 zpodcli-0.5.0/src/zpodcli/lib/zpod_client.py
--rw-r--r--   0        0        0     1750 2024-03-21 09:35:36.945672 zpodcli-0.5.0/src/zpodcli/main_cli.py
--rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 zpodcli-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      519 2024-03-13 14:21:21.635846 zpodcli-0.6.0/README.md
+-rw-r--r--   0        0        0      613 2024-04-30 17:04:56.153887 zpodcli-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-30 17:04:45.121879 zpodcli-0.6.0/src/zpodcli/__init__.py
+-rw-r--r--   0        0        0     4595 2024-03-25 13:13:27.045284 zpodcli-0.6.0/src/zpodcli/cmd/component_cli.py
+-rw-r--r--   0        0        0    13037 2024-04-30 16:57:22.313577 zpodcli-0.6.0/src/zpodcli/cmd/endpoint_cli.py
+-rw-r--r--   0        0        0     5184 2024-04-15 14:23:40.295079 zpodcli-0.6.0/src/zpodcli/cmd/endpoint_permission_cli.py
+-rw-r--r--   0        0        0     2548 2024-03-25 13:13:27.045284 zpodcli-0.6.0/src/zpodcli/cmd/enet_cli.py
+-rw-r--r--   0        0        0     5367 2024-03-25 13:13:27.045284 zpodcli-0.6.0/src/zpodcli/cmd/factory_cli.py
+-rw-r--r--   0        0        0     5160 2024-03-25 13:13:27.045284 zpodcli-0.6.0/src/zpodcli/cmd/library_cli.py
+-rw-r--r--   0        0        0     3272 2024-03-25 13:13:27.045284 zpodcli-0.6.0/src/zpodcli/cmd/permission_group_cli.py
+-rw-r--r--   0        0        0     1960 2024-03-25 13:13:27.045284 zpodcli-0.6.0/src/zpodcli/cmd/permission_group_user_cli.py
+-rw-r--r--   0        0        0     7518 2024-04-15 14:23:40.295079 zpodcli-0.6.0/src/zpodcli/cmd/profile_cli.py
+-rw-r--r--   0        0        0     2128 2024-03-25 13:13:27.045284 zpodcli-0.6.0/src/zpodcli/cmd/setting_cli.py
+-rw-r--r--   0        0        0     5447 2024-03-25 13:13:27.045284 zpodcli-0.6.0/src/zpodcli/cmd/user_cli.py
+-rw-r--r--   0        0        0     5243 2024-03-20 17:51:37.453853 zpodcli-0.6.0/src/zpodcli/cmd/zpod_cli.py
+-rw-r--r--   0        0        0     5419 2024-04-15 14:23:40.295079 zpodcli-0.6.0/src/zpodcli/cmd/zpod_component_cli.py
+-rw-r--r--   0        0        0     5611 2024-03-20 17:51:37.453853 zpodcli-0.6.0/src/zpodcli/cmd/zpod_permission_cli.py
+-rw-r--r--   0        0        0     2409 2024-03-19 13:51:03.280476 zpodcli-0.6.0/src/zpodcli/lib/factory_config.py
+-rw-r--r--   0        0        0      624 2024-04-15 14:23:40.295079 zpodcli-0.6.0/src/zpodcli/lib/file.py
+-rw-r--r--   0        0        0       40 2024-03-12 19:29:59.732397 zpodcli-0.6.0/src/zpodcli/lib/global_flags.py
+-rw-r--r--   0        0        0     1006 2024-04-15 14:23:40.295079 zpodcli-0.6.0/src/zpodcli/lib/prompt.py
+-rw-r--r--   0        0        0      422 2024-04-15 14:23:40.295079 zpodcli-0.6.0/src/zpodcli/lib/utils.py
+-rw-r--r--   0        0        0     2696 2024-04-15 14:23:40.295079 zpodcli-0.6.0/src/zpodcli/lib/zpod_client.py
+-rw-r--r--   0        0        0     1750 2024-03-20 17:51:37.545861 zpodcli-0.6.0/src/zpodcli/main_cli.py
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 zpodcli-0.6.0/PKG-INFO
```

### Comparing `zpodcli-0.5.0/README.md` & `zpodcli-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `zpodcli-0.5.0/pyproject.toml` & `zpodcli-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "zpodcli"
-version = "0.5.0"
+version = "0.6.0"
 description = ""
 authors = ["Timo Sugliani <timo.sugliani@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "zpodcli", from = "src"}]
 
 [tool.poetry.scripts]
 zcli = "zpodcli.main_cli:launch"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.6.3"
 typer = {extras = ["all"], version = "0.10.0"}
 #zpodsdk = {path = "../zpodsdk", develop = true}
-zpodsdk = "0.5.0"
+zpodsdk = "0.6.0"
 pyyaml = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3"
 ipython = "^8.9.0"
```

### Comparing `zpodcli-0.5.0/src/zpodcli/cmd/component_cli.py` & `zpodcli-0.6.0/src/zpodcli/cmd/component_cli.py`

 * *Files identical despite different names*

### Comparing `zpodcli-0.5.0/src/zpodcli/cmd/endpoint_permission_cli.py` & `zpodcli-0.6.0/src/zpodcli/cmd/endpoint_permission_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 class EndpointPermission(str, Enum):
     USER = "USER"
 
 
 app = typer.Typer(
-    help="Manage zPods Endpoint Permissions",
+    help="Endpoint Permissions",
     no_args_is_help=True,
 )
 
 console = Console()
 
 
 def generate_table(
```

### Comparing `zpodcli-0.5.0/src/zpodcli/cmd/enet_cli.py` & `zpodcli-0.6.0/src/zpodcli/cmd/enet_cli.py`

 * *Files identical despite different names*

### Comparing `zpodcli-0.5.0/src/zpodcli/cmd/factory_cli.py` & `zpodcli-0.6.0/src/zpodcli/cmd/factory_cli.py`

 * *Files identical despite different names*

### Comparing `zpodcli-0.5.0/src/zpodcli/cmd/library_cli.py` & `zpodcli-0.6.0/src/zpodcli/cmd/library_cli.py`

 * *Files identical despite different names*

### Comparing `zpodcli-0.5.0/src/zpodcli/cmd/permission_group_cli.py` & `zpodcli-0.6.0/src/zpodcli/cmd/permission_group_cli.py`

 * *Files identical despite different names*

### Comparing `zpodcli-0.5.0/src/zpodcli/cmd/permission_group_user_cli.py` & `zpodcli-0.6.0/src/zpodcli/cmd/permission_group_user_cli.py`

 * *Files identical despite different names*

### Comparing `zpodcli-0.5.0/src/zpodcli/cmd/profile_cli.py` & `zpodcli-0.6.0/src/zpodcli/cmd/profile_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
 from pathlib import Path
 from typing import Optional
 
 import typer
-import yaml
 from rich import print
+from rich.json import JSON
 from rich.table import Table
 from typing_extensions import Annotated
 
+from zpodcli.lib.file import load_json_or_yaml_file
 from zpodcli.lib.utils import exit_with_error
 from zpodcli.lib.zpod_client import ZpodClient, unexpected_status_handler
 from zpodsdk.models.profile_create import ProfileCreate
 from zpodsdk.models.profile_item_create import ProfileItemCreate
 from zpodsdk.models.profile_item_update import ProfileItemUpdate
 from zpodsdk.models.profile_update import ProfileUpdate
 
@@ -89,32 +90,32 @@
     ] = False,
 ):
     """
     Profile Info
     """
     z: ZpodClient = ZpodClient()
     profile = z.profiles_get.sync(id=f"name={profile_name}")
-
     if json_:
-        print(json.dumps(profile.to_dict()["profile"]))
+        profile_dict = profile.to_dict()["profile"]
+        print(JSON.from_data(profile_dict, sort_keys=True))
     else:
         print(generate_table([profile], "Info"))
 
 
 @app.command(name="create", no_args_is_help=True)
 @unexpected_status_handler
 def profile_create(
     profile_name: Annotated[
         str,
         typer.Argument(
             help="Profile name",
             show_default=False,
         ),
     ],
-    profile: Annotated[
+    profile_str: Annotated[
         Optional[str],
         typer.Option(
             "--profile",
             "-p",
             help="Profile json",
             show_default=False,
         ),
@@ -128,26 +129,28 @@
             show_default=False,
         ),
     ] = None,
 ):
     """
     Profile Create
     """
-    if not profile_file and not profile:
+    if not profile_file and not profile_str:
         exit_with_error("Must have either profile file or profile")
-    if profile_file and profile:
+    if profile_file and profile_str:
         exit_with_error("Can not have both profile file and profile")
 
     if profile_file:
-        profile_obj = load_profile_file(profile_file)
-    elif profile:
-        profile_obj = json.loads(profile)
+        profile_obj = load_json_or_yaml_file(profile_file)
+    else:
+        try:
+            profile_obj = json.loads(profile_str)
+        except json.JSONDecodeError:
+            exit_with_error("Invalid JSON")
 
     z: ZpodClient = ZpodClient()
-
     z.profiles_create.sync(
         body=ProfileCreate(
             name=profile_name,
             profile=build_profile(profile_obj),
         )
     )
 
@@ -193,27 +196,29 @@
 ):
     """
     Profile Update
     """
     if profile_file and profile:
         exit_with_error("Can not have both profile file and profile")
 
+    z: ZpodClient = ZpodClient()
+    if not profile_file and not profile and not newname:
+        exit_with_error("No changes provided")
+
     profile_update = ProfileUpdate()
     if newname and newname != profile_name:
         profile_update.name = newname
 
     if profile_file:
-        profile_obj = load_profile_file(profile_file)
+        profile_obj = load_json_or_yaml_file(profile_file)
         profile_update.profile = build_profile(profile_obj, False)
     elif profile:
         profile_obj = json.loads(profile)
         profile_update.profile = build_profile(profile_obj, False)
 
-    z: ZpodClient = ZpodClient()
-
     z.profiles_update.sync(
         id=f"name={profile_name}",
         body=profile_update,
     )
     print(f"Profile [magenta]{profile_name}[/magenta] has been updated.")
 
 
@@ -232,23 +237,14 @@
     Profile Delete
     """
     z: ZpodClient = ZpodClient()
     z.profiles_delete.sync(id=f"name={profile_name}")
     print(f"Profile [magenta]{profile_name}[/magenta] has been deleted successfully")
 
 
-def load_profile_file(profile_file):
-    extension = profile_file.suffix
-    with profile_file.open() as f:
-        if extension in (".yaml", ".yml"):
-            return yaml.safe_load(f)
-        elif extension == ".json":
-            return json.load(f)
-
-
 def build_profile(profile_obj, is_create=True):
     profile_objects = []
     for profile_item in profile_obj:
         if isinstance(profile_item, list):
             item = [
                 parse_profile_item(sub_profile_item)
                 for sub_profile_item in profile_item
```

### Comparing `zpodcli-0.5.0/src/zpodcli/cmd/setting_cli.py` & `zpodcli-0.6.0/src/zpodcli/cmd/setting_cli.py`

 * *Files identical despite different names*

### Comparing `zpodcli-0.5.0/src/zpodcli/cmd/user_cli.py` & `zpodcli-0.6.0/src/zpodcli/cmd/user_cli.py`

 * *Files identical despite different names*

### Comparing `zpodcli-0.5.0/src/zpodcli/cmd/zpod_cli.py` & `zpodcli-0.6.0/src/zpodcli/cmd/zpod_cli.py`

 * *Files identical despite different names*

### Comparing `zpodcli-0.5.0/src/zpodcli/cmd/zpod_component_cli.py` & `zpodcli-0.6.0/src/zpodcli/cmd/zpod_component_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import typer
 from rich import print
 from rich.console import Console
 from rich.table import Table
 from typing_extensions import Annotated
 
-from zpodcli.lib.utils import confirm
+from zpodcli.lib.prompt import confirm
 from zpodcli.lib.zpod_client import ZpodClient, unexpected_status_handler
 from zpodsdk.models.zpod_component_create import ZpodComponentCreate
 from zpodsdk.models.zpod_component_view import ZpodComponentView
 from zpodsdk.models.zpod_view import ZpodView
 
 app = typer.Typer(help="Manage zPod Components", no_args_is_help=True)
```

### Comparing `zpodcli-0.5.0/src/zpodcli/cmd/zpod_permission_cli.py` & `zpodcli-0.6.0/src/zpodcli/cmd/zpod_permission_cli.py`

 * *Files identical despite different names*

### Comparing `zpodcli-0.5.0/src/zpodcli/lib/factory_config.py` & `zpodcli-0.6.0/src/zpodcli/lib/factory_config.py`

 * *Files identical despite different names*

### Comparing `zpodcli-0.5.0/src/zpodcli/lib/zpod_client.py` & `zpodcli-0.6.0/src/zpodcli/lib/zpod_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 f"    pip install zpodcli=={expected_version}\n"
             )
         elif status_code == 422:
             messages = [
                 rf"{error['msg']} \[{', '.join(error['loc'][1:])}]"
                 for error in content_json["detail"]
             ]
-            exit_with_error("  \n".join(messages))
+            exit_with_error("\n  ".join(messages))
         else:
             exit_with_error(f"{content_json['detail']} [{status_code}]")
     elif 500 <= status_code < 600:
         exit_with_error(f"{content} [{status_code}]")
 
 
 def unexpected_status_handler(func):
```

### Comparing `zpodcli-0.5.0/src/zpodcli/main_cli.py` & `zpodcli-0.6.0/src/zpodcli/main_cli.py`

 * *Files identical despite different names*

### Comparing `zpodcli-0.5.0/PKG-INFO` & `zpodcli-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: zpodcli
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 License: MIT
 Author: Timo Sugliani
 Author-email: timo.sugliani@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (==2.6.3)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: typer[all] (==0.10.0)
-Requires-Dist: zpodsdk (==0.5.0)
+Requires-Dist: zpodsdk (==0.6.0)
 Description-Content-Type: text/markdown
 
 # zPodFactory CLI
 
 `zcli` is a command line interface for zPodFactory. It is used to create, manage and deploy zPods.
 
 The documentation for `zcli` is available on the main zPodFactory website: https://zpodfactory.github.io
```

