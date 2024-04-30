# Comparing `tmp/invisibleroads-macros-web-0.3.6.tar.gz` & `tmp/invisibleroads_macros_web-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invisibleroads-macros-web-0.3.6.tar", last modified: Thu Sep 28 16:42:16 2023, max compression
+gzip compressed data, was "invisibleroads_macros_web-0.3.7.tar", last modified: Tue Apr 30 10:49:51 2024, max compression
```

## Comparing `invisibleroads-macros-web-0.3.6.tar` & `invisibleroads_macros_web-0.3.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-09-28 16:42:16.320618 invisibleroads-macros-web-0.3.6/
--rw-r--r--   0 rhh       (1000) rhh       (1000)      376 2023-09-28 16:40:56.000000 invisibleroads-macros-web-0.3.6/CHANGES.md
--rw-r--r--   0 rhh       (1000) rhh       (1000)       13 2023-08-18 19:33:41.000000 invisibleroads-macros-web-0.3.6/MANIFEST.in
--rw-r--r--   0 rhh       (1000) rhh       (1000)     2302 2023-09-28 16:42:16.320618 invisibleroads-macros-web-0.3.6/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1104 2023-08-18 19:33:41.000000 invisibleroads-macros-web-0.3.6/README.md
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-09-28 16:42:16.318618 invisibleroads-macros-web-0.3.6/invisibleroads_macros_web/
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-08-18 19:33:41.000000 invisibleroads-macros-web-0.3.6/invisibleroads_macros_web/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      846 2023-08-18 19:33:41.000000 invisibleroads-macros-web-0.3.6/invisibleroads_macros_web/browser.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      290 2023-08-18 19:33:41.000000 invisibleroads-macros-web-0.3.6/invisibleroads_macros_web/escape.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1773 2023-08-18 19:33:41.000000 invisibleroads-macros-web-0.3.6/invisibleroads_macros_web/jinja.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      854 2023-08-18 19:33:41.000000 invisibleroads-macros-web-0.3.6/invisibleroads_macros_web/markdown.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      882 2023-08-18 19:33:41.000000 invisibleroads-macros-web-0.3.6/invisibleroads_macros_web/port.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1117 2023-08-18 19:33:41.000000 invisibleroads-macros-web-0.3.6/invisibleroads_macros_web/starlette.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-09-28 16:42:16.319618 invisibleroads-macros-web-0.3.6/invisibleroads_macros_web.egg-info/
--rw-r--r--   0 rhh       (1000) rhh       (1000)     2302 2023-09-28 16:42:16.000000 invisibleroads-macros-web-0.3.6/invisibleroads_macros_web.egg-info/PKG-INFO
--rw-r--r--   0 rhh       (1000) rhh       (1000)      667 2023-09-28 16:42:16.000000 invisibleroads-macros-web-0.3.6/invisibleroads_macros_web.egg-info/SOURCES.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-09-28 16:42:16.000000 invisibleroads-macros-web-0.3.6/invisibleroads_macros_web.egg-info/dependency_links.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)      163 2023-09-28 16:42:16.000000 invisibleroads-macros-web-0.3.6/invisibleroads_macros_web.egg-info/requires.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)       32 2023-09-28 16:42:16.000000 invisibleroads-macros-web-0.3.6/invisibleroads_macros_web.egg-info/top_level.txt
--rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2023-08-18 19:33:49.000000 invisibleroads-macros-web-0.3.6/invisibleroads_macros_web.egg-info/zip-safe
--rw-r--r--   0 rhh       (1000) rhh       (1000)       38 2023-09-28 16:42:16.320618 invisibleroads-macros-web-0.3.6/setup.cfg
--rw-r--r--   0 rhh       (1000) rhh       (1000)     1374 2023-09-28 16:21:19.000000 invisibleroads-macros-web-0.3.6/setup.py
-drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2023-09-28 16:42:16.319618 invisibleroads-macros-web-0.3.6/tests/
--rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2023-08-18 19:33:41.000000 invisibleroads-macros-web-0.3.6/tests/__init__.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      344 2023-08-18 19:33:41.000000 invisibleroads-macros-web-0.3.6/tests/test_escape.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      865 2023-08-18 19:33:41.000000 invisibleroads-macros-web-0.3.6/tests/test_markdown.py
--rw-r--r--   0 rhh       (1000) rhh       (1000)      882 2023-08-18 19:33:41.000000 invisibleroads-macros-web-0.3.6/tests/test_port.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2024-04-30 10:49:51.545905 invisibleroads_macros_web-0.3.7/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      376 2024-04-30 10:40:52.000000 invisibleroads_macros_web-0.3.7/CHANGES.md
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       13 2024-04-30 10:40:52.000000 invisibleroads_macros_web-0.3.7/MANIFEST.in
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     2417 2024-04-30 10:49:51.545905 invisibleroads_macros_web-0.3.7/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1219 2024-04-30 10:47:11.000000 invisibleroads_macros_web-0.3.7/README.md
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2024-04-30 10:49:51.542905 invisibleroads_macros_web-0.3.7/invisibleroads_macros_web/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2024-04-30 10:40:52.000000 invisibleroads_macros_web-0.3.7/invisibleroads_macros_web/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      846 2024-04-30 10:40:52.000000 invisibleroads_macros_web-0.3.7/invisibleroads_macros_web/browser.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      290 2024-04-30 10:40:52.000000 invisibleroads_macros_web-0.3.7/invisibleroads_macros_web/escape.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1657 2024-04-30 10:46:36.000000 invisibleroads_macros_web-0.3.7/invisibleroads_macros_web/jinja.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      944 2024-04-30 10:45:25.000000 invisibleroads_macros_web-0.3.7/invisibleroads_macros_web/markdown.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      882 2024-04-30 10:47:12.000000 invisibleroads_macros_web-0.3.7/invisibleroads_macros_web/port.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1117 2024-04-30 10:40:52.000000 invisibleroads_macros_web-0.3.7/invisibleroads_macros_web/starlette.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2024-04-30 10:49:51.543905 invisibleroads_macros_web-0.3.7/invisibleroads_macros_web.egg-info/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     2417 2024-04-30 10:49:51.000000 invisibleroads_macros_web-0.3.7/invisibleroads_macros_web.egg-info/PKG-INFO
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      667 2024-04-30 10:49:51.000000 invisibleroads_macros_web-0.3.7/invisibleroads_macros_web.egg-info/SOURCES.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2024-04-30 10:49:51.000000 invisibleroads_macros_web-0.3.7/invisibleroads_macros_web.egg-info/dependency_links.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      163 2024-04-30 10:49:51.000000 invisibleroads_macros_web-0.3.7/invisibleroads_macros_web.egg-info/requires.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       32 2024-04-30 10:49:51.000000 invisibleroads_macros_web-0.3.7/invisibleroads_macros_web.egg-info/top_level.txt
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        1 2024-04-30 10:49:51.000000 invisibleroads_macros_web-0.3.7/invisibleroads_macros_web.egg-info/zip-safe
+-rw-r--r--   0 rhh       (1000) rhh       (1000)       38 2024-04-30 10:49:51.545905 invisibleroads_macros_web-0.3.7/setup.cfg
+-rw-r--r--   0 rhh       (1000) rhh       (1000)     1374 2024-04-30 10:48:26.000000 invisibleroads_macros_web-0.3.7/setup.py
+drwxr-xr-x   0 rhh       (1000) rhh       (1000)        0 2024-04-30 10:49:51.543905 invisibleroads_macros_web-0.3.7/tests/
+-rw-r--r--   0 rhh       (1000) rhh       (1000)        0 2024-04-30 10:40:52.000000 invisibleroads_macros_web-0.3.7/tests/__init__.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      344 2024-04-30 10:40:52.000000 invisibleroads_macros_web-0.3.7/tests/test_escape.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      865 2024-04-30 10:40:52.000000 invisibleroads_macros_web-0.3.7/tests/test_markdown.py
+-rw-r--r--   0 rhh       (1000) rhh       (1000)      882 2024-04-30 10:40:52.000000 invisibleroads_macros_web-0.3.7/tests/test_port.py
```

### Comparing `invisibleroads-macros-web-0.3.6/PKG-INFO` & `invisibleroads_macros_web-0.3.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invisibleroads-macros-web
-Version: 0.3.6
+Version: 0.3.7
 Summary: Shortcut functions for web operations
 Home-page: https://github.com/invisibleroads/invisibleroads-macros-web
 Author: Roy Hyunjin Han
 Author-email: rhh@crosscompute.com
 Keywords: invisibleroads
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
@@ -47,23 +47,26 @@
 # Check ports
 from invisibleroads_macros_web.port import (
     find_open_port,
     is_port_in_use)
 
 # Render markdown
 from invisibleroads_macros_web.markdown import (
-    get_html_from_markdown)
+    get_html_from_markdown,
+    remove_single_paragraph,
+    remove_parent_paragraphs,
+    remove_line_break_after_div)
 
 # Configure templates
 from invisibleroads_macros_web.jinja import (
     AssetStorage,
     RelativeTemplateEnvironment,
-    TemplatePathLoader,
-    url_for)
+    PathTemplateLoader)
 from invisibleroads_macros_web.starlette import (
+    ExtraResponseHeadersMiddleware,
     TemplateResponseFactory)
 ```
 
 ## Test
 
 ```bash
 git clone https://github.com/invisibleroads/invisibleroads-macros-web
