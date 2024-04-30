# Comparing `tmp/gradema-0.0.1.tar.gz` & `tmp/gradema-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gradema-0.0.1.tar", max compression
+gzip compressed data, was "gradema-0.0.2.tar", max compression
```

## Comparing `gradema-0.0.1.tar` & `gradema-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0     1056 2024-03-21 22:01:48.859372 gradema-0.0.1/LICENSE
--rw-r--r--   0        0        0     1682 2024-04-26 00:55:25.790849 gradema-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-04-18 00:37:04.937481 gradema-0.0.1/gradema/__init__.py
--rw-r--r--   0        0        0      125 2024-04-18 04:26:39.541385 gradema-0.0.1/gradema/grader/__init__.py
--rw-r--r--   0        0        0     6196 2024-04-23 03:17:43.500074 gradema-0.0.1/gradema/grader/_grader.py
--rw-r--r--   0        0        0      952 2024-04-23 03:17:43.476074 gradema-0.0.1/gradema/grader/_reporter.py
--rw-r--r--   0        0        0       81 2024-04-18 04:40:01.722764 gradema-0.0.1/gradema/grader/console/__init__.py
--rw-r--r--   0        0        0    10232 2024-04-27 22:21:26.639240 gradema-0.0.1/gradema/grader/console/_console.py
--rw-r--r--   0        0        0     1207 2024-04-23 03:17:09.439666 gradema-0.0.1/gradema/grader/console/_indent.py
--rw-r--r--   0        0        0      752 2024-04-27 03:22:41.296861 gradema-0.0.1/gradema/grader/console/_util.py
--rw-r--r--   0        0        0       81 2024-04-18 04:40:01.722764 gradema-0.0.1/gradema/section/__init__.py
--rw-r--r--   0        0        0     1806 2024-04-18 04:09:33.425423 gradema-0.0.1/gradema/section/_section.py
--rw-r--r--   0        0        0      781 2024-04-26 21:21:14.507316 gradema-0.0.1/gradema/test/__init__.py
--rw-r--r--   0        0        0      855 2024-04-23 03:17:22.591823 gradema-0.0.1/gradema/test/_command.py
--rw-r--r--   0        0        0      350 2024-04-17 19:25:39.477795 gradema-0.0.1/gradema/test/_dummy.py
--rw-r--r--   0        0        0     1453 2024-04-27 03:24:06.049816 gradema-0.0.1/gradema/test/_exists.py
--rw-r--r--   0        0        0     1799 2024-04-25 23:45:12.620864 gradema-0.0.1/gradema/test/_python.py
--rw-r--r--   0        0        0     5021 2024-04-26 21:13:22.593885 gradema-0.0.1/gradema/test/_reporter.py
--rw-r--r--   0        0        0     2452 2024-04-25 23:38:09.803835 gradema-0.0.1/gradema/test/_stdio.py
--rw-r--r--   0        0        0      524 2024-04-18 03:58:41.889813 gradema-0.0.1/gradema/test/_test.py
--rw-r--r--   0        0        0      127 2024-04-26 21:06:42.185277 gradema-0.0.1/gradema/test/argument.py
--rw-r--r--   0        0        0      506 2024-04-28 00:13:44.384177 gradema-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2386 1970-01-01 00:00:00.000000 gradema-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1056 2024-03-21 22:01:48.859372 gradema-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1837 2024-04-29 04:47:49.112134 gradema-0.0.2/README.md
+-rw-r--r--   0        0        0       76 2024-04-29 15:19:53.229011 gradema-0.0.2/gradema/__init__.py
+-rw-r--r--   0        0        0      216 2024-04-29 15:40:40.187785 gradema-0.0.2/gradema/grader/__init__.py
+-rw-r--r--   0        0        0     3572 2024-04-29 15:40:40.179785 gradema-0.0.2/gradema/grader/_grader.py
+-rw-r--r--   0        0        0      952 2024-04-23 03:17:43.476074 gradema-0.0.2/gradema/grader/_reporter.py
+-rw-r--r--   0        0        0      138 2024-04-28 23:22:30.124159 gradema-0.0.2/gradema/grader/console/__init__.py
+-rw-r--r--   0        0        0    10240 2024-04-29 01:37:23.692749 gradema-0.0.2/gradema/grader/console/_console.py
+-rw-r--r--   0        0        0     1207 2024-04-23 03:17:09.439666 gradema-0.0.2/gradema/grader/console/_indent.py
+-rw-r--r--   0        0        0     2675 2024-04-29 01:36:25.808074 gradema-0.0.2/gradema/grader/console/_runner.py
+-rw-r--r--   0        0        0      752 2024-04-27 03:22:41.296861 gradema-0.0.2/gradema/grader/console/_util.py
+-rw-r--r--   0        0        0       81 2024-04-18 04:40:01.722764 gradema-0.0.2/gradema/section/__init__.py
+-rw-r--r--   0        0        0     1806 2024-04-18 04:09:33.425423 gradema-0.0.2/gradema/section/_section.py
+-rw-r--r--   0        0        0      831 2024-04-29 17:43:37.451646 gradema-0.0.2/gradema/test/__init__.py
+-rw-r--r--   0        0        0      895 2024-04-28 23:17:24.376395 gradema-0.0.2/gradema/test/_command.py
+-rw-r--r--   0        0        0      339 2024-04-29 15:39:17.702812 gradema-0.0.2/gradema/test/_dummy.py
+-rw-r--r--   0        0        0     1442 2024-04-29 15:39:17.694812 gradema-0.0.2/gradema/test/_exists.py
+-rw-r--r--   0        0        0     1761 2024-04-29 15:38:21.746151 gradema-0.0.2/gradema/test/_python.py
+-rw-r--r--   0        0        0     5021 2024-04-26 21:13:22.593885 gradema-0.0.2/gradema/test/_reporter.py
+-rw-r--r--   0        0        0     1382 2024-04-29 17:38:28.687870 gradema-0.0.2/gradema/test/_rust.py
+-rw-r--r--   0        0        0     2492 2024-04-28 23:17:24.376395 gradema-0.0.2/gradema/test/_stdio.py
+-rw-r--r--   0        0        0      511 2024-04-29 15:38:21.742151 gradema-0.0.2/gradema/test/_test.py
+-rw-r--r--   0        0        0      127 2024-04-26 21:06:42.185277 gradema-0.0.2/gradema/test/argument.py
+-rw-r--r--   0        0        0      603 2024-04-29 17:44:32.472319 gradema-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 gradema-0.0.2/PKG-INFO
```

### Comparing `gradema-0.0.1/LICENSE` & `gradema-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gradema-0.0.1/README.md` & `gradema-0.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Gradema
 
 The utility you need to easily configure auto-grading.
 
