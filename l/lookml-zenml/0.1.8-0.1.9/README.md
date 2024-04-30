# Comparing `tmp/lookml_zenml-0.1.8.tar.gz` & `tmp/lookml_zenml-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lookml_zenml-0.1.8.tar", max compression
+gzip compressed data, was "lookml_zenml-0.1.9.tar", max compression
```

## Comparing `lookml_zenml-0.1.8.tar` & `lookml_zenml-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2023-07-04 01:20:53.638233 lookml_zenml-0.1.8/LICENSE
--rw-r--r--   0        0        0     1969 2024-03-30 16:06:06.708233 lookml_zenml-0.1.8/README.md
--rw-r--r--   0        0        0      109 2023-10-31 16:38:51.887928 lookml_zenml-0.1.8/lookml_zenml/__init__.py
--rw-r--r--   0        0        0     4843 2023-11-08 22:37:29.473621 lookml_zenml-0.1.8/lookml_zenml/cli.py
--rw-r--r--   0        0        0    30568 2024-04-20 21:29:06.320222 lookml_zenml-0.1.8/lookml_zenml/lookml_project.py
--rw-r--r--   0        0        0      581 2024-04-20 20:44:57.331189 lookml_zenml-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 lookml_zenml-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-04 01:20:53.638233 lookml_zenml-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1969 2024-03-30 16:06:06.708233 lookml_zenml-0.1.9/README.md
+-rw-r--r--   0        0        0      109 2023-10-31 16:38:51.887928 lookml_zenml-0.1.9/lookml_zenml/__init__.py
+-rw-r--r--   0        0        0     4843 2023-11-08 22:37:29.473621 lookml_zenml-0.1.9/lookml_zenml/cli.py
+-rw-r--r--   0        0        0    30655 2024-04-29 21:03:49.225148 lookml_zenml-0.1.9/lookml_zenml/lookml_project.py
+-rw-r--r--   0        0        0      581 2024-04-29 21:04:25.043003 lookml_zenml-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 lookml_zenml-0.1.9/PKG-INFO
```

### Comparing `lookml_zenml-0.1.8/LICENSE` & `lookml_zenml-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lookml_zenml-0.1.8/README.md` & `lookml_zenml-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lookml_zenml-0.1.8/lookml_zenml/cli.py` & `lookml_zenml-0.1.9/lookml_zenml/cli.py`

 * *Files identical despite different names*

### Comparing `lookml_zenml-0.1.8/lookml_zenml/lookml_project.py` & `lookml_zenml-0.1.9/lookml_zenml/lookml_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,17 @@
                     f["field"], self._views, model_name=f.get("model"), explore_name=f.get("explore")
                 )
                 default_value = f.get("default_value")
                 if default_value == "No":
                     default_value = False
                 elif default_value == "Yes":
                     default_value = True
-                zenml_data["filters"].append({"field": field["id"], "value": default_value})
+                zenml_data["filters"].append(
+                    {"name": f["name"], "field": field["id"], "value": default_value}
+                )
 
         sorted_elements = sorted(dashboard["elements"], key=lambda x: (x.get("row", 0), x.get("col", 0)))
         for element in sorted_elements:
             zenml_element = self._translate_dashboard_element(element)
             if zenml_element:
                 zenml_data["elements"].append(zenml_element)
 
@@ -320,15 +322,14 @@
     def _translate_dashboard_element(self, element: dict):
         if "merged_queries" in element:
             return self._translate_merged_queries_element(element)
         return self._translate_vanilla_element(element)
 
     def _translate_vanilla_element(self, element: dict):
         # We do not support conditional formatting in dashboards
-        # We do not support non-query elements yet, either
         if "model" not in element and element.get("type") not in {"button", "text"}:
             return None
 
         elif element.get("type") == "text":
             model_name = self._default_model_name if self._default_model_name else "todo"
             zenml_element = {"model": model_name, "type": "markdown", "size": "quarter"}
             zenml_element["content"] = element.get("body_text", "")
@@ -382,14 +383,17 @@
                 if v != "":
                     if v == "No":
                         v = False
                     elif v == "Yes":
                         v = True
                     zenml_element["filters"].append({"field": field["id"].lower(), "value": v})
 
+        if "listen" in element:
+            zenml_element["listen"] = element["listen"]
+
         if "sorts" in element:
             zenml_element["sort"] = []
             for sort_str in element["sorts"]:
                 split_str = sort_str.split(" ")
                 field = self._get_field(
                     split_str[0],
                     self._views,
```

### Comparing `lookml_zenml-0.1.8/pyproject.toml` & `lookml_zenml-0.1.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lookml-zenml"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Paul Blankley <paul@zenlytic.com>"]
 readme = "README.md"
 packages = [{include = "lookml_zenml"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1, <3.12"
```

### Comparing `lookml_zenml-0.1.8/PKG-INFO` & `lookml_zenml-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lookml-zenml
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Paul Blankley
 Author-email: paul@zenlytic.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

