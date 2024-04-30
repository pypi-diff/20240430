# Comparing `tmp/pytvpaint-1.0.0b6.tar.gz` & `tmp/pytvpaint-1.0.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytvpaint-1.0.0b6.tar", max compression
+gzip compressed data, was "pytvpaint-1.0.0b7.tar", max compression
```

## Comparing `pytvpaint-1.0.0b6.tar` & `pytvpaint-1.0.0b7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1070 2024-04-22 16:20:48.841740 pytvpaint-1.0.0b6/LICENSE.md
--rw-r--r--   0        0        0     3515 2024-04-22 16:20:48.841740 pytvpaint-1.0.0b6/README.md
--rw-r--r--   0        0        0     2229 2024-04-22 16:20:48.849740 pytvpaint-1.0.0b6/pyproject.toml
--rw-r--r--   0        0        0     1233 2024-04-22 16:20:48.849740 pytvpaint-1.0.0b6/pytvpaint/__init__.py
--rw-r--r--   0        0        0     8570 2024-04-22 16:20:48.849740 pytvpaint-1.0.0b6/pytvpaint/camera.py
--rw-r--r--   0        0        0    33280 2024-04-22 16:20:48.849740 pytvpaint-1.0.0b6/pytvpaint/clip.py
--rw-r--r--   0        0        0      573 2024-04-22 16:20:48.849740 pytvpaint-1.0.0b6/pytvpaint/george/__init__.py
--rw-r--r--   0        0        0     4890 2024-04-22 16:20:48.849740 pytvpaint-1.0.0b6/pytvpaint/george/client/__init__.py
--rw-r--r--   0        0        0     9747 2024-04-22 16:20:48.849740 pytvpaint-1.0.0b6/pytvpaint/george/client/parse.py
--rw-r--r--   0        0        0     5389 2024-04-22 16:20:48.849740 pytvpaint-1.0.0b6/pytvpaint/george/client/rpc.py
--rw-r--r--   0        0        0      687 2024-04-22 16:20:48.849740 pytvpaint-1.0.0b6/pytvpaint/george/exceptions.py
--rw-r--r--   0        0        0    28228 2024-04-22 16:20:48.849740 pytvpaint-1.0.0b6/pytvpaint/george/grg_base.py
--rw-r--r--   0        0        0     2719 2024-04-22 16:20:48.849740 pytvpaint-1.0.0b6/pytvpaint/george/grg_camera.py
--rw-r--r--   0        0        0    19243 2024-04-22 16:20:48.849740 pytvpaint-1.0.0b6/pytvpaint/george/grg_clip.py
--rw-r--r--   0        0        0    31138 2024-04-22 16:20:48.849740 pytvpaint-1.0.0b6/pytvpaint/george/grg_layer.py
--rw-r--r--   0        0        0    14902 2024-04-22 16:20:48.849740 pytvpaint-1.0.0b6/pytvpaint/george/grg_project.py
--rw-r--r--   0        0        0     1189 2024-04-22 16:20:48.849740 pytvpaint-1.0.0b6/pytvpaint/george/grg_scene.py
--rw-r--r--   0        0        0    41808 2024-04-22 16:20:48.849740 pytvpaint-1.0.0b6/pytvpaint/layer.py
--rw-r--r--   0        0        0    23105 2024-04-22 16:20:48.853740 pytvpaint-1.0.0b6/pytvpaint/project.py
--rw-r--r--   0        0        0        0 2024-04-22 16:20:48.853740 pytvpaint-1.0.0b6/pytvpaint/py.typed
--rw-r--r--   0        0        0     4384 2024-04-22 16:20:48.853740 pytvpaint-1.0.0b6/pytvpaint/scene.py
--rw-r--r--   0        0        0     8745 2024-04-22 16:20:48.853740 pytvpaint-1.0.0b6/pytvpaint/sound.py
--rw-r--r--   0        0        0    17136 2024-04-22 16:20:48.853740 pytvpaint-1.0.0b6/pytvpaint/utils.py
--rw-r--r--   0        0        0     4420 1970-01-01 00:00:00.000000 pytvpaint-1.0.0b6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-30 10:31:39.746839 pytvpaint-1.0.0b7/LICENSE.md
+-rw-r--r--   0        0        0     3515 2024-04-30 10:31:39.746839 pytvpaint-1.0.0b7/README.md
+-rw-r--r--   0        0        0     2229 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pyproject.toml
+-rw-r--r--   0        0        0     1233 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/__init__.py
+-rw-r--r--   0        0        0     8570 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/camera.py
+-rw-r--r--   0        0        0    33490 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/clip.py
+-rw-r--r--   0        0        0      573 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/__init__.py
+-rw-r--r--   0        0        0     4890 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/client/__init__.py
+-rw-r--r--   0        0        0     9747 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/client/parse.py
+-rw-r--r--   0        0        0     5389 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/client/rpc.py
+-rw-r--r--   0        0        0      687 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/exceptions.py
+-rw-r--r--   0        0        0    28228 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/grg_base.py
+-rw-r--r--   0        0        0     2719 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/grg_camera.py
+-rw-r--r--   0        0        0    19188 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/grg_clip.py
+-rw-r--r--   0        0        0    31138 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/grg_layer.py
+-rw-r--r--   0        0        0    14902 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/grg_project.py
+-rw-r--r--   0        0        0     1189 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/grg_scene.py
+-rw-r--r--   0        0        0    41808 2024-04-30 10:31:39.758839 pytvpaint-1.0.0b7/pytvpaint/layer.py
+-rw-r--r--   0        0        0    23105 2024-04-30 10:31:39.758839 pytvpaint-1.0.0b7/pytvpaint/project.py
+-rw-r--r--   0        0        0        0 2024-04-30 10:31:39.758839 pytvpaint-1.0.0b7/pytvpaint/py.typed
+-rw-r--r--   0        0        0     4384 2024-04-30 10:31:39.758839 pytvpaint-1.0.0b7/pytvpaint/scene.py
+-rw-r--r--   0        0        0     8745 2024-04-30 10:31:39.758839 pytvpaint-1.0.0b7/pytvpaint/sound.py
+-rw-r--r--   0        0        0    17136 2024-04-30 10:31:39.758839 pytvpaint-1.0.0b7/pytvpaint/utils.py
+-rw-r--r--   0        0        0     4420 1970-01-01 00:00:00.000000 pytvpaint-1.0.0b7/PKG-INFO
```

### Comparing `pytvpaint-1.0.0b6/LICENSE.md` & `pytvpaint-1.0.0b7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b6/README.md` & `pytvpaint-1.0.0b7/README.md`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b6/pyproject.toml` & `pytvpaint-1.0.0b7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytvpaint"
-version = "1.0.0b6"
+version = "1.0.0b7"
 description = "Python scripting for TVPaint"
 authors = [
     "Brunch Studio Developers <dev@brunchstudio.tv>",
     "Radouane Lahmidi <rlahmidi@brunchstudio.tv>",
     "Joseph Henry <jhenry@brunchstudio.tv>",
 ]
 license = "MIT"
```