+https://pypi.org/project/gradema/
+
+https://gradema.readthedocs.io
+
 Python 3.10 required.
 
 ## Try it out
 
 ```shell
 poetry install
 poetry run python -m example.binaryconvert.autograder
@@ -44,8 +48,11 @@
 All tests are located in the `tests` directory, so you must explicitly state that directory, otherwise some tests will be incorrectly picked up in other directories.
 
 ```shell
 poetry run pytest tests
 ```
 
 
+# TODO
+
+* Use [py2cfg](https://pypi.org/project/py2cfg/) to produce control flow graphs
```

### Comparing `gradema-0.0.1/gradema/grader/_reporter.py` & `gradema-0.0.2/gradema/grader/_reporter.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.1/gradema/grader/console/_console.py` & `gradema-0.0.2/gradema/grader/console/_console.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,23 +67,23 @@
         ],
         stdin=subprocess.DEVNULL,
         stdout=subprocess.DEVNULL,
         stderr=subprocess.DEVNULL,
     )
 
 
-def html_diff(left_path: Path, right_path: Path, html_output_path: Path):
-    with left_path.open('r') as left, right_path.open('r') as right:
+def html_diff(left_path: Path, right_path: Path, html_output_path: Path) -> None:
+    with left_path.open("r") as left, right_path.open("r") as right:
         diff = difflib.HtmlDiff().make_file(
             left.readlines(),
             right.readlines(),
             str(left_path),
             str(right_path),
         )
-        with html_output_path.open('w') as f_out:
+        with html_output_path.open("w") as f_out:
             f_out.write(diff)
 
 
 @dataclasses.dataclass
 class ConsoleTestReporter(TestReporter):
     reporter: "ConsoleGraderReporter"
```

### Comparing `gradema-0.0.1/gradema/grader/console/_indent.py` & `gradema-0.0.2/gradema/grader/console/_indent.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.1/gradema/grader/console/_util.py` & `gradema-0.0.2/gradema/grader/console/_util.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.1/gradema/section/_section.py` & `gradema-0.0.2/gradema/section/_section.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.1/gradema/test/__init__.py` & `gradema-0.0.2/gradema/test/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     create_python_format_check,
     create_python_format_check_from_path,
     create_python_type_check,
     create_python_stdio_test,
 )
 from ._dummy import dummy_test
 from ._exists import create_file_exists_test
+from ._rust import RustProgram
 
 __all__ = [
     "TestReporter",
     "CommandData",
     "StdioCommandData",
     "Test",
     "FractionalTestResult",
@@ -21,8 +22,9 @@
     "create_python_test",
     "create_python_stdio_test",
     "create_python_format_check",
     "create_python_format_check_from_path",
     "create_python_type_check",
     "dummy_test",
     "create_file_exists_test",
+    "RustProgram",
 ]
```

### Comparing `gradema-0.0.1/gradema/test/_command.py` & `gradema-0.0.2/gradema/test/_command.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import subprocess
 
