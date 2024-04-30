# Comparing `tmp/raw-image-converter-1.1.2.tar.gz` & `tmp/raw_image_converter-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raw-image-converter-1.1.2.tar", last modified: Wed Apr  3 20:55:53 2024, max compression
+gzip compressed data, was "raw_image_converter-1.1.3.tar", max compression
```

## Comparing `raw-image-converter-1.1.2.tar` & `raw_image_converter-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,7 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:55:53.238681 raw-image-converter-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-03 20:55:53.238681 raw-image-converter-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:55:53.234681 raw-image-converter-1.1.2/raw_image_converter/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/raw_image_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/raw_image_converter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/raw_image_converter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:55:53.234681 raw-image-converter-1.1.2/raw_image_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-03 20:55:53.000000 raw-image-converter-1.1.2/raw_image_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-03 20:55:53.000000 raw-image-converter-1.1.2/raw_image_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:55:53.000000 raw-image-converter-1.1.2/raw_image_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 20:55:53.000000 raw-image-converter-1.1.2/raw_image_converter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-03 20:55:53.000000 raw-image-converter-1.1.2/raw_image_converter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 20:55:53.000000 raw-image-converter-1.1.2/raw_image_converter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:55:53.238681 raw-image-converter-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:55:53.234681 raw-image-converter-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/tests/test_utils_calculate_image_dimension.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/tests/test_utils_check_file_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/tests/test_utils_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/tests/test_utils_split_file_extension.py
+-rw-r--r--   0        0        0     1074 2024-04-30 21:44:21.700794 raw_image_converter-1.1.3/LICENSE
+-rw-r--r--   0        0        0     5627 2024-04-30 21:44:21.700794 raw_image_converter-1.1.3/README.md
+-rw-r--r--   0        0        0      910 2024-04-30 21:44:21.700794 raw_image_converter-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      199 2024-04-30 21:44:21.700794 raw_image_converter-1.1.3/raw_image_converter/__init__.py
+-rw-r--r--   0        0        0     3715 2024-04-30 21:44:21.700794 raw_image_converter-1.1.3/raw_image_converter/__main__.py
+-rw-r--r--   0        0        0     4044 2024-04-30 21:44:21.700794 raw_image_converter-1.1.3/raw_image_converter/utils.py
+-rw-r--r--   0        0        0     6547 1970-01-01 00:00:00.000000 raw_image_converter-1.1.3/PKG-INFO
```

### Comparing `raw-image-converter-1.1.2/LICENSE` & `raw_image_converter-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `raw-image-converter-1.1.2/PKG-INFO` & `raw_image_converter-1.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: raw-image-converter
-Version: 1.1.2
-Summary: Batch conversions of raw images
-Home-page: https://github.com/achimoraites/Python-Image-Converter
-Author: Achilles Moraites
-Author-email: achimoraites@yahoo.gr
-License: MIT
-Keywords: cli,converter,raw,images
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy==1.26.4
-Requires-Dist: rawpy==0.19.1
-Requires-Dist: imageio==2.16.2
-Requires-Dist: Pillow==10.3.0
-Requires-Dist: colorama==0.4.6
-
 # Python Image Converter
 [![PyPI version](https://badge.fury.io/py/raw-image-converter.svg)](https://pypi.org/project/raw-image-converter/)
 [![All Contributors](https://img.shields.io/github/all-contributors/achimoraites/Python-Image-Converter?color=ee8449&style=flat-square)](#contributors)
 
 The Python Image Converter is a user-friendly CLI tool designed for hassle-free batch conversion of image files.
 
 Once upon a time, converting multiple images came with either slow, tedious processes or even paid tools. 
@@ -45,15 +24,16 @@
 
 ### Running it from the repo 
 
 ```bash
  git clone https://github.com/achimoraites/Python-Image-Converter.git [my-app-name]
  cd [my-app-name]
 
- pip install -r requirements.txt
+poetry install
+poetry shell
 
  python -m raw_image_converter --s <Enter-Path-Of-Directory>
 ```
 ## Example usage
 
 ### Arguments
 - `-s, --src` (required): set the path to the directory you want to convert (source)!
```

#### html2text {}

