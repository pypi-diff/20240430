# Comparing `tmp/rich_rst-1.3.0.tar.gz` & `tmp/rich_rst-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rich_rst-1.3.0.tar", last modified: Thu Apr 25 18:51:41 2024, max compression
+gzip compressed data, was "rich_rst-1.3.1.tar", last modified: Tue Apr 30 04:33:08 2024, max compression
```

## Comparing `rich_rst-1.3.0.tar` & `rich_rst-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 18:51:41.292364 rich_rst-1.3.0/
--rw-rw-rw-   0        0        0     1056 2022-02-06 12:37:40.000000 rich_rst-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     5962 2024-04-25 18:51:41.292364 rich_rst-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4520 2022-02-10 16:31:46.000000 rich_rst-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 18:51:41.263064 rich_rst-1.3.0/rich_rst/
--rw-rw-rw-   0        0        0    29705 2024-04-25 18:49:52.000000 rich_rst-1.3.0/rich_rst/__init__.py
--rw-rw-rw-   0        0        0     4681 2024-01-26 19:01:42.000000 rich_rst-1.3.0/rich_rst/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:51:41.291387 rich_rst-1.3.0/rich_rst.egg-info/
--rw-rw-rw-   0        0        0     5962 2024-04-25 18:51:41.000000 rich_rst-1.3.0/rich_rst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-04-25 18:51:41.000000 rich_rst-1.3.0/rich_rst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 18:51:41.000000 rich_rst-1.3.0/rich_rst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-25 18:51:41.000000 rich_rst-1.3.0/rich_rst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-25 18:51:41.000000 rich_rst-1.3.0/rich_rst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1412 2024-04-25 18:51:41.300175 rich_rst-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2022-02-06 05:09:36.000000 rich_rst-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 18:51:41.289433 rich_rst-1.3.0/tests/
--rw-rw-rw-   0        0        0     1593 2024-04-25 18:47:41.000000 rich_rst-1.3.0/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2024-04-30 04:33:08.981884 rich_rst-1.3.1/
+-rw-rw-rw-   0        0        0     1056 2022-02-06 12:37:40.000000 rich_rst-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0     5962 2024-04-30 04:33:08.980906 rich_rst-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4520 2022-02-10 16:31:46.000000 rich_rst-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 04:33:08.924192 rich_rst-1.3.1/rich_rst/
+-rw-rw-rw-   0        0        0    30146 2024-04-30 04:31:16.000000 rich_rst-1.3.1/rich_rst/__init__.py
+-rw-rw-rw-   0        0        0     4681 2024-01-26 19:01:42.000000 rich_rst-1.3.1/rich_rst/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 04:33:08.977002 rich_rst-1.3.1/rich_rst.egg-info/
+-rw-rw-rw-   0        0        0     5962 2024-04-30 04:33:08.000000 rich_rst-1.3.1/rich_rst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-04-30 04:33:08.000000 rich_rst-1.3.1/rich_rst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 04:33:08.000000 rich_rst-1.3.1/rich_rst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-30 04:33:08.000000 rich_rst-1.3.1/rich_rst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-30 04:33:08.000000 rich_rst-1.3.1/rich_rst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1412 2024-04-30 04:33:08.983839 rich_rst-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2022-02-06 05:09:36.000000 rich_rst-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 04:33:08.975049 rich_rst-1.3.1/tests/
+-rw-rw-rw-   0        0        0     1593 2024-04-25 18:47:41.000000 rich_rst-1.3.1/tests/test_main.py
```

### Comparing `rich_rst-1.3.0/LICENSE` & `rich_rst-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rich_rst-1.3.0/PKG-INFO` & `rich_rst-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-rst
-Version: 1.3.0
+Version: 1.3.1
 Summary: A beautiful reStructuredText renderer for rich
 Home-page: https://wasi-master.github.io/rich-rst
 Author: Wasi Master
 Author-email: arianmollik323@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/wasi-master/rich-rst/issues
 Project-URL: Source, https://github.com/wasi-master/rich-rst
