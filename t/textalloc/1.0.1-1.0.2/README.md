# Comparing `tmp/textalloc-1.0.1.tar.gz` & `tmp/textalloc-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textalloc-1.0.1.tar", last modified: Tue Apr 30 21:14:03 2024, max compression
+gzip compressed data, was "textalloc-1.0.2.tar", last modified: Tue Apr 30 21:26:26 2024, max compression
```

## Comparing `textalloc-1.0.1.tar` & `textalloc-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-30 21:14:03.794313 textalloc-1.0.1/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     1077 2023-02-14 19:18:58.000000 textalloc-1.0.1/LICENSE
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9452 2024-04-30 21:14:03.794313 textalloc-1.0.1/PKG-INFO
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     8788 2024-04-30 21:07:51.000000 textalloc-1.0.1/README.md
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      741 2024-04-30 21:13:50.000000 textalloc-1.0.1/pyproject.toml
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       38 2024-04-30 21:14:03.794313 textalloc-1.0.1/setup.cfg
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-30 21:14:03.377790 textalloc-1.0.1/src/
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-30 21:14:03.561073 textalloc-1.0.1/src/textalloc/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    14205 2024-04-30 20:51:26.000000 textalloc-1.0.1/src/textalloc/__init__.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6539 2024-02-20 19:23:50.000000 textalloc-1.0.1/src/textalloc/candidates.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9803 2024-04-30 19:38:17.000000 textalloc-1.0.1/src/textalloc/non_overlapping_boxes.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    10042 2024-02-20 19:25:04.000000 textalloc-1.0.1/src/textalloc/overlap_functions.py
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-30 21:14:03.777628 textalloc-1.0.1/src/textalloc.egg-info/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9452 2024-04-30 21:14:03.000000 textalloc-1.0.1/src/textalloc.egg-info/PKG-INFO
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      344 2024-04-30 21:14:03.000000 textalloc-1.0.1/src/textalloc.egg-info/SOURCES.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        1 2024-04-30 21:14:03.000000 textalloc-1.0.1/src/textalloc.egg-info/dependency_links.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       49 2024-04-30 21:14:03.000000 textalloc-1.0.1/src/textalloc.egg-info/requires.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       10 2024-04-30 21:14:03.000000 textalloc-1.0.1/src/textalloc.egg-info/top_level.txt
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-30 21:26:26.577473 textalloc-1.0.2/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     1077 2023-02-14 19:18:58.000000 textalloc-1.0.2/LICENSE
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9452 2024-04-30 21:26:26.573975 textalloc-1.0.2/PKG-INFO
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     8788 2024-04-30 21:07:51.000000 textalloc-1.0.2/README.md
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      741 2024-04-30 21:25:54.000000 textalloc-1.0.2/pyproject.toml
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       38 2024-04-30 21:26:26.577473 textalloc-1.0.2/setup.cfg
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-30 21:26:26.136902 textalloc-1.0.2/src/
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-30 21:26:26.401833 textalloc-1.0.2/src/textalloc/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    14201 2024-04-30 21:25:20.000000 textalloc-1.0.2/src/textalloc/__init__.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6539 2024-02-20 19:23:50.000000 textalloc-1.0.2/src/textalloc/candidates.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9795 2024-04-30 21:25:34.000000 textalloc-1.0.2/src/textalloc/non_overlapping_boxes.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    10042 2024-02-20 19:25:04.000000 textalloc-1.0.2/src/textalloc/overlap_functions.py
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-30 21:26:26.559842 textalloc-1.0.2/src/textalloc.egg-info/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9452 2024-04-30 21:26:25.000000 textalloc-1.0.2/src/textalloc.egg-info/PKG-INFO
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      344 2024-04-30 21:26:26.000000 textalloc-1.0.2/src/textalloc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        1 2024-04-30 21:26:25.000000 textalloc-1.0.2/src/textalloc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       49 2024-04-30 21:26:26.000000 textalloc-1.0.2/src/textalloc.egg-info/requires.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       10 2024-04-30 21:26:26.000000 textalloc-1.0.2/src/textalloc.egg-info/top_level.txt
```

### Comparing `textalloc-1.0.1/LICENSE` & `textalloc-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `textalloc-1.0.1/PKG-INFO` & `textalloc-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textalloc
-Version: 1.0.1
+Version: 1.0.2
 Summary: Efficient Text Allocation in matplotlib using NumPy Broadcasting
 Author-email: Christoffer Kjellson <c.kjellson@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/ckjellson/textalloc
 Project-URL: Bug Tracker, https://github.com/ckjellson/textalloc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `textalloc-1.0.1/README.md` & `textalloc-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `textalloc-1.0.1/pyproject.toml` & `textalloc-1.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "textalloc"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Christoffer Kjellson", email="c.kjellson@gmail.com" },
 ]
 license = {text = "MIT License"}
 description = "Efficient Text Allocation in matplotlib using NumPy Broadcasting"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `textalloc-1.0.1/src/textalloc/__init__.py` & `textalloc-1.0.2/src/textalloc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from matplotlib.path import get_path_collection_extents
-from src.textalloc.non_overlapping_boxes import (
+from textalloc.non_overlapping_boxes import (
     get_non_overlapping_boxes,
     find_nearest_point_on_box,
 )
 import numpy as np
 import time
 from typing import Any, Dict, List, Union
```

### Comparing `textalloc-1.0.1/src/textalloc/candidates.py` & `textalloc-1.0.2/src/textalloc/candidates.py`

 * *Files identical despite different names*

### Comparing `textalloc-1.0.1/src/textalloc/non_overlapping_boxes.py` & `textalloc-1.0.2/src/textalloc/non_overlapping_boxes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from typing import Tuple, List
-from src.textalloc.candidates import generate_candidates
-from src.textalloc.overlap_functions import (
+from textalloc.candidates import generate_candidates
+from textalloc.overlap_functions import (
     non_overlapping_with_points,
     non_overlapping_with_lines,
     non_overlapping_with_boxes,
     inside_plot,
 )
 
 try:
```

### Comparing `textalloc-1.0.1/src/textalloc/overlap_functions.py` & `textalloc-1.0.2/src/textalloc/overlap_functions.py`

 * *Files identical despite different names*

### Comparing `textalloc-1.0.1/src/textalloc.egg-info/PKG-INFO` & `textalloc-1.0.2/src/textalloc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textalloc
-Version: 1.0.1
+Version: 1.0.2
 Summary: Efficient Text Allocation in matplotlib using NumPy Broadcasting
 Author-email: Christoffer Kjellson <c.kjellson@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/ckjellson/textalloc
 Project-URL: Bug Tracker, https://github.com/ckjellson/textalloc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