```diff
@@ -1,17 +1,8 @@
-Metadata-Version: 2.1 Name: raw-image-converter Version: 1.1.2 Summary: Batch
-conversions of raw images Home-page: https://github.com/achimoraites/Python-
-Image-Converter Author: Achilles Moraites Author-email: achimoraites@yahoo.gr
-License: MIT Keywords: cli,converter,raw,images Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Topic ::
-Utilities Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: numpy==1.26.4 Requires-Dist: rawpy==0.19.1 Requires-Dist:
-imageio==2.16.2 Requires-Dist: Pillow==10.3.0 Requires-Dist: colorama==0.4.6 #
-Python Image Converter [![PyPI version](https://badge.fury.io/py/raw-image-
+# Python Image Converter [![PyPI version](https://badge.fury.io/py/raw-image-
 converter.svg)](https://pypi.org/project/raw-image-converter/) [![All
 Contributors](https://img.shields.io/github/all-contributors/achimoraites/
 Python-Image-Converter?color=ee8449&style=flat-square)](#contributors) The
 Python Image Converter is a user-friendly CLI tool designed for hassle-free
 batch conversion of image files. Once upon a time, converting multiple images
 came with either slow, tedious processes or even paid tools. Not anymore! This
 open-source image converter can empower anyone, from busy image professionals
@@ -19,17 +10,17 @@
 Say goodbye to the tedious one-by-one image conversion. Convert hundreds of
 images at once. - **Supported File Types:** DNG, CR2, CRW, NEF, PEF, ERF, ORF,
 PPM, MOS, MRF, MRW, SRW, PSD, TIF, and more. - **Fast:** Multi-core support. -
 **Customizable Output:** Specify your converted images' output directory,
 resolution, and format ## Install ### Using pip (recommended) ```bash $ pip3
 install raw_image_converter ``` ### Running it from the repo ```bash git clone
 https://github.com/achimoraites/Python-Image-Converter.git [my-app-name] cd
-[my-app-name] pip install -r requirements.txt python -m raw_image_converter --
-s ``` ## Example usage ### Arguments - `-s, --src` (required): set the path to
-the directory you want to convert (source)! - `-t, --tgt`: where to store the
+[my-app-name] poetry install poetry shell python -m raw_image_converter --s ```
+## Example usage ### Arguments - `-s, --src` (required): set the path to the
+directory you want to convert (source)! - `-t, --tgt`: where to store the
 converted images (target); by default, they are stored in the "converted"
 folder. - `-d, --delete-source-directory`: removes the directory with the
 original images (source). - `-r, --resolution`: allows to set the converted
 image resolutions; you can use numbers or percentages: e.g., 75% -> width and
 height are 75% of the original size, 1000,1500 -> width to 1000px and the
 height to 1500px - `-e, --ext`: specify the output image format for the
 converted images; by default, it is JPG. Valid options are: - `.jpg` - `.png`
