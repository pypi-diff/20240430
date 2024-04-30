# Comparing `tmp/clear-html-0.4.0.tar.gz` & `tmp/clear_html-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear-html-0.4.0.tar", last modified: Tue Aug 29 07:12:23 2023, max compression
+gzip compressed data, was "clear_html-0.4.1.tar", last modified: Tue Apr 30 14:00:07 2024, max compression
```

## Comparing `clear-html-0.4.0.tar` & `clear_html-0.4.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 07:12:23.195807 clear-html-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (999)     1081 2023-08-29 07:12:04.000000 clear-html-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     4539 2023-08-29 07:12:23.195807 clear-html-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2455 2023-08-29 07:12:04.000000 clear-html-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 07:12:23.195807 clear-html-0.4.0/clear_html/
--rw-r--r--   0 runner    (1001) docker     (999)      110 2023-08-29 07:12:04.000000 clear-html-0.4.0/clear_html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1050 2023-08-29 07:12:04.000000 clear-html-0.4.0/clear_html/body_annotations.py
--rw-r--r--   0 runner    (1001) docker     (999)     2721 2023-08-29 07:12:04.000000 clear-html-0.4.0/clear_html/clean.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 07:12:23.195807 clear-html-0.4.0/clear_html/formatted_text/
--rw-r--r--   0 runner    (1001) docker     (999)     2269 2023-08-29 07:12:04.000000 clear-html-0.4.0/clear_html/formatted_text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3348 2023-08-29 07:12:04.000000 clear-html-0.4.0/clear_html/formatted_text/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (999)     4366 2023-08-29 07:12:04.000000 clear-html-0.4.0/clear_html/formatted_text/defs.py
--rw-r--r--   0 runner    (1001) docker     (999)    13418 2023-08-29 07:12:04.000000 clear-html-0.4.0/clear_html/formatted_text/figures.py
--rw-r--r--   0 runner    (1001) docker     (999)     1653 2023-08-29 07:12:04.000000 clear-html-0.4.0/clear_html/formatted_text/headings.py
--rw-r--r--   0 runner    (1001) docker     (999)     9310 2023-08-29 07:12:04.000000 clear-html-0.4.0/clear_html/formatted_text/main.py
--rw-r--r--   0 runner    (1001) docker     (999)    15588 2023-08-29 07:12:04.000000 clear-html-0.4.0/clear_html/formatted_text/utils.py
--rw-r--r--   0 runner    (1001) docker     (999)     2055 2023-08-29 07:12:04.000000 clear-html-0.4.0/clear_html/html_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (999)     6296 2023-08-29 07:12:04.000000 clear-html-0.4.0/clear_html/lxml_utils.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 07:12:04.000000 clear-html-0.4.0/clear_html/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 07:12:23.195807 clear-html-0.4.0/clear_html.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     4539 2023-08-29 07:12:23.000000 clear-html-0.4.0/clear_html.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      724 2023-08-29 07:12:23.000000 clear-html-0.4.0/clear_html.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-29 07:12:23.000000 clear-html-0.4.0/clear_html.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       43 2023-08-29 07:12:23.000000 clear-html-0.4.0/clear_html.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       11 2023-08-29 07:12:23.000000 clear-html-0.4.0/clear_html.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)     1427 2023-08-29 07:12:04.000000 clear-html-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)      137 2023-08-29 07:12:23.195807 clear-html-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 07:12:23.195807 clear-html-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (999)     2105 2023-08-29 07:12:04.000000 clear-html-0.4.0/tests/test_body_annotations.py
--rw-r--r--   0 runner    (1001) docker     (999)     1014 2023-08-29 07:12:04.000000 clear-html-0.4.0/tests/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (999)     9242 2023-08-29 07:12:04.000000 clear-html-0.4.0/tests/test_formatted_text.py
--rw-r--r--   0 runner    (1001) docker     (999)     2158 2023-08-29 07:12:04.000000 clear-html-0.4.0/tests/test_html_embeddings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:00:07.516429 clear_html-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-30 13:59:57.000000 clear_html-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-30 14:00:07.516429 clear_html-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-30 13:59:57.000000 clear_html-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:00:07.512429 clear_html-0.4.1/clear_html/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-30 13:59:57.000000 clear_html-0.4.1/clear_html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-30 13:59:57.000000 clear_html-0.4.1/clear_html/body_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-30 13:59:57.000000 clear_html-0.4.1/clear_html/clean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:00:07.516429 clear_html-0.4.1/clear_html/formatted_text/
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-30 13:59:57.000000 clear_html-0.4.1/clear_html/formatted_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-30 13:59:57.000000 clear_html-0.4.1/clear_html/formatted_text/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-04-30 13:59:57.000000 clear_html-0.4.1/clear_html/formatted_text/defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13418 2024-04-30 13:59:57.000000 clear_html-0.4.1/clear_html/formatted_text/figures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-30 13:59:57.000000 clear_html-0.4.1/clear_html/formatted_text/headings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-04-30 13:59:57.000000 clear_html-0.4.1/clear_html/formatted_text/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15489 2024-04-30 13:59:57.000000 clear_html-0.4.1/clear_html/formatted_text/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-30 13:59:57.000000 clear_html-0.4.1/clear_html/html_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-04-30 13:59:57.000000 clear_html-0.4.1/clear_html/lxml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:59:57.000000 clear_html-0.4.1/clear_html/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:00:07.516429 clear_html-0.4.1/clear_html.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-30 14:00:07.000000 clear_html-0.4.1/clear_html.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-30 14:00:07.000000 clear_html-0.4.1/clear_html.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:00:07.000000 clear_html-0.4.1/clear_html.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 14:00:07.000000 clear_html-0.4.1/clear_html.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 14:00:07.000000 clear_html-0.4.1/clear_html.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-30 13:59:57.000000 clear_html-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-30 14:00:07.516429 clear_html-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:00:07.516429 clear_html-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-30 13:59:57.000000 clear_html-0.4.1/tests/test_body_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-30 13:59:57.000000 clear_html-0.4.1/tests/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9242 2024-04-30 13:59:57.000000 clear_html-0.4.1/tests/test_formatted_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-30 13:59:57.000000 clear_html-0.4.1/tests/test_html_embeddings.py
```

### Comparing `clear-html-0.4.0/LICENSE` & `clear_html-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clear-html-0.4.0/PKG-INFO` & `clear_html-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-html
-Version: 0.4.0
+Version: 0.4.1
 Summary: Clean and normalize HTML.
 Author-email: Zyte Group Ltd <info@zyte.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Zyte Group Ltd
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,14 +36,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: attrs>=20.3.0
+Requires-Dist: html-text>=0.5.2
+Requires-Dist: lxml>=4.4.3
 
 ==========
 clear-html
 ==========
 
 .. image:: https://img.shields.io/pypi/v/clear-html.svg
    :target: https://pypi.python.org/pypi/clear-html
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clear-html Version: 0.4.0 Summary: Clean and
+Metadata-Version: 2.1 Name: clear-html Version: 0.4.1 Summary: Clean and
 normalize HTML. Author-email: Zyte Group Ltd
 zyte.com> License: The MIT License (MIT) Copyright (c) 2023 Zyte Group Ltd
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
@@ -19,17 +19,18 @@
 Audience :: Developers Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: Implementation :: CPython Requires-Python: >=3.8 Description-Content-
