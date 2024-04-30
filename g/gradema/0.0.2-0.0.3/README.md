# Comparing `tmp/gradema-0.0.2.tar.gz` & `tmp/gradema-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gradema-0.0.2.tar", max compression
+gzip compressed data, was "gradema-0.0.3.tar", max compression
```

## Comparing `gradema-0.0.2.tar` & `gradema-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1056 2024-03-21 22:01:48.859372 gradema-0.0.2/LICENSE
--rw-r--r--   0        0        0     1837 2024-04-29 04:47:49.112134 gradema-0.0.2/README.md
--rw-r--r--   0        0        0       76 2024-04-29 15:19:53.229011 gradema-0.0.2/gradema/__init__.py
--rw-r--r--   0        0        0      216 2024-04-29 15:40:40.187785 gradema-0.0.2/gradema/grader/__init__.py
--rw-r--r--   0        0        0     3572 2024-04-29 15:40:40.179785 gradema-0.0.2/gradema/grader/_grader.py
--rw-r--r--   0        0        0      952 2024-04-23 03:17:43.476074 gradema-0.0.2/gradema/grader/_reporter.py
--rw-r--r--   0        0        0      138 2024-04-28 23:22:30.124159 gradema-0.0.2/gradema/grader/console/__init__.py
--rw-r--r--   0        0        0    10240 2024-04-29 01:37:23.692749 gradema-0.0.2/gradema/grader/console/_console.py
--rw-r--r--   0        0        0     1207 2024-04-23 03:17:09.439666 gradema-0.0.2/gradema/grader/console/_indent.py
--rw-r--r--   0        0        0     2675 2024-04-29 01:36:25.808074 gradema-0.0.2/gradema/grader/console/_runner.py
--rw-r--r--   0        0        0      752 2024-04-27 03:22:41.296861 gradema-0.0.2/gradema/grader/console/_util.py
--rw-r--r--   0        0        0       81 2024-04-18 04:40:01.722764 gradema-0.0.2/gradema/section/__init__.py
--rw-r--r--   0        0        0     1806 2024-04-18 04:09:33.425423 gradema-0.0.2/gradema/section/_section.py
--rw-r--r--   0        0        0      831 2024-04-29 17:43:37.451646 gradema-0.0.2/gradema/test/__init__.py
--rw-r--r--   0        0        0      895 2024-04-28 23:17:24.376395 gradema-0.0.2/gradema/test/_command.py
--rw-r--r--   0        0        0      339 2024-04-29 15:39:17.702812 gradema-0.0.2/gradema/test/_dummy.py
--rw-r--r--   0        0        0     1442 2024-04-29 15:39:17.694812 gradema-0.0.2/gradema/test/_exists.py
--rw-r--r--   0        0        0     1761 2024-04-29 15:38:21.746151 gradema-0.0.2/gradema/test/_python.py
--rw-r--r--   0        0        0     5021 2024-04-26 21:13:22.593885 gradema-0.0.2/gradema/test/_reporter.py
--rw-r--r--   0        0        0     1382 2024-04-29 17:38:28.687870 gradema-0.0.2/gradema/test/_rust.py
--rw-r--r--   0        0        0     2492 2024-04-28 23:17:24.376395 gradema-0.0.2/gradema/test/_stdio.py
--rw-r--r--   0        0        0      511 2024-04-29 15:38:21.742151 gradema-0.0.2/gradema/test/_test.py
--rw-r--r--   0        0        0      127 2024-04-26 21:06:42.185277 gradema-0.0.2/gradema/test/argument.py
--rw-r--r--   0        0        0      603 2024-04-29 17:44:32.472319 gradema-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 gradema-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1056 2024-03-21 22:01:48.859372 gradema-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2072 2024-04-29 22:14:51.217676 gradema-0.0.3/README.md
+-rw-r--r--   0        0        0       76 2024-04-29 15:19:53.229011 gradema-0.0.3/gradema/__init__.py
+-rw-r--r--   0        0        0      216 2024-04-29 15:40:40.187785 gradema-0.0.3/gradema/grader/__init__.py
+-rw-r--r--   0        0        0     3572 2024-04-29 15:40:40.179785 gradema-0.0.3/gradema/grader/_grader.py
+-rw-r--r--   0        0        0      952 2024-04-23 03:17:43.476074 gradema-0.0.3/gradema/grader/_reporter.py
+-rw-r--r--   0        0        0      138 2024-04-28 23:22:30.124159 gradema-0.0.3/gradema/grader/console/__init__.py
+-rw-r--r--   0        0        0    10414 2024-04-29 21:47:36.529334 gradema-0.0.3/gradema/grader/console/_console.py
+-rw-r--r--   0        0        0     1207 2024-04-23 03:17:09.439666 gradema-0.0.3/gradema/grader/console/_indent.py
+-rw-r--r--   0        0        0     2675 2024-04-29 01:36:25.808074 gradema-0.0.3/gradema/grader/console/_runner.py
+-rw-r--r--   0        0        0      752 2024-04-27 03:22:41.296861 gradema-0.0.3/gradema/grader/console/_util.py
+-rw-r--r--   0        0        0       81 2024-04-18 04:40:01.722764 gradema-0.0.3/gradema/section/__init__.py
+-rw-r--r--   0        0        0     1806 2024-04-18 04:09:33.425423 gradema-0.0.3/gradema/section/_section.py
+-rw-r--r--   0        0        0      889 2024-04-29 22:00:57.623296 gradema-0.0.3/gradema/test/__init__.py
+-rw-r--r--   0        0        0      895 2024-04-28 23:17:24.376395 gradema-0.0.3/gradema/test/_command.py
+-rw-r--r--   0        0        0      339 2024-04-29 15:39:17.702812 gradema-0.0.3/gradema/test/_dummy.py
+-rw-r--r--   0        0        0     1442 2024-04-29 15:39:17.694812 gradema-0.0.3/gradema/test/_exists.py
+-rw-r--r--   0        0        0     1797 2024-04-29 21:57:56.165041 gradema-0.0.3/gradema/test/_python.py
+-rw-r--r--   0        0        0     5021 2024-04-26 21:13:22.593885 gradema-0.0.3/gradema/test/_reporter.py
+-rw-r--r--   0        0        0     1558 2024-04-30 05:13:07.916008 gradema-0.0.3/gradema/test/_rust.py
+-rw-r--r--   0        0        0     2540 2024-04-29 22:00:57.619296 gradema-0.0.3/gradema/test/_stdio.py
+-rw-r--r--   0        0        0      511 2024-04-29 15:38:21.742151 gradema-0.0.3/gradema/test/_test.py
+-rw-r--r--   0        0        0      127 2024-04-29 22:20:37.974000 gradema-0.0.3/gradema/test/argument.py
+-rw-r--r--   0        0        0      603 2024-04-30 05:16:43.766688 gradema-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2880 1970-01-01 00:00:00.000000 gradema-0.0.3/PKG-INFO
```

### Comparing `gradema-0.0.2/LICENSE` & `gradema-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gradema-0.0.2/README.md` & `gradema-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -51,8 +51,13 @@
 poetry run pytest tests
 ```
 
 
 # TODO
 
 * Use [py2cfg](https://pypi.org/project/py2cfg/) to produce control flow graphs
-
+* Use pytest instead of basic python3 and asserts
+* Text diff (not critical)
+* Arg tests and the OUTPUT_FILE interpolation thing
+* Think about where to put unit tests
+  * Rust - move tests inside src?
+* Do C++ example - lowest priority
```

