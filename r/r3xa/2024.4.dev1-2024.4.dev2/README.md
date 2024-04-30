# Comparing `tmp/r3xa-2024.4.dev1.tar.gz` & `tmp/r3xa-2024.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r3xa-2024.4.dev1.tar", max compression
+gzip compressed data, was "r3xa-2024.4.dev2.tar", max compression
```

## Comparing `r3xa-2024.4.dev1.tar` & `r3xa-2024.4.dev2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      778 2024-04-14 14:26:17.692098 r3xa-2024.4.dev1/README.md
--rw-r--r--   0        0        0     1693 2024-04-14 14:26:17.692098 r3xa-2024.4.dev1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-14 14:26:17.716098 r3xa-2024.4.dev1/r3xa/__init__.py
--rw-r--r--   0        0        0    24788 2024-04-14 14:26:17.692098 r3xa-2024.4.dev1/r3xa/gui.py
--rw-r--r--   0        0        0    10884 2024-04-14 14:26:17.692098 r3xa-2024.4.dev1/r3xa/metadata.py
--rw-r--r--   0        0        0     1432 2024-04-14 14:26:17.692098 r3xa-2024.4.dev1/r3xa/scripts.py
--rw-r--r--   0        0        0     3122 2024-04-14 14:26:17.692098 r3xa-2024.4.dev1/r3xa/utils.py
--rw-r--r--   0        0        0      517 2024-04-14 14:26:17.692098 r3xa-2024.4.dev1/r3xa/validation.py
--rw-r--r--   0        0        0    33758 2024-04-14 14:26:17.693098 r3xa-2024.4.dev1/resources/schema.json
--rw-r--r--   0        0        0     1718 1970-01-01 00:00:00.000000 r3xa-2024.4.dev1/PKG-INFO
+-rw-r--r--   0        0        0      778 2024-04-30 09:24:50.435803 r3xa-2024.4.dev2/README.md
+-rw-r--r--   0        0        0     1758 2024-04-30 09:24:50.436803 r3xa-2024.4.dev2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-30 09:24:50.461803 r3xa-2024.4.dev2/r3xa/__init__.py
+-rw-r--r--   0        0        0    26052 2024-04-30 09:24:50.436803 r3xa-2024.4.dev2/r3xa/gui.py
+-rw-r--r--   0        0        0    10884 2024-04-30 09:24:50.436803 r3xa-2024.4.dev2/r3xa/metadata.py
+-rw-r--r--   0        0        0     2644 2024-04-30 09:24:50.436803 r3xa-2024.4.dev2/r3xa/scripts.py
+-rw-r--r--   0        0        0     3183 2024-04-30 09:24:50.436803 r3xa-2024.4.dev2/r3xa/utils.py
+-rw-r--r--   0        0        0      517 2024-04-30 09:24:50.436803 r3xa-2024.4.dev2/r3xa/validation.py
+-rw-r--r--   0        0        0     3468 2024-04-30 09:24:50.436803 r3xa-2024.4.dev2/r3xa/visualisation.py
+-rw-r--r--   0        0        0    33678 2024-04-30 09:24:50.436803 r3xa-2024.4.dev2/resources/schema.json
+-rw-r--r--   0        0        0     1749 1970-01-01 00:00:00.000000 r3xa-2024.4.dev2/PKG-INFO
```

### Comparing `r3xa-2024.4.dev1/README.md` & `r3xa-2024.4.dev2/README.md`

 * *Files identical despite different names*

### Comparing `r3xa-2024.4.dev1/pyproject.toml` & `r3xa-2024.4.dev2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "r3xa"
-version = "2024.4.dev1"
+version = "2024.4.dev2"
 description = "Remember, Reuse and Replicate eXperiments and Analyses"
 authors = ["Emmanuel Roubin <emmanuel.roubin@univ-grenoble-alpes.fr>"]
 maintainers = ["Emmanuel Roubin <emmanuel.roubin@univ-grenoble-alpes.fr>"]
 homepage = "https://photomecanics.gitlab.io/r3xa/doc"
 repository = "https://gitlab.com/photomecanics/r3xa"
 keywords = []
 readme = "README.md"
