# Comparing `tmp/opencf-0.3.0.tar.gz` & `tmp/opencf-0.3.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencf-0.3.0.tar", max compression
+gzip compressed data, was "opencf-0.3.1a0.tar", max compression
```

## Comparing `opencf-0.3.0.tar` & `opencf-0.3.1a0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     5030 2024-04-22 22:29:52.576924 opencf-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-04-22 22:28:19.435526 opencf-0.3.0/opencf/__init__.py
--rw-r--r--   0        0        0     1938 2024-04-22 22:42:11.740523 opencf-0.3.0/opencf/app.py
--rw-r--r--   0        0        0      631 2024-04-22 22:28:19.439526 opencf-0.3.0/opencf/converters/__init__.py
--rw-r--r--   0        0        0     5390 2024-04-22 22:42:11.744523 opencf-0.3.0/opencf/converters/document.py
--rw-r--r--   0        0        0        0 2024-04-22 22:28:19.435526 opencf-0.3.0/opencf/converters/image.py
--rw-r--r--   0        0        0     1027 2024-04-22 22:42:11.744523 opencf-0.3.0/opencf/converters/markup.py
--rw-r--r--   0        0        0     2877 2024-04-22 22:42:11.748523 opencf-0.3.0/opencf/converters/structured.py
--rw-r--r--   0        0        0     3162 2024-04-22 22:46:08.854979 opencf-0.3.0/opencf/converters/video.py
--rw-r--r--   0        0        0      347 2024-04-22 22:28:19.439526 opencf-0.3.0/opencf/io_handlers/__init__.py
--rw-r--r--   0        0        0     2124 2024-04-22 22:42:11.740523 opencf-0.3.0/opencf/io_handlers/img_opencv.py
--rw-r--r--   0        0        0     2311 2024-04-22 22:42:11.744523 opencf-0.3.0/opencf/io_handlers/img_pillow.py
--rw-r--r--   0        0        0     2444 2024-04-22 22:42:11.740523 opencf-0.3.0/opencf/io_handlers/pdf.py
--rw-r--r--   0        0        0     2344 2024-04-22 22:42:11.740523 opencf-0.3.0/opencf/io_handlers/spreadsheet.py
--rw-r--r--   0        0        0     5596 2024-04-22 22:47:54.180103 opencf-0.3.0/opencf/io_handlers/video.py
--rw-r--r--   0        0        0     3620 2024-04-22 22:28:19.439526 opencf-0.3.0/opencf/utils/image_to_video.py
--rw-r--r--   0        0        0     1430 2024-04-22 22:43:40.357593 opencf-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6435 1970-01-01 00:00:00.000000 opencf-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     5030 2024-04-22 22:29:52.576924 opencf-0.3.1a0/README.md
+-rw-r--r--   0        0        0       29 2024-04-29 11:56:13.924976 opencf-0.3.1a0/opencf/__init__.py
+-rw-r--r--   0        0        0     2026 2024-04-29 11:29:55.833368 opencf-0.3.1a0/opencf/app.py
+-rw-r--r--   0        0        0      671 2024-04-29 10:24:31.696290 opencf-0.3.1a0/opencf/converters/__init__.py
+-rw-r--r--   0        0        0     7058 2024-04-29 11:16:57.206075 opencf-0.3.1a0/opencf/converters/document.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:28:19.435526 opencf-0.3.1a0/opencf/converters/image.py
+-rw-r--r--   0        0        0     1027 2024-04-22 22:42:11.744523 opencf-0.3.1a0/opencf/converters/markup.py
+-rw-r--r--   0        0        0     2877 2024-04-22 22:42:11.748523 opencf-0.3.1a0/opencf/converters/structured.py
+-rw-r--r--   0        0        0     3162 2024-04-22 23:19:10.399407 opencf-0.3.1a0/opencf/converters/video.py
+-rw-r--r--   0        0        0      419 2024-04-29 11:55:19.000013 opencf-0.3.1a0/opencf/import_script.py
+-rw-r--r--   0        0        0      347 2024-04-22 22:28:19.439526 opencf-0.3.1a0/opencf/io_handlers/__init__.py
+-rw-r--r--   0        0        0     2124 2024-04-22 22:42:11.740523 opencf-0.3.1a0/opencf/io_handlers/img_opencv.py
+-rw-r--r--   0        0        0     2311 2024-04-22 22:42:11.744523 opencf-0.3.1a0/opencf/io_handlers/img_pillow.py
+-rw-r--r--   0        0        0     2444 2024-04-22 22:42:11.740523 opencf-0.3.1a0/opencf/io_handlers/pdf.py
+-rw-r--r--   0        0        0     2344 2024-04-22 22:42:11.740523 opencf-0.3.1a0/opencf/io_handlers/spreadsheet.py
+-rw-r--r--   0        0        0     5596 2024-04-22 23:19:10.399407 opencf-0.3.1a0/opencf/io_handlers/video.py
+-rw-r--r--   0        0        0     3620 2024-04-22 22:28:19.439526 opencf-0.3.1a0/opencf/utils/image_to_video.py
+-rw-r--r--   0        0        0     1888 2024-04-30 14:37:40.978845 opencf-0.3.1a0/pyproject.toml
+-rw-r--r--   0        0        0     6705 1970-01-01 00:00:00.000000 opencf-0.3.1a0/PKG-INFO
```

### Comparing `opencf-0.3.0/README.md` & `opencf-0.3.1a0/README.md`

 * *Files identical despite different names*

### Comparing `opencf-0.3.0/opencf/app.py` & `opencf-0.3.1a0/opencf/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from .converters import (
     CSVToXMLConverter,
     ImageToPDFConverter,
     ImageToVideoConverterWithOpenCV,
     ImageToVideoConverterWithPillow,
     JSONToCSVConverter,
     PDFToDocxConvertor,
+    MergePDFs,
+    PDFToDocxWithAspose,
     PDFToImageExtractor,
     TXTToMDConverter,
     VideoToGIFConverter,
     XLSXToCSVConverter,
     XMLToJSONConverter,
 )
 