```

### Comparing `invisibleroads-macros-web-0.3.6/README.md` & `invisibleroads_macros_web-0.3.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,23 +24,26 @@
 # Check ports
 from invisibleroads_macros_web.port import (
     find_open_port,
     is_port_in_use)
 
 # Render markdown
 from invisibleroads_macros_web.markdown import (
-    get_html_from_markdown)
+    get_html_from_markdown,
+    remove_single_paragraph,
+    remove_parent_paragraphs,
+    remove_line_break_after_div)
 
 # Configure templates
 from invisibleroads_macros_web.jinja import (
     AssetStorage,
     RelativeTemplateEnvironment,
-    TemplatePathLoader,
-    url_for)
+    PathTemplateLoader)
 from invisibleroads_macros_web.starlette import (
+    ExtraResponseHeadersMiddleware,
     TemplateResponseFactory)
 ```
 
 ## Test
 
 ```bash
 git clone https://github.com/invisibleroads/invisibleroads-macros-web
```

### Comparing `invisibleroads-macros-web-0.3.6/invisibleroads_macros_web/browser.py` & `invisibleroads_macros_web-0.3.7/invisibleroads_macros_web/browser.py`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.6/invisibleroads_macros_web/jinja.py` & `invisibleroads_macros_web-0.3.7/invisibleroads_macros_web/jinja.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from string import Template as StringTemplate
 
 from invisibleroads_macros_disk import get_asset_path
 from jinja2 import (
     BaseLoader,
     Environment,
     Template as JinjaTemplate,
-    TemplateNotFound,
-    pass_context)
+    TemplateNotFound)
 
 
 class AssetStorage():
 
     def __init__(self, folder):
         self.folder = folder
 
@@ -51,12 +50,7 @@
 class RelativeTemplateEnvironment(Environment):
 
     def join_path(self, template, parent):
         'Support relative template paths via extends, import, include'
         template = get_asset_path(template)
         return normpath(join(dirname(
             parent), template)) if template else template
-
-
-@pass_context
-def url_for(context, name, **d):
-    return context['request'].url_for(name, **d)
```