### Comparing `gradema-0.0.2/gradema/grader/_grader.py` & `gradema-0.0.3/gradema/grader/_grader.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.2/gradema/grader/_reporter.py` & `gradema-0.0.3/gradema/grader/_reporter.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.2/gradema/grader/console/_console.py` & `gradema-0.0.3/gradema/grader/console/_console.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,16 @@
         stdin=subprocess.DEVNULL,
         stdout=subprocess.DEVNULL,
         stderr=subprocess.DEVNULL,
     )
 
 
 def html_diff(left_path: Path, right_path: Path, html_output_path: Path) -> None:
+    # TODO remember that file.readlines() LOADS THE ENTIRE FILE INTO MEMORY
+    #   We might not care about that right now, but this could be a problem later with huge files
     with left_path.open("r") as left, right_path.open("r") as right:
         diff = difflib.HtmlDiff().make_file(
             left.readlines(),
             right.readlines(),
             str(left_path),
             str(right_path),
         )
```

### Comparing `gradema-0.0.2/gradema/grader/console/_indent.py` & `gradema-0.0.3/gradema/grader/console/_indent.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.2/gradema/grader/console/_runner.py` & `gradema-0.0.3/gradema/grader/console/_runner.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.2/gradema/grader/console/_util.py` & `gradema-0.0.3/gradema/grader/console/_util.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.2/gradema/section/_section.py` & `gradema-0.0.3/gradema/section/_section.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.2/gradema/test/__init__.py` & `gradema-0.0.3/gradema/test/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from ._test import Test, FractionalTestResult, PercentTestResult, TestResult
 from ._python import (
     create_python_test,
     create_python_format_check,
     create_python_format_check_from_path,
     create_python_type_check,
     create_python_stdio_test,
+    create_python_arg_test,
 )
 from ._dummy import dummy_test
 from ._exists import create_file_exists_test
 from ._rust import RustProgram
 
 __all__ = [
     "TestReporter",
@@ -23,8 +24,9 @@
     "create_python_stdio_test",
     "create_python_format_check",
     "create_python_format_check_from_path",
     "create_python_type_check",
     "dummy_test",
     "create_file_exists_test",
     "RustProgram",
+    "create_python_arg_test",
 ]
