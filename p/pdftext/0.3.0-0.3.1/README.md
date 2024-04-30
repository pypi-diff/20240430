# Comparing `tmp/pdftext-0.3.0.tar.gz` & `tmp/pdftext-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdftext-0.3.0.tar", max compression
+gzip compressed data, was "pdftext-0.3.1.tar", max compression
```

## Comparing `pdftext-0.3.0.tar` & `pdftext-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11269 2024-04-29 21:33:48.672356 pdftext-0.3.0/LICENSE
--rw-r--r--   0        0        0     6770 2024-04-29 21:33:48.672356 pdftext-0.3.0/README.md
--rw-r--r--   0        0        0     1333 2024-04-29 21:33:48.672356 pdftext-0.3.0/extract_text.py
--rw-r--r--   0        0        0    14097 2024-04-29 21:33:48.672356 pdftext-0.3.0/models/dt.joblib
--rw-r--r--   0        0        0     2014 2024-04-29 21:33:48.672356 pdftext-0.3.0/pdftext/extraction.py
--rw-r--r--   0        0        0     6826 2024-04-29 21:33:48.672356 pdftext-0.3.0/pdftext/inference.py
--rw-r--r--   0        0        0      153 2024-04-29 21:33:48.672356 pdftext-0.3.0/pdftext/model.py
--rw-r--r--   0        0        0     3720 2024-04-29 21:33:48.672356 pdftext-0.3.0/pdftext/pdf/chars.py
--rw-r--r--   0        0        0     4707 2024-04-29 21:33:48.672356 pdftext-0.3.0/pdftext/pdf/utils.py
--rw-r--r--   0        0        0     3249 2024-04-29 21:33:48.672356 pdftext-0.3.0/pdftext/postprocessing.py
--rw-r--r--   0        0        0      478 2024-04-29 21:33:48.672356 pdftext-0.3.0/pdftext/settings.py
--rw-r--r--   0        0        0      856 2024-04-29 21:33:48.672356 pdftext-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7746 1970-01-01 00:00:00.000000 pdftext-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11269 2024-04-29 22:48:52.015107 pdftext-0.3.1/LICENSE
+-rw-r--r--   0        0        0     7088 2024-04-29 22:48:52.015107 pdftext-0.3.1/README.md
+-rw-r--r--   0        0        0     1581 2024-04-29 22:48:52.015107 pdftext-0.3.1/extract_text.py
+-rw-r--r--   0        0        0    14097 2024-04-29 22:48:52.015107 pdftext-0.3.1/models/dt.joblib
+-rw-r--r--   0        0        0     2144 2024-04-29 22:48:52.015107 pdftext-0.3.1/pdftext/extraction.py
+-rw-r--r--   0        0        0     6826 2024-04-29 22:48:52.015107 pdftext-0.3.1/pdftext/inference.py
+-rw-r--r--   0        0        0      153 2024-04-29 22:48:52.015107 pdftext-0.3.1/pdftext/model.py
+-rw-r--r--   0        0        0     3752 2024-04-29 22:48:52.015107 pdftext-0.3.1/pdftext/pdf/chars.py
+-rw-r--r--   0        0        0     4707 2024-04-29 22:48:52.015107 pdftext-0.3.1/pdftext/pdf/utils.py
+-rw-r--r--   0        0        0     3249 2024-04-29 22:48:52.015107 pdftext-0.3.1/pdftext/postprocessing.py
+-rw-r--r--   0        0        0      478 2024-04-29 22:48:52.015107 pdftext-0.3.1/pdftext/settings.py
+-rw-r--r--   0        0        0      856 2024-04-29 22:48:52.019107 pdftext-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8064 1970-01-01 00:00:00.000000 pdftext-0.3.1/PKG-INFO
```

### Comparing `pdftext-0.3.0/LICENSE` & `pdftext-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.0/README.md` & `pdftext-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,27 +22,29 @@
 pdftext PDF_PATH --out_path output.txt
 ```
 
 - `PDF_PATH` must be a single pdf file.
 - `--out_path` path to the output txt file.  If not specified, will write to stdout.
 - `--sort` will attempt to sort in reading order if specified.
 - `--keep_hyphens` will keep hyphens in the output (they will be stripped and words joined otherwise)
+- `--pages` will specify pages (comma separated) to extract
 
 ## JSON
 
 This command outputs structured blocks and lines with font and other information.
 
 ```shell
