# Comparing `tmp/textboard-0.1.0.tar.gz` & `tmp/textboard-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textboard-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "textboard-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `textboard-0.1.0.tar` & `textboard-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      117 2024-04-30 16:59:41.616421 textboard-0.1.0/.gitignore
--rw-r--r--   0        0        0     3414 2024-04-30 17:27:48.706129 textboard-0.1.0/README.md
--rw-r--r--   0        0        0      302 2024-04-30 17:37:57.026052 textboard-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4736 2024-04-30 17:36:29.254015 textboard-0.1.0/textboard/__init__.py
--rw-r--r--   0        0        0     1343 2024-04-30 17:34:51.201988 textboard-0.1.0/textboard/__main__.py
--rw-r--r--   0        0        0      204 1970-01-01 00:00:00.000000 textboard-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      117 2024-04-30 16:59:41.616421 textboard-0.1.1/.gitignore
+-rw-r--r--   0        0        0      475 2024-04-30 17:44:30.358319 textboard-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0     3414 2024-04-30 17:27:48.706129 textboard-0.1.1/README.md
+-rw-r--r--   0        0        0      302 2024-04-30 17:37:57.026052 textboard-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4683 2024-04-30 17:52:00.498741 textboard-0.1.1/textboard/__init__.py
+-rw-r--r--   0        0        0     1343 2024-04-30 17:34:51.201988 textboard-0.1.1/textboard/__main__.py
+-rw-r--r--   0        0        0      204 1970-01-01 00:00:00.000000 textboard-0.1.1/PKG-INFO
```

### Comparing `textboard-0.1.0/README.md` & `textboard-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `textboard-0.1.0/textboard/__init__.py` & `textboard-0.1.1/textboard/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A thing to make text-based training loggers"""
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 import os
 import re
 import scipy
 
 
 def get_terminal_width():
@@ -24,15 +24,15 @@
 def resample(values, length):
     return scipy.signal.resample(values, length)
 
 
 boxes = "▁▂▃▄▅▆▇█"
 
 
-def sparklines(values, num_lines: int = 2) -> list[str]:
+def sparklines(values, num_lines=2):
     # shift values to be positive
     mn = min(values)
     values = [v - mn for v in values]
     mx = max(values)
     mn = 0
     segment_per_box = (mx - mn) / (num_lines * len(boxes))
     lines = []
@@ -47,25 +47,25 @@
                 # clamp to top box if we're just providing something for a higher box to sit on
                 box_index = min(len(boxes) - 1, box_index)
                 line += boxes[box_index]
         lines.append(line)
     return lines
 
 
-def plot(values, height: int = 4, title=None, length=None) -> list[str]:
+def plot(values, height=4, title=None, length=None):
     length = target_length(length)
     if length < len(values):
         values = resample(values, length)
     lines = sparklines(values, num_lines=height)
     if title:
         return text(title, bold=True, length=length) + lines
     return lines
 
 
-def hist1d(values, height, labels=None, title=None, length=None) -> list[str]:
+def hist1d(values, height, labels=None, title=None, length=None):
     length = target_length(length)
     lines = sparklines(values, num_lines=height)
     if title:
         lines = text(title, bold=True) + lines
     if labels:
         lines.append("".join(labels))
     return lines
```

### Comparing `textboard-0.1.0/textboard/__main__.py` & `textboard-0.1.1/textboard/__main__.py`

 * *Files identical despite different names*

