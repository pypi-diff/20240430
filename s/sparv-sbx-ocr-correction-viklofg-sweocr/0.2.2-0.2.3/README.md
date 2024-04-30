# Comparing `tmp/sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2.tar.gz` & `tmp/sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3.tar.gz`

## Comparing `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2.tar` & `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/.bumpversion.toml
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/Makefile
--rw-r--r--   0        0        0   161468 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/pdm.lock
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/src/sbx_ocr_correction_viklofg_sweocr/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0    79065 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/tests/requirements-testing.lock
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/tests/test_ocr_suggestor.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/.gitignore
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/README.md
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/.bumpversion.toml
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/CHANGELOG.md
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/Makefile
+-rw-r--r--   0        0        0   161468 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/pdm.lock
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/src/sbx_ocr_correction_viklofg_sweocr/__init__.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/src/sbx_ocr_correction_viklofg_sweocr/annotations.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/src/sbx_ocr_correction_viklofg_sweocr/ocr_corrector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/src/sbx_ocr_correction_viklofg_sweocr/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/tests/conftest.py
+-rw-r--r--   0        0        0    79065 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/tests/requirements-testing.lock
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/tests/test_ocr_suggestor.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/README.md
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/PKG-INFO
```

### Comparing `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/.bumpversion.toml` & `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/.bumpversion.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.bumpversion]
-current_version = "0.2.2"
+current_version = "0.2.3"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 tag = true
 sign_tags = true
 tag_name = "ocr-correction-viklofg-sweocr-v{new_version}"
 tag_message = "bump version(ocr-correction-viklofg-sweocr): {current_version} → {new_version}"
 allow_dirty = false
```

### Comparing `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/CHANGELOG.md` & `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.2.3] - 2024-04-30
+
+### 🐛 Bug Fixes
+
+- Write annotations at correct index
+- Add py.typed marker
+- *(typing)* Ignore type-checking on modules
+- Missing import
+
+### 📚 Documentation
+
+- Fix description
+
 ## [0.2.2] - 2024-03-27
 
 ### 🚀 Features
 
 - Add support for python 3.8
 - Don't support 3.12
```

### Comparing `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/Makefile` & `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/pdm.lock` & `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/pdm.lock`

 * *Files identical despite different names*

### Comparing `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/tests/requirements-testing.lock` & `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/tests/requirements-testing.lock`

 * *Files identical despite different names*

### Comparing `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/tests/test_ocr_suggestor.py` & `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/tests/test_ocr_suggestor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sbx_ocr_correction_viklofg_sweocr import OcrCorrector
+from sbx_ocr_correction_viklofg_sweocr.ocr_corrector import OcrCorrector
 
 
 def test_short_text(ocr_corrector: OcrCorrector):
     text = [
         "Den",
         "i",
         "HandelstidniDgens",
```

### Comparing `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/.gitignore` & `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/README.md` & `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/pyproject.toml` & `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sparv-sbx-ocr-correction-viklofg-sweocr"
-version = "0.2.2"
+version = "0.2.3"
 description = "A sparv plugin for computing suggested OCR improvements."
 authors = [
     { name = "Kristoffer Andersson", email = "kristoffer.andersson@gu.se" },
 ]
 dependencies = ["sparv-pipeline >=5.2.0", "transformers>=4.34.1"]
 license = { text = "MIT" }
 readme = "README.md"
```

### Comparing `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.2/PKG-INFO` & `sparv_sbx_ocr_correction_viklofg_sweocr-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sparv-sbx-ocr-correction-viklofg-sweocr
-Version: 0.2.2
+Version: 0.2.3
 Summary: A sparv plugin for computing suggested OCR improvements.
 Project-URL: Homepage, https://spraakbanken.gu.se
 Project-URL: Repository, https://github.com/spraakbanken/sparv-sbx-ocr-correction
 Project-URL: Bug Tracker, https://github.com/spraakbanken/sparv-sbx-ocr-correction/labels/project%3Aocr-correction-viklofg-sweocr
 Author-email: Kristoffer Andersson <kristoffer.andersson@gu.se>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
```

