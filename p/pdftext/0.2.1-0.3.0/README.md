# Comparing `tmp/pdftext-0.2.1.tar.gz` & `tmp/pdftext-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdftext-0.2.1.tar", max compression
+gzip compressed data, was "pdftext-0.3.0.tar", max compression
```

## Comparing `pdftext-0.2.1.tar` & `pdftext-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11269 2024-04-26 23:32:59.959509 pdftext-0.2.1/LICENSE
--rw-r--r--   0        0        0     6599 2024-04-26 23:32:59.959509 pdftext-0.2.1/README.md
--rw-r--r--   0        0        0     1198 2024-04-26 23:32:59.959509 pdftext-0.2.1/extract_text.py
--rw-r--r--   0        0        0    17369 2024-04-26 23:32:59.959509 pdftext-0.2.1/models/dt.joblib
--rw-r--r--   0        0        0     1850 2024-04-26 23:32:59.959509 pdftext-0.2.1/pdftext/extraction.py
--rw-r--r--   0        0        0     5867 2024-04-26 23:32:59.959509 pdftext-0.2.1/pdftext/inference.py
--rw-r--r--   0        0        0      153 2024-04-26 23:32:59.959509 pdftext-0.2.1/pdftext/model.py
--rw-r--r--   0        0        0     3720 2024-04-26 23:32:59.963508 pdftext-0.2.1/pdftext/pdf/chars.py
--rw-r--r--   0        0        0     4859 2024-04-26 23:32:59.963508 pdftext-0.2.1/pdftext/pdf/utils.py
--rw-r--r--   0        0        0     2129 2024-04-26 23:32:59.963508 pdftext-0.2.1/pdftext/postprocessing.py
--rw-r--r--   0        0        0      478 2024-04-26 23:32:59.963508 pdftext-0.2.1/pdftext/settings.py
--rw-r--r--   0        0        0      856 2024-04-26 23:32:59.963508 pdftext-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7575 1970-01-01 00:00:00.000000 pdftext-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11269 2024-04-29 21:33:48.672356 pdftext-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6770 2024-04-29 21:33:48.672356 pdftext-0.3.0/README.md
+-rw-r--r--   0        0        0     1333 2024-04-29 21:33:48.672356 pdftext-0.3.0/extract_text.py
+-rw-r--r--   0        0        0    14097 2024-04-29 21:33:48.672356 pdftext-0.3.0/models/dt.joblib
+-rw-r--r--   0        0        0     2014 2024-04-29 21:33:48.672356 pdftext-0.3.0/pdftext/extraction.py
+-rw-r--r--   0        0        0     6826 2024-04-29 21:33:48.672356 pdftext-0.3.0/pdftext/inference.py
+-rw-r--r--   0        0        0      153 2024-04-29 21:33:48.672356 pdftext-0.3.0/pdftext/model.py
+-rw-r--r--   0        0        0     3720 2024-04-29 21:33:48.672356 pdftext-0.3.0/pdftext/pdf/chars.py
+-rw-r--r--   0        0        0     4707 2024-04-29 21:33:48.672356 pdftext-0.3.0/pdftext/pdf/utils.py
+-rw-r--r--   0        0        0     3249 2024-04-29 21:33:48.672356 pdftext-0.3.0/pdftext/postprocessing.py
+-rw-r--r--   0        0        0      478 2024-04-29 21:33:48.672356 pdftext-0.3.0/pdftext/settings.py
+-rw-r--r--   0        0        0      856 2024-04-29 21:33:48.672356 pdftext-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7746 1970-01-01 00:00:00.000000 pdftext-0.3.0/PKG-INFO
```

### Comparing `pdftext-0.2.1/LICENSE` & `pdftext-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdftext-0.2.1/README.md` & `pdftext-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 ```shell
 pdftext PDF_PATH --out_path output.txt
 ```
 
 - `PDF_PATH` must be a single pdf file.
 - `--out_path` path to the output txt file.  If not specified, will write to stdout.
 - `--sort` will attempt to sort in reading order if specified.