-from gradema.test import Test, TestReporter, TestResult, FractionalTestResult
+from gradema.test._reporter import TestReporter
+from gradema.test._test import Test, TestResult, FractionalTestResult
 
 
 class CommandTest(Test):
     def __init__(self, command: list[str], debug_command: list[str] | None = None):
         self.command = command
         self.debug_command = debug_command
```

### Comparing `gradema-0.0.1/gradema/test/_exists.py` & `gradema-0.0.2/gradema/test/_exists.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from os import PathLike
 from pathlib import Path
 
 import magic
 
-from gradema.test import Test, TestReporter, TestResult, FractionalTestResult
+from . import TestReporter, Test, TestResult, FractionalTestResult
 
 
 def create_file_exists_test(files: list[tuple[str | Path | PathLike[str], str]], mime: bool = False) -> Test:
     return FileExistsTest(files, mime)
 
 
 class FileExistsTest(Test):
```

### Comparing `gradema-0.0.1/gradema/test/_python.py` & `gradema-0.0.2/gradema/test/_python.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import importlib
 from pathlib import Path
 
 import editorconfig  # type: ignore
 
-from gradema.test import Test
-from gradema.test._command import CommandTest
-from gradema.test._stdio import StdioTest
+from . import Test
+from ._command import CommandTest
+from ._stdio import StdioTest
 
 
 def create_python_test(module_name: str) -> Test:
     try:
         # TODO importing the module could run student code in the autograder's process. Maybe we shouldn't do this
         importlib.import_module(module_name)
     except ModuleNotFoundError:
         raise ValueError(f"Module {module_name} not found")
 
-    return CommandTest(["python3", "-m", module_name], ["pudb", "-m", module_name])
+    return CommandTest(["python", "-m", module_name], ["pudb", "-m", module_name])
 
 
 def create_python_stdio_test(module_name: str, test_identifier: str, input_file: Path, goal_file: Path) -> Test:
     """
     Creates a traditional stdio test
 
     :param module_name:
     :param test_identifier:
     :param input_file:
     :param goal_file:
     :return:
     """
-    command = ["python3", "-m", module_name]
+    command = ["python", "-m", module_name]
     return StdioTest(command, test_identifier, input_file, goal_file)
 
 
 def create_python_arg_test(module_name: str, test_identifier: str, args: list[str], goal_file: Path) -> Test:
-    command = ["python3", "-m", module_name] + args
+    command = ["python", "-m", module_name] + args
     return StdioTest(command, test_identifier, None, goal_file)
 
 
 def create_python_format_check_from_path(path: str) -> Test:
     line_length = editorconfig.get_properties(str((Path(path) / "some_random_file.py").absolute())).get("max_line_length")
     command = ["black", "--check"]
     if line_length is not None:
```

### Comparing `gradema-0.0.1/gradema/test/_reporter.py` & `gradema-0.0.2/gradema/test/_reporter.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.1/gradema/test/_stdio.py` & `gradema-0.0.2/gradema/test/_stdio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import filecmp
 import subprocess
 from pathlib import Path
 from typing import Optional, TextIO
 
-from gradema.test import Test, TestReporter, TestResult, FractionalTestResult
+from gradema.test._reporter import TestReporter
+from gradema.test._test import Test, TestResult, FractionalTestResult
 
 
 class StdioTest(Test):
     """
     A Standard Input/Output Test
 
     Traditionally, a stdio test would have no arguments passed to the command, it would have an input file, and a goal file.
```

### Comparing `gradema-0.0.1/PKG-INFO` & `gradema-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: gradema
-Version: 0.0.1
+Version: 0.0.2
 Summary: The utility you need to easily configure auto-grading
+Home-page: https://gradema.readthedocs.io
 License: MIT
 Author: Lavender Shannon
 Author-email: jdsfz4@mst.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: editorconfig (>=0.12.4,<0.13.0)
-Requires-Dist: mypy (>=1.9.0,<2.0.0)
+Requires-Dist: mypy (>=1.10.0,<2.0.0)
 Requires-Dist: pudb (>=2024.1,<2025.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0)
 Requires-Dist: rich (==13.7.1)
+Project-URL: Repository, https://git.mst.edu/gradema/gradema
 Description-Content-Type: text/markdown
 
 # Gradema
 
 The utility you need to easily configure auto-grading.
 
+https://pypi.org/project/gradema/
+
+https://gradema.readthedocs.io
+
 Python 3.10 required.
 
 ## Try it out
 
 ```shell
 poetry install
 poetry run python -m example.binaryconvert.autograder
@@ -64,9 +70,12 @@
 All tests are located in the `tests` directory, so you must explicitly state that directory, otherwise some tests will be incorrectly picked up in other directories.
 
 ```shell
 poetry run pytest tests
 ```
 
 
+# TODO
+
+* Use [py2cfg](https://pypi.org/project/py2cfg/) to produce control flow graphs
```

