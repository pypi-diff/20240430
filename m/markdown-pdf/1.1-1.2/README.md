# Comparing `tmp/markdown_pdf-1.1.tar.gz` & `tmp/markdown_pdf-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_pdf-1.1.tar", last modified: Tue Feb 13 07:29:11 2024, max compression
+gzip compressed data, was "markdown_pdf-1.2.tar", last modified: Tue Apr 30 08:40:49 2024, max compression
```

## Comparing `markdown_pdf-1.1.tar` & `markdown_pdf-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-13 07:29:11.177169 markdown_pdf-1.1/
--rw-rw-rw-   0        0        0     1094 2023-09-30 14:52:08.000000 markdown_pdf-1.1/LICENSE
--rw-rw-rw-   0        0        0       60 2023-09-30 15:14:36.000000 markdown_pdf-1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3743 2024-02-13 07:29:11.177669 markdown_pdf-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2671 2024-02-13 06:37:57.000000 markdown_pdf-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-13 07:29:11.147928 markdown_pdf-1.1/markdown_pdf/
--rw-rw-rw-   0        0        0     2941 2024-02-13 06:07:09.000000 markdown_pdf-1.1/markdown_pdf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-13 07:29:11.175166 markdown_pdf-1.1/markdown_pdf.egg-info/
--rw-rw-rw-   0        0        0     3743 2024-02-13 07:29:10.000000 markdown_pdf-1.1/markdown_pdf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-02-13 07:29:11.000000 markdown_pdf-1.1/markdown_pdf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-13 07:29:10.000000 markdown_pdf-1.1/markdown_pdf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-02-13 07:29:10.000000 markdown_pdf-1.1/markdown_pdf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-02-13 07:29:10.000000 markdown_pdf-1.1/markdown_pdf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2023-04-28 10:20:43.000000 markdown_pdf-1.1/pyproject.toml
--rw-rw-rw-   0        0        0      678 2024-02-13 07:29:11.181671 markdown_pdf-1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 08:40:49.059628 markdown_pdf-1.2/
+-rw-rw-rw-   0        0        0     1094 2023-09-30 14:52:08.000000 markdown_pdf-1.2/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-09-30 15:14:36.000000 markdown_pdf-1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4647 2024-04-30 08:40:49.059628 markdown_pdf-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4060 2024-03-09 12:04:11.000000 markdown_pdf-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 08:40:49.044003 markdown_pdf-1.2/markdown_pdf/
+-rw-rw-rw-   0        0        0     2941 2024-03-09 11:24:51.000000 markdown_pdf-1.2/markdown_pdf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 08:40:49.059628 markdown_pdf-1.2/markdown_pdf.egg-info/
+-rw-rw-rw-   0        0        0     4647 2024-04-30 08:40:48.000000 markdown_pdf-1.2/markdown_pdf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-04-30 08:40:48.000000 markdown_pdf-1.2/markdown_pdf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 08:40:48.000000 markdown_pdf-1.2/markdown_pdf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-30 08:40:48.000000 markdown_pdf-1.2/markdown_pdf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-30 08:40:48.000000 markdown_pdf-1.2/markdown_pdf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2023-04-28 10:20:43.000000 markdown_pdf-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      678 2024-04-30 08:40:49.059628 markdown_pdf-1.2/setup.cfg
```

### Comparing `markdown_pdf-1.1/LICENSE` & `markdown_pdf-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_pdf-1.1/markdown_pdf/__init__.py` & `markdown_pdf-1.2/markdown_pdf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Markdown to pdf converter baset on markdown_it and fitz."""
+"""Markdown to pdf converter based on markdown_it and fitz."""
 import io
 from markdown_it import MarkdownIt
 import fitz
 
 
 class Section:
     """Markdown section."""
```

### Comparing `markdown_pdf-1.1/setup.cfg` & `markdown_pdf-1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6172 6b64 6f77 6e5f 7064 660d   = markdown_pdf.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e31 0d0a  .version = 1.1..
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e32 0d0a  .version = 1.2..
 00000030: 6175 7468 6f72 203d 2056 6974 616c 7920  author = Vitaly 
 00000040: 426f 676f 6d6f 6c6f 760d 0a61 7574 686f  Bogomolov..autho
 00000050: 725f 656d 6169 6c20 3d20 6d61 696c 4076  r_email = mail@v
 00000060: 6974 616c 792d 626f 676f 6d6f 6c6f 762e  italy-bogomolov.
 00000070: 7275 0d0a 6465 7363 7269 7074 696f 6e20  ru..description 
 00000080: 3d20 4d61 726b 646f 776e 2074 6f20 7064  = Markdown to pd
 00000090: 6620 7265 6e64 6572 6572 0d0a 6c6f 6e67  f renderer..long
@@ -31,13 +31,13 @@
 000001e0: 6e64 6570 656e 6465 6e74 0d0a 0d0a 5b6f  ndependent....[o
 000001f0: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
 00000200: 5f64 6972 203d 200d 0a70 6163 6b61 6765  _dir = ..package
 00000210: 7320 3d20 6d61 726b 646f 776e 5f70 6466  s = markdown_pdf
 00000220: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
 00000230: 7320 3d20 3e3d 332e 380d 0a69 6e73 7461  s = >=3.8..insta
 00000240: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
-00000250: 0950 794d 7550 4446 3d3d 312e 3233 2e33  .PyMuPDF==1.23.3
+00000250: 0950 794d 7550 4446 3d3d 312e 3234 2e32  .PyMuPDF==1.24.2
 00000260: 0d0a 096d 6172 6b64 6f77 6e2d 6974 2d70  ...markdown-it-p
 00000270: 793d 3d33 2e30 2e30 0d0a 0d0a 5b65 6767  y==3.0.0....[egg
 00000280: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
 00000290: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
 000002a0: 2030 0d0a 0d0a                            0....
```

