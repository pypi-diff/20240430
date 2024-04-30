# Comparing `tmp/openbharatocr-0.1.2.tar.gz` & `tmp/openbharatocr-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbharatocr-0.1.2.tar", last modified: Thu Apr 18 12:48:53 2024, max compression
+gzip compressed data, was "openbharatocr-0.2.0.tar", last modified: Tue Apr 30 08:41:52 2024, max compression
```

## Comparing `openbharatocr-0.1.2.tar` & `openbharatocr-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:48:53.242819 openbharatocr-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-18 12:48:53.242819 openbharatocr-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:48:53.238819 openbharatocr-0.1.2/openbharatocr/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/openbharatocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:48:53.242819 openbharatocr-0.1.2/openbharatocr/ocr/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/openbharatocr/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/openbharatocr/ocr/aadhaar.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/openbharatocr/ocr/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/openbharatocr/ocr/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/openbharatocr/ocr/driving_licence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/openbharatocr/ocr/pan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/openbharatocr/ocr/passport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:48:53.242819 openbharatocr-0.1.2/openbharatocr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-18 12:48:53.000000 openbharatocr-0.1.2/openbharatocr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-18 12:48:53.000000 openbharatocr-0.1.2/openbharatocr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:48:53.000000 openbharatocr-0.1.2/openbharatocr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:48:53.000000 openbharatocr-0.1.2/openbharatocr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 12:48:53.000000 openbharatocr-0.1.2/openbharatocr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 12:48:53.000000 openbharatocr-0.1.2/openbharatocr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-18 12:48:53.242819 openbharatocr-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-18 12:48:48.000000 openbharatocr-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:41:52.658633 openbharatocr-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-30 08:41:52.658633 openbharatocr-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:41:52.658633 openbharatocr-0.2.0/openbharatocr/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/openbharatocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:41:52.658633 openbharatocr-0.2.0/openbharatocr/ocr/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/openbharatocr/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/openbharatocr/ocr/aadhaar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/openbharatocr/ocr/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/openbharatocr/ocr/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/openbharatocr/ocr/driving_licence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/openbharatocr/ocr/pan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/openbharatocr/ocr/passport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/openbharatocr/ocr/voter_id.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:41:52.658633 openbharatocr-0.2.0/openbharatocr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-30 08:41:52.000000 openbharatocr-0.2.0/openbharatocr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-30 08:41:52.000000 openbharatocr-0.2.0/openbharatocr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:41:52.000000 openbharatocr-0.2.0/openbharatocr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:41:52.000000 openbharatocr-0.2.0/openbharatocr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 08:41:52.000000 openbharatocr-0.2.0/openbharatocr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 08:41:52.000000 openbharatocr-0.2.0/openbharatocr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-30 08:41:52.658633 openbharatocr-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-30 08:41:47.000000 openbharatocr-0.2.0/setup.py
```

### Comparing `openbharatocr-0.1.2/LICENSE` & `openbharatocr-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.1.2/PKG-INFO` & `openbharatocr-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbharatocr
-Version: 0.1.2
+Version: 0.2.0
 Summary: openbharatocr is an opensource python library for ocr Indian government documents 
 Home-page: https://github.com/essentiasoftserv/openbharatocr
 Author: essentiasoftserv
 Author-email: kunal@essentia.dev
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -63,14 +63,32 @@
 This function takes the path of a Passport image as input and returns its information in the form of a dictionary.
 
 ```
     import openbharatocr 
     dict_output = openbharatocr.passport(image_path)
 ```
 