-pdftext PDF_PATH --out_path output.txt --output_type json
+pdftext PDF_PATH --out_path output.txt --json
 ```
 
 - `PDF_PATH` must be a single pdf file.
 - `--out_path` path to the output txt file.  If not specified, will write to stdout.
-- `--output_type` specifies whether to write out plain text (default) or json
+- `--json` specifies json output
 - `--sort` will attempt to sort in reading order if specified.
+- `--pages` will specify pages (comma separated) to extract
 
 The output will be a json list, with each item in the list corresponding to a single page in the input pdf (in order).  Each page will include the following keys:
 
 - `bbox` - the page bbox, in `[x1, y1, x2, y2]` format
 - `rotation` - how much the page is rotated, in degrees (`0`, `90`, `180`, or `270`)
 - `page_idx` - the index of the page
 - `blocks` - the blocks that make up the text in the pdf.  Approximately equal to a paragraph.
@@ -64,25 +66,29 @@
 If the pdf is rotated, the bboxes will be relative to the rotated page (they're rotated after being extracted).
 
 # Programmatic usage
 
 Extract plain text:
 
 ```python
+import pypdfium2 as pdfium
 from pdftext.extraction import plain_text_output
 
-text = plain_text_output(PDF_PATH, sort=False)
+pdf = pdfium.PdfDocument(PDF_PATH)
+text = plain_text_output(pdf, sort=False, hyphens=False, page_range=[1,2,3]) # Optional arguments explained above
 ```
 
 Extract structured blocks and lines:
 
 ```python
+import pypdfium2 as pdfium
 from pdftext.extraction import dictionary_output
 
-text = dictionary_output(PDF_PATH)
+pdf = pdfium.PdfDocument(PDF_PATH)
+text = dictionary_output(pdf, sort=False, page_range=[1,2,3]) # Optional arguments explained above
 ```
 
 If you want more customization, check out the `pdftext.extraction._get_pages` function for a starting point to dig deeper.  pdftext is a pretty thin wrapper around [pypdfium2](https://pypdfium2.readthedocs.io/en/stable/), so you might want to look at the documentation for that as well.
 
 # Benchmarks
 
 I benchmarked extraction speed and accuracy of [pymupdf](https://pymupdf.readthedocs.io/en/latest/), [pdfplumber](https://github.com/jsvine/pdfplumber), and pdftext.  I chose pymupdf because it extracts blocks and lines.  Pdfplumber extracts words and bboxes.  I did not benchmark pypdf, even though it is a great library, because it doesn't provide individual character/line/block and bbox information.
```

### Comparing `pdftext-0.3.0/extract_text.py` & `pdftext-0.3.1/extract_text.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 import argparse
 import json
+import pypdfium2 as pdfium
 
 from pdftext.extraction import plain_text_output, dictionary_output
 
 
 def main():
     parser = argparse.ArgumentParser(description="Extract plain text from PDF.  Not guaranteed to be in order.")
     parser.add_argument("pdf_path", type=str, help="Path to the PDF file")
     parser.add_argument("--out_path", type=str, help="Path to the output text file, defaults to stdout", default=None)
-    parser.add_argument("--output_type", type=str, help="Type of output to generate", default="plain_text")
+    parser.add_argument("--json", action="store_true", help="Output json instead of plain text", default=False)
     parser.add_argument("--sort", action="store_true", help="Attempt to sort the text by reading order", default=False)
     parser.add_argument("--keep_hyphens", action="store_true", help="Keep hyphens in words", default=False)
+    parser.add_argument("--pages", type=str, help="Comma separated pages to extract, like 1,2,3", default=None)
     args = parser.parse_args()
 
-    assert args.output_type in ["plain_text", "json"], "Invalid output type, must be 'plain_text' or 'json'"
+    pdf_doc = pdfium.PdfDocument(args.pdf_path)
+    pages = None
+    if args.pages is not None:
+        pages = [int(p) for p in args.pages.split(",")]
+        assert all(p <= len(pdf_doc) for p in pages), "Invalid page number(s) provided"
 
-    if args.output_type == "plain_text":
-        text = plain_text_output(args.pdf_path, sort=args.sort, hyphens=args.keep_hyphens)
-    elif args.output_type == "json":
-        text = dictionary_output(args.pdf_path, sort=args.sort)
+    if args.json:
+        text = dictionary_output(pdf_doc, sort=args.sort, page_range=pages)
         text = json.dumps(text)
+    else:
+        text = plain_text_output(pdf_doc, sort=args.sort, hyphens=args.keep_hyphens, page_range=pages)
 
     if args.out_path is None:
         print(text)
     else:
         with open(args.out_path, "w+") as f:
             f.write(text)