-Type: text/x-rst License-File: LICENSE ========== clear-html ========== ..
-image:: https://img.shields.io/pypi/v/clear-html.svg :target: https://
-pypi.python.org/pypi/clear-html :alt: PyPI Version .. image:: https://
+Type: text/x-rst License-File: LICENSE Requires-Dist: attrs>=20.3.0 Requires-
+Dist: html-text>=0.5.2 Requires-Dist: lxml>=4.4.3 ========== clear-html
+========== .. image:: https://img.shields.io/pypi/v/clear-html.svg :target:
+https://pypi.python.org/pypi/clear-html :alt: PyPI Version .. image:: https://
 img.shields.io/pypi/pyversions/clear-html.svg :target: https://pypi.python.org/
 pypi/clear-html :alt: Supported Python Versions .. image:: https://github.com/
 zytedata/clear-html/workflows/tox/badge.svg :target: https://github.com/
 zytedata/clear-html/actions :alt: Build Status .. image:: https://codecov.io/
 github/zytedata/clear-html/coverage.svg?branch=master :target: https://
 codecov.io/gh/zytedata/clear-html :alt: Coverage report Clean and normalize
 HTML. Preserve embeddings (e.g. Twitter, Instagram, etc) .. contents:: Quick
```

### Comparing `clear-html-0.4.0/README.rst` & `clear_html-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `clear-html-0.4.0/clear_html/body_annotations.py` & `clear_html-0.4.1/clear_html/body_annotations.py`

 * *Files identical despite different names*

### Comparing `clear-html-0.4.0/clear_html/clean.py` & `clear_html-0.4.1/clear_html/clean.py`

 * *Files identical despite different names*

### Comparing `clear-html-0.4.0/clear_html/formatted_text/__init__.py` & `clear_html-0.4.1/clear_html/formatted_text/__init__.py`

 * *Files identical despite different names*

### Comparing `clear-html-0.4.0/clear_html/formatted_text/cleaner.py` & `clear_html-0.4.1/clear_html/formatted_text/cleaner.py`

 * *Files identical despite different names*