+**VoterID**
+
+The two functions accepts the file paths of the front and back images of a voterID as input and returns their corresponding information encapsulated in a dictionary.
+
+```
+    import openbharatocr 
+    # Download YOLOv3 models from links(added below) and set the path of YOLO_CFG, YOLO_WEIGHT
+    dict_output = openbharatocr.voter_id_front(image_path)
+    dict_output = openbharatocr.voter_id_back(image_path)
+```
+
+
+### Download Resources
+Some Resources need to download and set the path in the variables.
+- YOLO_CFG = https://drive.google.com/file/d/1SEst2lVoFDOgUVLZ5kje9GTb2tHRA8U-/view?usp=sharing
+- YOLO_WEIGHT = https://drive.google.com/file/d/1cGGstycfogmO6O7ToB2DAEXOgTWVgINh/view?usp=drive_link
+
+
 ### Contribute & support
 We are so pleased to your help and help you. If you wanna develop openbharatocr, Congrats! If you have problem, don't worry, create an issue here:
 
 ```
     https://github.com/essentiasoftserv/openbharatocr/issues
 ```
```

### Comparing `openbharatocr-0.1.2/README.md` & `openbharatocr-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -49,14 +49,32 @@
 This function takes the path of a Passport image as input and returns its information in the form of a dictionary.
 
 ```
     import openbharatocr 
     dict_output = openbharatocr.passport(image_path)
 ```
 
+**VoterID**
+
+The two functions accepts the file paths of the front and back images of a voterID as input and returns their corresponding information encapsulated in a dictionary.
+
+```
+    import openbharatocr 
+    # Download YOLOv3 models from links(added below) and set the path of YOLO_CFG, YOLO_WEIGHT
+    dict_output = openbharatocr.voter_id_front(image_path)
+    dict_output = openbharatocr.voter_id_back(image_path)
+```
+
+
+### Download Resources
+Some Resources need to download and set the path in the variables.
+- YOLO_CFG = https://drive.google.com/file/d/1SEst2lVoFDOgUVLZ5kje9GTb2tHRA8U-/view?usp=sharing
+- YOLO_WEIGHT = https://drive.google.com/file/d/1cGGstycfogmO6O7ToB2DAEXOgTWVgINh/view?usp=drive_link
+
+
 ### Contribute & support
 We are so pleased to your help and help you. If you wanna develop openbharatocr, Congrats! If you have problem, don't worry, create an issue here:
 
 ```
     https://github.com/essentiasoftserv/openbharatocr/issues
 ```
```

### Comparing `openbharatocr-0.1.2/openbharatocr/ocr/aadhaar.py` & `openbharatocr-0.2.0/openbharatocr/ocr/aadhaar.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             break
 
     return full_name
 
 
 def extract_fathers_name(input):
 
-    regex = r"(?:S/O|D/O)[:\s]*([A-Za-z]+(?: [A-Za-z]+)*)"
+    regex = r"(?:S.?O|D.?O)[:\s]*([A-Za-z]+(?: [A-Za-z]+)*)"
     match = re.findall(regex, input)
     fathers_name = ""
     if match:
         fathers_name = match[-1]
 
     return fathers_name
 
@@ -62,66 +62,31 @@
     if re.search("Female", input) or re.search("FEMALE", input):
         return "Female"
     if re.search("Male", input) or re.search("MALE", input):
         return "Male"
     return "Other"
 
 
-def extract_address(image_path):
+def extract_address(input):
 
-    image = Image.open(image_path)
-    text = pytesseract.image_to_string(image)
-
-    if "Address" not in text:
-        return ""
-    rgb = image.convert("RGB")
-    with tempfile.TemporaryDirectory() as tempdir:
-        tempfile_path = f"{tempdir}/{str(uuid.uuid4())}.jpg"
-        rgb.save(tempfile_path)
-        image = cv2.imread(tempfile_path)
-
-        gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
-
-        config = r"--oem 3 --psm 6"
-        boxes_data = pytesseract.image_to_data(gray_image, config=config)
-
-        boxes = boxes_data.splitlines()
-        boxes = [b.split() for b in boxes]
-
-        left, top = 0, 0
-        for box in boxes[1:]:
-            if len(box) == 12:
-                if "Address" in box[11]:
-                    left = int(box[6])
-                    top = int(box[7])
-
-        h, w = gray_image.shape
-
-        if left < int(0.4 * w):
-            h = int(0.9 * h)
-            w = int(0.6 * w)
-
-        roi = gray_image[top:h, left:w]
-        address = pytesseract.image_to_string(roi, config=config)
-
-        split_add = address.split(" ")
-        split_add.remove(split_add[0])
+    regex = r"Address:\s*((?:.|\n)*?\d{6})"
+    match = re.search(regex, input)
+    address = match.group(1) if match else ""
 
