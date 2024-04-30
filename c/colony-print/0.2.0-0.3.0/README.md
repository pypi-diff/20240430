# Comparing `tmp/colony-print-0.2.0.tar.gz` & `tmp/colony-print-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/colony-print-0.2.0.tar", last modified: Sun May  7 15:55:20 2023, max compression
+gzip compressed data, was "dist/colony-print-0.3.0.tar", last modified: Tue Apr 30 14:28:37 2024, max compression
```

## Comparing `colony-print-0.2.0.tar` & `colony-print-0.3.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-07 15:55:20.000000 colony-print-0.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/static/example/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/static/example/js/
--rw-r--r--   0 root         (0) root         (0)     3555 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/static/example/js/main.js
--rw-r--r--   0 root         (0) root         (0)      594 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/static/example/print.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/static/example/xml/
--rw-r--r--   0 root         (0) root         (0)    26876 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/static/example/xml/money_sale_slip.xml
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/static/example/xml/hello.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/printing/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/printing/pdf/
--rw-r--r--   0 root         (0) root         (0)      973 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/pdf/system.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/pdf/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/pdf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33615 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/pdf/visitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/printing/manager/
--rw-r--r--   0 root         (0) root         (0)     4300 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/manager/system.py
--rw-r--r--   0 root         (0) root         (0)      870 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/manager/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2274 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/manager/ast.py
--rw-r--r--   0 root         (0) root         (0)      448 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/manager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2768 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/manager/visitor.py
--rw-r--r--   0 root         (0) root         (0)     7540 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/manager/parser.py
--rw-r--r--   0 root         (0) root         (0)      222 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/printing/binie/
--rw-r--r--   0 root         (0) root         (0)      879 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/binie/system.py
--rw-r--r--   0 root         (0) root         (0)      866 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/binie/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      263 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/binie/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20628 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/binie/visitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/printing/common/
--rw-r--r--   0 root         (0) root         (0)     2695 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/common/base.py
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/controllers/
--rw-r--r--   0 root         (0) root         (0)      115 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/controllers/base.py
--rw-r--r--   0 root         (0) root         (0)      995 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/controllers/printer.py
--rw-r--r--   0 root         (0) root         (0)     2794 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/controllers/document.py
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4965 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/controllers/node.py
--rw-r--r--   0 root         (0) root         (0)      534 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/main.py
--rw-r--r--   0 root         (0) root         (0)      206 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2474 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print.egg-info/
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1463 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     3515 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 15:55:15.000000 colony-print-0.2.0/src/colony_print.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     2067 2023-05-07 15:54:48.000000 colony-print-0.2.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     1945 2023-05-07 15:54:48.000000 colony-print-0.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)     3515 2023-05-07 15:55:20.000000 colony-print-0.2.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1979 2024-04-30 14:28:07.000000 colony-print-0.3.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2024-04-30 14:28:07.000000 colony-print-0.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-30 14:28:37.000000 colony-print-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4677 2024-04-30 14:28:37.000000 colony-print-0.3.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1463 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     4677 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 14:28:33.000000 colony-print-0.3.0/src/colony_print.egg-info/not-zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/printing/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/printing/binie/
+-rw-r--r--   0 root         (0) root         (0)      875 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/binie/system.py
+-rw-r--r--   0 root         (0) root         (0)      263 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/binie/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20906 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/binie/visitor.py
+-rw-r--r--   0 root         (0) root         (0)      870 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/binie/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/printing/manager/
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/manager/system.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/manager/ast.py
+-rw-r--r--   0 root         (0) root         (0)      488 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/manager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7810 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/manager/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/manager/visitor.py
+-rw-r--r--   0 root         (0) root         (0)      874 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/manager/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      222 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/printing/common/
+-rw-r--r--   0 root         (0) root         (0)     2712 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/common/base.py
+-rw-r--r--   0 root         (0) root         (0)      111 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/printing/pdf/
+-rw-r--r--   0 root         (0) root         (0)      969 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/pdf/system.py
+-rw-r--r--   0 root         (0) root         (0)      272 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/pdf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33965 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/pdf/visitor.py
+-rw-r--r--   0 root         (0) root         (0)     1462 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/printing/pdf/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/static/example/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/static/example/js/
+-rw-r--r--   0 root         (0) root         (0)     3555 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/static/example/js/main.js
+-rw-r--r--   0 root         (0) root         (0)      594 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/static/example/print.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/static/example/xml/
+-rw-r--r--   0 root         (0) root         (0)      251 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/static/example/xml/hello.xml
+-rw-r--r--   0 root         (0) root         (0)    26876 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/static/example/xml/money_sale_slip.xml
+-rw-r--r--   0 root         (0) root         (0)     3210 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/node.py
+-rw-r--r--   0 root         (0) root         (0)      206 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      461 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:28:37.000000 colony-print-0.3.0/src/colony_print/controllers/
+-rw-r--r--   0 root         (0) root         (0)      117 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/controllers/base.py
+-rw-r--r--   0 root         (0) root         (0)      981 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/controllers/printer.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/controllers/node.py
+-rw-r--r--   0 root         (0) root         (0)      285 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2790 2024-04-30 14:28:07.000000 colony-print-0.3.0/src/colony_print/controllers/document.py
```

### Comparing `colony-print-0.2.0/src/colony_print/static/example/js/main.js` & `colony-print-0.3.0/src/colony_print/static/example/js/main.js`

 * *Files identical despite different names*

### Comparing `colony-print-0.2.0/src/colony_print/static/example/print.html` & `colony-print-0.3.0/src/colony_print/static/example/print.html`

 * *Files identical despite different names*

### Comparing `colony-print-0.2.0/src/colony_print/static/example/xml/money_sale_slip.xml` & `colony-print-0.3.0/src/colony_print/static/example/xml/money_sale_slip.xml`

 * *Files identical despite different names*

### Comparing `colony-print-0.2.0/src/colony_print/printing/pdf/system.py` & `colony-print-0.3.0/src/colony_print/printing/pdf/system.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,31 +3,32 @@
 
 from . import visitor
 
 PRINTING_NAME = "pdf"
 """ The printing name, for the current PDF
 infra-structure (as defined in spec) """
 
+
 class PrintingPDF(object):
     """
     The printing PDF class, that is responsible for
     the handling of the logic for the printing of PDF
     files based on the XML template language.
     """
 
     def get_name(self):
         return PRINTING_NAME
 
-    def print_test(self, options = {}):
+    def print_test(self, options={}):
         pass
 
-    def print_test_image(self, image_path, options = {}):
+    def print_test_image(self, image_path, options={}):
         pass
 
-    def print_language(self, printing_document, options = {}):
+    def print_language(self, printing_document, options={}):
         # creates the PDF printing visitor then sets the
         # provided printing options in the visitor
         _visitor = visitor.Visitor()
         _visitor.set_options(options)
 
         # accepts the visitor in the printing document,
         # using double visiting mode
```

### Comparing `colony-print-0.2.0/src/colony_print/printing/pdf/exceptions.py` & `colony-print-0.3.0/src/colony_print/printing/pdf/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
+
 class PrintingPdfException(Exception):
     """
     The printing PDF exception class.
     """
 
     message = None
     """ The exception's message """
 
+
 class InvalidContextInformationName(PrintingPdfException):
     """
     The invalid context information name class.
     """
 
     def __init__(self, message):
         """
@@ -31,14 +33,15 @@
 
         :rtype: String
         :return: The string representation of the class.
         """
 
         return "Invalid context information name - %s" % self.message
 
