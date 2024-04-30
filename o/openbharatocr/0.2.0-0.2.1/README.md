# Comparing `tmp/openbharatocr-0.2.0.tar.gz` & `tmp/openbharatocr-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbharatocr-0.2.0.tar", last modified: Tue Apr 30 08:41:52 2024, max compression
+gzip compressed data, was "openbharatocr-0.2.1.tar", last modified: Tue Apr 30 09:06:41 2024, max compression
```

## Comparing `openbharatocr-0.2.0.tar` & `openbharatocr-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:41:52.658633 openbharatocr-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-30 08:41:52.658633 openbharatocr-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:41:52.658633 openbharatocr-0.2.0/openbharatocr/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/openbharatocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:41:52.658633 openbharatocr-0.2.0/openbharatocr/ocr/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/openbharatocr/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/openbharatocr/ocr/aadhaar.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/openbharatocr/ocr/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/openbharatocr/ocr/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/openbharatocr/ocr/driving_licence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/openbharatocr/ocr/pan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/openbharatocr/ocr/passport.py
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/openbharatocr/ocr/voter_id.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:41:52.658633 openbharatocr-0.2.0/openbharatocr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-30 08:41:52.000000 openbharatocr-0.2.0/openbharatocr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-30 08:41:52.000000 openbharatocr-0.2.0/openbharatocr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:41:52.000000 openbharatocr-0.2.0/openbharatocr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:41:52.000000 openbharatocr-0.2.0/openbharatocr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 08:41:52.000000 openbharatocr-0.2.0/openbharatocr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 08:41:52.000000 openbharatocr-0.2.0/openbharatocr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-30 08:41:52.658633 openbharatocr-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:41.710052 openbharatocr-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-30 09:06:41.710052 openbharatocr-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:41.706052 openbharatocr-0.2.1/openbharatocr/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/openbharatocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:41.710052 openbharatocr-0.2.1/openbharatocr/ocr/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/openbharatocr/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/openbharatocr/ocr/aadhaar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/openbharatocr/ocr/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/openbharatocr/ocr/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/openbharatocr/ocr/driving_licence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/openbharatocr/ocr/pan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/openbharatocr/ocr/passport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/openbharatocr/ocr/voter_id.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:41.710052 openbharatocr-0.2.1/openbharatocr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-30 09:06:41.000000 openbharatocr-0.2.1/openbharatocr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-30 09:06:41.000000 openbharatocr-0.2.1/openbharatocr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:06:41.000000 openbharatocr-0.2.1/openbharatocr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:06:41.000000 openbharatocr-0.2.1/openbharatocr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 09:06:41.000000 openbharatocr-0.2.1/openbharatocr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 09:06:41.000000 openbharatocr-0.2.1/openbharatocr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-30 09:06:41.710052 openbharatocr-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/setup.py
```

### Comparing `openbharatocr-0.2.0/LICENSE` & `openbharatocr-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.2.0/PKG-INFO` & `openbharatocr-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbharatocr
-Version: 0.2.0
+Version: 0.2.1
 Summary: openbharatocr is an opensource python library for ocr Indian government documents 
 Home-page: https://github.com/essentiasoftserv/openbharatocr
 Author: essentiasoftserv
 Author-email: kunal@essentia.dev
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -69,15 +69,15 @@
 
 **VoterID**
 
 The two functions accepts the file paths of the front and back images of a voterID as input and returns their corresponding information encapsulated in a dictionary.
 
 ```
     import openbharatocr 
-    # Download YOLOv3 models from links(added below) and set the path of YOLO_CFG, YOLO_WEIGHT
+    # Download YOLOv3 models from links(added below) and set local downloaded path to YOLO_CFG, YOLO_WEIGHT env variables
     dict_output = openbharatocr.voter_id_front(image_path)
     dict_output = openbharatocr.voter_id_back(image_path)
 ```
 
 
 ### Download Resources
 Some Resources need to download and set the path in the variables.
