# Comparing `tmp/progress-table-2.2.2.tar.gz` & `tmp/progress-table-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progress-table-2.2.2.tar", last modified: Mon Apr 29 18:22:13 2024, max compression
+gzip compressed data, was "progress-table-2.2.3.tar", last modified: Tue Apr 30 12:52:45 2024, max compression
```

## Comparing `progress-table-2.2.2.tar` & `progress-table-2.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:22:13.621395 progress-table-2.2.2/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1052 2022-11-17 19:44:00.000000 progress-table-2.2.2/LICENSE.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)     5159 2024-04-29 18:22:13.621395 progress-table-2.2.2/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4017 2024-04-29 18:22:09.000000 progress-table-2.2.2/README.md
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:22:13.621395 progress-table-2.2.2/progress_table/
--rw-r--r--   0 gaha      (1000) gaha      (1000)      334 2024-04-29 18:22:09.000000 progress-table-2.2.2/progress_table/__init__.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:22:13.621395 progress-table-2.2.2/progress_table/v0/
--rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-05 19:18:13.000000 progress-table-2.2.2/progress_table/v0/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)    23444 2024-04-05 20:02:34.000000 progress-table-2.2.2/progress_table/v0/progress_table.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     3028 2024-04-04 15:47:39.000000 progress-table-2.2.2/progress_table/v0/symbols.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:22:13.621395 progress-table-2.2.2/progress_table/v1/
--rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-04 15:47:39.000000 progress-table-2.2.2/progress_table/v1/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1500 2024-04-29 17:54:03.000000 progress-table-2.2.2/progress_table/v1/common.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)    46305 2024-04-29 17:54:03.000000 progress-table-2.2.2/progress_table/v1/progress_table.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     7475 2024-04-29 18:02:33.000000 progress-table-2.2.2/progress_table/v1/styles.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:22:13.621395 progress-table-2.2.2/progress_table.egg-info/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     5159 2024-04-29 18:22:13.000000 progress-table-2.2.2/progress_table.egg-info/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4883 2024-03-12 12:10:39.000000 progress-table-2.2.2/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO
--rw-r--r--   0 gaha      (1000) gaha      (1000)      621 2024-04-29 18:22:13.000000 progress-table-2.2.2/progress_table.egg-info/SOURCES.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-04-29 18:22:13.000000 progress-table-2.2.2/progress_table.egg-info/dependency_links.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        9 2024-04-29 18:22:13.000000 progress-table-2.2.2/progress_table.egg-info/requires.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)       15 2024-04-29 18:22:13.000000 progress-table-2.2.2/progress_table.egg-info/top_level.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-03-11 20:11:56.000000 progress-table-2.2.2/pyproject.toml
--rw-r--r--   0 gaha      (1000) gaha      (1000)      110 2024-04-29 18:22:13.621395 progress-table-2.2.2/setup.cfg
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1725 2024-04-29 18:22:09.000000 progress-table-2.2.2/setup.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 18:22:13.621395 progress-table-2.2.2/tests/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1804 2024-04-06 12:00:21.000000 progress-table-2.2.2/tests/test_docs_automated.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1867 2024-04-28 20:30:31.000000 progress-table-2.2.2/tests/test_examples_automated.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-30 12:52:45.224407 progress-table-2.2.3/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1052 2022-11-17 19:44:00.000000 progress-table-2.2.3/LICENSE.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     5161 2024-04-30 12:52:45.224407 progress-table-2.2.3/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     3911 2024-04-30 12:52:25.000000 progress-table-2.2.3/README.md
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-30 12:52:45.224407 progress-table-2.2.3/progress_table/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      334 2024-04-30 12:52:25.000000 progress-table-2.2.3/progress_table/__init__.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-30 12:52:45.224407 progress-table-2.2.3/progress_table/v0/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-05 19:18:13.000000 progress-table-2.2.3/progress_table/v0/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)    23444 2024-04-05 20:02:34.000000 progress-table-2.2.3/progress_table/v0/progress_table.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     3028 2024-04-04 15:47:39.000000 progress-table-2.2.3/progress_table/v0/symbols.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-30 12:52:45.224407 progress-table-2.2.3/progress_table/v1/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-04 15:47:39.000000 progress-table-2.2.3/progress_table/v1/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1500 2024-04-29 17:54:03.000000 progress-table-2.2.3/progress_table/v1/common.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)    46305 2024-04-30 12:52:25.000000 progress-table-2.2.3/progress_table/v1/progress_table.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     7801 2024-04-30 12:52:25.000000 progress-table-2.2.3/progress_table/v1/styles.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-30 12:52:45.224407 progress-table-2.2.3/progress_table.egg-info/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     5161 2024-04-30 12:52:45.000000 progress-table-2.2.3/progress_table.egg-info/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4883 2024-03-12 12:10:39.000000 progress-table-2.2.3/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      621 2024-04-30 12:52:45.000000 progress-table-2.2.3/progress_table.egg-info/SOURCES.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-04-30 12:52:45.000000 progress-table-2.2.3/progress_table.egg-info/dependency_links.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        9 2024-04-30 12:52:45.000000 progress-table-2.2.3/progress_table.egg-info/requires.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       15 2024-04-30 12:52:45.000000 progress-table-2.2.3/progress_table.egg-info/top_level.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-03-11 20:11:56.000000 progress-table-2.2.3/pyproject.toml
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      110 2024-04-30 12:52:45.224407 progress-table-2.2.3/setup.cfg
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1925 2024-04-30 12:52:25.000000 progress-table-2.2.3/setup.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-30 12:52:45.224407 progress-table-2.2.3/tests/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1854 2024-04-30 12:52:25.000000 progress-table-2.2.3/tests/test_docs_automated.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1867 2024-04-30 12:39:49.000000 progress-table-2.2.3/tests/test_examples_automated.py
```

### Comparing `progress-table-2.2.2/LICENSE.txt` & `progress-table-2.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.2/PKG-INFO` & `progress-table-2.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-table
-Version: 2.2.2
+Version: 2.2.3
 Summary: Display progress as a pretty table in the command line.
 Home-page: https://github.com/gahaalt/progress-table.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -96,20 +96,20 @@
     table.next_row()
 
 # Close the table when it's finished
 table.close()
 
 ```
 
-> Go to [integrations](https://github.com/sjmikler/progress-table/blob/main/docs/integrations.md)
+> Go to [integrations](https://github.com/sjmikler/progress-table/blob/main/docs//integrations.md)
 > page to see examples of integration with deep learning libraries.
 
 ## Advanced usage
 
-Go to [advanced usage](https://github.com/sjmikler/progress-table/blob/main/docs/advanced-usage.md) page for more information.
+Go to [advanced usage](https://github.com/sjmikler/progress-table/blob/main/docs//advanced-usage.md) page for more information.
 
 ## Troubleshooting
 
 ### Exceesive output
 
 Progress Table works correctly in most consoles, but there are some exceptions:
```