+
 class InvalidFont(PrintingPdfException):
     """
     The invalid font class.
     """
 
     def __init__(self, message):
         """
```

### Comparing `colony-print-0.2.0/src/colony_print/printing/pdf/visitor.py` & `colony-print-0.3.0/src/colony_print/printing/pdf/visitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,24 +51,19 @@
     "accept_post_order",
     "add_child_node",
     "remove_child_node",
     "set_indent",
     "set_value",
     "indent",
     "value",
-    "child_nodes"
+    "child_nodes",
 ]
 """ The exclusion list """
 
-FONT_SUFFIX_MAP = {
-    "regular" : "",
-    "bold" : "b",
-    "italic" : "i",
-    "bold_italic" : "z"
-}
+FONT_SUFFIX_MAP = {"regular": "", "bold": "b", "italic": "i", "bold_italic": "z"}
 """ The map associating the type of font
 and the suffix to be appended to the name
 to created the full font name """
 
 DEFAULT_ENCODER = "utf-8"
 """ The default encoder """
 
@@ -94,14 +89,15 @@
 """ The default paper size to be used when no paper
 size value is defined for the print operation """
 
 FONT_PATHS = ("", "~/.fonts/", "/usr/share/fonts/truetype/")
 """ The set of base paths to be used for searching
 for fonts on the current system """
 
+
 class Visitor(object):
     """
     The visitor class for the PDF printing infra-structure
     this visitor should be able to generate a PDF file
     using the reportlab library as basics.
     """
 
@@ -179,15 +175,16 @@
         # iterates over all the name of the elements
         for self_class_element in self_class_elements:
             # retrieves the real element value
             self_class_real_element = getattr(self_class, self_class_element)
 
             # in case the current class real element does not contain
             # an AST node class reference must continue the loop
-            if not hasattr(self_class_real_element, "ast_node_class"): continue
+            if not hasattr(self_class_real_element, "ast_node_class"):
+                continue
 
             # retrieves the AST node class from the current class real element
             # and sets it in the node method map
             ast_node_class = getattr(self_class_real_element, "ast_node_class")
             self.node_method_map[ast_node_class] = self_class_real_element
 
     def get_options(self):
@@ -253,35 +250,30 @@
             # in case both the printing document with and height values are
             # available the size tuple for the current document is defined
             # using their values, note that these values are defined as tenth
             # of the millimeter values (100 units equals 1 centimeter)
             if not printing_document_width == 0 and not printing_document_height == 0:
                 size = (
                     printing_document_width / 100 * SCALE,
-                    printing_document_height / 100 * SCALE
+                    printing_document_height / 100 * SCALE,
                 )
 
             # unpacks the size tuple into the width and height
             # components and sets the tuple containing both values
             # as the size to be used for the document
             self.width, self.height = size
             self.size = (self.width, self.height)
 
             # creates the canvas object to be used as the primary
             # entry point for operation on the PDF
-            self.canvas = reportlab.pdfgen.canvas.Canvas(
-                file,
-                pagesize = self.size
-            )
+            self.canvas = reportlab.pdfgen.canvas.Canvas(file, pagesize=self.size)
 
             # sets the initial position so that the "virtual" cursor
             # position is situated at the top left corner of the page
-            self.current_position = (
-                0, self.height
-            )
+            self.current_position = (0, self.height)
 
         # in case it's the second visit
         elif self.visit_index == 1:
             # saves the final canvas structure flushing the data to
             # the associated file object, this is considered the final
             # operation for the creation of the PDF file
             self.canvas.save()
@@ -301,16 +293,18 @@
         # in case it's the second visit
         elif self.visit_index == 1:
             # removes the context information
             self.remove_context(node)
 
     @visited(Paragraph)
     def visit_paragraph(self, node):
-        if self.visit_index == 0: self.add_context(node)
-        elif self.visit_index == 1: self.remove_context(node)
+        if self.visit_index == 0:
+            self.add_context(node)
+        elif self.visit_index == 1:
+            self.remove_context(node)
 
     @visited(Line)
     def visit_line(self, node):
         if self.visit_index == 0:
             self.add_context(node)
             self.push_context("biggest_height", 0)
 
@@ -319,30 +313,31 @@
             margin_top = int(self.get_context("margin_top", "0"))
 
             # retrieves the current position in x and y
             # and then updates the current position
             current_position_x, current_position_y = self.current_position
             self.current_position = (
                 current_position_x,
-                current_position_y - margin_top * FONT_SCALE_FACTOR
+                current_position_y - margin_top * FONT_SCALE_FACTOR,
             )
 
         elif self.visit_index == 1:
             biggest_height = self.get_context("biggest_height")
             self.pop_context("biggest_height")
 
             # retrieves the margin bottom value defined
             # for the current context
             margin_bottom = int(self.get_context("margin_bottom", "0"))
 
             # retrieves the current position in x and y
             # and then updates the current position
             current_position_x, current_position_y = self.current_position
             self.current_position = (
-                0, current_position_y - biggest_height - margin_bottom * FONT_SCALE_FACTOR
+                0,
+                current_position_y - biggest_height - margin_bottom * FONT_SCALE_FACTOR,
             )
 
             # removes the context information
             self.remove_context(node)
 
     @visited(Text)
     def visit_text(self, node):
@@ -408,15 +403,15 @@
             self.ensure_font(font_name_c)
 
             # sets the complete computed font in the current canvas context
             # note that the leading value is overriden to avoid font sizing
             # problems in accordance with the printing language specification,
             # this is the "first" font setting and ensures that the measuring
             # of the font size is the correct one (required by algorithm)
-            self.canvas.setFont(font_name_c, font_size_r, leading = 1.0)
+            self.canvas.setFont(font_name_c, font_size_r, leading=1.0)
 
             # retrieves the current position in x and y unpacking the values
             # from the current position tuple (as expected)
             _current_position_x, current_position_y = self.current_position
 
             # calculates the text height from the font scale factor
             # and measures the text width using the underlying rendering
@@ -427,48 +422,52 @@
 
             # initializes the text x coordinate with the margin defined
             # for the current node (difference of margins)
             text_x = (margin_left - margin_right) * FONT_SCALE_FACTOR
 
             # calculates the appropriate text position according to the
             # "requested" horizontal text alignment
-            if text_align == "left": text_x += clip_left
-            elif text_align == "right": text_x += clip_right - text_width
+            if text_align == "left":
+                text_x += clip_left
+            elif text_align == "right":
+                text_x += clip_right - text_width
             elif text_align == "center":
-                text_x += clip_left + int((clip_right - clip_left) / 2) - int(text_width / 2)
+                text_x += (
+                    clip_left + int((clip_right - clip_left) / 2) - int(text_width / 2)
+                )
 
             # sets the text y as the current position context y
             # default position for the text is the current position
             text_y = clip_top + current_position_y - text_height_r
-            text_y = self.ensure_y(text_y, offset = text_height)
+            text_y = self.ensure_y(text_y, offset=text_height)
 
             # updates the fill color to a white color and then uses
             # this color to draw a white (background) rectangle around
             # the area that is going to be filled with the text
             self.canvas.setFillColorRGB(1.0, 1.0, 1.0)
             self.canvas.rect(
                 text_x,
                 text_y - (font_size - font_size_r),
                 text_width,
                 text_height,
-                stroke = 0,
-                fill = 1
+                stroke=0,
+                fill=1,
             )
 
             # "resets" the fill color of the current canvas context to
             # the black color so that it's possible to draw the text with
             # the expected color values as defined in specification
             self.canvas.setFillColorRGB(0, 0, 0)
 
             # sets the complete computed font in the current canvas context
             # note that the leading value is overriden to avoid font sizing
             # problems in accordance with the printing language specification,
             # the font must be set after the ensure vertical operation so that
             # in case a new page is created the new font is set correctly in it
-            self.canvas.setFont(font_name_c, font_size_r, leading = 1.0)
+            self.canvas.setFont(font_name_c, font_size_r, leading=1.0)
 
             # draws the text string at the calculated position the text
             # is encoded in the expected encoding so that no encoding
             # problems occur (as expected)
             self.canvas.drawString(text_x, text_y, text_encoded)
 
             # in case the current text height is bigger than the current
@@ -493,16 +492,18 @@
             # sets the default values for both the image path
             # and source, both values are unset by default
             image_path = None
             image_source = None
 
             # retrieves the path or source value to be used
             # in the retrieval (only one value is set)
-            if self.has_context("path"): image_path = self.get_context("path")
-            elif self.has_context("source"): image_source = self.get_context("source")
+            if self.has_context("path"):
+                image_path = self.get_context("path")
+            elif self.has_context("source"):
+                image_source = self.get_context("source")
 
             # retrieves the complete set of attributes for the current
             # context to be used for the processing of the node
             text_align = self.get_context("text_align")
             position_x = int(self.get_context("x", "0"))
             position_y = int(self.get_context("y", "0"))
             block_width = int(self.get_context("width", "0"))
@@ -559,59 +560,66 @@
 
             # retrieves the bitmap image width and height
             bitmap_image_width, bitmap_image_height = bitmap_image.size
 
             # creates a new image without transparency settings, so that
             # no extra color is used ands copies the bitmap image into it
             other_image = PIL.Image.new(
-                "RGB",
-                (bitmap_image_width, bitmap_image_height),
-                color = "white"
+                "RGB", (bitmap_image_width, bitmap_image_height), color="white"
             )
             other_image.paste(bitmap_image, bitmap_image)
 
             # retrieves the current position in x and y unpacking the values
             # from the current position tuple
             _current_position_x, current_position_y = self.current_position
 
             # calculates the appropriate bitmap position according to the
             # "requested" horizontal text alignment
-            if text_align == "left": real_bitmap_x = clip_left
+            if text_align == "left":
+                real_bitmap_x = clip_left
             elif text_align == "right":
                 real_bitmap_x = clip_right - bitmap_image_width * IMAGE_SCALE_FACTOR
             elif text_align == "center":
-                real_bitmap_x = clip_left + int((clip_right - clip_left) / 2) -\
-                    int(bitmap_image_width * IMAGE_SCALE_FACTOR / 2)
+                real_bitmap_x = (
+                    clip_left
+                    + int((clip_right - clip_left) / 2)
+                    - int(bitmap_image_width * IMAGE_SCALE_FACTOR / 2)
+                )
 
             # calculates the real bitmap vertical position from the current
             # vertical position minus the height of the image and ensures the
             # position, recalculating a new y position in case the page overflows
-            real_bitmap_y = clip_top + current_position_y - (bitmap_image_height * IMAGE_SCALE_FACTOR)
+            real_bitmap_y = (
+                clip_top
+                + current_position_y
+                - (bitmap_image_height * IMAGE_SCALE_FACTOR)
+            )
             real_bitmap_y = self.ensure_y(
-                real_bitmap_y,
-                offset = bitmap_image_height * IMAGE_SCALE_FACTOR
+                real_bitmap_y, offset=bitmap_image_height * IMAGE_SCALE_FACTOR
             )
 
             # loads the image image using the proper image reader structure
             # and uses the structure to "draw" the image into the canvas at
             # the current position
             image_reader = reportlab.lib.utils.ImageReader(other_image)
             self.canvas.drawImage(
                 image_reader,
                 real_bitmap_x,
                 real_bitmap_y,
                 bitmap_image_width * IMAGE_SCALE_FACTOR,
-                bitmap_image_height * IMAGE_SCALE_FACTOR
+                bitmap_image_height * IMAGE_SCALE_FACTOR,
             )
 
             # in case the current image height is bigger than the current
             # context biggest height, updates the information
             biggest_height = self.get_context("biggest_height")
             if biggest_height < bitmap_image_height * IMAGE_SCALE_FACTOR:
-                self.put_context("biggest_height", bitmap_image_height * IMAGE_SCALE_FACTOR)
+                self.put_context(
+                    "biggest_height", bitmap_image_height * IMAGE_SCALE_FACTOR
+                )
 
         elif self.visit_index == 1:
             self.remove_context(node)
 
     def ensure_y(self, y_position, offset):
         """
         Ensures that the provided vertical position is valid for