```

### Comparing `raw-image-converter-1.1.2/README.md` & `raw_image_converter-1.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: raw-image-converter
+Version: 1.1.3
+Summary: Batch image convertions
+Home-page: https://github.com/achimoraites/Python-Image-Converter
+License: MIT
+Keywords: cli,converter,raw,images
+Author: Achilles Moraites
+Author-email: achimoraites@yahoo.gr
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Utilities
+Requires-Dist: colorama (==0.4.6)
+Requires-Dist: imageio (==2.16.2)
+Requires-Dist: numpy (==1.26.4)
+Requires-Dist: pillow (==10.3.0)
+Requires-Dist: rawpy (==0.19.1)
+Project-URL: Repository, https://github.com/achimoraites/Python-Image-Converter
+Description-Content-Type: text/markdown
+
 # Python Image Converter
 [![PyPI version](https://badge.fury.io/py/raw-image-converter.svg)](https://pypi.org/project/raw-image-converter/)
 [![All Contributors](https://img.shields.io/github/all-contributors/achimoraites/Python-Image-Converter?color=ee8449&style=flat-square)](#contributors)
 
 The Python Image Converter is a user-friendly CLI tool designed for hassle-free batch conversion of image files.
 
 Once upon a time, converting multiple images came with either slow, tedious processes or even paid tools. 
@@ -24,15 +49,16 @@
 
 ### Running it from the repo 
 
 ```bash
  git clone https://github.com/achimoraites/Python-Image-Converter.git [my-app-name]
  cd [my-app-name]
 
- pip install -r requirements.txt
+poetry install
+poetry shell
 
  python -m raw_image_converter --s <Enter-Path-Of-Directory>
 ```
 ## Example usage
 
 ### Arguments
 - `-s, --src` (required): set the path to the directory you want to convert (source)! 
@@ -86,7 +112,8 @@
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
+
```

#### html2text {}

```diff
@@ -1,26 +1,38 @@
-# Python Image Converter [![PyPI version](https://badge.fury.io/py/raw-image-
-converter.svg)](https://pypi.org/project/raw-image-converter/) [![All
+Metadata-Version: 2.1 Name: raw-image-converter Version: 1.1.3 Summary: Batch
+image convertions Home-page: https://github.com/achimoraites/Python-Image-
+Converter License: MIT Keywords: cli,converter,raw,images Author: Achilles
+Moraites Author-email: achimoraites@yahoo.gr Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Utilities Requires-Dist: colorama (==0.4.6) Requires-Dist:
+imageio (==2.16.2) Requires-Dist: numpy (==1.26.4) Requires-Dist: pillow
+(==10.3.0) Requires-Dist: rawpy (==0.19.1) Project-URL: Repository, https://
+github.com/achimoraites/Python-Image-Converter Description-Content-Type: text/
+markdown # Python Image Converter [![PyPI version](https://badge.fury.io/py/
+raw-image-converter.svg)](https://pypi.org/project/raw-image-converter/) [![All
 Contributors](https://img.shields.io/github/all-contributors/achimoraites/
 Python-Image-Converter?color=ee8449&style=flat-square)](#contributors) The
 Python Image Converter is a user-friendly CLI tool designed for hassle-free
 batch conversion of image files. Once upon a time, converting multiple images
 came with either slow, tedious processes or even paid tools. Not anymore! This
 open-source image converter can empower anyone, from busy image professionals
 to individuals passionate about photography. ## Features - **Bulk Conversion:**
 Say goodbye to the tedious one-by-one image conversion. Convert hundreds of
 images at once. - **Supported File Types:** DNG, CR2, CRW, NEF, PEF, ERF, ORF,
 PPM, MOS, MRF, MRW, SRW, PSD, TIF, and more. - **Fast:** Multi-core support. -
 **Customizable Output:** Specify your converted images' output directory,
 resolution, and format ## Install ### Using pip (recommended) ```bash $ pip3
 install raw_image_converter ``` ### Running it from the repo ```bash git clone
 https://github.com/achimoraites/Python-Image-Converter.git [my-app-name] cd
-[my-app-name] pip install -r requirements.txt python -m raw_image_converter --
-s ``` ## Example usage ### Arguments - `-s, --src` (required): set the path to
-the directory you want to convert (source)! - `-t, --tgt`: where to store the
+[my-app-name] poetry install poetry shell python -m raw_image_converter --s ```
+## Example usage ### Arguments - `-s, --src` (required): set the path to the
+directory you want to convert (source)! - `-t, --tgt`: where to store the
 converted images (target); by default, they are stored in the "converted"
 folder. - `-d, --delete-source-directory`: removes the directory with the
 original images (source). - `-r, --resolution`: allows to set the converted
 image resolutions; you can use numbers or percentages: e.g., 75% -> width and
 height are 75% of the original size, 1000,1500 -> width to 1000px and the
 height to 1500px - `-e, --ext`: specify the output image format for the
 converted images; by default, it is JPG. Valid options are: - `.jpg` - `.png`
```

### Comparing `raw-image-converter-1.1.2/raw_image_converter/__main__.py` & `raw_image_converter-1.1.3/raw_image_converter/__main__.py`

 * *Files identical despite different names*

### Comparing `raw-image-converter-1.1.2/raw_image_converter/utils.py` & `raw_image_converter-1.1.3/raw_image_converter/utils.py`

 * *Files identical despite different names*