### Comparing `pytvpaint-1.0.0b6/pytvpaint/__init__.py` & `pytvpaint-1.0.0b7/pytvpaint/__init__.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b6/pytvpaint/camera.py` & `pytvpaint-1.0.0b7/pytvpaint/camera.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b6/pytvpaint/clip.py` & `pytvpaint-1.0.0b7/pytvpaint/clip.py`

 * *Files 1% similar despite different names*

```diff
@@ -554,23 +554,28 @@
 
         Raises:
             FileNotFoundError: if the export failed and no files were found on disk
         """
         export_path = Path(export_path)
         export_path.parent.mkdir(exist_ok=True, parents=True)
 
+        fill_background = bool(
+            background_mode not in [None, george.BackgroundMode.NONE]
+        )
+
         with utils.render_context(
             alpha_mode, background_mode, save_format, format_opts, layer_selection
         ):
             george.tv_clip_save_structure_json(
                 export_path,
                 save_format,
-                None,
-                folder_pattern,
-                file_pattern,
+                fill_background=fill_background,
+                folder_pattern=folder_pattern,
+                file_pattern=file_pattern,
+                visible_layers_only=True,
                 all_images=all_images,
                 ignore_duplicates=ignore_duplicates,
             )
 
         if not export_path.exists():
             raise FileNotFoundError(
                 f"Could not find output at : {export_path.as_posix()}"
```

