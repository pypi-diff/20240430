# Comparing `tmp/receipt_enhancer-0.1.5.tar.gz` & `tmp/receipt_enhancer-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "receipt_enhancer-0.1.5.tar", max compression
+gzip compressed data, was "receipt_enhancer-0.1.6.tar", max compression
```

## Comparing `receipt_enhancer-0.1.5.tar` & `receipt_enhancer-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1071 2024-04-26 23:46:02.339918 receipt_enhancer-0.1.5/LICENSE
--rw-r--r--   0        0        0     2381 2024-04-26 23:46:02.339918 receipt_enhancer-0.1.5/README.md
--rw-r--r--   0        0        0      500 2024-04-26 23:55:19.491916 receipt_enhancer-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       93 2024-04-26 23:46:02.339918 receipt_enhancer-0.1.5/receipt_enhancer/__init__.py
--rw-r--r--   0        0        0    15114 2024-04-26 23:53:11.519916 receipt_enhancer-0.1.5/receipt_enhancer/receipt_enhancer.py
--rw-r--r--   0        0        0     3188 1970-01-01 00:00:00.000000 receipt_enhancer-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-26 23:46:02.339918 receipt_enhancer-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2381 2024-04-26 23:46:02.339918 receipt_enhancer-0.1.6/README.md
+-rw-r--r--   0        0        0      500 2024-04-30 01:54:15.631988 receipt_enhancer-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       93 2024-04-26 23:46:02.339918 receipt_enhancer-0.1.6/receipt_enhancer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 05:57:30.307992 receipt_enhancer-0.1.6/receipt_enhancer/asdf.py
+-rw-r--r--   0        0        0    15122 2024-04-30 01:53:20.147988 receipt_enhancer-0.1.6/receipt_enhancer/receipt_enhancer.py
+-rw-r--r--   0        0        0     3188 1970-01-01 00:00:00.000000 receipt_enhancer-0.1.6/PKG-INFO
```

### Comparing `receipt_enhancer-0.1.5/LICENSE` & `receipt_enhancer-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `receipt_enhancer-0.1.5/README.md` & `receipt_enhancer-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `receipt_enhancer-0.1.5/receipt_enhancer/receipt_enhancer.py` & `receipt_enhancer-0.1.6/receipt_enhancer/receipt_enhancer.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         if np.count_nonzero(binary) == 0:
             return []
 
         resolution = min(image.shape[0], image.shape[1])
         mean_intensity = np.mean(image)
         canny_lower_threshold = int(max(0, mean_intensity * 0.5))
         canny_upper_threshold = int(min(255, mean_intensity * 1.5))
-        aperture_size = max(3, int(resolution / 500))
+        aperture_size = min(max(3, int(resolution / 500)), 7)
 
         edges = cv2.Canny(binary, canny_lower_threshold, canny_upper_threshold, apertureSize=aperture_size)
 
         roi_size_fraction = self.calculate_roi_size_fraction(image)
         roi_size = min(image.shape[0], image.shape[1]) * roi_size_fraction
         intersection_distance_threshold = roi_size * 0.01
```

### Comparing `receipt_enhancer-0.1.5/PKG-INFO` & `receipt_enhancer-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: receipt-enhancer
-Version: 0.1.5
+Version: 0.1.6
 Summary: This module is essential for preprocessing receipt images to improve visual quality and facilitate automatic analysis.
 License: MIT
 Keywords: document,nfe,invoice,receipt
 Author: Ricardo Castro
 Author-email: srrenks@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