```

### Comparing `pdftext-0.3.0/models/dt.joblib` & `pdftext-0.3.1/models/dt.joblib`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.0/pdftext/extraction.py` & `pdftext-0.3.1/pdftext/extraction.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 from pdftext.inference import inference
 from pdftext.model import get_model
 from pdftext.pdf.chars import get_pdfium_chars
 from pdftext.pdf.utils import unnormalize_bbox
 from pdftext.postprocessing import merge_text, sort_blocks, postprocess_text, handle_hyphens
 
 
-def _get_pages(pdf_path, model=None):
+def _get_pages(pdf_doc, model=None, page_range=None):
     if model is None:
         model = get_model()
-    text_chars = get_pdfium_chars(pdf_path)
+    text_chars = get_pdfium_chars(pdf_doc, page_range=page_range)
     pages = inference(text_chars, model)
     return pages
 
 
-def plain_text_output(pdf_path, sort=False, model=None, hyphens=False) -> str:
-    text = paginated_plain_text_output(pdf_path, sort=sort, model=model, hyphens=hyphens)
+def plain_text_output(pdf_doc, sort=False, model=None, hyphens=False, page_range=None) -> str:
+    text = paginated_plain_text_output(pdf_doc, sort=sort, model=model, hyphens=hyphens, page_range=page_range)
     return "\n".join(text)
 
 
-def paginated_plain_text_output(pdf_path, sort=False, model=None, hyphens=False) -> List[str]:
-    pages = _get_pages(pdf_path, model)
+def paginated_plain_text_output(pdf_doc, sort=False, model=None, hyphens=False, page_range=None) -> List[str]:
+    pages = _get_pages(pdf_doc, model, page_range)
     text = []
     for page in pages:
         text.append(merge_text(page, sort=sort, hyphens=hyphens).strip())
     return text
 
 
-def dictionary_output(pdf_path, sort=False, model=None):
-    pages = _get_pages(pdf_path, model)
+def dictionary_output(pdf_doc, sort=False, model=None, page_range=None):
+    pages = _get_pages(pdf_doc, model, page_range)
     for page in pages:
         for block in page["blocks"]:
             bad_keys = [key for key in block.keys() if key not in ["lines", "bbox"]]
             for key in bad_keys:
                 del block[key]
             for line in block["lines"]:
                 bad_keys = [key for key in line.keys() if key not in ["bbox", "spans"]]
```

### Comparing `pdftext-0.3.0/pdftext/inference.py` & `pdftext-0.3.1/pdftext/inference.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.0/pdftext/pdf/chars.py` & `pdftext-0.3.1/pdftext/pdf/chars.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,19 +19,20 @@
         # If we hit the region with the previous fontname, we can bail out
         if fontname == prev_fontname:
             break
         text_chars["chars"][j]["font"]["name"] = fontname
         text_chars["chars"][j]["font"]["flags"] = fontflags
 
 
-def get_pdfium_chars(pdf_path, fontname_sample_freq=settings.FONTNAME_SAMPLE_FREQ):
-    pdf = pdfium.PdfDocument(pdf_path)
+def get_pdfium_chars(pdf, fontname_sample_freq=settings.FONTNAME_SAMPLE_FREQ, page_range=None):
     blocks = []
+    if page_range is None:
+        page_range = range(len(pdf))
 
-    for page_idx in range(len(pdf)):
+    for page_idx in page_range:
         page = pdf.get_page(page_idx)
         text_page = page.get_textpage()
         mediabox = page.get_mediabox()
         page_rotation = page.get_rotation()
         bbox = page.get_bbox()
         page_width = math.ceil(abs(bbox[2] - bbox[0]))
         page_height = math.ceil(abs(bbox[1] - bbox[3]))
```

### Comparing `pdftext-0.3.0/pdftext/pdf/utils.py` & `pdftext-0.3.1/pdftext/pdf/utils.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.0/pdftext/postprocessing.py` & `pdftext-0.3.1/pdftext/postprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     text = replace_control_chars(text)
     text = replace_ligatures(text)
     return text
 
 
 def handle_hyphens(text: str, keep_hyphens=False) -> str:
     if keep_hyphens:
-        text = text.replace(HYPHEN_CHAR, "-")
+        text = text.replace(HYPHEN_CHAR, "-\n")
     elif len(text) == 0:
         pass
     else:
         new_text = ""
         found_hyphen = False
         for i in range(len(text) - 1):
             if text[i] == HYPHEN_CHAR and text[i+1] in LINE_BREAKS:
