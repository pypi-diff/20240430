# Comparing `tmp/dj_component_view-1.1.0.tar.gz` & `tmp/dj_component_view-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_component_view-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dj_component_view-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dj_component_view-1.1.0.tar` & `dj_component_view-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3078 2024-04-29 05:31:20.582104 dj_component_view-1.1.0/.gitignore
--rw-r--r--   0        0        0     1086 2024-04-29 05:24:52.851465 dj_component_view-1.1.0/LICENSE
--rw-r--r--   0        0        0      432 2024-04-29 05:31:39.694978 dj_component_view-1.1.0/README.md
--rw-r--r--   0        0        0     1211 2024-04-29 05:27:52.055192 dj_component_view-1.1.0/dj_component_view.py
--rw-r--r--   0        0        0      423 2024-04-29 05:35:07.152445 dj_component_view-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 dj_component_view-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3078 2024-04-29 05:31:20.582104 dj_component_view-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1086 2024-04-29 05:24:52.851465 dj_component_view-1.2.0/LICENSE
+-rw-r--r--   0        0        0      432 2024-04-29 05:31:39.694978 dj_component_view-1.2.0/README.md
+-rw-r--r--   0        0        0     1346 2024-04-29 05:42:00.228350 dj_component_view-1.2.0/dj_component_view.py
+-rw-r--r--   0        0        0      423 2024-04-29 05:42:10.678561 dj_component_view-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 dj_component_view-1.2.0/PKG-INFO
```

### Comparing `dj_component_view-1.1.0/.gitignore` & `dj_component_view-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dj_component_view-1.1.0/LICENSE` & `dj_component_view-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_component_view-1.1.0/dj_component_view.py` & `dj_component_view-1.2.0/dj_component_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,9 +24,13 @@
             raise ValueError("ComponentView subclasses must define a component.")
         return HttpResponse(str(catalog.render(self.component, **context)))
 
     def get(self, request, *args, **kwargs):
         context = self.context(request)
         return self.render_to_response(context)
 
+    def post(self, request, *args, **kwargs):
+        context = self.context(request)
+        return self.render_to_response(context)
+
     def context(self, request):
         return {}
```

### Comparing `dj_component_view-1.1.0/PKG-INFO` & `dj_component_view-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_component_view
-Version: 1.1.0
+Version: 1.2.0
 Summary: Django component view for jinjax
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: django
 Requires-Dist: jinjax
```