-        address = " ".join(split_add)
-        return address
+    return address
 
 
 def extract_back_aadhaar_details(image_path):
 
     image = Image.open(image_path)
 
     extracted_text = pytesseract.image_to_string(image)
 
     fathers_name = extract_fathers_name(extracted_text)
-    address = extract_address(image_path)
+    address = extract_address(extracted_text)
 
     return {
         "Father's Name": fathers_name,
         "Address": address,
     }
```

### Comparing `openbharatocr-0.1.2/openbharatocr/ocr/driving_licence.py` & `openbharatocr-0.2.0/openbharatocr/ocr/driving_licence.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.1.2/openbharatocr/ocr/pan.py` & `openbharatocr-0.2.0/openbharatocr/ocr/pan.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.1.2/openbharatocr/ocr/passport.py` & `openbharatocr-0.2.0/openbharatocr/ocr/passport.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.1.2/openbharatocr.egg-info/PKG-INFO` & `openbharatocr-0.2.0/openbharatocr.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbharatocr
-Version: 0.1.2
+Version: 0.2.0
 Summary: openbharatocr is an opensource python library for ocr Indian government documents 
 Home-page: https://github.com/essentiasoftserv/openbharatocr
 Author: essentiasoftserv
 Author-email: kunal@essentia.dev
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -63,14 +63,32 @@
 This function takes the path of a Passport image as input and returns its information in the form of a dictionary.
 
 ```
     import openbharatocr 
     dict_output = openbharatocr.passport(image_path)
 ```
 
+**VoterID**
+
+The two functions accepts the file paths of the front and back images of a voterID as input and returns their corresponding information encapsulated in a dictionary.
+
+```
+    import openbharatocr 
+    # Download YOLOv3 models from links(added below) and set the path of YOLO_CFG, YOLO_WEIGHT
+    dict_output = openbharatocr.voter_id_front(image_path)
+    dict_output = openbharatocr.voter_id_back(image_path)
+```
+
+
+### Download Resources
+Some Resources need to download and set the path in the variables.
+- YOLO_CFG = https://drive.google.com/file/d/1SEst2lVoFDOgUVLZ5kje9GTb2tHRA8U-/view?usp=sharing
+- YOLO_WEIGHT = https://drive.google.com/file/d/1cGGstycfogmO6O7ToB2DAEXOgTWVgINh/view?usp=drive_link
+
+
 ### Contribute & support
 We are so pleased to your help and help you. If you wanna develop openbharatocr, Congrats! If you have problem, don't worry, create an issue here:
 
 ```
     https://github.com/essentiasoftserv/openbharatocr/issues
 ```
```

### Comparing `openbharatocr-0.1.2/openbharatocr.egg-info/SOURCES.txt` & `openbharatocr-0.2.0/openbharatocr.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 openbharatocr.egg-info/top_level.txt
 openbharatocr/ocr/__init__.py
 openbharatocr/ocr/aadhaar.py
 openbharatocr/ocr/api.py
 openbharatocr/ocr/common.py
 openbharatocr/ocr/driving_licence.py
 openbharatocr/ocr/pan.py
-openbharatocr/ocr/passport.py
+openbharatocr/ocr/passport.py
+openbharatocr/ocr/voter_id.py
```

### Comparing `openbharatocr-0.1.2/setup.py` & `openbharatocr-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fp:
     install_requires = fp.read()
 
 setuptools.setup(
     name="openbharatocr",
-    version="0.1.2",
+    version="0.2.0",
     description="openbharatocr is an opensource python library for ocr Indian government documents ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/essentiasoftserv/openbharatocr",
     author="essentiasoftserv",
     python_requires=">=3.6",
     install_requires=install_requires,
```

