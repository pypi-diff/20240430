# Comparing `tmp/docprompt-0.3.1.tar.gz` & `tmp/docprompt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docprompt-0.3.1.tar", max compression
+gzip compressed data, was "docprompt-0.4.0.tar", max compression
```

## Comparing `docprompt-0.3.1.tar` & `docprompt-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0      585 2024-04-18 22:55:47.915108 docprompt-0.3.1/LICENSE
--rw-r--r--   0        0        0     4917 2024-04-18 22:55:47.915108 docprompt-0.3.1/README.md
--rw-r--r--   0        0        0      674 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/_exec/__init__.py
--rw-r--r--   0        0        0     2395 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/_exec/ghostscript.py
--rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/provenance/__init__.py
--rw-r--r--   0        0        0     9850 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/provenance/search.py
--rw-r--r--   0        0        0     1357 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/provenance/source.py
--rw-r--r--   0        0        0     6054 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/provenance/util.py
--rw-r--r--   0        0        0     7095 2024-04-23 00:28:28.294162 docprompt-0.3.1/docprompt/rasterize.py
--rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/schema/__init__.py
--rw-r--r--   0        0        0     8981 2024-04-23 00:27:13.953736 docprompt-0.3.1/docprompt/schema/document.py
--rw-r--r--   0        0        0     6649 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/schema/layout.py
--rw-r--r--   0        0        0     8282 2024-04-23 01:58:23.242580 docprompt-0.3.1/docprompt/schema/pipeline.py
--rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/tasks/__init__.py
--rw-r--r--   0        0        0     5103 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/tasks/base.py
--rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/tasks/classification/__init__.py
--rw-r--r--   0        0        0     2522 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/tasks/message.py
--rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/tasks/ocr/__init__.py
--rw-r--r--   0        0        0    18558 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/tasks/ocr/gcp.py
--rw-r--r--   0        0        0     1170 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/tasks/ocr/result.py
--rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/tasks/table_extraction/__init__.py
--rw-r--r--   0        0        0      746 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/tasks/table_extraction/base.py
--rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/tasks/table_extraction/providers/__init__.py
--rw-r--r--   0        0        0     3420 2024-04-18 22:55:47.915108 docprompt-0.3.1/docprompt/tasks/table_extraction/providers/claude.py
--rw-r--r--   0        0        0      783 2024-04-18 22:55:47.919108 docprompt-0.3.1/docprompt/tasks/table_extraction/result.py
--rw-r--r--   0        0        0      351 2024-04-18 22:55:47.919108 docprompt-0.3.1/docprompt/utils/__init__.py
--rw-r--r--   0        0        0      421 2024-04-18 22:55:47.919108 docprompt-0.3.1/docprompt/utils/compressor.py
--rw-r--r--   0        0        0     4915 2024-04-18 22:55:47.919108 docprompt-0.3.1/docprompt/utils/date_extraction.py
--rw-r--r--   0        0        0        0 2024-04-18 22:55:47.919108 docprompt-0.3.1/docprompt/utils/masking/__init__.py
--rw-r--r--   0        0        0      707 2024-04-18 22:55:47.919108 docprompt-0.3.1/docprompt/utils/masking/image.py
--rw-r--r--   0        0        0     4015 2024-04-18 22:55:47.919108 docprompt-0.3.1/docprompt/utils/splitter.py
--rw-r--r--   0        0        0     3994 2024-04-18 22:55:47.919108 docprompt-0.3.1/docprompt/utils/util.py
--rw-r--r--   0        0        0     4131 2024-04-23 02:00:06.882944 docprompt-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       39 2024-04-18 22:55:47.935108 docprompt-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0   123638 2024-04-18 22:55:47.935108 docprompt-0.3.1/tests/fixtures/1.pdf
--rw-r--r--   0        0        0  2788655 2024-04-18 22:55:47.943108 docprompt-0.3.1/tests/fixtures/1_ocr.json
--rw-r--r--   0        0        0      202 2024-04-18 22:55:47.935108 docprompt-0.3.1/tests/fixtures.py
--rw-r--r--   0        0        0      830 2024-04-18 22:55:47.943108 docprompt-0.3.1/tests/test_date_extraction.py
--rw-r--r--   0        0        0     3656 2024-04-18 22:55:47.943108 docprompt-0.3.1/tests/test_document.py
--rw-r--r--   0        0        0      916 2024-04-23 01:59:30.430813 docprompt-0.3.1/tests/test_documentnode.py
--rw-r--r--   0        0        0     1361 2024-04-18 22:55:47.943108 docprompt-0.3.1/tests/test_layout_models.py
--rw-r--r--   0        0        0     1227 2024-04-18 22:55:47.943108 docprompt-0.3.1/tests/test_search.py
--rw-r--r--   0        0        0      878 2024-04-18 22:55:47.943108 docprompt-0.3.1/tests/test_threadpool.py
--rw-r--r--   0        0        0     1003 2024-04-18 22:55:47.943108 docprompt-0.3.1/tests/util.py
--rw-r--r--   0        0        0     7726 1970-01-01 00:00:00.000000 docprompt-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      585 2024-04-18 22:55:47.915108 docprompt-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4917 2024-04-18 22:55:47.915108 docprompt-0.4.0/README.md
+-rw-r--r--   0        0        0      752 2024-04-30 02:41:36.793371 docprompt-0.4.0/docprompt/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/_exec/__init__.py
+-rw-r--r--   0        0        0     2395 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/_exec/ghostscript.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/provenance/__init__.py
+-rw-r--r--   0        0        0     9850 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/provenance/search.py
+-rw-r--r--   0        0        0     1357 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/provenance/source.py
+-rw-r--r--   0        0        0     6054 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/provenance/util.py
+-rw-r--r--   0        0        0     7095 2024-04-23 00:28:28.294162 docprompt-0.4.0/docprompt/rasterize.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/schema/__init__.py
+-rw-r--r--   0        0        0     8981 2024-04-23 00:27:13.953736 docprompt-0.4.0/docprompt/schema/document.py
+-rw-r--r--   0        0        0     6649 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/schema/layout.py
+-rw-r--r--   0        0        0     8157 2024-04-29 23:28:32.792877 docprompt-0.4.0/docprompt/schema/pipeline.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/__init__.py
+-rw-r--r--   0        0        0     5103 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/base.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/classification/__init__.py
+-rw-r--r--   0        0        0     2522 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/message.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/ocr/__init__.py
+-rw-r--r--   0        0        0    18558 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/ocr/gcp.py
+-rw-r--r--   0        0        0     1170 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/ocr/result.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/table_extraction/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/table_extraction/base.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/table_extraction/providers/__init__.py
+-rw-r--r--   0        0        0     3420 2024-04-18 22:55:47.915108 docprompt-0.4.0/docprompt/tasks/table_extraction/providers/claude.py
+-rw-r--r--   0        0        0      783 2024-04-18 22:55:47.919108 docprompt-0.4.0/docprompt/tasks/table_extraction/result.py
+-rw-r--r--   0        0        0      375 2024-04-29 23:28:32.792877 docprompt-0.4.0/docprompt/utils/__init__.py
+-rw-r--r--   0        0        0      421 2024-04-18 22:55:47.919108 docprompt-0.4.0/docprompt/utils/compressor.py
+-rw-r--r--   0        0        0     4915 2024-04-18 22:55:47.919108 docprompt-0.4.0/docprompt/utils/date_extraction.py
+-rw-r--r--   0        0        0        0 2024-04-18 22:55:47.919108 docprompt-0.4.0/docprompt/utils/masking/__init__.py
+-rw-r--r--   0        0        0      707 2024-04-18 22:55:47.919108 docprompt-0.4.0/docprompt/utils/masking/image.py
+-rw-r--r--   0        0        0     4015 2024-04-18 22:55:47.919108 docprompt-0.4.0/docprompt/utils/splitter.py
+-rw-r--r--   0        0        0     4061 2024-04-29 23:28:32.792877 docprompt-0.4.0/docprompt/utils/util.py
+-rw-r--r--   0        0        0     4131 2024-04-30 02:41:16.997263 docprompt-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-04-18 22:55:47.935108 docprompt-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0   123638 2024-04-18 22:55:47.935108 docprompt-0.4.0/tests/fixtures/1.pdf
+-rw-r--r--   0        0        0  2788655 2024-04-18 22:55:47.943108 docprompt-0.4.0/tests/fixtures/1_ocr.json
+-rw-r--r--   0        0        0      202 2024-04-18 22:55:47.935108 docprompt-0.4.0/tests/fixtures.py
+-rw-r--r--   0        0        0      830 2024-04-18 22:55:47.943108 docprompt-0.4.0/tests/test_date_extraction.py
+-rw-r--r--   0        0        0     5225 2024-04-30 00:05:31.753210 docprompt-0.4.0/tests/test_document.py
+-rw-r--r--   0        0        0      916 2024-04-23 01:59:30.430813 docprompt-0.4.0/tests/test_documentnode.py
+-rw-r--r--   0        0        0     1361 2024-04-18 22:55:47.943108 docprompt-0.4.0/tests/test_layout_models.py
+-rw-r--r--   0        0        0     1227 2024-04-18 22:55:47.943108 docprompt-0.4.0/tests/test_search.py
+-rw-r--r--   0        0        0      878 2024-04-18 22:55:47.943108 docprompt-0.4.0/tests/test_threadpool.py
+-rw-r--r--   0        0        0     1003 2024-04-18 22:55:47.943108 docprompt-0.4.0/tests/util.py
+-rw-r--r--   0        0        0     7726 1970-01-01 00:00:00.000000 docprompt-0.4.0/PKG-INFO
```

### Comparing `docprompt-0.3.1/LICENSE` & `docprompt-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/README.md` & `docprompt-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/docprompt/__init__.py` & `docprompt-0.4.0/docprompt/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """Top-level package for Docprompt."""
 
 __author__ = """Frankie Colson"""
 __email__ = "frank@pageleaf.io"