```

### Comparing `openbharatocr-0.2.0/README.md` & `openbharatocr-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 **VoterID**
 
 The two functions accepts the file paths of the front and back images of a voterID as input and returns their corresponding information encapsulated in a dictionary.
 
 ```
     import openbharatocr 
-    # Download YOLOv3 models from links(added below) and set the path of YOLO_CFG, YOLO_WEIGHT
+    # Download YOLOv3 models from links(added below) and set local downloaded path to YOLO_CFG, YOLO_WEIGHT env variables
     dict_output = openbharatocr.voter_id_front(image_path)
     dict_output = openbharatocr.voter_id_back(image_path)
 ```
 
 
 ### Download Resources
 Some Resources need to download and set the path in the variables.
```

### Comparing `openbharatocr-0.2.0/openbharatocr/ocr/aadhaar.py` & `openbharatocr-0.2.1/openbharatocr/ocr/aadhaar.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.2.0/openbharatocr/ocr/driving_licence.py` & `openbharatocr-0.2.1/openbharatocr/ocr/driving_licence.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.2.0/openbharatocr/ocr/pan.py` & `openbharatocr-0.2.1/openbharatocr/ocr/pan.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.2.0/openbharatocr/ocr/passport.py` & `openbharatocr-0.2.1/openbharatocr/ocr/passport.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.2.0/openbharatocr/ocr/voter_id.py` & `openbharatocr-0.2.1/openbharatocr/ocr/voter_id.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import re
 import cv2
 import pytesseract
 from PIL import Image
 import numpy as np
+import os
 
-# Download the models from links and set the path
-YOLO_CFG = "yolov3_custom.cfg"  # https://drive.google.com/file/d/1SEst2lVoFDOgUVLZ5kje9GTb2tHRA8U-/view?usp=sharing
-YOLO_WEIGHT = "yolov3_custom_6000.weights"  # https://drive.google.com/file/d/1cGGstycfogmO6O7ToB2DAEXOgTWVgINh/view?usp=drive_link
+# Download the models from links and set in the environment
+YOLO_CFG = os.environ.get(
+    "YOLO_CFG", "yolov3_custom.cfg"
+)  # https://drive.google.com/file/d/1SEst2lVoFDOgUVLZ5kje9GTb2tHRA8U-/view?usp=sharing
+YOLO_WEIGHT = os.environ.get(
+    "YOLO_WEIGHT", "yolov3_custom_6000.weights"
+)  # https://drive.google.com/file/d/1cGGstycfogmO6O7ToB2DAEXOgTWVgINh/view?usp=drive_link
 
 
 def preprocess_for_bold_text(image):
 
     gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
 
     kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (1, 1))
```

### Comparing `openbharatocr-0.2.0/openbharatocr.egg-info/PKG-INFO` & `openbharatocr-0.2.1/openbharatocr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbharatocr
-Version: 0.2.0
+Version: 0.2.1
 Summary: openbharatocr is an opensource python library for ocr Indian government documents 
 Home-page: https://github.com/essentiasoftserv/openbharatocr
 Author: essentiasoftserv
 Author-email: kunal@essentia.dev
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -69,15 +69,15 @@
 
 **VoterID**
 
 The two functions accepts the file paths of the front and back images of a voterID as input and returns their corresponding information encapsulated in a dictionary.
 
 ```
     import openbharatocr 
-    # Download YOLOv3 models from links(added below) and set the path of YOLO_CFG, YOLO_WEIGHT
+    # Download YOLOv3 models from links(added below) and set local downloaded path to YOLO_CFG, YOLO_WEIGHT env variables
     dict_output = openbharatocr.voter_id_front(image_path)
     dict_output = openbharatocr.voter_id_back(image_path)
 ```
 
 
 ### Download Resources
 Some Resources need to download and set the path in the variables.
```

### Comparing `openbharatocr-0.2.0/openbharatocr.egg-info/SOURCES.txt` & `openbharatocr-0.2.1/openbharatocr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.2.0/setup.py` & `openbharatocr-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fp:
     install_requires = fp.read()
 
 setuptools.setup(
     name="openbharatocr",
-    version="0.2.0",
+    version="0.2.1",
     description="openbharatocr is an opensource python library for ocr Indian government documents ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/essentiasoftserv/openbharatocr",
     author="essentiasoftserv",
     python_requires=">=3.6",
     install_requires=install_requires,
```

