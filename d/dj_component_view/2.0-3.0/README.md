# Comparing `tmp/dj_component_view-2.0.tar.gz` & `tmp/dj_component_view-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_component_view-2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dj_component_view-3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dj_component_view-2.0.tar` & `dj_component_view-3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3078 2024-04-29 05:31:20.582104 dj_component_view-2.0/.gitignore
--rw-r--r--   0        0        0     1086 2024-04-29 05:24:52.851465 dj_component_view-2.0/LICENSE
--rw-r--r--   0        0        0     2395 2024-04-29 22:03:34.762510 dj_component_view-2.0/README.md
--rw-r--r--   0        0        0     1880 2024-04-29 21:53:33.082254 dj_component_view-2.0/dj_component_view.py
--rw-r--r--   0        0        0      500 2024-04-29 19:36:09.877362 dj_component_view-2.0/pyproject.toml
--rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 dj_component_view-2.0/PKG-INFO
+-rw-r--r--   0        0        0     3078 2024-04-29 05:31:20.582104 dj_component_view-3.0/.gitignore
+-rw-r--r--   0        0        0     1086 2024-04-29 05:24:52.851465 dj_component_view-3.0/LICENSE
+-rw-r--r--   0        0        0     1709 2024-04-29 22:47:30.260505 dj_component_view-3.0/README.md
+-rw-r--r--   0        0        0     1614 2024-04-29 22:45:49.350973 dj_component_view-3.0/dj_component_view.py
+-rw-r--r--   0        0        0      500 2024-04-29 22:45:57.795947 dj_component_view-3.0/pyproject.toml
+-rw-r--r--   0        0        0     2081 1970-01-01 00:00:00.000000 dj_component_view-3.0/PKG-INFO
```

### Comparing `dj_component_view-2.0/.gitignore` & `dj_component_view-3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dj_component_view-2.0/LICENSE` & `dj_component_view-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_component_view-2.0/README.md` & `dj_component_view-3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # dj_component_view
 