-__version__ = "0.2.1"
+__version__ = "0.4.0"
 
 from docprompt.schema.document import Document, PdfDocument  # noqa
 from docprompt.schema.layout import NormBBox, TextBlock  # noqa
 from docprompt.schema.pipeline import DocumentCollection, DocumentNode, PageNode  # noqa
-from docprompt.utils import load_document  # noqa
+from docprompt.utils import load_document, load_documents, hash_from_bytes  # noqa
 from docprompt.rasterize import ProviderResizeRatios
 
 Document.model_rebuild()
 
 
 __all__ = [
     "Document",
     "PdfDocument",
     "DocumentCollection",
     "DocumentNode",
     "NormBBox",
     "PageNode",
     "TextBlock",
     "load_document",
+    "load_documents",
+    "hash_from_bytes",
     "ProviderResizeRatios",
 ]
```

### Comparing `docprompt-0.3.1/docprompt/_exec/ghostscript.py` & `docprompt-0.4.0/docprompt/_exec/ghostscript.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/docprompt/provenance/search.py` & `docprompt-0.4.0/docprompt/provenance/search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/docprompt/provenance/source.py` & `docprompt-0.4.0/docprompt/provenance/source.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/docprompt/provenance/util.py` & `docprompt-0.4.0/docprompt/provenance/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/docprompt/rasterize.py` & `docprompt-0.4.0/docprompt/rasterize.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/docprompt/schema/document.py` & `docprompt-0.4.0/docprompt/schema/document.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/docprompt/schema/layout.py` & `docprompt-0.4.0/docprompt/schema/layout.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/docprompt/schema/pipeline.py` & `docprompt-0.4.0/docprompt/schema/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -143,19 +143,14 @@
     def clear_cache(self):
         self.raster_cache.clear()
 
     def pop(self, name: str, default=None):
         return self.raster_cache.pop(name, default=default)
 
 