```

### Comparing `gradema-0.0.2/gradema/test/_command.py` & `gradema-0.0.3/gradema/test/_command.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.2/gradema/test/_exists.py` & `gradema-0.0.3/gradema/test/_exists.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.2/gradema/test/_python.py` & `gradema-0.0.3/gradema/test/_python.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pathlib import Path
 
 import editorconfig  # type: ignore
 
 from . import Test
 from ._command import CommandTest
 from ._stdio import StdioTest
+from .argument import Argument
 
 
 def create_python_test(module_name: str) -> Test:
     try:
         # TODO importing the module could run student code in the autograder's process. Maybe we shouldn't do this
         importlib.import_module(module_name)
     except ModuleNotFoundError:
@@ -28,15 +29,15 @@
     :param goal_file:
     :return:
     """
     command = ["python", "-m", module_name]
     return StdioTest(command, test_identifier, input_file, goal_file)
 
 
-def create_python_arg_test(module_name: str, test_identifier: str, args: list[str], goal_file: Path) -> Test:
+def create_python_arg_test(module_name: str, test_identifier: str, args: list[Argument], goal_file: Path) -> Test:
     command = ["python", "-m", module_name] + args
     return StdioTest(command, test_identifier, None, goal_file)
 
 
 def create_python_format_check_from_path(path: str) -> Test:
     line_length = editorconfig.get_properties(str((Path(path) / "some_random_file.py").absolute())).get("max_line_length")
     command = ["black", "--check"]
```

### Comparing `gradema-0.0.2/gradema/test/_reporter.py` & `gradema-0.0.3/gradema/test/_reporter.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.2/gradema/test/_rust.py` & `gradema-0.0.3/gradema/test/_rust.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,13 +19,17 @@
         command = [str(self.binary_location)]
         return StdioTest(command, test_identifier, input_file, goal_file)
 
     def create_format_check(self) -> Test:
         """
         Creates a rustfmt check.
 
-        Note that the resulting command will be something like `rustfmt --check src/main.rs`.
+        Note that the resulting command will be something like ``rustfmt --check src/main.rs``.
         Even though this only includes the main file, all files referenced by main will also be format checked -- it's not necessary to list all the files here!
+        https://github.com/rust-lang/rustfmt/issues/2426
 
         :return: A test that completes successfully when there are no formatting errors
         """
         return CommandTest(["rustfmt", "--check", str(self.main_location)])
+
+    def create_cargo_command(self, arguments: list[str]) -> Test:
+        return CommandTest(["cargo"] + arguments)
```

### Comparing `gradema-0.0.2/gradema/test/_stdio.py` & `gradema-0.0.3/gradema/test/_stdio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import filecmp
 import subprocess
 from pathlib import Path
 from typing import Optional, TextIO
 
 from gradema.test._reporter import TestReporter
 from gradema.test._test import Test, TestResult, FractionalTestResult
+from gradema.test.argument import Argument
 
 
 class StdioTest(Test):
     """
     A Standard Input/Output Test
 
     Traditionally, a stdio test would have no arguments passed to the command, it would have an input file, and a goal file.
@@ -16,15 +17,15 @@
 
     This new stdio test is very similar, but it can also do what a traditional arg test could do:
     take no input, and have custom arguments passed to the command.
     If you don't want anything directed into the command's stdin, then just assign None to input_file.
     If you want custom arguments passed to the command, give those custom arguments to the command argument (you may have to do that manually).
     """
 
-    def __init__(self, command: list[str], test_identifier: str, input_file: Optional[Path], goal_file: Path):
+    def __init__(self, command: list[Argument], test_identifier: str, input_file: Optional[Path], goal_file: Path):
         self.command = command
         self.test_identifier = test_identifier
         self.input_file = input_file
         self.goal_file = goal_file
 
     def run(self, reporter: TestReporter) -> TestResult:
         data = reporter.report_stdio_command(self.command, self.test_identifier, self.input_file)
```

### Comparing `gradema-0.0.2/pyproject.toml` & `gradema-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gradema"
-version = "0.0.2"
+version = "0.0.3"
 description = "The utility you need to easily configure auto-grading"
 authors = ["Lavender Shannon <jdsfz4@mst.edu>"]
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://gradema.readthedocs.io"
 repository = "https://git.mst.edu/gradema/gradema"
```

### Comparing `gradema-0.0.2/PKG-INFO` & `gradema-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradema
-Version: 0.0.2
+Version: 0.0.3
 Summary: The utility you need to easily configure auto-grading
 Home-page: https://gradema.readthedocs.io
 License: MIT
 Author: Lavender Shannon
 Author-email: jdsfz4@mst.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -73,9 +73,14 @@
 poetry run pytest tests
 ```
 
 
 # TODO
 
 * Use [py2cfg](https://pypi.org/project/py2cfg/) to produce control flow graphs
-
+* Use pytest instead of basic python3 and asserts
+* Text diff (not critical)
+* Arg tests and the OUTPUT_FILE interpolation thing
+* Think about where to put unit tests
+  * Rust - move tests inside src?
+* Do C++ example - lowest priority
```