-This project lets you create reusable Django views from [jinjax](https://jinjax.scaletti.dev/) templates. By default, the `.post` method is implemented. You only need to override the `.context`
-method to pass data to the `jinjax` component.
+This project lets you create reusable Django views from [jinjax](https://jinjax.scaletti.dev/) templates.
 
 ## Usage
 
+### Greeting.jinja
+
+```jinja
+{#def name #}
+
+<h1>hello, {{ name }}</h1>
+```
+
+### views.py
+
 ```python
 from dj_component_view import ComponentView
 from djecorator import Route
 
 route = Route()
 
 @route("/greet")
@@ -18,60 +27,39 @@
     def context(self, request):
         return {
             # by default, the view expects a POST request
             "name": request.POST.get("name", "World"),
         }
 ```
 
+### index.html with [htmx](https://htmx.org)
+
+```html
+<form hx-post="/greet" hx-trigger="submit">
+  <input type="text" name="name" placeholder="Enter your name" />
+  <button type="submit">Greet</button>
+</form>
+```
+
 ### Specifying the Allowed HTTP Method
 
 You can set the method class variable in your ComponentView subclass to specify the allowed HTTP method for the view. The default value is None, which means both GET and POST methods are allowed.
 
-* If `method` is set to `"GET"`, only GET requests will be allowed.
-* If `method` is set to `"POST"`, only POST requests will be allowed.
-* If `method` is set to `None` (default), both GET and POST requests will be allowed.
+- If `method` is set to `"GET"`, only GET requests will be allowed.
+- If `method` is set to `"POST"`, only POST requests will be allowed.
 
 If the incoming request's method does not match the specified method, a 405 Method Not Allowed response will be returned.
 
 ### Overriding the get and post Methods
 
 If you need more control over the handling of GET and POST requests, you can override the get and post methods in your ComponentView subclass.
 
 ```python
 @route("/custom")
 class CustomView(ComponentView):
     component = "CustomComponent"
+    method = "get"
 
     def get(self, request, *args, **kwargs):
         # Custom implementation of the GET method
         ...
-
-    def post(self, request, *args, **kwargs):
-        # Custom implementation of the POST method
-        ...
-```
-
-### Providing Context Data
-
-To provide context data to the rendered component, you can override the context method in your ComponentView subclass.
-
-```python
-@route("/greet")
-class GreetView(ComponentView):
-    component = "Greeting"
-
-    def context(self, request):
-        return {
-            "name": request.POST.get("name", "World"),
-        }
-```
-
-The context method should return a dictionary containing the data that will be passed to the component for rendering.
-
-### with [htmx](https://htmx.org)
-
-```html
-<form hx-post="/greet" hx-trigger="submit">
-    <input type="text" name="name" placeholder="Enter your name">
-    <button type="submit">Greet</button>
-</form>
 ```
```

### Comparing `dj_component_view-2.0/PKG-INFO` & `dj_component_view-3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 Metadata-Version: 2.1
 Name: dj_component_view
-Version: 2.0
+Version: 3.0
 Summary: Django component view for jinjax
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: django
 Requires-Dist: jinjax
 Project-URL: Source, https://github.com/knowsuchagency/dj_component_view
 
 # dj_component_view
 
-This project lets you create reusable Django views from [jinjax](https://jinjax.scaletti.dev/) templates. By default, the `.post` method is implemented. You only need to override the `.context`
-method to pass data to the `jinjax` component.
+This project lets you create reusable Django views from [jinjax](https://jinjax.scaletti.dev/) templates.
 
 ## Usage
 
+### Greeting.jinja
+
+```jinja
+{#def name #}
+
+<h1>hello, {{ name }}</h1>
+```
+
+### views.py
+
 ```python
 from dj_component_view import ComponentView
 from djecorator import Route
 
 route = Route()
 
 @route("/greet")
@@ -29,61 +38,40 @@
     def context(self, request):
         return {
             # by default, the view expects a POST request
             "name": request.POST.get("name", "World"),
         }
 ```
 
+### index.html with [htmx](https://htmx.org)
+
+```html
+<form hx-post="/greet" hx-trigger="submit">
+  <input type="text" name="name" placeholder="Enter your name" />
+  <button type="submit">Greet</button>
+</form>
+```
+
 ### Specifying the Allowed HTTP Method
 
 You can set the method class variable in your ComponentView subclass to specify the allowed HTTP method for the view. The default value is None, which means both GET and POST methods are allowed.
 
-* If `method` is set to `"GET"`, only GET requests will be allowed.
-* If `method` is set to `"POST"`, only POST requests will be allowed.
-* If `method` is set to `None` (default), both GET and POST requests will be allowed.
+- If `method` is set to `"GET"`, only GET requests will be allowed.
+- If `method` is set to `"POST"`, only POST requests will be allowed.
 
 If the incoming request's method does not match the specified method, a 405 Method Not Allowed response will be returned.
 
 ### Overriding the get and post Methods
 
 If you need more control over the handling of GET and POST requests, you can override the get and post methods in your ComponentView subclass.
 
 ```python
 @route("/custom")
 class CustomView(ComponentView):
     component = "CustomComponent"
+    method = "get"
 
     def get(self, request, *args, **kwargs):
         # Custom implementation of the GET method
         ...
-
-    def post(self, request, *args, **kwargs):
-        # Custom implementation of the POST method
-        ...
-```
-
-### Providing Context Data
-
-To provide context data to the rendered component, you can override the context method in your ComponentView subclass.
-
-```python
-@route("/greet")
-class GreetView(ComponentView):
-    component = "Greeting"
-
-    def context(self, request):
-        return {
-            "name": request.POST.get("name", "World"),
-        }
-```
-
-The context method should return a dictionary containing the data that will be passed to the component for rendering.
-
-### with [htmx](https://htmx.org)
-
-```html
-<form hx-post="/greet" hx-trigger="submit">
-    <input type="text" name="name" placeholder="Enter your name">
-    <button type="submit">Greet</button>
-</form>
 ```
```