@@ -631,22 +639,24 @@
         :return: The resulting vertical position taking into account
         creation of new pages.
         """
 
         # in case the current document in parsing has been marked
         # as single page oriented (absolute positioning), there's
         # no need to verify for new page creation
-        if self.single: return y_position
+        if self.single:
+            return y_position
 
         # verifies if the current vertical position "overflows"
         # the page value (lower than zero) in case it does not
         # returns immediately with the provided position (no
         # overflow has occurred)
         b_position = y_position - offset
-        if b_position >= 0.0: return y_position
+        if b_position >= 0.0:
+            return y_position
 
         # calculates the delta position (inside the new page)
         # according to the current y position in case it's positive
         # it should be ignored otherwise uses it as the offset
         d_position = 0.0 if y_position >= 0.0 else y_position
 
         # updates the current position with the initial top left
@@ -658,15 +668,15 @@
 
         # shows a new page in the current canvas (creating a new
         # page) and then returns the new vertical position to the
         # caller method
         self.canvas.showPage()
         return y_position
 
-    def ensure_font(self, font_name, file_path = None):
+    def ensure_font(self, font_name, file_path=None):
         """
         Ensures that the font is present in the current
         canvas object, loading it into the PDF context
         in case it's required.
 
         The provided file path may be an absolute path
         or a relative (file name) to the system's default
@@ -683,15 +693,16 @@
 
         import reportlab.pdfbase.ttfonts
         import reportlab.pdfbase.pdfmetrics
 
         # in case the font is already present in the fonts
         # map it's considered to be loaded and so the control
         # must be returned immediately
-        if font_name in self.fonts: return
+        if font_name in self.fonts:
+            return
 
         # converts the font name into a lower cased version and
         # then uses it to create the default font path in case
         # none is provided (uses the default true type extension)
         font_name_l = font_name.lower()
         file_path = file_path or font_name_l + ".ttf"
 
@@ -721,17 +732,18 @@
             else:
                 error = False
                 break
 
         # in case the error flag is set raises the invalid font
         # exception, indicating that it was not possible to load
         # the associated font file
-        if error: raise exceptions.InvalidFont(
-            "not possible to load '%s' - '%s'" % (font_name, file_path)
-        )
+        if error:
+            raise exceptions.InvalidFont(
+                "not possible to load '%s' - '%s'" % (font_name, file_path)
+            )
 
         # updates the fonts map so that the current font is associated
         # with the corresponding loaded file path, this marks the
         # font as loaded for the current context
         self.fonts[font_name] = file_path
 
     def get_current_position_context(self):
@@ -746,37 +758,44 @@
 
         # retrieves the current position in x and y
         current_position_x, current_position_y = self.current_position
 
         # converts the current position to context
         current_position_context = (
             FONT_SCALE_FACTOR * current_position_x,
-            -1 * FONT_SCALE_FACTOR * current_position_y
+            -1 * FONT_SCALE_FACTOR * current_position_y,
         )
 
         # returns the current position context
         return current_position_context
 
-    def get_context(self, context_name, default = None):
+    def get_context(self, context_name, default=None):
         if not self.has_context(context_name):
-            if not default == None: return default
+            if not default == None:
+                return default
             raise exceptions.InvalidContextInformationName(
                 "the context information name: " + context_name + " is invalid"
             )
 
         return self.peek_context(context_name)
 
     def add_context(self, node):
-        valid_attributes = [(value, getattr(node, value)) for value in dir(node) if not value in EXCLUSION_LIST]
+        valid_attributes = [
+            (value, getattr(node, value))
+            for value in dir(node)
+            if not value in EXCLUSION_LIST
+        ]
 
         for valid_attribute_name, valid_attribute_value in valid_attributes:
             self.push_context(valid_attribute_name, valid_attribute_value)
 
     def remove_context(self, node):
-        valid_attribute_names = [value for value in dir(node) if not value in EXCLUSION_LIST]
+        valid_attribute_names = [
+            value for value in dir(node) if not value in EXCLUSION_LIST
+        ]
 
         for valid_attribute_name in valid_attribute_names:
             self.pop_context(valid_attribute_name)
 
     def push_context(self, context_name, context_value):
         if not context_name in self.context_map:
             self.context_map[context_name] = []
@@ -830,10 +849,11 @@
         :rtype: bool
         :return: If the context information name exists in the
         current context information map (and is valid).
         """
 
         # in case the context information name exists in the
         # context information map and is not invalid
-        if context_name in self.context_map and\
-            self.context_map[context_name]: return True
-        else: return False
+        if context_name in self.context_map and self.context_map[context_name]:
+            return True
+        else:
+            return False
```

### Comparing `colony-print-0.2.0/src/colony_print/printing/manager/system.py` & `colony-print-0.3.0/src/colony_print/printing/manager/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from . import parser
 from . import exceptions
 
 TEST_IMAGE_PATH = "resources/test_logo.png"
 """ The test image relative path to the current
 file path (considered the base path) """
 
+
 class PrintingManager(object):
     """
     The printing manager class, that is responsible for the
     top level handling of the printing operations.
     """
 
     handlers_map = {}
@@ -24,30 +25,31 @@
     that may be used for printing processing """
 
     def __init__(self):
         self.handlers_map = {}
 
     def load(self):
         import colony_print