@@ -36,15 +38,17 @@
         XLSXToCSVConverter,
         ImageToPDFConverter,
         # PDFToImageConverter,
         PDFToImageExtractor,
         ImageToVideoConverterWithPillow,
         ImageToVideoConverterWithOpenCV,
         VideoToGIFConverter,
+        PDFToDocxWithAspose,
         PDFToDocxConvertor,
+        MergePDFs,
     ]
 
 
 def main():
     """
     Main function to run the file conversion application.
     """
```

### Comparing `opencf-0.3.0/opencf/converters/__init__.py` & `opencf-0.3.1a0/opencf/converters/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 This module provides classes for converting between different file formats. It includes concrete implementations of conversion classes for various file types.
 """
 
 from .document import (
     ImageToPDFConverter,
     ImageToPDFConverterWithPyPdf2,
+    MergePDFs,
     PDFToDocxConvertor,
+    PDFToDocxWithAspose,
     PDFToImageConverter,
     PDFToImageExtractor,
 )
 from .markup import TXTToMDConverter
 from .structured import (
     CSVToXMLConverter,
     JSONToCSVConverter,
```

### Comparing `opencf-0.3.0/opencf/converters/document.py` & `opencf-0.3.1a0/opencf/converters/document.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 This module provides classes for converting between document different file formats. It includes concrete implementations of conversion classes for various file types (pdf, docx, epub, ...).
 """
 
 from pathlib import Path
 from typing import List
 
+import aspose.words as aw
 from opencf_core.base_converter import BaseConverter
 from opencf_core.filetypes import FileType
 from pdf2docx import Converter as pdf2docx_converter
 from PIL import Image as PillowImage
 from PyPDF2 import PdfReader, PdfWriter
 
 from ..io_handlers import ImageToPillowReader, PdfToPyPdfReader, PyPdfToPdfWriter
@@ -175,11 +176,72 @@
         pdf_file = input_contents[0]
 
         cv = pdf2docx_converter(pdf_file)
         cv.convert(output_file, start=0, end=None)
         cv.close()
 
 
+class PDFToDocxWithAspose(BaseConverter):
+    """
+    Converts PDF files to docx format using Aspose.Words for Python.
+    """
+
+    file_reader = None
+    file_writer = None
+    folder_as_output = False
+
+    @classmethod
+    def _get_supported_input_type(cls) -> FileType:
+        return FileType.PDF
+
+    @classmethod
+    def _get_supported_output_type(cls) -> FileType:
+        return FileType.MSWORD
+
+    def _convert(self, input_contents: List[Path], output_file: Path):
+        # Load the PDF document
+        pdf_path = input_contents[0]
+        pdf_doc = aw.Document(str(pdf_path))
+
+        # Load the document from the disc.
+        # doc = aw.Document()
+
+        # # Use DocumentBuilder to add content to the document
+        # builder = aw.DocumentBuilder(doc)
+        # for paragraph in pdf_doc.get_child_nodes(aw.NodeType.PARAGRAPH, True):
+        #     builder.write(paragraph.get_text())
+
+        # Save the document in DOCX format
+        pdf_doc.save(str(output_file))
+
+
 class PDFToHTML(BaseConverter):
     """
     i could use this [tool](https://linux.die.net/man/1/pdftohtml) to do it
     """