```

### Comparing `rich_rst-1.3.0/README.md` & `rich_rst-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `rich_rst-1.3.0/rich_rst/__init__.py` & `rich_rst-1.3.1/rich_rst/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,30 +16,30 @@
 import docutils.parsers.rst
 import docutils.utils
 
 # Imports from the rich package for the printing
 import rich
 from rich import box
 from rich.align import Align
-from rich.console import Console, ConsoleOptions, RenderResult
+from rich.console import Console, ConsoleOptions, RenderResult, NewLine
 from rich.jupyter import JupyterMixin
 from rich.panel import Panel
 from rich.style import Style
 from rich.syntax import Syntax, SyntaxTheme
 from rich.text import Text
 from rich.table import Table
 from rich.traceback import install
 from rich.rule import Rule
 
 from pygments.lexers import guess_lexer
 from pygments.util import ClassNotFound
 
 __all__ = ("RST", "ReStructuredText", "reStructuredText", "RestructuredText")
 __author__ = "Arian Mollik Wasi (aka. Wasi Master)"
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 install()
 
 
 class MLStripper(HTMLParser):
     """Utility class to strip out html for raw html source"""
     def __init__(self):
@@ -282,25 +282,25 @@
                     self.renderables.append(Text(list_item.astext().replace("\n", " "), style=text_style))
                     if isinstance(list_item, docutils.nodes.bullet_list):
                         for list_item in list_item.children:
                             self.renderables.append(Text("    ", end="") + Text(" ▪ ", end="", style=marker_style))
                             self.renderables.append(Text(list_item.astext().replace("\n", " "), style=text_style))
             self.renderables.append(Text(" • ", end="", style=marker_style))
             self.renderables.append(Text(list_item.astext().replace("\n", " "), style=text_style))
-        self.renderables.append(Text())
+        self.renderables.append(NewLine())
         raise docutils.nodes.SkipChildren()
 
     def visit_enumerated_list(self, node):
         marker_style = self.console.get_style("restructuredtext.enumerated_list_marker", default="bold yellow")
         text_style = self.console.get_style("restructuredtext.enumerated_text", default="none")
         for i, list_item in enumerate(node.children, 1):
             self.renderables.append(Text(f" {i}", end=" ", style=marker_style))
             self.renderables.append(Text(list_item.astext().replace("\n", " "), style=text_style))
 
-        self.renderables.append(Text())
+        self.renderables.append(NewLine())
         raise docutils.nodes.SkipChildren()
 
     def visit_literal(self, node):
         style = self.console.get_style("restructuredtext.inline_codeblock", default="grey78 on grey7")
         if self.renderables and isinstance(self.renderables[-1], Text):
             self.renderables[-1].append_text(Text(node.astext().replace("\n", " "), style=style, end=" "))
             raise docutils.nodes.SkipChildren()
@@ -603,17 +603,28 @@
             console=console,
             code_theme=self.code_theme,
             guess_lexer=self.guess_lexer,
             default_lexer=self.default_lexer,
         )
         document.walkabout(visitor)
 
-        if visitor.renderables and isinstance(visitor.renderables[-1], Text):
-            visitor.renderables[-1].rstrip()
-            visitor.renderables[-1].end = "\n"
+        # Strip all trailing newlines and newline-like rich objects
+        while visitor.renderables:
+            if isinstance(visitor.renderables[-1], Text):
+                visitor.renderables[-1].rstrip()
+                visitor.renderables[-1].end = "\n"
+                if visitor.renderables[-1]:  # The Text object still contains data.
+                    break
+                else:
+                    visitor.renderables.pop()
+            elif isinstance(visitor.renderables[-1], NewLine):
+                visitor.renderables.pop()
+            else:
+                break
+
         for renderable in visitor.renderables:
             yield from console.render(renderable, options)
         if self.log_errors and visitor.errors:
             for error in visitor.errors:
                 yield from console.render(error, options)
         style = console.get_style("restructuredtext.footer", default="none")
         border_style = console.get_style("restructuredtext.footer_border", default="grey74")
```

### Comparing `rich_rst-1.3.0/rich_rst/__main__.py` & `rich_rst-1.3.1/rich_rst/__main__.py`

 * *Files identical despite different names*

### Comparing `rich_rst-1.3.0/rich_rst.egg-info/PKG-INFO` & `rich_rst-1.3.1/rich_rst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-rst
-Version: 1.3.0
+Version: 1.3.1
 Summary: A beautiful reStructuredText renderer for rich
 Home-page: https://wasi-master.github.io/rich-rst
 Author: Wasi Master
 Author-email: arianmollik323@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/wasi-master/rich-rst/issues
 Project-URL: Source, https://github.com/wasi-master/rich-rst
```

### Comparing `rich_rst-1.3.0/setup.cfg` & `rich_rst-1.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `rich_rst-1.3.0/tests/test_main.py` & `rich_rst-1.3.1/tests/test_main.py`

 * *Files identical despite different names*