+
         pdf_handler = colony_print.PrintingPDF()
         binie_handler = colony_print.PrintingBinie()
         self.load_handler(pdf_handler)
         self.load_handler(binie_handler)
 
     def unload(self):
         for _name, handler in appier.legacy.items(self.handlers_map):
             self.unload_handler(handler)
 
-    def print_test(self, options = {}):
+    def print_test(self, options={}):
         # retrieves the proper handler using the provided map of options
         # and then uses the same options to run a test print operation
         handler = self._get_handler(options)
         handler.print_test(options)
 
-    def print_test_image(self, options = {}):
+    def print_test_image(self, options={}):
         # retrieves the complete path for the current file and then
         # retrieves it's directory path, to be used in the calculus
         # of the image path to be used
         file_path = os.path.realpath(__file__)
         base_path = os.path.dirname(file_path)
 
         # creates the complete image path using the calculated base
@@ -56,15 +58,15 @@
         image_path = os.path.join(base_path, TEST_IMAGE_PATH)
 
         # retrieves the proper printing handler for the provided options
         # and then uses it to print the test image in the calculated path
         handler = self._get_handler(options)
         handler.print_test_image(image_path, options)
 
-    def print_language(self, data, options = {}):
+    def print_language(self, data, options={}):
         # creates a new printing language parser and sets the
         # proper data in it running then the parse string operation
         # that is going to be parsing the provided string
         _parser = parser.PrintingLanguageParser()
         _parser.string = data
         _parser.parse_string()
 
@@ -90,15 +92,16 @@
         printing_name = handler.get_name()
         del self.handlers_map[printing_name]
 
     def _get_handler(self, options):
         # retrieves the printing name (engine) from the printing options
         # this value is going to be used to select the proper handler
         printing_name = options.get("name", None)
-        if not printing_name: raise exceptions.PrintingPluginNotAvailable("missing name")
+        if not printing_name:
+            raise exceptions.PrintingPluginNotAvailable("missing name")
 
         # tries to retrieve the proper handler for the requested name that
         # exists in the handlers map in case it's not available raises an
         # exception indicating the problem
         handler = self.handlers_map.get(printing_name, None)
         if not handler:
             raise exceptions.PrintingPluginNotAvailable("no handler for requested name")
```

### Comparing `colony-print-0.2.0/src/colony_print/printing/manager/exceptions.py` & `colony-print-0.3.0/src/colony_print/printing/manager/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
+
 class PrintingManagerException(Exception):
     """
     The printing manager exception class.
     """
 
     message = None
     """ The exception's message """
 
+
 class PrintingPluginNotAvailable(PrintingManagerException):
     """
     The printing plugin not available name class.
     """
 
     def __init__(self, message):
         """
```

### Comparing `colony-print-0.2.0/src/colony_print/printing/manager/ast.py` & `colony-print-0.3.0/src/colony_print/printing/manager/ast.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
+
 class AstNode(object):
     """
     The AST node class, that represents a generic node
     to be percolated as part of the AST (abstract syntax tree).
     """
 
     value = None
@@ -16,15 +17,18 @@
     child_nodes = []
     """ The list of child nodes """
 
     def __init__(self):
         self.child_nodes = []
 
     def __repr__(self):
-        return "<ast_node indent:%s child_nodes:%s>" % (self.indent, len(self.child_nodes))
+        return "<ast_node indent:%s child_nodes:%s>" % (
+            self.indent,
+            len(self.child_nodes),
+        )
 
     def accept(self, visitor):
         visitor.visit(self)
 
         if visitor.visit_childs:
             for child_node in self.child_nodes:
                 child_node.accept(visitor)
@@ -55,44 +59,44 @@
 
     def add_child_node(self, child_node):
         self.child_nodes.append(child_node)
 
     def remove_child_node(self, child_node):
         self.child_nodes.remove(child_node)
 
-class GenericElement(AstNode):
 
+class GenericElement(AstNode):
     element_name = "none"
 
-    def __init__(self, element_name = "none"):
+    def __init__(self, element_name="none"):
         AstNode.__init__(self)
         self.element_name = element_name
 
-class PrintingDocument(AstNode):
 
+class PrintingDocument(AstNode):
     def __init__(self):
         AstNode.__init__(self)
 
-class Block(AstNode):
 
+class Block(AstNode):
     def __init__(self):
         AstNode.__init__(self)
 
-class Paragraph(AstNode):
 
+class Paragraph(AstNode):
     def __init__(self):
         AstNode.__init__(self)
 
-class Line(AstNode):
 
+class Line(AstNode):
     def __init__(self):
         AstNode.__init__(self)
 
-class Text(AstNode):
 
+class Text(AstNode):
     def __init__(self):
         AstNode.__init__(self)
 
-class Image(AstNode):
 
+class Image(AstNode):
     def __init__(self):
         AstNode.__init__(self)
```

### Comparing `colony-print-0.2.0/src/colony_print/printing/manager/visitor.py` & `colony-print-0.3.0/src/colony_print/printing/manager/visitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 from . import ast
 
 from ..common.base import *
 
+
 class Visitor(object):
     """
     The visitor class.
     """
 
     node_method_map = {}
     """ The node method map """
@@ -40,15 +41,16 @@
         # iterates over all the name of the elements
         for self_class_element in self_class_elements:
             # retrieves the real element value
             self_class_real_element = getattr(self_class, self_class_element)
 
             # in case the current class real element does not contain
             # an AST node class reference must continue the loop
-            if not hasattr(self_class_real_element, "ast_node_class"): continue
+            if not hasattr(self_class_real_element, "ast_node_class"):
+                continue
 
             # retrieves the AST node class from the current class real element
             # and sets it in the node method map
             ast_node_class = getattr(self_class_real_element, "ast_node_class")
             self.node_method_map[ast_node_class] = self_class_real_element
 
     @dispatch_visit()
```

### Comparing `colony-print-0.2.0/src/colony_print/printing/manager/parser.py` & `colony-print-0.3.0/src/colony_print/printing/manager/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import xml.dom.minidom
 
 from . import ast
 
 DEFAULT_CHARSET = "utf-8"
 """ The default charset """
 
+
 class Parser(object):
     """
     The abstract parser class
     """
 
     def __init__(self):
         """
@@ -44,29 +45,30 @@
 
         for index in range(attributes.length):
             attribute_node = attributes.item(index)
             attribute_node_name = attribute_node.name
             attribute_node_value = attribute_node.value
             setattr(element, attribute_node_name, attribute_node_value)
 
+
 class PrintingLanguageParser(Parser):
     """
     The printing language parser class.
     """
 
     file = None
     """ The file path """
 
     string = None
     """ The string contents """
 
     printing_document = None
     """ The printing document """
 
-    def __init__(self, file = None, string = "none"):
+    def __init__(self, file=None, string="none"):
         Parser.__init__(self)
         self.file = file
         self.string = string
 
     def parse(self):
         self.load_printing_language_file(self.file)
 
@@ -84,15 +86,19 @@
         xml_document = xml.dom.minidom.parse(file)
 
         self.load_printing_language(xml_document)
 
     def load_printing_language_string(self, string):
         # creates the XML document DOM object, the provided
         # string is encoded to avoid possible parsing problems
-        string = type(string) == appier.legacy.UNICODE and string.encode(DEFAULT_CHARSET) or string
+        string = (
+            type(string) == appier.legacy.UNICODE
+            and string.encode(DEFAULT_CHARSET)
+            or string
+        )
         xml_document = xml.dom.minidom.parseString(string)
 
         self.load_printing_language(xml_document)
 
     def load_printing_language(self, xml_document):
         child_nodes = xml_document.childNodes
 
@@ -105,32 +111,46 @@
         child_nodes = printing_document.childNodes
 
         # parses the element attributes
         self.parse_element_attributes(printing_document, printing_document_structure)
 
         for child_node in child_nodes:
             if valid_node(child_node):
-                self.parse_printing_document_element(child_node, printing_document_structure)
+                self.parse_printing_document_element(
+                    child_node, printing_document_structure
+                )
 
         return printing_document_structure
 