@@ -17,14 +17,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 jsonschema = "4.21.1"
 python-slugify = "8.0.4"
 Pygments = "2.17.2"
 PyQt5 = "=5.15.2"
+pyvis = "0.3.2"
 
 [tool.poetry.group.dev]
 optional = true
 [tool.poetry.group.dev.dependencies]
 pytest = "8.1.1"
 pre-commit = "3.5.0"
 coverage = "7.4.4"
@@ -34,14 +35,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 r3xa = "r3xa.scripts:script_gui"
 r3xa-validate = "r3xa.scripts:script_validate"
+r3xa-visualise = "r3xa.scripts:script_visualise"
 
 [tool.poe.tasks]
 # build html doc
 doc_fold = "mkdir -p doc"
 doc_json = "poetry run generate-schema-doc --config no_link_to_reused_ref --config copy_js --config no_collapse_long_descriptions --config no_collapse_long_examples resources/schema.json doc/index.html"
 doc = ["doc_fold", "doc_json"]
 # build coverage
```

### Comparing `r3xa-2024.4.dev1/r3xa/gui.py` & `r3xa-2024.4.dev2/r3xa/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -315,21 +315,38 @@
 
         self.settingComboBox.clear()
 
         # default un triggreable
         self.settingComboBox.addItem(f"--- Manage your settings ---", userData=None)
         self.settingComboBox.model().item(0).setEnabled(False)
 
-        # create a new settings from schema
+        self.settingComboBox.addItem(f"--- Add a new setting ---", userData=None)
+        self.settingComboBox.model().item(1).setEnabled(False)
+
+        item_id = 2
+        # CREATE a new settings from schema
         for k, v in self.schema["$defs"]["settings"].items():
-            self.settingComboBox.addItem(f"New {k} setting", userData=f"new_{k}")
+            self.settingComboBox.addItem(f"New {k}", userData=f"new_{k}")
+            item_id += 1
 
-        # get all settings from schema
+        # EDIT get all settings from schema
+        self.settingComboBox.addItem(f"--- Edit a setting ---", userData=None)
+        self.settingComboBox.model().item(item_id).setEnabled(False)
+        item_id += 1
         for setting in self.metadata.settings:
             self.settingComboBox.addItem(f"Edit {setting.title}", userData=f"edit_{setting.id}")
+            item_id += 1
+
+        # DELETE get all settings from schema
+        self.settingComboBox.addItem(f"--- Delete a setting ---", userData=None)
+        self.settingComboBox.model().item(item_id).setEnabled(False)
+        item_id += 1
+        for setting in self.metadata.settings:
+            self.settingComboBox.addItem(f"Delete {setting.title}", userData=f"delete_{setting.id}")
+            item_id += 1
 
         # reconnect again
         self.settingComboBox.currentIndexChanged.connect(self.onSettingComboBox)
 
     def settingsTab(self):
         mainLayout = QVBoxLayout()
 
@@ -374,30 +391,42 @@
 
         # parse key
         # new settings
         #     new_generic
         #     new_specimen
         # edit settings
         #     edit_lskhdflqsdhf
+        # delete settings
+        #     delete_lskhdflqsdhf
 
         action = key.split("_")[0]
 
         print(key, action)
 
         if action == "edit":
             setting_id = "_".join(key.split("_")[1:])
             # get setting from json
-            setting = [s for s in self.json["settings"] if s["id"] == setting_id][0]
-            kind = setting["kind"].split("/")[1]
+            setting = [s for s in self.metadata.settings if s.id == setting_id][0]
+            kind = setting.kind.split("/")[1]
             section_key = f"field:settings/{kind}"
-            self.display_form(section_key, setting, self.settingFormLayout)
+            self.display_form(section_key, dict(setting), self.settingFormLayout)
 
             title = getattr(self, section_key + "/title")
             self.outputText.setText(f"{action.title()} {title.text()} [{setting_id}]")
             self.outputText.setStyleSheet("color: #aaa;")