### Comparing `progress-table-2.2.2/README.md` & `progress-table-2.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -75,20 +75,20 @@
     table.next_row()
 
 # Close the table when it's finished
 table.close()
 
 ```
 
-> Go to [integrations](https://github.com/sjmikler/progress-table/blob/main/docs/integrations.md)
+> Go to [integrations](docs/integrations.md)
 > page to see examples of integration with deep learning libraries.
 
 ## Advanced usage
 
-Go to [advanced usage](https://github.com/sjmikler/progress-table/blob/main/docs/advanced-usage.md) page for more information.
+Go to [advanced usage](docs/advanced-usage.md) page for more information.
 
 ## Troubleshooting
 
 ### Exceesive output
 
 Progress Table works correctly in most consoles, but there are some exceptions:
```

### Comparing `progress-table-2.2.2/progress_table/v0/progress_table.py` & `progress-table-2.2.3/progress_table/v0/progress_table.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.2/progress_table/v0/symbols.py` & `progress-table-2.2.3/progress_table/v0/symbols.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.2/progress_table/v1/common.py` & `progress-table-2.2.3/progress_table/v1/common.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.2/progress_table/v1/progress_table.py` & `progress-table-2.2.3/progress_table/v1/progress_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         default_row_color: ColorFormat = None,
         pbar_show_throughput: bool = True,
         pbar_show_progress: bool = False,
         pbar_show_percents: bool = False,
         pbar_show_eta: bool = False,
         pbar_embedded: bool = True,
         pbar_style: str | Type[styles.PbarStyleBase] = "square",
-        pbar_style_embed: str | Type[styles.PbarStyleBase] = "embed",
+        pbar_style_embed: str | Type[styles.PbarStyleBase] = "cdots",
         print_header_on_top: bool = True,
         print_header_every_n_rows: int = 30,
         custom_cell_format: Callable[[Any], str] | None = None,
         table_style: str | Type[styles.TableStyleBase] = "round",
         file=None,
         # Deprecated arguments
         custom_format: None = None,
```

### Comparing `progress-table-2.2.2/progress_table/v1/styles.py` & `progress-table-2.2.3/progress_table/v1/styles.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,21 +130,14 @@
 class PbarStyleAngled(PbarStyleBase):
     name = "angled"
     filled = "▰"
     empty = "▱"
     head = "▰"
 
 
-class PbarStyleEmbed(PbarStyleBase):
-    name = "embed"
-    filled = "ꞏ"
-    empty = " "
-    head = ">"
-
-
 class PbarStyleRich(PbarStyleBase):
     name = "rich"
     filled = "━"
     empty = " "
     head = "━"
 
     def __init__(self, *args, **kwds):
@@ -152,14 +145,42 @@
         super().__init__(*args, **kwds)
         if not self.color and not self.color_empty:
             self.color = maybe_convert_to_colorama("red")
             self.color_empty = maybe_convert_to_colorama("black")
             self.empty = self.filled
 
 