-    def parse_printing_document_element(self, printing_document_element, printing_document):
+    def parse_printing_document_element(
+        self, printing_document_element, printing_document
+    ):
         node_name = printing_document_element.nodeName
         printing_document_child_nodes = printing_document.child_nodes
 
         if node_name == "block":
-            printing_document_child_nodes.append(self.parse_block(printing_document_element))
+            printing_document_child_nodes.append(
+                self.parse_block(printing_document_element)
+            )
         elif node_name == "paragraph":
-            printing_document_child_nodes.append(self.parse_paragraph(printing_document_element))
+            printing_document_child_nodes.append(
+                self.parse_paragraph(printing_document_element)
+            )
         elif node_name == "line":
-            printing_document_child_nodes.append(self.parse_line(printing_document_element))
+            printing_document_child_nodes.append(
+                self.parse_line(printing_document_element)
+            )
         elif node_name == "text":
-            printing_document_child_nodes.append(self.parse_text(printing_document_element))
+            printing_document_child_nodes.append(
+                self.parse_text(printing_document_element)
+            )
         elif node_name == "image":
-            printing_document_child_nodes.append(self.parse_image(printing_document_element))
+            printing_document_child_nodes.append(
+                self.parse_image(printing_document_element)
+            )
 
     def parse_block(self, block):
         block_structure = ast.Block()
         child_nodes = block.childNodes
 
         # parses the element attributes
         self.parse_element_attributes(block, block_structure)
@@ -213,14 +233,15 @@
         image_structure = ast.Image()
 
         # parses the element attributes
         self.parse_element_attributes(image, image_structure)
 
         return image_structure
 
+
 def valid_node(node):
     """
     Gets if a node is valid or not for parsing.
 
     :type node: Node
     :param node: The Xml node to be validated.
     :rtype: bool
```

### Comparing `colony-print-0.2.0/src/colony_print/printing/binie/system.py` & `colony-print-0.3.0/src/colony_print/printing/binie/system.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,30 +2,31 @@
 # -*- coding: utf-8 -*-
 
 from . import visitor
 
 PRINTING_NAME = "binie"
 """ The printing name """
 
+
 class PrintingBinie(object):
     """
     The printing binie class, responsible for the handling
     of the front-end of the printing to binie support.
     """
 
     def get_name(self):
         return PRINTING_NAME
 
-    def print_test(self, options = {}):
+    def print_test(self, options={}):
         pass
 
-    def print_test_image(self, image_path, options = {}):
+    def print_test_image(self, image_path, options={}):
         pass
 
-    def print_language(self, printing_document, options = {}):
+    def print_language(self, printing_document, options={}):
         # creates the PDF printing visitor then sets the
         # provided printing options in the visitor
         _visitor = visitor.Visitor()
         _visitor.set_options(options)
 
         # accepts the visitor in the printing document,
         # using double visiting mode
```

### Comparing `colony-print-0.2.0/src/colony_print/printing/binie/exceptions.py` & `colony-print-0.3.0/src/colony_print/printing/binie/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
+
 class PrintingBinieException(Exception):
     """
     The printing binie exception class.
     """
 
     message = None
     """ The exception's message """
 
+
 class InvalidContextInformationName(PrintingBinieException):
     """
     The invalid context information name class.
     """
 
     def __init__(self, message):
         """
```

### Comparing `colony-print-0.2.0/src/colony_print/printing/binie/visitor.py` & `colony-print-0.3.0/src/colony_print/printing/binie/visitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,21 +42,22 @@
     "accept_post_order",
     "add_child_node",
     "remove_child_node",
     "set_indent",
     "set_value",
     "indent",
     "value",
-    "child_nodes"
+    "child_nodes",
 ]
 """ The exclusion list """
 
 DEFAULT_ENCODER = "utf-8"
 """ The default encoder """
 
+
 class Visitor(object):
     """
     The visitor class.
     """
 
     node_method_map = {}
     """ The node method map """
@@ -104,15 +105,16 @@
         # iterates over all the name of the elements
         for self_class_element in self_class_elements:
             # retrieves the real element value
             self_class_real_element = getattr(self_class, self_class_element)
 
             # in case the current class real element does not contain
             # an AST node class reference must continue the loop
-            if not hasattr(self_class_real_element, "ast_node_class"): continue
+            if not hasattr(self_class_real_element, "ast_node_class"):
+                continue
 
             # retrieves the AST node class from the current class real element
             # and sets it in the node method map
             ast_node_class = getattr(self_class_real_element, "ast_node_class")
             self.node_method_map[ast_node_class] = self_class_real_element
 
     def get_options(self):
@@ -164,17 +166,15 @@
             # retrieves the printing document name
             printing_document_name = node.name
 
             # resets the list of elements in the document
             self.elements_list = []
 
             # sets the initial position
-            self.current_position = (
-                0, 0
-            )
+            self.current_position = (0, 0)
         # in case it's the second visit
         elif self.visit_index == 1:
             # retrieves the printing document name and dimensions
             # to be able to update the structure
             printing_document_name = node.name
             printing_document_width = hasattr(node, "width") and int(node.width) or 0
             printing_document_height = hasattr(node, "height") and int(node.height) or 0
@@ -186,15 +186,15 @@
 
             # packs the header value as a binary string
             header = struct.pack(
                 "<256sIII",
                 printing_document_name,
                 printing_document_width,
                 printing_document_height,
-                len(self.elements_list)
+                len(self.elements_list),
             )
             self.options["file"].write(header)
 
             # iterates over all the elements list to create their header
             # and then add the element data
             for element in self.elements_list:
                 # unpacks the element into the type and its
@@ -224,16 +224,18 @@
         # in case it's the second visit
         elif self.visit_index == 1:
             # removes the context information
             self.remove_context(node)
 
     @visited(Paragraph)
     def visit_paragraph(self, node):
-        if self.visit_index == 0: self.add_context(node)
-        elif self.visit_index == 1: self.remove_context(node)
+        if self.visit_index == 0:
+            self.add_context(node)
+        elif self.visit_index == 1:
+            self.remove_context(node)
 
     @visited(Line)
     def visit_line(self, node):
         if self.visit_index == 0:
             self.add_context(node)
             self.push_context("biggest_height", 0)
 
@@ -242,30 +244,31 @@
             margin_top = int(self.get_context("margin_top", "0"))
 
             # retrieves the current position in x and y
             # and then updates the current position
             current_position_x, current_position_y = self.current_position
             self.current_position = (
                 current_position_x,
-                current_position_y - margin_top * FONT_SCALE_FACTOR
+                current_position_y - margin_top * FONT_SCALE_FACTOR,
             )
 
         elif self.visit_index == 1:
             biggest_height = self.get_context("biggest_height")
             self.pop_context("biggest_height")
 
             # retrieves the margin bottom value defined
             # for the current context
             margin_bottom = int(self.get_context("margin_bottom", "0"))
 
             # retrieves the current position in x and y
             # and then updates the current position
             current_position_x, current_position_y = self.current_position
             self.current_position = (
-                0, current_position_y - biggest_height - margin_bottom * FONT_SCALE_FACTOR
+                0,
+                current_position_y - biggest_height - margin_bottom * FONT_SCALE_FACTOR,
             )
 
             # removes the context information
             self.remove_context(node)
 
     @visited(Text)
     def visit_text(self, node):
@@ -307,17 +310,20 @@
                 text_italic_int = 1
 
             # retrieves the current position in x and y
             _current_position_x, _current_position_y = self.current_position
 
             # converts the provided text align value into the
             # appropriate integer value representing it
-            if text_align == "left": text_align_int = 1
-            elif text_align == "right": text_align_int = 2
-            elif text_align == "center": text_align_int = 3
+            if text_align == "left":
+                text_align_int = 1
+            elif text_align == "right":
+                text_align_int = 2
+            elif text_align == "center":
+                text_align_int = 3
 
             # calculates the text height from the font scale factor
             text_height = font_size * FONT_SCALE_FACTOR
 
             # packs the element text element structure containing all the meta
             # information that makes part of it then adds the "just" created
             # element to the elements list
@@ -332,15 +338,15 @@
                 text_italic_int,
                 margin_left,
                 margin_right,
                 position_x,
                 position_y,
                 block_width,
                 block_height,
-                len(text_encoded) + 1
+                len(text_encoded) + 1,
             )
             element += text_encoded
             element += b"\0"
             self.elements_list.append((1, element))
 
             # in case the current text height is bigger than the current
             # context biggest height, updates the information
@@ -362,16 +368,18 @@
             # sets the default values for both the image path
             # and source, both values are unset by default
             image_path = None
             image_source = None
 
             # retrieves the path or source value to be used
             # in the retrieval (only one value is set)
-            if self.has_context("path"): image_path = self.get_context("path")
-            elif self.has_context("source"): image_source = self.get_context("source")
+            if self.has_context("path"):
+                image_path = self.get_context("path")
+            elif self.has_context("source"):
+                image_source = self.get_context("source")
 
             # retrieves the complete set of attributes for the current
             # context to be used for the processing of the node
             text_align = self.get_context("text_align")
             position_x = int(self.get_context("x", "0"))
             position_y = int(self.get_context("y", "0"))
             block_width = int(self.get_context("width", "0"))
@@ -401,28 +409,29 @@
 
             # retrieves the bitmap image width and height
             bitmap_image_width, bitmap_image_height = bitmap_image.size
 
             # creates a new image without transparency settings, so that
             # no extra color is used ands copies the bitmap image into it
             other_image = PIL.Image.new(
-                "RGB",
-                (bitmap_image_width, bitmap_image_height),
-                color = "white"
+                "RGB", (bitmap_image_width, bitmap_image_height), color="white"
             )
             other_image.paste(bitmap_image, bitmap_image)
 
             # retrieves the current position in x and y
             _current_position_x, current_position_y = self.current_position
 
             # converts the provided text align value into the
             # appropriate integer value representing it
-            if text_align == "left": text_align_int = 1
-            elif text_align == "right": text_align_int = 2
-            elif text_align == "center": text_align_int = 3
+            if text_align == "left":
+                text_align_int = 1
+            elif text_align == "right":
+                text_align_int = 2
+            elif text_align == "center":
+                text_align_int = 3
 
             # sets the real bitmap image height as the bitmap
             # image height (value copy)
             real_bitmap_image_height = bitmap_image_height
 
             # creates a new string buffer for the image
             string_buffer = appier.legacy.BytesIO()
@@ -440,22 +449,24 @@
                 0,
                 current_position_y,
                 text_align_int,
                 position_x,
                 position_y,
                 block_width,
                 block_height,
-                len(buffer)
+                len(buffer),
             )
             element += buffer
             self.elements_list.append((2, element))
 
             biggest_height = self.get_context("biggest_height")
             if biggest_height < real_bitmap_image_height * IMAGE_SCALE_FACTOR:
-                self.put_context("biggest_height", real_bitmap_image_height * IMAGE_SCALE_FACTOR)
+                self.put_context(
+                    "biggest_height", real_bitmap_image_height * IMAGE_SCALE_FACTOR
+                )
 
         elif self.visit_index == 1:
             self.remove_context(node)
 
     def get_current_position_context(self):
         """
         Retrieves the current position based on the current