+
+        elif action == "delete":
+            setting_id = "_".join(key.split("_")[1:])
+            # remove setting
+            for setting in [s for s in self.metadata.settings if s.id == setting_id]:
+                self.outputText.setText(f"Setting {setting.title} [{setting.id}] deleted")
+            self.metadata.settings = [s for s in self.metadata.settings if s.id != setting_id]
+
+            self.setSettingsComboBox()
+
         elif action == "new":
             kind = "_".join(key.split("_")[1:])
             section_key = f"field:settings/{kind}"
             title = f"New {kind}"
             setting = Setting(title=title, kind=f"settings/{kind}", check=False)
             self.display_form(section_key, dict(setting), self.settingFormLayout)
 
@@ -584,15 +613,15 @@
         pprint(payload)
         self.metadata.load(payload)
         print("------------")
         print(self.metadata)
         self.json = dict(self.metadata)
 
         # update combo boxes:
-        print("UPDATE settings combo boc")
+        print("UPDATE settings combo box")
         self.setSettingsComboBox()
 
     def validate_metadata(self):
         try:
             validate(self.json)
         except Exception as e:
             print(e)
```

### Comparing `r3xa-2024.4.dev1/r3xa/metadata.py` & `r3xa-2024.4.dev2/r3xa/metadata.py`

 * *Files identical despite different names*

### Comparing `r3xa-2024.4.dev1/r3xa/utils.py` & `r3xa-2024.4.dev2/r3xa/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -83,15 +83,19 @@
     try:
         return float(f)
     except (ValueError, TypeError):
         return None
 
 
 def slugify_file_name(path):
-    """Slugify a file name while considering it to be a path"""
+    """Slugify a file name.
+    - doesn't slugify the path
+    - conserve the .
+    - gives random name if only path
+    """
 
     # get basename if the file and slugify
     basename = os.path.basename(path)
     basename = ".".join([slugify.slugify(_) for _ in basename.split(".")])
     # get path
     directory_path = os.path.dirname(path)
     if not len(basename):