+- `--keep_hyphens` will keep hyphens in the output (they will be stripped and words joined otherwise)
 
 ## JSON
 
 This command outputs structured blocks and lines with font and other information.
 
 ```shell
 pdftext PDF_PATH --out_path output.txt --output_type json
@@ -44,21 +45,22 @@
 - `bbox` - the page bbox, in `[x1, y1, x2, y2]` format
 - `rotation` - how much the page is rotated, in degrees (`0`, `90`, `180`, or `270`)
 - `page_idx` - the index of the page
 - `blocks` - the blocks that make up the text in the pdf.  Approximately equal to a paragraph.
   - `bbox` - the block bbox, in `[x1, y1, x2, y2]` format
   - `lines` - the lines inside the block
     - `bbox` - the line bbox, in `[x1, y1, x2, y2]` format
-    - `chars` - the individual characters in the line
-      - `char` - the actual character, encoded in utf-8
-      - `rotation` - how much the character is rotated, in degrees
-      - `bbox` - the character bbox, in `[x1, y1, x2, y2]` format
-      - `char_idx` - the index of the character on the page (from `0` to number of characters, in original pdf order)
+    - `spans` - the individual text spans in the line (text spans have the same font/weight/etc)
+      - `text` - the text in the span, encoded in utf-8
+      - `rotation` - how much the span is rotated, in degrees
+      - `bbox` - the span bbox, in `[x1, y1, x2, y2]` format
+      - `char_start_idx` - the start index of the first span character in the pdf
+      - `char_end_idx` - the end index of the last span character in the pdf
       - `font` this is font info straight from the pdf, see [this pdfium code](https://pdfium.googlesource.com/pdfium/+/refs/heads/main/public/fpdf_text.h)
-        - `size` - the size of the font used for the character
+        - `size` - the size of the font used for the text
         - `weight` - font weight
         - `name` - font name, may be None
         - `flags` - font flags, in the format of the `PDF spec 1.7 Section 5.7.1 Font Descriptor Flags`
 
 If the pdf is rotated, the bboxes will be relative to the rotated page (they're rotated after being extracted).
 
 # Programmatic usage
```

### Comparing `pdftext-0.2.1/extract_text.py` & `pdftext-0.3.0/extract_text.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 
 def main():
     parser = argparse.ArgumentParser(description="Extract plain text from PDF.  Not guaranteed to be in order.")
     parser.add_argument("pdf_path", type=str, help="Path to the PDF file")
     parser.add_argument("--out_path", type=str, help="Path to the output text file, defaults to stdout", default=None)
     parser.add_argument("--output_type", type=str, help="Type of output to generate", default="plain_text")
     parser.add_argument("--sort", action="store_true", help="Attempt to sort the text by reading order", default=False)
+    parser.add_argument("--keep_hyphens", action="store_true", help="Keep hyphens in words", default=False)
     args = parser.parse_args()
 
     assert args.output_type in ["plain_text", "json"], "Invalid output type, must be 'plain_text' or 'json'"
 
     if args.output_type == "plain_text":
-        text = plain_text_output(args.pdf_path, sort=args.sort)
+        text = plain_text_output(args.pdf_path, sort=args.sort, hyphens=args.keep_hyphens)
     elif args.output_type == "json":
         text = dictionary_output(args.pdf_path, sort=args.sort)
         text = json.dumps(text)
 
     if args.out_path is None:
         print(text)
     else:
```

### Comparing `pdftext-0.2.1/pdftext/extraction.py` & `pdftext-0.3.0/pdftext/extraction.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 from typing import List
 
 from pdftext.inference import inference
 from pdftext.model import get_model
 from pdftext.pdf.chars import get_pdfium_chars
 from pdftext.pdf.utils import unnormalize_bbox
-from pdftext.postprocessing import merge_text, sort_blocks, postprocess_text
+from pdftext.postprocessing import merge_text, sort_blocks, postprocess_text, handle_hyphens
 
 
 def _get_pages(pdf_path, model=None):
     if model is None:
         model = get_model()
     text_chars = get_pdfium_chars(pdf_path)
     pages = inference(text_chars, model)
     return pages
 
 
-def plain_text_output(pdf_path, sort=False, model=None) -> str:
-    text = paginated_plain_text_output(pdf_path, sort=sort, model=model)
+def plain_text_output(pdf_path, sort=False, model=None, hyphens=False) -> str:
+    text = paginated_plain_text_output(pdf_path, sort=sort, model=model, hyphens=hyphens)
     return "\n".join(text)
 
 
-def paginated_plain_text_output(pdf_path, sort=False, model=None) -> List[str]:
+def paginated_plain_text_output(pdf_path, sort=False, model=None, hyphens=False) -> List[str]:
     pages = _get_pages(pdf_path, model)
     text = []
     for page in pages:
-        text.append(merge_text(page, sort=sort).strip())
+        text.append(merge_text(page, sort=sort, hyphens=hyphens).strip())
     return text
 
 
 def dictionary_output(pdf_path, sort=False, model=None):
     pages = _get_pages(pdf_path, model)
     for page in pages:
         for block in page["blocks"]:
             bad_keys = [key for key in block.keys() if key not in ["lines", "bbox"]]
             for key in bad_keys:
                 del block[key]
             for line in block["lines"]:
-                bad_keys = [key for key in line.keys() if key not in ["chars", "bbox"]]
+                bad_keys = [key for key in line.keys() if key not in ["bbox", "spans"]]
                 for key in bad_keys:
                     del line[key]
-                for char in line["chars"]:
-                    char["bbox"] = unnormalize_bbox(char["bbox"], page["width"], page["height"])
-                    char["char"] = postprocess_text(char["char"])
+                for span in line["spans"]:
+                    span["bbox"] = unnormalize_bbox(span["bbox"], page["width"], page["height"])
+                    span["text"] = postprocess_text(span["text"])
+                    span["text"] = handle_hyphens(span["text"], keep_hyphens=True)
+
                 line["bbox"] = unnormalize_bbox(line["bbox"], page["width"], page["height"])
             block["bbox"] = unnormalize_bbox(block["bbox"], page["width"], page["height"])
         if sort:
             page["blocks"] = sort_blocks(page["blocks"])
     return pages
```

### Comparing `pdftext-0.2.1/pdftext/inference.py` & `pdftext-0.3.0/pdftext/inference.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,71 +64,85 @@
         "block_y_start_gap": char_y1 - currblock["bbox"][1]
     }
 
     return training_row
 
 
 def update_span(line, span):
+    if len(span["chars"]) > 0:
+        span["font"] = span["chars"][0]["font"]
+        span["rotation"] = span["chars"][0]["rotation"]
+        char_bboxes = [char["bbox"] for char in span["chars"]]
+        span["bbox"] = [min([bbox[0] for bbox in char_bboxes]),
+                        min([bbox[1] for bbox in char_bboxes]),
+                        max([bbox[2] for bbox in char_bboxes]),
+                        max([bbox[3] for bbox in char_bboxes])]
+        span["text"] = "".join([char["char"] for char in span["chars"]])
+        span["char_start_idx"] = span["chars"][0]["char_idx"]
+        span["char_end_idx"] = span["chars"][-1]["char_idx"]
+
+    del span["chars"]
     line["spans"].append(span)
     span = {"chars": []}
     return span
 
 
 def update_line(block, line):
-    line["chars"] = list(chain.from_iterable(s["chars"] for s in line["spans"]))
-    del line["spans"]
     block["lines"].append(line)
     line = {"spans": []}
     return line
 
 
 def update_block(blocks, block):
     blocks["blocks"].append(block)
     block = {"lines": []}
     return block
 
 
 def infer_single_page(text_chars):
     prev_char = None
+    prev_font_info = None
 
     blocks = {
         "blocks": [],
         "page": text_chars["page"],
         "rotation": text_chars["rotation"],
         "bbox": text_chars["bbox"],
         "width": text_chars["width"],
         "height": text_chars["height"],
     }
     block = {"lines": []}
     line = {"spans": []}
     span = {"chars": []}
     for i, char_info in enumerate(text_chars["chars"]):
+        font_info = f"{char_info['font']['name']}_{char_info['font']['size']}_{char_info['font']['weight']}_{char_info['font']['flags']}_{char_info['rotation']}"
         if prev_char:
             training_row = create_training_row(char_info, prev_char, block, line)
             sorted_keys = sorted(training_row.keys())
             training_row = [training_row[key] for key in sorted_keys]
 
             prediction = yield training_row
             if prediction == 0:
                 pass
-            elif prediction == 1:
-                span = update_span(line, span)
-            elif prediction == 2:
+            elif prediction == 2 and prev_char["char"] in LINE_BREAKS:
                 span = update_span(line, span)
                 line = update_line(block, line)
-            else:
+                block = update_block(blocks, block)
+            elif prev_char["char"] in LINE_BREAKS and prediction == 1: # Look for newline character as a forcing signal for a new line
                 span = update_span(line, span)
                 line = update_line(block, line)
-                block = update_block(blocks, block)
+            elif prev_font_info != font_info:
+                span = update_span(line, span)
 
         span["chars"].append(char_info)
         update_current(line, char_info)
         update_current(block, char_info)
 
         prev_char = char_info
+        prev_font_info = font_info
     if len(span["chars"]) > 0:
         update_span(line, span)
     if len(line["spans"]) > 0:
         update_line(block, line)
     if len(block["lines"]) > 0:
         update_block(blocks, block)