@@ -468,37 +479,44 @@
 
         # retrieves the current position in x and y
         current_position_x, current_position_y = self.current_position
 
         # converts the current position to context
         current_position_context = (
             FONT_SCALE_FACTOR * current_position_x,
-            -1 * FONT_SCALE_FACTOR * current_position_y
+            -1 * FONT_SCALE_FACTOR * current_position_y,
         )
 
         # returns the current position context
         return current_position_context
 
-    def get_context(self, context_name, default = None):
+    def get_context(self, context_name, default=None):
         if not self.has_context(context_name):
-            if not default == None: return default
+            if not default == None:
+                return default
             raise exceptions.InvalidContextInformationName(
                 "the context information name: " + context_name + " is invalid"
             )
 
         return self.peek_context(context_name)
 
     def add_context(self, node):
-        valid_attributes = [(value, getattr(node, value)) for value in dir(node) if value not in EXCLUSION_LIST]
+        valid_attributes = [
+            (value, getattr(node, value))
+            for value in dir(node)
+            if value not in EXCLUSION_LIST
+        ]
 
         for valid_attribute_name, valid_attribute_value in valid_attributes:
             self.push_context(valid_attribute_name, valid_attribute_value)
 
     def remove_context(self, node):
-        valid_attribute_names = [value for value in dir(node) if value not in EXCLUSION_LIST]
+        valid_attribute_names = [
+            value for value in dir(node) if value not in EXCLUSION_LIST
+        ]
 
         for valid_attribute_name in valid_attribute_names:
             self.pop_context(valid_attribute_name)
 
     def push_context(self, context_name, context_value):
         if not context_name in self.context_map:
             self.context_map[context_name] = []
@@ -552,10 +570,11 @@
         :rtype: bool
         :return: If the context information name exists in the
         current context information map (and is valid).
         """
 
         # in case the context information name exists in the
         # context information map and is not invalid
-        if context_name in self.context_map and\
-            self.context_map[context_name]: return True
-        else: return False
+        if context_name in self.context_map and self.context_map[context_name]:
+            return True
+        else:
+            return False
```

### Comparing `colony-print-0.2.0/src/colony_print/printing/common/base.py` & `colony-print-0.3.0/src/colony_print/printing/common/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
-def visited(ast_node_class):
 
+def visited(ast_node_class):
     def decorator(function, *args, **kwargs):
         function.ast_node_class = ast_node_class
         return function
 
     return decorator
 
-def dispatch_visit(map_name = "node_method_map"):
 
+def dispatch_visit(map_name="node_method_map"):
     def create_interceptor(function):
-
         def decorator_interceptor(*args, **kwargs):
             # unpacks the first two "unnamed" arguments as the self
             # instance reference and the node element to be visited
             self = args[0]
             node = args[1]
 
             # verifies if the current instance contains the node method
@@ -33,15 +32,16 @@
 
             # iterates over the complete class hierarchy for the provided
             # node (from bottom to up) so that the best match for the
             # visit operation is found and properly called
             for mro_item in mro:
                 # in case the current mro item class level is nor found
                 # skips the current iteration (cannot visit at this level)
-                if not mro_item in node_method_map: continue
+                if not mro_item in node_method_map:
+                    continue
 
                 # the current class level is valid and so the proper method
                 # is retrieved from the map and then called with the provided
                 # arguments, note that a before visit and an after visit calls
                 # are done so that proper "notification" exists
                 visit_method = node_method_map[mro_item]
                 self.before_visit(*args[1:], **kwargs)
```

### Comparing `colony-print-0.2.0/src/colony_print/controllers/printer.py` & `colony-print-0.3.0/src/colony_print/controllers/printer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 import appier
 
-class PrinterController(appier.Controller):
 
-    @appier.route("/printers", "GET", json = True)
-    @appier.ensure(token = "admin")
+class PrinterController(appier.Controller):
+    @appier.route("/printers", "GET", json=True)
+    @appier.ensure(token="admin")
     def list(self):
         return self.npcolony.get_devices()
 
-    @appier.route("/printers/hello", "GET", json = True)
-    @appier.ensure(token = "admin")
+    @appier.route("/printers/hello", "GET", json=True)
+    @appier.ensure(token="admin")
     def hello(self):
         self.npcolony.print_hello()
 
-    @appier.route("/printers/print", "GET", json = True)
-    @appier.ensure(token = "admin")
+    @appier.route("/printers/print", "GET", json=True)
+    @appier.ensure(token="admin")
     def print_document_f(self):
         printer = self.field("printer")
         return self.print_document(printer)
 
-    @appier.route("/printers/<str:printer>/print", ("GET", "POST"), json = True)
-    @appier.ensure(token = "admin")
+    @appier.route("/printers/<str:printer>/print", ("GET", "POST"), json=True)
+    @appier.ensure(token="admin")
     def print_document(self, printer):
         data_b64 = self.field("data_b64")
         self.npcolony.print_printer_base64(printer, data_b64)
 
     @property
     def npcolony(self):
         import npcolony
+
         return npcolony
```

### Comparing `colony-print-0.2.0/src/colony_print/controllers/document.py` & `colony-print-0.3.0/src/colony_print/controllers/document.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 import base64
 
 import appier
 
-MIME = dict(
-    binie = "text/x-binie",
-    pdf = "application/pdf"
-)
+MIME = dict(binie="text/x-binie", pdf="application/pdf")
 """ Map defining the association between the print
 format naming and the associated base mime type value
 (note that this value may be complemented with base64) """
 
-EXAMPLE = "<?xml version=\"1.0\" encoding=\"UTF-8\"?>\
-    <printing_document name=\"hello_world\" font=\"Calibri\" font_size=\"9\">\
-        <paragraph text_align=\"center\">\
+EXAMPLE = '<?xml version="1.0" encoding="UTF-8"?>\
+    <printing_document name="hello_world" font="Calibri" font_size="9">\
+        <paragraph text_align="center">\
             <line><text>Hello World</text></line>\
         </paragraph>\
-    </printing_document>"
+    </printing_document>'
 """ Example XML string that should display an hello world