### Comparing `clear-html-0.4.0/clear_html/formatted_text/defs.py` & `clear_html-0.4.1/clear_html/formatted_text/defs.py`

 * *Files identical despite different names*

### Comparing `clear-html-0.4.0/clear_html/formatted_text/figures.py` & `clear_html-0.4.1/clear_html/formatted_text/figures.py`

 * *Files identical despite different names*

### Comparing `clear-html-0.4.0/clear_html/formatted_text/headings.py` & `clear_html-0.4.1/clear_html/formatted_text/headings.py`

 * *Files identical despite different names*

### Comparing `clear-html-0.4.0/clear_html/formatted_text/main.py` & `clear_html-0.4.1/clear_html/formatted_text/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     infer_img_url_from_data_src_attr,
     remove_figures_without_content,
     top_level_media_within_figure,
 )
 from clear_html.formatted_text.headings import normalize_headings_level
 from clear_html.formatted_text.utils import (
     clean_incomplete_structures,
+    double_br,
     kill_tag_content,
     remove_empty_tags,
     set_article_tag_as_root,
     translate_tags,
 )
 from clear_html.lxml_utils import has_tail, has_text
 
@@ -112,18 +113,18 @@
     """
     # Let's detect the sequences of consecutive br
     n_children = len(doc)
     br_sequences: List[Tuple[int, int]] = []
     start, end = None, None
     for idx, child in enumerate(doc):
         if child.tag == "br":
-            if idx == 0 or doc[idx - 1].tag != "br" or has_tail(doc[idx - 1]):
+            if not double_br(child.getprevious()):
                 # A br without previous consecutive br was found
                 start = idx
-            if idx == n_children - 1 or doc[idx + 1].tag != "br" or has_tail(child):
+            if not double_br(child):
                 # A br without next consecutive br was found
                 end = idx
                 if start == end:
                     # Single br found. We don't do anything
                     start, end = None, None
                 if start is not None and end is not None:
                     # Sequence of consecutive br found
```

### Comparing `clear-html-0.4.0/clear_html/formatted_text/utils.py` & `clear_html-0.4.1/clear_html/formatted_text/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,57 +153,57 @@
         return  # Root node cannot be removed
 
     if not is_phrasing_content(doc):
         # If tag to remove is a block tag then we should
         # carefully add double brs in some cases to
         # respect the separation between text chunks
         # Not known html tags are considered as inline elements by default.
-        idx = parent.index(doc)
+        doc_prev = doc.getprevious()
+        doc_next = doc.getnext()
 
         prev_is_inline = (
-            idx != 0
-            and parent[idx - 1].tag in PHRASING_CONTENT
-            and not _double_br(parent, idx - 2, idx - 1)
+            doc_prev is not None
+            and doc_prev.tag in PHRASING_CONTENT
+            and not double_br(doc_prev.getprevious())
         )
         after_is_inline = (
-            idx != len(parent) - 1
-            and parent[idx + 1].tag in PHRASING_CONTENT
-            and not _double_br(parent, idx + 1, idx + 2)
+            doc_next is not None
+            and doc_next.tag in PHRASING_CONTENT
+            and not double_br(doc_next)
         )
 
         has_text_prev = bool(prev_text(doc).strip()) or prev_is_inline
         has_text_inside = preserve_content and (has_text(doc) or len(doc) > 0)
         has_text_after = has_tail(doc) or after_is_inline
 
         if has_text_prev and (has_text_inside or has_text_after):
             # Insert double br before
             for i in range(2):
-                parent.insert(idx, Element("br"))
-            idx += 2
+                doc.addprevious(Element("br"))
         if has_text_inside and has_text_after:
             # Insert brs after
             last_br = Element("br")
             last_br.tail = doc.tail
             doc.tail = None
-            parent.insert(idx + 1, last_br)
-            parent.insert(idx + 1, Element("br"))
+            doc.addnext(last_br)
+            doc.addnext(Element("br"))
     if preserve_content:
         doc.drop_tag()
     else:
         doc.drop_tree()
 
 
-def _double_br(doc: HtmlElement, start: int, end: int):
-    """True if double br in doc[start:end] (end-start must be 1)"""
-    if end - start != 1:
+def double_br(doc: Optional[HtmlElement]):
+    """True if doc and next element are "br" tags without text in between."""
+    if doc is None or doc.tag != "br":
         return False
-    if not all(idx >= 0 and idx < len(doc) for idx in (start, end)):
+    doc_next = doc.getnext()
+    if doc_next is None or doc_next.tag != "br":
         return False
-    both_brs = (doc[start].tag == "br") and (doc[end].tag == "br")
-    return both_brs and not has_tail(doc[start])
+    return not has_tail(doc)
 
 
 def has_no_content(doc: HtmlElement) -> bool:
     """Checks if a node contains content. A node has content if it has
     any text in the tree or if has any tags that handle non textual
     content like ``img`` or ``iframe``. ``br``, ``dt``, ``dd``, ``td`` tags are
     considered as non content. Implementation detail: a copy of the doc is done.