```

### Comparing `pdftext-0.2.1/pdftext/pdf/chars.py` & `pdftext-0.3.0/pdftext/pdf/chars.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.2.1/pdftext/pdf/utils.py` & `pdftext-0.3.0/pdftext/pdf/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,17 @@
 import pypdfium2.raw as pdfium_c
 import ctypes
 import math
 
 from pdftext.settings import settings
 
-LINE_BREAKS = ["\n", "\u000D", "\u000A", "\u000C"]
-TABS = ["\t", "\u0009"]
+LINE_BREAKS = ["\n", "\u000D", "\u000A"]
+TABS = ["\t", "\u0009", "\x09"]
 SPACES = [" ", "\ufffe", "\uFEFF", "\xa0"]
-HYPHEN = "-"
 WHITESPACE_CHARS = ["\n", "\r", "\f", "\t", " "]
-LIGATURES = {
-    "ﬀ": "ff",
-    "ﬃ": "ffi",
-    "ﬄ": "ffl",
-    "ﬁ": "fi",
-    "ﬂ": "fl",
-    "ﬆ": "st",
-    "ﬅ": "st",
-}
 
 
 def char_count(textpage, *rect):
     args = (textpage, *rect)
     n_chars = pdfium_c.FPDFText_GetBoundedText(*args, None, 0)
     if n_chars <= 0:
         return 0
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pdftext-0.2.1/pyproject.toml` & `pdftext-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdftext"
-version = "0.2.1"
+version = "0.3.0"
 description = "Extract structured text from pdfs quickly"
 authors = ["Vik Paruchuri <vik.paruchuri@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/VikParuchuri/pdftext"
 keywords = ["pdf", "text", "extraction"]
 packages = [
```

### Comparing `pdftext-0.2.1/PKG-INFO` & `pdftext-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdftext
-Version: 0.2.1
+Version: 0.3.0
 Summary: Extract structured text from pdfs quickly
 Home-page: https://github.com/VikParuchuri/pdftext
 License: Apache-2.0
 Keywords: pdf,text,extraction
 Author: Vik Paruchuri
 Author-email: vik.paruchuri@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
@@ -44,14 +44,15 @@
 ```shell
 pdftext PDF_PATH --out_path output.txt
 ```
 
 - `PDF_PATH` must be a single pdf file.
 - `--out_path` path to the output txt file.  If not specified, will write to stdout.
 - `--sort` will attempt to sort in reading order if specified.
+- `--keep_hyphens` will keep hyphens in the output (they will be stripped and words joined otherwise)
 
 ## JSON
 
 This command outputs structured blocks and lines with font and other information.
 
 ```shell
 pdftext PDF_PATH --out_path output.txt --output_type json
@@ -67,21 +68,22 @@
 - `bbox` - the page bbox, in `[x1, y1, x2, y2]` format
 - `rotation` - how much the page is rotated, in degrees (`0`, `90`, `180`, or `270`)
 - `page_idx` - the index of the page
 - `blocks` - the blocks that make up the text in the pdf.  Approximately equal to a paragraph.
   - `bbox` - the block bbox, in `[x1, y1, x2, y2]` format
   - `lines` - the lines inside the block
     - `bbox` - the line bbox, in `[x1, y1, x2, y2]` format
-    - `chars` - the individual characters in the line
-      - `char` - the actual character, encoded in utf-8
-      - `rotation` - how much the character is rotated, in degrees
-      - `bbox` - the character bbox, in `[x1, y1, x2, y2]` format
-      - `char_idx` - the index of the character on the page (from `0` to number of characters, in original pdf order)
+    - `spans` - the individual text spans in the line (text spans have the same font/weight/etc)
+      - `text` - the text in the span, encoded in utf-8
+      - `rotation` - how much the span is rotated, in degrees
+      - `bbox` - the span bbox, in `[x1, y1, x2, y2]` format
+      - `char_start_idx` - the start index of the first span character in the pdf
+      - `char_end_idx` - the end index of the last span character in the pdf
       - `font` this is font info straight from the pdf, see [this pdfium code](https://pdfium.googlesource.com/pdfium/+/refs/heads/main/public/fpdf_text.h)
-        - `size` - the size of the font used for the character
+        - `size` - the size of the font used for the text
         - `weight` - font weight
         - `name` - font name, may be None
         - `flags` - font flags, in the format of the `PDF spec 1.7 Section 5.7.1 Font Descriptor Flags`
 
 If the pdf is rotated, the bboxes will be relative to the rotated page (they're rotated after being extracted).
 
 # Programmatic usage
```