-message using the XML printing language """
+message using the XML printing language (XMPL) """
 
-class DocumentController(appier.Controller):
 
+class DocumentController(appier.Controller):
     def __init__(self, owner, *args, **kwargs):
         appier.Controller.__init__(self, owner, *args, **kwargs)
         self.manager = None
 
     @appier.route("/documents/example.<format>", "GET")
     def example(self, format):
         return self.send_print(EXAMPLE, format)
 
     @appier.route("/documents.<format>", "POST")
     def convert(self, format):
         # retrieves the current request reference and then
-        # uses it to retrieve its "raw" data, that should
-        # contain the XML string for the generation of the
+        # uses it to retrieve its "raw" data, which should
+        # contain the XML string (XMPL) for the generation of the
         # of binie result and then sends the value for print
         request = self.get_request()
         data = request.get_data()
-        return self.send_print(data, format = format)
+        return self.send_print(data, format=format)
 
-    def send_print(self, data, format = "binie"):
+    def send_print(self, data, format="binie"):
         # retrieves the various optional fields for printing
         # and then parses them creating the composite values
         # (should include the size tuple)
-        b64 = self.field("base64", False, cast = bool)
-        width = self.field("width", 0.0, cast = float)
-        height = self.field("height", 0.0, cast = float)
+        b64 = self.field("base64", False, cast=bool)
+        width = self.field("width", 0.0, cast=float)
+        height = self.field("height", 0.0, cast=float)
         has_size = width > 0.0 and width > 0.0
 
-        mime = self.get_mime(format, b64 = base64)
+        mime = self.get_mime(format, b64=base64)
         manager = self.get_manager()
 
         data = data
         file = appier.legacy.BytesIO()
-        options = dict(name = format, file = file)
-        if has_size: options["size"] = (width, height)
+        options = dict(name=format, file=file)
+        if has_size:
+            options["size"] = (width, height)
 
         manager.print_language(data, options)
         value = file.getvalue()
         value = base64.b64encode(value) if b64 else value
 
         self.content_type(mime)
         return value
 
-    def get_mime(self, format, b64 = False):
+    def get_mime(self, format, b64=False):
         mime = MIME.get(format, "application/octet-stream")
         mime = mime + "-base64" if b64 else mime
         return mime
 
     def get_manager(self):
         import colony_print
-        if self.manager: return self.manager
+
+        if self.manager:
+            return self.manager
         self.manager = colony_print.PrintingManager()
         self.manager.load()
         return self.manager
```

### Comparing `colony-print-0.2.0/src/colony_print/controllers/node.py` & `colony-print-0.3.0/src/colony_print/controllers/node.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,113 +14,132 @@
 AAAAAAAABDYWxpYnJpAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\
 AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\
 AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\
 AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\
 AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACQAAAAMAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\
 AAAAAAAAAwAAABIZWxsbyBXb3JsZAA="
 
-class NodeController(appier.Controller):
 
-    @appier.route("/nodes", "GET", json = True)
-    @appier.ensure(token = "admin")
+class NodeController(appier.Controller):
+    @appier.route("/nodes", "GET", json=True)
+    @appier.ensure(token="admin")
     def list(self):
         return self.owner.nodes
 
-    @appier.route("/nodes/<str:id>", "POST", json = True)
-    @appier.ensure(token = "admin")
+    @appier.route("/nodes/<str:id>", "POST", json=True)
+    @appier.ensure(token="admin")
     def create(self, id):
         node = appier.get_object()
         self.owner.nodes[id] = node
 
-    @appier.route("/nodes/<str:id>", "GET", json = True)
-    @appier.ensure(token = "admin")
+    @appier.route("/nodes/<str:id>", "GET", json=True)
+    @appier.ensure(token="admin")
     def show(self, id):
         return self.owner.nodes[id]
 
-    @appier.route("/nodes/<str:id>/jobs", "GET", json = True)
-    @appier.ensure(token = "admin")
+    @appier.route("/nodes/<str:id>/jobs", "GET", json=True)
+    @appier.ensure(token="admin")
     def jobs(self, id):
         self.request.set_content_type("application/json")
-        for value in appier.header_a(): yield value
-        for value in self.wait_jobs(id): yield value
+        for value in appier.header_a():
+            yield value
+        for value in self.wait_jobs(id):
+            yield value
 
-    @appier.route("/nodes/<str:id>/jobs_peek", "GET", json = True)
-    @appier.ensure(token = "admin")
+    @appier.route("/nodes/<str:id>/jobs_peek", "GET", json=True)
+    @appier.ensure(token="admin")
     def jobs_peek(self, id):
         jobs = self.owner.jobs.get(id, [])
         return jobs
 
-    @appier.route("/nodes/<str:id>/print", ("GET", "POST"), json = True)
-    @appier.ensure(token = "admin")
+    @appier.route("/nodes/<str:id>/print", ("GET", "POST"), json=True)
+    @appier.ensure(token="admin")
     def print_default(self, id):
-        data_b64 = self.field("data_b64", mandatory = True, not_empty = True)
+        data_b64 = self.field("data_b64", mandatory=True, not_empty=True)
         name = self.field("name", None)
+        type = self.field("type", None)
+        options = self.field("options", None)
         name = name or str(uuid.uuid4())
-        job = dict(data_b64 = data_b64)
-        if name: job["name"] = name
+        job = dict(data_b64=data_b64)
+        if name:
+            job["name"] = name
+        if type:
+            job["type"] = type
+        if options:
+            job["options"] = options
         jobs = self.owner.jobs.get(id, [])
         jobs.append(job)
         self.owner.jobs[id] = jobs
         appier.notify("jobs:%s" % id)
 
     @appier.route("/nodes/<str:id>/print", "OPTIONS")
     def print_default_o(self, id):
         return ""
 
-    @appier.route("/nodes/<str:id>/print_hello", ("GET", "POST"), json = True)
-    @appier.ensure(token = "admin")
+    @appier.route("/nodes/<str:id>/print_hello", ("GET", "POST"), json=True)
+    @appier.ensure(token="admin")
     def print_hello_default(self, id):
         self.set_field("data_b64", HELLO_WORLD_B64)
         self.set_field("name", "hello_world")
         self.print_default(id)
 
-    @appier.route("/nodes/<str:id>/printers/print", ("GET", "POST"), json = True)
-    @appier.ensure(token = "admin")
+    @appier.route("/nodes/<str:id>/printers/print", ("GET", "POST"), json=True)
+    @appier.ensure(token="admin")
     def print_printer_f(self, id):
         printer = self.field("printer")
         return self.print_printer(id, printer)
 
     @appier.route("/nodes/<str:id>/printers/print", "OPTIONS")
     def print_printer_of(self, id):
         printer = self.field("printer")
         return self.print_printer_o(id, printer)
 
-    @appier.route("/nodes/<str:id>/printers/print_hello", ("GET", "POST"), json = True)
-    @appier.ensure(token = "admin")
+    @appier.route("/nodes/<str:id>/printers/print_hello", ("GET", "POST"), json=True)
+    @appier.ensure(token="admin")
     def print_hello_printer_f(self, id):
         printer = self.field("printer")
         return self.print_hello_printer(id, printer)
 