```

### Comparing `clear-html-0.4.0/clear_html/html_embeddings.py` & `clear_html-0.4.1/clear_html/html_embeddings.py`

 * *Files identical despite different names*

### Comparing `clear-html-0.4.0/clear_html/lxml_utils.py` & `clear_html-0.4.1/clear_html/lxml_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,20 +79,24 @@
     'h'
     >>> prev_text(html.find(".//c"))
     'l'
     """
     parent = doc.getparent()
     if parent is None:
         return ""
-    idx = parent.index(doc)
-    if idx == 0:
-        text = parent.text
+    previous = doc.getprevious()
+    if previous is None:
+        parent = doc.getparent()
+        if parent is None:
+            text = ""
+        else:
+            text = parent.text or ""
     else:
-        text = parent[idx - 1].tail
-    return text or ""
+        text = previous.tail or ""
+    return text
 
 
 def iter_deep_first_post_order(doc: HtmlElement) -> Generator[HtmlElement, Any, None]:
     """Iterate over a document in a deep first fashion returning
     elements post-order https://en.wikipedia.org/wiki/Tree_traversal#Post-order_(LRN)"""
     for el in doc:
         yield from iter_deep_first_post_order(el)
```

### Comparing `clear-html-0.4.0/clear_html.egg-info/PKG-INFO` & `clear_html-0.4.1/clear_html.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-html
-Version: 0.4.0
+Version: 0.4.1
 Summary: Clean and normalize HTML.
 Author-email: Zyte Group Ltd <info@zyte.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Zyte Group Ltd
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,14 +36,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: attrs>=20.3.0
+Requires-Dist: html-text>=0.5.2
+Requires-Dist: lxml>=4.4.3
 
 ==========
 clear-html
 ==========
 
 .. image:: https://img.shields.io/pypi/v/clear-html.svg
    :target: https://pypi.python.org/pypi/clear-html
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clear-html Version: 0.4.0 Summary: Clean and
+Metadata-Version: 2.1 Name: clear-html Version: 0.4.1 Summary: Clean and
 normalize HTML. Author-email: Zyte Group Ltd
 zyte.com> License: The MIT License (MIT) Copyright (c) 2023 Zyte Group Ltd
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
@@ -19,17 +19,18 @@
 Audience :: Developers Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: Implementation :: CPython Requires-Python: >=3.8 Description-Content-
-Type: text/x-rst License-File: LICENSE ========== clear-html ========== ..
-image:: https://img.shields.io/pypi/v/clear-html.svg :target: https://
-pypi.python.org/pypi/clear-html :alt: PyPI Version .. image:: https://
+Type: text/x-rst License-File: LICENSE Requires-Dist: attrs>=20.3.0 Requires-
+Dist: html-text>=0.5.2 Requires-Dist: lxml>=4.4.3 ========== clear-html
+========== .. image:: https://img.shields.io/pypi/v/clear-html.svg :target:
+https://pypi.python.org/pypi/clear-html :alt: PyPI Version .. image:: https://
 img.shields.io/pypi/pyversions/clear-html.svg :target: https://pypi.python.org/
 pypi/clear-html :alt: Supported Python Versions .. image:: https://github.com/
 zytedata/clear-html/workflows/tox/badge.svg :target: https://github.com/
 zytedata/clear-html/actions :alt: Build Status .. image:: https://codecov.io/
 github/zytedata/clear-html/coverage.svg?branch=master :target: https://
 codecov.io/gh/zytedata/clear-html :alt: Coverage report Clean and normalize
 HTML. Preserve embeddings (e.g. Twitter, Instagram, etc) .. contents:: Quick
```

### Comparing `clear-html-0.4.0/clear_html.egg-info/SOURCES.txt` & `clear_html-0.4.1/clear_html.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clear-html-0.4.0/pyproject.toml` & `clear_html-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clear-html-0.4.0/tests/test_body_annotations.py` & `clear_html-0.4.1/tests/test_body_annotations.py`

 * *Files identical despite different names*

### Comparing `clear-html-0.4.0/tests/test_clean.py` & `clear_html-0.4.1/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `clear-html-0.4.0/tests/test_formatted_text.py` & `clear_html-0.4.1/tests/test_formatted_text.py`

 * *Files identical despite different names*

### Comparing `clear-html-0.4.0/tests/test_html_embeddings.py` & `clear_html-0.4.1/tests/test_html_embeddings.py`

 * *Files identical despite different names*

