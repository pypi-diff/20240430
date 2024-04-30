# Comparing `tmp/pytest_embedded_wokwi-1.9.0.tar.gz` & `tmp/pytest_embedded_wokwi-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded_wokwi-1.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded_wokwi-1.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded_wokwi-1.9.0.tar` & `pytest_embedded_wokwi-1.9.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1094 2024-04-25 11:36:08.627318 pytest_embedded_wokwi-1.9.0/LICENSE
--rw-r--r--   0        0        0     1911 2024-04-25 11:36:08.631318 pytest_embedded_wokwi-1.9.0/README.md
--rw-r--r--   0        0        0     3420 2024-04-25 11:36:08.631318 pytest_embedded_wokwi-1.9.0/pyproject.toml
--rw-r--r--   0        0        0      188 2024-04-25 11:36:08.631318 pytest_embedded_wokwi-1.9.0/pytest_embedded_wokwi/__init__.py
--rw-r--r--   0        0        0      352 2024-04-25 11:36:08.631318 pytest_embedded_wokwi-1.9.0/pytest_embedded_wokwi/arduino.py
--rw-r--r--   0        0        0      434 2024-04-25 11:36:08.631318 pytest_embedded_wokwi-1.9.0/pytest_embedded_wokwi/dut.py
--rw-r--r--   0        0        0      293 2024-04-25 11:36:08.631318 pytest_embedded_wokwi-1.9.0/pytest_embedded_wokwi/idf.py
--rw-r--r--   0        0        0     5044 2024-04-25 11:36:08.631318 pytest_embedded_wokwi-1.9.0/pytest_embedded_wokwi/wokwi_cli.py
--rw-r--r--   0        0        0     1664 2024-04-25 11:36:08.631318 pytest_embedded_wokwi-1.9.0/tests/test_wokwi.py
--rw-r--r--   0        0        0     3377 1970-01-01 00:00:00.000000 pytest_embedded_wokwi-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-04-26 05:38:44.157606 pytest_embedded_wokwi-1.9.1/LICENSE
+-rw-r--r--   0        0        0     1911 2024-04-26 05:38:44.157606 pytest_embedded_wokwi-1.9.1/README.md
+-rw-r--r--   0        0        0     3420 2024-04-26 05:38:44.157606 pytest_embedded_wokwi-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0      188 2024-04-26 05:38:44.161606 pytest_embedded_wokwi-1.9.1/pytest_embedded_wokwi/__init__.py
+-rw-r--r--   0        0        0      352 2024-04-26 05:38:44.161606 pytest_embedded_wokwi-1.9.1/pytest_embedded_wokwi/arduino.py
+-rw-r--r--   0        0        0      434 2024-04-26 05:38:44.161606 pytest_embedded_wokwi-1.9.1/pytest_embedded_wokwi/dut.py
+-rw-r--r--   0        0        0      293 2024-04-26 05:38:44.161606 pytest_embedded_wokwi-1.9.1/pytest_embedded_wokwi/idf.py
+-rw-r--r--   0        0        0     5044 2024-04-26 05:38:44.161606 pytest_embedded_wokwi-1.9.1/pytest_embedded_wokwi/wokwi_cli.py
+-rw-r--r--   0        0        0     1664 2024-04-26 05:38:44.161606 pytest_embedded_wokwi-1.9.1/tests/test_wokwi.py
+-rw-r--r--   0        0        0     3377 1970-01-01 00:00:00.000000 pytest_embedded_wokwi-1.9.1/PKG-INFO
```

### Comparing `pytest_embedded_wokwi-1.9.0/LICENSE` & `pytest_embedded_wokwi-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded_wokwi-1.9.0/README.md` & `pytest_embedded_wokwi-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_embedded_wokwi-1.9.0/pyproject.toml` & `pytest_embedded_wokwi-1.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -27,21 +27,21 @@
     "Programming Language :: Python",
     "Topic :: Software Development :: Testing",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 
 dependencies = [
-    "pytest-embedded~=1.9.0",
+    "pytest-embedded~=1.9.1",
     "toml~=0.10.2",
 ]
 
 [project.optional-dependencies]
 idf = [
-    "pytest-embedded-idf~=1.9.0",
+    "pytest-embedded-idf~=1.9.1",
 ]
 
 [project.urls]
 homepage = "https://github.com/espressif/pytest-embedded"
 repository = "https://github.com/espressif/pytest-embedded"
 documentation = "https://docs.espressif.com/projects/pytest-embedded/en/latest/"
 changelog = "https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md"
```

### Comparing `pytest_embedded_wokwi-1.9.0/pytest_embedded_wokwi/wokwi_cli.py` & `pytest_embedded_wokwi-1.9.1/pytest_embedded_wokwi/wokwi_cli.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_wokwi-1.9.0/tests/test_wokwi.py` & `pytest_embedded_wokwi-1.9.1/tests/test_wokwi.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_wokwi-1.9.0/PKG-INFO` & `pytest_embedded_wokwi-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-wokwi
-Version: 1.9.0
+Version: 1.9.1
 Summary: Make pytest-embedded plugin work with the Wokwi CLI.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>, Uri Shaked <uri@wokwi.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
@@ -16,17 +16,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: pytest-embedded~=1.9.0
+Requires-Dist: pytest-embedded~=1.9.1
 Requires-Dist: toml~=0.10.2
-Requires-Dist: pytest-embedded-idf~=1.9.0 ; extra == "idf"
+Requires-Dist: pytest-embedded-idf~=1.9.1 ; extra == "idf"
 Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
 Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Project-URL: homepage, https://github.com/espressif/pytest-embedded
 Project-URL: repository, https://github.com/espressif/pytest-embedded
 Provides-Extra: idf
 
 ### pytest-embedded-wokwi
```