+
+
+class MergePDFs(BaseConverter):
+    """
+    Merges multiple PDF files into a single PDF.
+    """
+
+    file_reader = PdfToPyPdfReader()
+    file_writer = PyPdfToPdfWriter()
+    folder_as_output = False
+
+    @classmethod
+    def _get_supported_input_type(cls) -> FileType:
+        return FileType.PDF
+
+    @classmethod
+    def _get_supported_output_type(cls) -> FileType:
+        return FileType.PDF
+
+    def _convert(self, input_contents: List[PdfReader]):
+        pdf_writer = PdfWriter()
+
+        for pdf_file_reader in input_contents:
+            for page in pdf_file_reader.pages:
+                pdf_writer.add_page(page)
+
+        return pdf_writer
```

### Comparing `opencf-0.3.0/opencf/converters/markup.py` & `opencf-0.3.1a0/opencf/converters/markup.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.0/opencf/converters/structured.py` & `opencf-0.3.1a0/opencf/converters/structured.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.0/opencf/converters/video.py` & `opencf-0.3.1a0/opencf/converters/video.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.0/opencf/io_handlers/img_opencv.py` & `opencf-0.3.1a0/opencf/io_handlers/img_opencv.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.0/opencf/io_handlers/img_pillow.py` & `opencf-0.3.1a0/opencf/io_handlers/img_pillow.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.0/opencf/io_handlers/pdf.py` & `opencf-0.3.1a0/opencf/io_handlers/pdf.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.0/opencf/io_handlers/spreadsheet.py` & `opencf-0.3.1a0/opencf/io_handlers/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.0/opencf/io_handlers/video.py` & `opencf-0.3.1a0/opencf/io_handlers/video.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.0/opencf/utils/image_to_video.py` & `opencf-0.3.1a0/opencf/utils/image_to_video.py`

 * *Files identical despite different names*

### Comparing `opencf-0.3.0/PKG-INFO` & `opencf-0.3.1a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: opencf
-Version: 0.3.0
+Version: 0.3.1a0
 Summary: A collection of Python scripts for file conversion tasks, built on top of the opencf-core framework.
 Home-page: https://github.com/Hermann-web/opencf
 License: MIT
 Keywords: file conversion,data processing,file formats
 Author: Hermann Agossou
 Author-email: agossouhermann7@gmail.com
 Maintainer: Hermann Agossou
 Maintainer-email: agossouhermann7@gmail.com
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: imageio (>=2.30.0,<3.0.0)
-Requires-Dist: numpy (>=1.24.0,<2.0.0)
+Provides-Extra: document
+Provides-Extra: media
+Provides-Extra: tabular
+Requires-Dist: aspose-words (>=24.4.0,<25.0.0) ; extra == "document"
+Requires-Dist: generalimport (==0.5.2)
+Requires-Dist: imageio (>=2.30.0,<3.0.0) ; extra == "media"
+Requires-Dist: numpy (>=1.24.0,<2.0.0) ; extra == "media"
 Requires-Dist: opencf-core (>=0.2.0,<0.3.0)
-Requires-Dist: opencv-python (>=4.8.1.78,<5.0.0.0)
-Requires-Dist: pandas (>=2.0.0,<3.0.0)
-Requires-Dist: pdf2docx (>=0.5.8,<0.6.0)
-Requires-Dist: pillow (>=10.3.0,<11.0.0)
-Requires-Dist: pypdf2 (>=3.0.1,<4.0.0)
+Requires-Dist: opencv-python (>=4.8.1.78,<5.0.0.0) ; extra == "media"
+Requires-Dist: pandas (>=2.0.0,<3.0.0) ; extra == "tabular"
+Requires-Dist: pdf2docx (>=0.5.8,<0.6.0) ; extra == "document"
+Requires-Dist: pillow (>=10.3.0,<11.0.0) ; extra == "media"
+Requires-Dist: pypdf2 (>=3.0.1,<4.0.0) ; extra == "document"
 Project-URL: Documentation, https://opencf.readthedocs.io
 Project-URL: Repository, https://github.com/Hermann-web/opencf
 Description-Content-Type: text/markdown
 
 # OpenCF: The File Conversion Scripts
 
 The `opencf` package provides a collection of Python scripts for file conversion tasks, built on top of the [opencf-core](https://test.pypi.org/project/opencf-core/) framework. These scripts offer functionalities to convert various file formats, including text, CSV, JSON, XML, Excel, and image files, making it easy to handle different types of data transformations efficiently.
```