-class PageRasterizationDescriptor:
-    def __get__(self, owner):
-        return PageRasterizer(owner._raster_cache, owner)
-
-
 class PageNode(BaseModel, Generic[PageNodeMetadata]):
     """
     Represents a single page in a document, with some metadata
     """
 
     document: "DocumentNode" = Field(exclude=True, repr=False)
     page_number: PositiveInt = Field(description="The page number")
```

### Comparing `docprompt-0.3.1/docprompt/tasks/base.py` & `docprompt-0.4.0/docprompt/tasks/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/docprompt/tasks/message.py` & `docprompt-0.4.0/docprompt/tasks/message.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/docprompt/tasks/ocr/gcp.py` & `docprompt-0.4.0/docprompt/tasks/ocr/gcp.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/docprompt/tasks/ocr/result.py` & `docprompt-0.4.0/docprompt/tasks/ocr/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/docprompt/tasks/table_extraction/base.py` & `docprompt-0.4.0/docprompt/tasks/table_extraction/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/docprompt/tasks/table_extraction/providers/claude.py` & `docprompt-0.4.0/docprompt/tasks/table_extraction/providers/claude.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/docprompt/tasks/table_extraction/result.py` & `docprompt-0.4.0/docprompt/tasks/table_extraction/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/docprompt/utils/date_extraction.py` & `docprompt-0.4.0/docprompt/utils/date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/docprompt/utils/masking/image.py` & `docprompt-0.4.0/docprompt/utils/masking/image.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/docprompt/utils/splitter.py` & `docprompt-0.4.0/docprompt/utils/splitter.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/pyproject.toml` & `docprompt-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "docprompt"
-version = "0.3.1"
+version = "0.4.0"
 homepage = "https://github.com/Page-Leaf/docprompt"
 description = "Documents and large language models."
 authors = ["Frankie Colson <frank@pageleaf.io>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `docprompt-0.3.1/tests/fixtures/1.pdf` & `docprompt-0.4.0/tests/fixtures/1.pdf`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/tests/fixtures/1_ocr.json` & `docprompt-0.4.0/tests/fixtures/1_ocr.json`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/tests/test_date_extraction.py` & `docprompt-0.4.0/tests/test_date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/tests/test_document.py` & `docprompt-0.4.0/tests/test_document.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,70 @@
-from docprompt import load_document
+import pytest
+from docprompt import load_document, load_documents
 from PIL import Image
 import io
 
 from .fixtures import PDF_FIXTURES
 
-from docprompt.utils.splitter import pdf_split_iter_fast
+from docprompt.utils.splitter import pdf_split_iter_fast, pdf_split_iter_with_max_bytes
+from docprompt.utils import is_pdf, hash_from_bytes
 from docprompt.rasterize import ProviderResizeRatios
 
 
 def test_load_document():
     for fixture in PDF_FIXTURES:
         doc = load_document(fixture.get_full_path())
         assert doc.page_count == fixture.page_count
         assert doc.document_hash == fixture.file_hash
 
 
+def test_load_document_from_bytes():
+    fixture = PDF_FIXTURES[0]
+
+    with open(fixture.get_full_path(), "rb") as f:
+        doc = load_document(f.read())
+
+    assert doc.page_count == fixture.page_count
+    assert doc.document_hash == fixture.file_hash
+    assert doc.name == f"document-{fixture.file_hash}.pdf"
+
+
+def test_is_pdf():
+    fixture = PDF_FIXTURES[0]
+
+    assert is_pdf(fixture.get_full_path())
+    assert is_pdf(fixture.get_full_path().read_bytes())
+
+
+def test_get_page_count():
+    fixture = PDF_FIXTURES[0]
+
+    assert fixture.page_count == load_document(fixture.get_full_path()).page_count
+    assert (
+        fixture.page_count
+        == load_document(fixture.get_full_path().read_bytes()).page_count
+    )
+
+
+def test_load_documents():
+    fixture = PDF_FIXTURES[0]
+
+    docs = load_documents([fixture.get_full_path()] * 3)
+
+    assert len(docs) == 3
+
+
+def test_hash_from_bytes__large_file():
+    # 200MB file
+
+    random_bytes = b"0" * 1024 * 1024 * 200
+
+    assert hash_from_bytes(random_bytes) == "8a9566fd729cce6410050771422e42b8"
+
+
 def test_rasterize():
     # Fow now just test PIL can open the image
     for fixture in PDF_FIXTURES:
         doc = load_document(fixture.get_full_path())
         img_bytes = doc.rasterize_page(1)
         Image.open(io.BytesIO(img_bytes))
 
@@ -109,22 +155,41 @@
 def test_split():
     doc = load_document(PDF_FIXTURES[0].get_full_path())
 
     new_docs = doc.split(start=2)
 
     assert len(new_docs) == len(doc) - 2
 
+    new_docs = doc.split(stop=2)
+
+    assert len(new_docs) == 2
+
+    with pytest.raises(ValueError):
+        doc.split()
+
 
 def test_pdf_split_iter_fast_1_sized():
     doc = load_document(PDF_FIXTURES[0].get_full_path())
 
     splits = list(pdf_split_iter_fast(doc.file_bytes, 1))
 
     assert len(splits) == len(doc)
 
 
+def test_pdf_split_iter_max_bytes():
+    doc = load_document(PDF_FIXTURES[0].get_full_path())
+
+    splits = list(
+        pdf_split_iter_with_max_bytes(
+            doc.file_bytes, max_page_count=1, max_bytes=1024 * 1024
+        )
+    )
+
+    assert len(splits) == len(doc)
+
+
 def test_compression():
     for fixture in PDF_FIXTURES:
         doc = load_document(fixture.get_full_path())
         compressed_bytes = doc.to_compressed_bytes()
 
         assert len(compressed_bytes) < len(doc.file_bytes)
```

### Comparing `docprompt-0.3.1/tests/test_documentnode.py` & `docprompt-0.4.0/tests/test_documentnode.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/tests/test_layout_models.py` & `docprompt-0.4.0/tests/test_layout_models.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/tests/test_search.py` & `docprompt-0.4.0/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/tests/test_threadpool.py` & `docprompt-0.4.0/tests/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/tests/util.py` & `docprompt-0.4.0/tests/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.3.1/PKG-INFO` & `docprompt-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docprompt
-Version: 0.3.1
+Version: 0.4.0
 Summary: Documents and large language models.
 Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0
 Author: Frankie Colson
 Author-email: frank@pageleaf.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docprompt Version: 0.3.1 Summary: Documents and
+Metadata-Version: 2.1 Name: docprompt Version: 0.4.0 Summary: Documents and
 large language models. Home-page: https://github.com/Page-Leaf/docprompt
 License: Apache-2.0 Author: Frankie Colson Author-email: frank@pageleaf.io
 Requires-Python: >=3.8.1,<3.13 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