-    @appier.route("/nodes/<str:id>/printers/<str:printer>/print", ("GET", "POST"), json = True)
-    @appier.ensure(token = "admin")
+    @appier.route(
+        "/nodes/<str:id>/printers/<str:printer>/print", ("GET", "POST"), json=True
+    )
+    @appier.ensure(token="admin")
     def print_printer(self, id, printer):
-        data_b64 = self.field("data_b64", mandatory = True, not_empty = True)
+        data_b64 = self.field("data_b64", mandatory=True, not_empty=True)
         name = self.field("name", None)
+        type = self.field("type", None)
+        options = self.field("options", None)
         name = name or str(uuid.uuid4())
-        job = dict(
-            data_b64 = data_b64,
-            printer = printer
-        )
-        if name: job["name"] = name
+        job = dict(data_b64=data_b64, printer=printer)
+        if name:
+            job["name"] = name
+        if type:
+            job["type"] = type
+        if options:
+            job["options"] = options
         jobs = self.owner.jobs.get(id, [])
         jobs.append(job)
         self.owner.jobs[id] = jobs
         appier.notify("jobs:%s" % id)
 
     @appier.route("/nodes/<str:id>/printers/<str:printer>/print", "OPTIONS")
     def print_printer_o(self, id, printer):
         return ""
 
-    @appier.route("/nodes/<str:id>/printers/<str:printer>/print_hello", ("GET", "POST"), json = True)
-    @appier.ensure(token = "admin")
+    @appier.route(
+        "/nodes/<str:id>/printers/<str:printer>/print_hello", ("GET", "POST"), json=True
+    )
+    @appier.ensure(token="admin")
     def print_hello_printer(self, id, printer):
         self.set_field("data_b64", HELLO_WORLD_B64)
         self.set_field("name", "hello_world")
         self.print_printer(id, printer)
 
     @appier.coroutine
     def wait_jobs(self, id):
         while True:
             jobs = self.owner.jobs.pop(id, [])
-            if jobs: break
-            for value in appier.wait("jobs:%s" % id): yield value
+            if jobs:
+                break
+            for value in appier.wait("jobs:%s" % id):
+                yield value
         yield json.dumps(jobs)
```

### Comparing `colony-print-0.2.0/src/colony_print/node.py` & `colony-print-0.3.0/src/colony_print/node.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,73 +3,92 @@
 
 import time
 import logging
 
 import appier
 
 BASE_URL = "https://print.bemisc.com/"
+""" The default base URL to be used for the communication with the
+Colony Print server """
 
 SLEEP_TIME = 3.0
+""" The default time to sleep between each iteration, this value
+is used to avoid overloading the server with requests """
 
-class ColonyPrintNode(object):
 
-    def __init__(self, sleep_time = SLEEP_TIME):
+class ColonyPrintNode(object):
+    def __init__(self, sleep_time=SLEEP_TIME):
         self.sleep_time = sleep_time
 
     def loop(self):
         logging.basicConfig(
-            format = "%(asctime)s [%(levelname)s] %(message)s",
-            level = logging.DEBUG
+            format="%(asctime)s [%(levelname)s] %(message)s", level=logging.DEBUG
         )
 
         base_url = appier.conf("BASE_URL", BASE_URL)
         secret_key = appier.conf("SECRET_KEY", None)
         node_id = appier.conf("NODE_ID", "node")
         node_name = appier.conf("NODE_NAME", "node")
         node_location = appier.conf("NODE_LOCATION", "undefined")
 
         headers = dict()
-        if secret_key: headers["X-Secret-Key"] = secret_key
+        if secret_key:
+            headers["X-Secret-Key"] = secret_key
 
         while True:
             try:
                 logging.info("Submitting node information")
                 appier.post(
                     base_url + "nodes/%s" % node_id,
-                    data_j = dict(
-                        name = node_name,
-                        location = node_location
-                    ),
-                    headers = headers
+                    data_j=dict(name=node_name, location=node_location),
+                    headers=headers,
                 )
                 logging.info("Retrieving jobs for node '%s'" % node_id)
                 jobs = appier.get(
-                    base_url + "nodes/%s/jobs" % node_id,
-                    headers = headers,
-                    timeout = 600
+                    base_url + "nodes/%s/jobs" % node_id, headers=headers, timeout=600
                 )
                 logging.info("Retrieved %d jobs for node '%s'" % (len(jobs), node_id))
-                for job in jobs: self.print_job(job)
+                for job in jobs:
+                    self.print_job(job)
             except Exception as exception:
                 logging.info("Exception while looping '%s'" % str(exception))
                 logging.info("Sleeping for %.2f seconds" % self.sleep_time)
                 time.sleep(self.sleep_time)
 
     def print_job(self, job):
         data_b64 = job["data_b64"]
         name = job.get("name", "undefined")
         printer = job.get("printer", None)
+        format = job.get("format", None)
+        options = job.get("options", dict())
         printer_s = printer if printer else "default"
+
+        # tries to make sure that the format is compatible with the current
+        # system, this is required to avoid problems with the printing of the
+        # data in printers of the current system
+        if (
+            format
+            and hasattr(self.npcolony, "get_format")
+            and not format == self.npcolony.get_format()
+        ):
+            raise appier.OperationalError(
+                "Format '%s' not compatible with system" % format
+            )
+
         logging.info("Printing job '%s' with '%s' printer" % (name, printer_s))
-        if printer: self.npcolony.print_printer_base64(printer, data_b64)
-        else: self.npcolony.print_base64(data_b64)
+        if printer:
+            self.npcolony.print_printer_base64(printer, data_b64, options=options)
+        else:
+            self.npcolony.print_base64(data_b64)
 
     @property
     def npcolony(self):
         import npcolony
+
         return npcolony
 
+
 if __name__ == "__main__":
     node = ColonyPrintNode()
     node.loop()
 else:
     __path__ = []
```

### Comparing `colony-print-0.2.0/src/colony_print.egg-info/SOURCES.txt` & `colony-print-0.3.0/src/colony_print.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `colony-print-0.2.0/setup.py` & `colony-print-0.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,57 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 import os
 import setuptools
 
 setuptools.setup(
-    name = "colony-print",
-    version = "0.2.0",
-    author = "Hive Solutions Lda.",
-    author_email = "development@hive.pt",
-    description = "Colony Print Infra-structure",
-    license = "Apache License, Version 2.0",
-    keywords = "colony print native",
-    url = "http://colony-print.hive.pt",
-    zip_safe = False,
-    packages = [
+    name="colony-print",
+    version="0.3.0",
+    author="Hive Solutions Lda.",
+    author_email="development@hive.pt",
+    description="Colony Print Infra-structure",
+    license="Apache License, Version 2.0",
+    keywords="colony print native",
+    url="http://colony-print.hive.pt",
+    zip_safe=False,
+    packages=[
         "colony_print",
         "colony_print.controllers",
         "colony_print.printing",
         "colony_print.printing.binie",
         "colony_print.printing.common",
         "colony_print.printing.manager",
-        "colony_print.printing.pdf"
+        "colony_print.printing.pdf",
     ],
-    test_suite = "colony_print.test",
-    package_dir = {
-        "" : os.path.normpath("src")
-    },
-    package_data = {
-        "colony_print" : [
+    test_suite="colony_print.test",
+    package_dir={"": os.path.normpath("src")},
+    package_data={
+        "colony_print": [
             "static/example/*",
             "static/example/js/*",
-            "static/example/xml/*"
+            "static/example/xml/*",
         ]
     },
-    install_requires = [
-        "appier",
-        "appier-extras",
-        "jinja2",
-        "pillow",
-        "reportlab"
-    ],
-    classifiers = [
+    install_requires=["appier", "appier-extras", "jinja2", "pillow", "reportlab"],
+    classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Topic :: Utilities",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.6",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.0",
         "Programming Language :: Python :: 3.1",
         "Programming Language :: Python :: 3.2",
         "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7"
+        "Programming Language :: Python :: 3.7",
     ],
-    long_description = open(os.path.join(os.path.dirname(__file__), "README.md"), "rb").read().decode("utf-8"),
-    long_description_content_type = "text/markdown"
+    long_description=open(os.path.join(os.path.dirname(__file__), "README.md"), "rb")
+    .read()
+    .decode("utf-8"),
+    long_description_content_type="text/markdown",
 )
```