```

### Comparing `r3xa-2024.4.dev1/r3xa/validation.py` & `r3xa-2024.4.dev2/r3xa/validation.py`

 * *Files identical despite different names*

### Comparing `r3xa-2024.4.dev1/resources/schema.json` & `r3xa-2024.4.dev2/resources/schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994013895629098%*

 * *Differences: {"'$defs'": "{'data_sources': {'generic': {'properties': {'id': {'description': 'ID of the data "*

 * *            "source'}}}, 'camera': {'properties': {'id': {'description': 'ID of the data source'}, "*

 * *            "'input_data_set': {'type': 'string', delete: ['$ref']}}}, 'tomograph': {'properties': "*

 * *            "{'id': {'description': 'ID of the data source'}, 'input_data_set': {'type': 'string', "*

 * *            "delete: ['$ref']}}}}, 'data_sets': {'file': {'properties': {'id': {'description': 'ID "*

 * *           […]*

```diff
@@ -28,15 +28,15 @@
                         "examples": [
                             "text/csv"
                         ],
                         "title": "Fiel type",
                         "type": "string"
                     },
                     "id": {
-                        "description": "ID of data set",
+                        "description": "ID of the data set",
                         "title": "ID",
                         "type": "string"
                     },
                     "kind": {
                         "const": "data_sets/file",
                         "description": "Only required for specs implementation purposes",
                         "title": "Kind of data source",
@@ -206,15 +206,15 @@
                     },
                     "focal_length": {
                         "$ref": "#/$defs/types/unit",
                         "description": "Focal length of the lens in mm",
                         "title": "Focal length"
                     },
                     "id": {
-                        "description": "ID of the data_source (should start at 0)",
+                        "description": "ID of the data source",
                         "title": "ID",
                         "type": "string"
                     },
                     "image_scale": {
                         "$ref": "#/$defs/types/unit",
                         "description": "Scale of the image in pix / m",
                         "title": "Image scale"
@@ -226,17 +226,17 @@
                         },
                         "maxItems": 2,
                         "minItems": 2,
                         "title": "Image size",
                         "type": "array"
                     },
                     "input_data_set": {
-                        "$ref": "#/$defs/types/uint",
                         "description": "The data set ID serving as an input source",
-                        "title": "Input data set"
+                        "title": "Input data set",
+                        "type": "string"
                     },
                     "kind": {
                         "const": "data_sources/camera",
                         "description": "Only required for specs implementation purposes",
                         "title": "Kind of data source",
                         "type": "string"
                     },
@@ -320,15 +320,15 @@
                     },
                     "documentation": {
                         "$ref": "#/$defs/types/uri",
                         "description": "Name, path or ULR of the documentation (no spaces, no accents)",
                         "title": "Documentation"
                     },
                     "id": {
-                        "description": "ID of the data_source (should start at 0)",
+                        "description": "ID of the data source",
                         "title": "ID",
                         "type": "string"
                     },
                     "input_data_set": {
                         "description": "The data set ID serving as an input source",
                         "title": "Input data set",
                         "type": "string"
@@ -421,15 +421,15 @@
                         },
                         "maxItems": 2,
                         "minItems": 2,
                         "title": "Field of view",
                         "type": "array"
                     },
                     "id": {
-                        "description": "ID of the data_source (should start at 0)",
+                        "description": "ID of the data source",
                         "title": "ID",
                         "type": "string"
                     },
                     "image_scale": {
                         "$ref": "#/$defs/types/unit",
                         "description": "Scale of the image in vox / m",
                         "title": "Image scale"
@@ -441,17 +441,17 @@
                         },
                         "maxItems": 3,
                         "minItems": 3,
                         "title": "Image size",
                         "type": "array"
                     },
                     "input_data_set": {
-                        "$ref": "#/$defs/types/uint",
                         "description": "The data set ID serving as an input source",
-                        "title": "Input data set"
+                        "title": "Input data set",
+                        "type": "string"
                     },
                     "kind": {
                         "const": "data_sources/tomograph",
                         "description": "Only required for specs implementation purposes",
                         "title": "Kind of data source",
                         "type": "string"
                     },
@@ -668,15 +668,15 @@
                             "type": "number"
                         }
                     ]
                 },
                 "type": "array"
             },
             "string": {
-                "minLength": 1,
+                "minLength": 4,
                 "type": "string"
             },
             "uint": {
                 "description": "Unsigned int",
                 "minimum": 0,
                 "title": "uint",
                 "type": "integer"
@@ -840,15 +840,15 @@
                 "DICComposite2.0",
                 "My awesome data sets"
             ],
             "title": "Title",
             "type": "string"
         },
         "version": {
-            "const": "2024.4.dev1",
+            "const": "2024.4.dev2",
             "description": "Version of the schema used",
             "title": "Version",
             "type": "string"
         }
     },
     "required": [
         "title",
```

### Comparing `r3xa-2024.4.dev1/PKG-INFO` & `r3xa-2024.4.dev2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r3xa
-Version: 2024.4.dev1
+Version: 2024.4.dev2
 Summary: Remember, Reuse and Replicate eXperiments and Analyses
 Home-page: https://photomecanics.gitlab.io/r3xa/doc
 Author: Emmanuel Roubin
 Author-email: emmanuel.roubin@univ-grenoble-alpes.fr
 Maintainer: Emmanuel Roubin
 Maintainer-email: emmanuel.roubin@univ-grenoble-alpes.fr
 Requires-Python: >=3.8.1,<4.0.0
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyQt5 (==5.15.2)
 Requires-Dist: Pygments (==2.17.2)
 Requires-Dist: jsonschema (==4.21.1)
 Requires-Dist: python-slugify (==8.0.4)
+Requires-Dist: pyvis (==0.3.2)
 Project-URL: Repository, https://gitlab.com/photomecanics/r3xa
 Description-Content-Type: text/markdown
 
 # R3XA
 ## Remember, Reuse and Replicate eXperiments and Analyses
 
 ### Specs
```

