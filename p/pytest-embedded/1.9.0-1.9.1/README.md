# Comparing `tmp/pytest_embedded-1.9.0.tar.gz` & `tmp/pytest_embedded-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded-1.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded-1.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded-1.9.0.tar` & `pytest_embedded-1.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1094 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/LICENSE
--rw-r--r--   0        0        0      120 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/README.md
--rw-r--r--   0        0        0     3345 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/pyproject.toml
--rw-r--r--   0        0        0      200 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/pytest_embedded/__init__.py
--rw-r--r--   0        0        0     1487 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/pytest_embedded/app.py
--rw-r--r--   0        0        0     7556 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/pytest_embedded/dut.py
--rw-r--r--   0        0        0    26482 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/pytest_embedded/dut_factory.py
--rw-r--r--   0        0        0     7125 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/pytest_embedded/log.py
--rw-r--r--   0        0        0    42768 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/pytest_embedded/plugin.py
--rw-r--r--   0        0        0    10807 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/pytest_embedded/unity.py
--rw-r--r--   0        0        0    10206 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/pytest_embedded/utils.py
--rw-r--r--   0        0        0    20777 2024-04-25 11:36:08.631318 pytest_embedded-1.9.0/tests/test_base.py
--rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 pytest_embedded-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-04-26 05:38:44.161606 pytest_embedded-1.9.1/LICENSE
+-rw-r--r--   0        0        0      120 2024-04-26 05:38:44.161606 pytest_embedded-1.9.1/README.md
+-rw-r--r--   0        0        0     3345 2024-04-26 05:38:44.161606 pytest_embedded-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0      200 2024-04-26 05:38:44.161606 pytest_embedded-1.9.1/pytest_embedded/__init__.py
+-rw-r--r--   0        0        0     1487 2024-04-26 05:38:44.161606 pytest_embedded-1.9.1/pytest_embedded/app.py
+-rw-r--r--   0        0        0     7556 2024-04-26 05:38:44.161606 pytest_embedded-1.9.1/pytest_embedded/dut.py
+-rw-r--r--   0        0        0    26490 2024-04-26 05:38:44.161606 pytest_embedded-1.9.1/pytest_embedded/dut_factory.py
+-rw-r--r--   0        0        0     7125 2024-04-26 05:38:44.161606 pytest_embedded-1.9.1/pytest_embedded/log.py
+-rw-r--r--   0        0        0    42768 2024-04-26 05:38:44.161606 pytest_embedded-1.9.1/pytest_embedded/plugin.py
+-rw-r--r--   0        0        0    10807 2024-04-26 05:38:44.161606 pytest_embedded-1.9.1/pytest_embedded/unity.py
+-rw-r--r--   0        0        0    10206 2024-04-26 05:38:44.161606 pytest_embedded-1.9.1/pytest_embedded/utils.py
+-rw-r--r--   0        0        0    20777 2024-04-26 05:38:44.161606 pytest_embedded-1.9.1/tests/test_base.py
+-rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 pytest_embedded-1.9.1/PKG-INFO
```

### Comparing `pytest_embedded-1.9.0/LICENSE` & `pytest_embedded-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.9.0/pyproject.toml` & `pytest_embedded-1.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.9.0/pytest_embedded/app.py` & `pytest_embedded-1.9.1/pytest_embedded/app.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.9.0/pytest_embedded/dut.py` & `pytest_embedded-1.9.1/pytest_embedded/dut.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.9.0/pytest_embedded/dut_factory.py` & `pytest_embedded-1.9.1/pytest_embedded/dut_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 import os
 import subprocess
 import sys
 import typing as t
 from collections import defaultdict
 from pathlib import Path
 
-from pytest_embedded_idf import CaseTester
-
 if t.TYPE_CHECKING:
     from pytest_embedded_idf import LinuxSerial
     from pytest_embedded_idf.dut import IdfDut
     from pytest_embedded_jtag import Gdb, OpenOcd
     from pytest_embedded_qemu import Qemu
     from pytest_embedded_serial import Serial
     from pytest_embedded_wokwi import WokwiCLI
@@ -564,14 +562,16 @@
                     _close_or_terminate(obj)
                 del layout
             del DutFactory.obj_stack
         cls.obj_stack = []
 
     @classmethod
     def unity_tester(cls, *args: 'IdfDut'):
+        from pytest_embedded_idf import CaseTester
+
         return CaseTester(args)
 
     @classmethod
     def create(
         cls,
         *,
         embedded_services: str = '',
```

### Comparing `pytest_embedded-1.9.0/pytest_embedded/log.py` & `pytest_embedded-1.9.1/pytest_embedded/log.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.9.0/pytest_embedded/plugin.py` & `pytest_embedded-1.9.1/pytest_embedded/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.9.0/pytest_embedded/unity.py` & `pytest_embedded-1.9.1/pytest_embedded/unity.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.9.0/pytest_embedded/utils.py` & `pytest_embedded-1.9.1/pytest_embedded/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.9.0/tests/test_base.py` & `pytest_embedded-1.9.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded-1.9.0/PKG-INFO` & `pytest_embedded-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded
-Version: 1.9.0
+Version: 1.9.1
 Summary: A pytest plugin that designed for embedded testing.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