@@ -102,11 +102,11 @@
             line_text = ""
             for span in line["spans"]:
                 line_text += span["text"]
             line_text = postprocess_text(line_text)
             line_text = line_text.rstrip() + "\n"
 
             block_text += line_text
-        block_text = block_text.rstrip() + "\n\n"
+        block_text = block_text.rstrip() + "\n"
         text += block_text
     text = handle_hyphens(text, keep_hyphens=hyphens)
     return text
```

### Comparing `pdftext-0.3.0/pyproject.toml` & `pdftext-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdftext"
-version = "0.3.0"
+version = "0.3.1"
 description = "Extract structured text from pdfs quickly"
 authors = ["Vik Paruchuri <vik.paruchuri@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/VikParuchuri/pdftext"
 keywords = ["pdf", "text", "extraction"]
 packages = [
```

### Comparing `pdftext-0.3.0/PKG-INFO` & `pdftext-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdftext
-Version: 0.3.0
+Version: 0.3.1
 Summary: Extract structured text from pdfs quickly
 Home-page: https://github.com/VikParuchuri/pdftext
 License: Apache-2.0
 Keywords: pdf,text,extraction
 Author: Vik Paruchuri
 Author-email: vik.paruchuri@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
@@ -45,27 +45,29 @@
 pdftext PDF_PATH --out_path output.txt
 ```
 
 - `PDF_PATH` must be a single pdf file.
 - `--out_path` path to the output txt file.  If not specified, will write to stdout.
 - `--sort` will attempt to sort in reading order if specified.
 - `--keep_hyphens` will keep hyphens in the output (they will be stripped and words joined otherwise)
+- `--pages` will specify pages (comma separated) to extract
 
 ## JSON
 
 This command outputs structured blocks and lines with font and other information.
 
 ```shell
-pdftext PDF_PATH --out_path output.txt --output_type json
+pdftext PDF_PATH --out_path output.txt --json
 ```
 
 - `PDF_PATH` must be a single pdf file.
 - `--out_path` path to the output txt file.  If not specified, will write to stdout.
-- `--output_type` specifies whether to write out plain text (default) or json
+- `--json` specifies json output
 - `--sort` will attempt to sort in reading order if specified.
+- `--pages` will specify pages (comma separated) to extract
 
 The output will be a json list, with each item in the list corresponding to a single page in the input pdf (in order).  Each page will include the following keys:
 
 - `bbox` - the page bbox, in `[x1, y1, x2, y2]` format
 - `rotation` - how much the page is rotated, in degrees (`0`, `90`, `180`, or `270`)
 - `page_idx` - the index of the page
 - `blocks` - the blocks that make up the text in the pdf.  Approximately equal to a paragraph.
@@ -87,25 +89,29 @@
 If the pdf is rotated, the bboxes will be relative to the rotated page (they're rotated after being extracted).
 
 # Programmatic usage
 
 Extract plain text:
 
 ```python
+import pypdfium2 as pdfium
 from pdftext.extraction import plain_text_output
 
-text = plain_text_output(PDF_PATH, sort=False)
+pdf = pdfium.PdfDocument(PDF_PATH)
+text = plain_text_output(pdf, sort=False, hyphens=False, page_range=[1,2,3]) # Optional arguments explained above
 ```
 
 Extract structured blocks and lines:
 
 ```python
+import pypdfium2 as pdfium
 from pdftext.extraction import dictionary_output
 
-text = dictionary_output(PDF_PATH)
+pdf = pdfium.PdfDocument(PDF_PATH)
+text = dictionary_output(pdf, sort=False, page_range=[1,2,3]) # Optional arguments explained above
 ```
 
 If you want more customization, check out the `pdftext.extraction._get_pages` function for a starting point to dig deeper.  pdftext is a pretty thin wrapper around [pypdfium2](https://pypdfium2.readthedocs.io/en/stable/), so you might want to look at the documentation for that as well.
 
 # Benchmarks
 
 I benchmarked extraction speed and accuracy of [pymupdf](https://pymupdf.readthedocs.io/en/latest/), [pdfplumber](https://github.com/jsvine/pdfplumber), and pdftext.  I chose pymupdf because it extracts blocks and lines.  Pdfplumber extracts words and bboxes.  I did not benchmark pypdf, even though it is a great library, because it doesn't provide individual character/line/block and bbox information.
```