### Comparing `invisibleroads-macros-web-0.3.6/invisibleroads_macros_web/port.py` & `invisibleroads_macros_web-0.3.7/invisibleroads_macros_web/port.py`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.6/invisibleroads_macros_web/starlette.py` & `invisibleroads_macros_web-0.3.7/invisibleroads_macros_web/starlette.py`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.6/invisibleroads_macros_web.egg-info/PKG-INFO` & `invisibleroads_macros_web-0.3.7/invisibleroads_macros_web.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invisibleroads-macros-web
-Version: 0.3.6
+Version: 0.3.7
 Summary: Shortcut functions for web operations
 Home-page: https://github.com/invisibleroads/invisibleroads-macros-web
 Author: Roy Hyunjin Han
 Author-email: rhh@crosscompute.com
 Keywords: invisibleroads
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
@@ -47,23 +47,26 @@
 # Check ports
 from invisibleroads_macros_web.port import (
     find_open_port,
     is_port_in_use)
 
 # Render markdown
 from invisibleroads_macros_web.markdown import (
-    get_html_from_markdown)
+    get_html_from_markdown,
+    remove_single_paragraph,
+    remove_parent_paragraphs,
+    remove_line_break_after_div)
 
 # Configure templates
 from invisibleroads_macros_web.jinja import (
     AssetStorage,
     RelativeTemplateEnvironment,
-    TemplatePathLoader,
-    url_for)
+    PathTemplateLoader)
 from invisibleroads_macros_web.starlette import (
+    ExtraResponseHeadersMiddleware,
     TemplateResponseFactory)
 ```
 
 ## Test
 
 ```bash
 git clone https://github.com/invisibleroads/invisibleroads-macros-web
```

### Comparing `invisibleroads-macros-web-0.3.6/invisibleroads_macros_web.egg-info/SOURCES.txt` & `invisibleroads_macros_web-0.3.7/invisibleroads_macros_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.6/setup.py` & `invisibleroads_macros_web-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 FOLDER = dirname(abspath(__file__))
 DESCRIPTION = '\n\n'.join(open(join(FOLDER, _)).read().strip() for _ in [
     'README.md', 'CHANGES.md'])
 
 
 setup(
     name='invisibleroads-macros-web',
-    version='0.3.6',
+    version='0.3.7',
     description='Shortcut functions for web operations',
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     classifiers=[
         'Programming Language :: Python',
         'License :: OSI Approved :: MIT License',
     ],
```

### Comparing `invisibleroads-macros-web-0.3.6/tests/test_markdown.py` & `invisibleroads_macros_web-0.3.7/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `invisibleroads-macros-web-0.3.6/tests/test_port.py` & `invisibleroads_macros_web-0.3.7/tests/test_port.py`

 * *Files identical despite different names*