+class PbarStyleCdots(PbarStyleBase):
+    name = "cdots"
+    filled = "ꞏ"
+    empty = " "
+    head = ">"
+
+
+class PbarStyleDash(PbarStyleBase):
+    name = "dash"
+    filled = "-"
+    empty = " "
+    head = ">"
+
+
+class PbarStyleUnder(PbarStyleBase):
+    name = "under"
+    filled = "_"
+    empty = " "
+    head = "_"
+
+
+class PbarStyleDoubleDash(PbarStyleBase):
+    name = "doubledash"
+    filled = "="
+    empty = " "
+    head = ">"
+
+
 class PbarStyleNone(PbarStyleBase):
     name = "hidden"
     filled = " "
     empty = " "
     head = " "
```

### Comparing `progress-table-2.2.2/progress_table.egg-info/PKG-INFO` & `progress-table-2.2.3/progress_table.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-table
-Version: 2.2.2
+Version: 2.2.3
 Summary: Display progress as a pretty table in the command line.
 Home-page: https://github.com/gahaalt/progress-table.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -96,20 +96,20 @@
     table.next_row()
 
 # Close the table when it's finished
 table.close()
 
 ```
 
-> Go to [integrations](https://github.com/sjmikler/progress-table/blob/main/docs/integrations.md)
+> Go to [integrations](https://github.com/sjmikler/progress-table/blob/main/docs//integrations.md)
 > page to see examples of integration with deep learning libraries.
 
 ## Advanced usage
 
-Go to [advanced usage](https://github.com/sjmikler/progress-table/blob/main/docs/advanced-usage.md) page for more information.
+Go to [advanced usage](https://github.com/sjmikler/progress-table/blob/main/docs//advanced-usage.md) page for more information.
 
 ## Troubleshooting
 
 ### Exceesive output
 
 Progress Table works correctly in most consoles, but there are some exceptions:
```

### Comparing `progress-table-2.2.2/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO` & `progress-table-2.2.3/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.2/progress_table.egg-info/SOURCES.txt` & `progress-table-2.2.3/progress_table.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `progress-table-2.2.2/setup.py` & `progress-table-2.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,16 +19,20 @@
         raise RuntimeError("Unable to find version string.")
 
 
 long_description = package_relative_path("README.md").read_text(encoding="UTF-8")
 
 
 def with_direct_github_urls(description):
-    github_link = "https://raw.githubusercontent.com/sjmikler/progress-table/main/images"
-    return description.replace("(images", "(" + github_link)
+    images_github_link = "https://raw.githubusercontent.com/sjmikler/progress-table/main/images"
+    description = description.replace("(images", "(" + images_github_link)
+
+    docs_github_link = "https://github.com/sjmikler/progress-table/blob/main/docs/"
+    description = description.replace("(docs", "(" + docs_github_link)
+    return description
 
 
 setup(
     name="progress-table",
     version=get_version(),
     url="https://github.com/gahaalt/progress-table.git",
     author="Szymon Mikler",
```

### Comparing `progress-table-2.2.2/tests/test_docs_automated.py` & `progress-table-2.2.3/tests/test_docs_automated.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 def scan_for_code_blobs(text):
     # Capture code blocks starting with py or python
     blobs = re.findall(r"```(py|python)\n([\s\S]+?)\n```", text)
 
     new_blobs = []
     for mode, blob in blobs:
         if "..." in blob:
+            # ignore blobs that are not complete
             continue
         header = get_header(f"Generated ({mode})")
         blob = header + blob
 
         # For `py` code blocks, we append them to previous existing block
         # But `python` block starts a new scope and finishes the previous block
         # They usually need to include imports
@@ -37,15 +38,15 @@
     return new_blobs
 
 
 def test_all_code_blobs():
     # Testing whether code blobs from the documentation run without errors
     all_code_blobs = []
 
-    for root, dirs, files in os.walk(""):
+    for root, dirs, files in os.walk("."):
         for file in files:
             path = pathlib.Path(os.path.join(root, file))
             if path.suffix == ".md":
                 code_blobs = scan_for_code_blobs(path.open("r").read())
                 for blob in code_blobs:
                     all_code_blobs.append(blob)
```

### Comparing `progress-table-2.2.2/tests/test_examples_automated.py` & `progress-table-2.2.3/tests/test_examples_automated.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import hashlib
 import importlib
 import sys
 from glob import glob
 from io import StringIO
 
 EXPECTED_OUTPUTS = {
-    "examples.training": "14af860a37118c16aec4604e5629e5ed",
+    "examples.training": "6993e60d3edc3cb48014480fc4890404",
     "examples.tictactoe": "378133fb7804a678282564d751068531",
     "examples.brown2d": "c0f37fdfcfc2db6ef465473c67c05d83",
 }
 
 
 def capture_example_stdout(main_fn):
     # To eliminate run to run variation of the example outputs we need to be independent from the execution speed
```