### Comparing `pytvpaint-1.0.0b6/pytvpaint/george/__init__.py` & `pytvpaint-1.0.0b7/pytvpaint/george/__init__.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b6/pytvpaint/george/client/__init__.py` & `pytvpaint-1.0.0b7/pytvpaint/george/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b6/pytvpaint/george/client/parse.py` & `pytvpaint-1.0.0b7/pytvpaint/george/client/parse.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b6/pytvpaint/george/client/rpc.py` & `pytvpaint-1.0.0b7/pytvpaint/george/client/rpc.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b6/pytvpaint/george/exceptions.py` & `pytvpaint-1.0.0b7/pytvpaint/george/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b6/pytvpaint/george/grg_base.py` & `pytvpaint-1.0.0b7/pytvpaint/george/grg_base.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b6/pytvpaint/george/grg_camera.py` & `pytvpaint-1.0.0b7/pytvpaint/george/grg_camera.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b6/pytvpaint/george/grg_clip.py` & `pytvpaint-1.0.0b7/pytvpaint/george/grg_clip.py`

 * *Files 2% similar despite different names*

```diff
@@ -400,20 +400,20 @@
     export_path = Path(export_path).resolve()
     send_cmd("tv_SaveDisplay", export_path.as_posix())
 
 
 def tv_clip_save_structure_json(
     export_path: Path | str,
     file_format: SaveFormat,
-    fill_background: bool | None = None,
+    fill_background: bool = False,
     folder_pattern: str | None = None,
     file_pattern: str | None = None,
-    visible_layers_only: bool | None = None,
-    all_images: bool | None = None,
-    ignore_duplicates: bool | None = None,
+    visible_layers_only: bool = True,
+    all_images: bool = False,
+    ignore_duplicates: bool = False,
     exclude_instance_names: list[str] | None = None,
 ) -> None:
     """Save the current clip structure in json.
 
     Args:
         export_path: the JSON export path
         file_format: file format to use for rendering
@@ -438,25 +438,24 @@
     args = [export_path.as_posix(), "JSON"]
 
     dict_args = {
         "fileformat": file_format.value,
         "background": int(fill_background) if fill_background else None,
         "patternfolder": folder_pattern,
         "patternfile": file_pattern,
-        "onlyvisiblelayers": visible_layers_only,
-        "allimages": int(all_images) if all_images else None,
-        "ignoreduplicateimages": ignore_duplicates,
+        "onlyvisiblelayers": int(visible_layers_only),
+        "allimages": int(all_images),
+        "ignoreduplicateimages": int(ignore_duplicates),
         "excludenames": (
             ";".join(exclude_instance_names) if exclude_instance_names else None
         ),
     }
+    args.extend(args_dict_to_list(dict_args))
 
-    args_inline = args_dict_to_list(dict_args)
-
-    send_cmd("tv_ClipSaveStructure", *args, *args_inline, error_values=[-1])
+    send_cmd("tv_ClipSaveStructure", *args, error_values=[-1])
 
 
 def tv_clip_save_structure_psd(
     export_path: Path | str,
     mode: PSDSaveMode,
     image: int | None = None,
     mark_in: int | None = None,
```

### Comparing `pytvpaint-1.0.0b6/pytvpaint/george/grg_layer.py` & `pytvpaint-1.0.0b7/pytvpaint/george/grg_layer.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b6/pytvpaint/george/grg_project.py` & `pytvpaint-1.0.0b7/pytvpaint/george/grg_project.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b6/pytvpaint/george/grg_scene.py` & `pytvpaint-1.0.0b7/pytvpaint/george/grg_scene.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b6/pytvpaint/layer.py` & `pytvpaint-1.0.0b7/pytvpaint/layer.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b6/pytvpaint/project.py` & `pytvpaint-1.0.0b7/pytvpaint/project.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b6/pytvpaint/scene.py` & `pytvpaint-1.0.0b7/pytvpaint/scene.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b6/pytvpaint/sound.py` & `pytvpaint-1.0.0b7/pytvpaint/sound.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b6/pytvpaint/utils.py` & `pytvpaint-1.0.0b7/pytvpaint/utils.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b6/PKG-INFO` & `pytvpaint-1.0.0b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytvpaint
-Version: 1.0.0b6
+Version: 1.0.0b7
 Summary: Python scripting for TVPaint
 Home-page: https://github.com/brunchstudio/pytvpaint
 License: MIT
 Keywords: tvpaint,brunch,tvp,george
 Author: Brunch Studio Developers
 Author-email: dev@brunchstudio.tv
 Requires-Python: >=3.9
```

