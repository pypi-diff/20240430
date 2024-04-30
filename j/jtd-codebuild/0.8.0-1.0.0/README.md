# Comparing `tmp/jtd_codebuild-0.8.0.tar.gz` & `tmp/jtd_codebuild-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jtd_codebuild-0.8.0.tar", max compression
+gzip compressed data, was "jtd_codebuild-1.0.0.tar", max compression
```

## Comparing `jtd_codebuild-0.8.0.tar` & `jtd_codebuild-1.0.0.tar`

### file list

```diff
@@ -1,39 +1,70 @@
--rw-r--r--   0        0        0     1056 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/LICENSE
--rw-r--r--   0        0        0    10115 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/README.md
--rw-r--r--   0        0        0        0 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/__init__.py
--rw-r--r--   0        0        0      397 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/__main__.py
--rw-r--r--   0        0        0     1520 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/bundle.py
--rw-r--r--   0        0        0     2067 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/codebuild.py
--rw-r--r--   0        0        0      577 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/config.py
--rw-r--r--   0        0        0      188 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/generators/__init__.py
--rw-r--r--   0        0        0     2142 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/generators/generator.py
--rw-r--r--   0        0        0    12254 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/generators/python_generator.py
--rw-r--r--   0        0        0     1620 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/generators/typescript_generator.py
--rw-r--r--   0        0        0     2044 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/inheritance.py
--rw-r--r--   0        0        0     2303 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/loaders.py
--rw-r--r--   0        0        0        0 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/__init__.py
--rw-r--r--   0        0        0       38 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_1/.gitignore
--rw-r--r--   0        0        0      600 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_1/jtd-codebuild.json
--rw-r--r--   0        0        0      134 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_1/src/definitions/book.jtd.yaml
--rw-r--r--   0        0        0      191 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_1/src/definitions/user.jtd.yaml
--rw-r--r--   0        0        0       41 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_1/src/schema.jtd.yaml
--rw-r--r--   0        0        0       38 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_2/.gitignore
--rw-r--r--   0        0        0      626 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_2/jtd-codebuild.json
--rw-r--r--   0        0        0      433 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_2/src/definitions/book.jtd.yaml
--rw-r--r--   0        0        0      191 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_2/src/definitions/user.jtd.yaml
--rw-r--r--   0        0        0      239 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_2/src/dtos/io.jtd.yaml
--rw-r--r--   0        0        0       41 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_2/src/schema.jtd.yaml
--rw-r--r--   0        0        0        3 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_3/.gitignore
--rw-r--r--   0        0        0      142 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_3/jtd-codebuild.json
--rw-r--r--   0        0        0       41 2024-04-13 06:08:02.259141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_3/src/schema.jtd.yaml
--rw-r--r--   0        0        0        3 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_4/.gitignore
--rw-r--r--   0        0        0      648 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_4/jtd-codebuild.json
--rw-r--r--   0        0        0      471 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_4/src/definitions/io.jtd.yaml
--rw-r--r--   0        0        0       41 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/jtd_codebuild/tests/fixtures/example_project_4/src/schema.jtd.yaml
--rw-r--r--   0        0        0     1619 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/jtd_codebuild/tests/test_example_project_1.py
--rw-r--r--   0        0        0      837 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/jtd_codebuild/tests/test_example_project_2.py
--rw-r--r--   0        0        0      519 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/jtd_codebuild/tests/test_example_project_3.py
--rw-r--r--   0        0        0      837 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/jtd_codebuild/tests/test_example_project_4.py
--rw-r--r--   0        0        0     3211 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/jtd_codebuild/utils.py
--rw-r--r--   0        0        0     1870 2024-04-13 06:08:02.263141 jtd_codebuild-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    11479 1970-01-01 00:00:00.000000 jtd_codebuild-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1056 2024-04-30 21:23:10.387424 jtd_codebuild-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3236 2024-04-30 21:23:10.387424 jtd_codebuild-1.0.0/README.md
+-rw-r--r--   0        0        0       55 2024-04-30 21:23:10.387424 jtd_codebuild-1.0.0/jtd_codebuild/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-30 21:23:10.387424 jtd_codebuild-1.0.0/jtd_codebuild/__main__.py
+-rw-r--r--   0        0        0     3374 2024-04-30 21:23:10.387424 jtd_codebuild-1.0.0/jtd_codebuild/bundler.py
+-rw-r--r--   0        0        0     1435 2024-04-30 21:23:10.387424 jtd_codebuild-1.0.0/jtd_codebuild/cli.py
+-rw-r--r--   0        0        0     2878 2024-04-30 21:23:10.387424 jtd_codebuild-1.0.0/jtd_codebuild/codebuild.py
+-rw-r--r--   0        0        0       86 2024-04-30 21:23:10.387424 jtd_codebuild-1.0.0/jtd_codebuild/commands/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-30 21:23:10.387424 jtd_codebuild-1.0.0/jtd_codebuild/commands/_build.py
+-rw-r--r--   0        0        0      365 2024-04-30 21:23:10.387424 jtd_codebuild-1.0.0/jtd_codebuild/commands/_command.py
+-rw-r--r--   0        0        0      868 2024-04-30 21:23:10.387424 jtd_codebuild-1.0.0/jtd_codebuild/commands/_init.py
+-rw-r--r--   0        0        0      218 2024-04-30 21:23:10.387424 jtd_codebuild-1.0.0/jtd_codebuild/component.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:23:10.387424 jtd_codebuild-1.0.0/jtd_codebuild/config/__init__.py
+-rw-r--r--   0        0        0       63 2024-04-30 21:23:10.387424 jtd_codebuild-1.0.0/jtd_codebuild/config/project/__init__.py
+-rw-r--r--   0        0        0     1032 2024-04-30 21:23:10.387424 jtd_codebuild-1.0.0/jtd_codebuild/config/project/_project.py
+-rw-r--r--   0        0        0     9341 2024-04-30 21:23:10.387424 jtd_codebuild-1.0.0/jtd_codebuild/config/project/config.json
+-rw-r--r--   0        0        0      327 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/config/project/model/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/config/project/model/_config.py
+-rw-r--r--   0        0        0     1499 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/config/project/model/_target.py
+-rw-r--r--   0        0        0      351 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/config/project/model/_types.py
+-rw-r--r--   0        0        0       73 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/config/workspace/__init__.py
+-rw-r--r--   0        0        0      447 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/config/workspace/_workspace.py
+-rw-r--r--   0        0        0       63 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/generators/__init__.py
+-rw-r--r--   0        0        0     2178 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/generators/_generator.py
+-rw-r--r--   0        0        0       44 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/generators/_values.py
+-rw-r--r--   0        0        0       69 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/generators/csharp/__init__.py
+-rw-r--r--   0        0        0      591 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/generators/csharp/_generator.py
+-rw-r--r--   0        0        0       65 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/generators/go/__init__.py
+-rw-r--r--   0        0        0      539 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/generators/go/_generator.py
+-rw-r--r--   0        0        0       67 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/generators/java/__init__.py
+-rw-r--r--   0        0        0      567 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/generators/java/_generator.py
+-rw-r--r--   0        0        0       69 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/generators/python/__init__.py
+-rw-r--r--   0        0        0    19508 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/generators/python/_generator.py
+-rw-r--r--   0        0        0       67 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/generators/ruby/__init__.py
+-rw-r--r--   0        0        0      549 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/generators/ruby/_generator.py
+-rw-r--r--   0        0        0       67 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/generators/rust/__init__.py
+-rw-r--r--   0        0        0      240 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/generators/rust/_generator.py
+-rw-r--r--   0        0        0       73 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/generators/typescript/__init__.py
+-rw-r--r--   0        0        0     2995 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/generators/typescript/_generator.py
+-rw-r--r--   0        0        0     2244 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/inheritance.py
+-rw-r--r--   0        0        0      126 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/logger/__init__.py
+-rw-r--r--   0        0        0     1354 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/logger/_click_logger.py
+-rw-r--r--   0        0        0      841 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/logger/_logger.py
+-rw-r--r--   0        0        0      428 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/logger/_noop_logger.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/preset/__init__.py
+-rw-r--r--   0        0        0      186 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/preset/_preset.py
+-rw-r--r--   0        0        0       56 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/preset/config/__init__.py
+-rw-r--r--   0        0        0      713 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/preset/config/_preset.py
+-rw-r--r--   0        0        0      228 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/preset/config/templates/jtd-codebuild.json
+-rw-r--r--   0        0        0       57 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/preset/project/__init__.py
+-rw-r--r--   0        0        0     1118 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/preset/project/_preset.py
+-rw-r--r--   0        0        0        4 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/preset/project/templates/.gitignore
+-rw-r--r--   0        0        0      233 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/preset/project/templates/jtd-codebuild.json
+-rw-r--r--   0        0        0       59 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/preset/workspace/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/preset/workspace/_preset.py
+-rw-r--r--   0        0        0        3 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/preset/workspace/templates/jtd-codebuild-workspace.json
+-rw-r--r--   0        0        0        0 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/utils/__init__.py
+-rw-r--r--   0        0        0     1205 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/utils/fs.py
+-rw-r--r--   0        0        0       51 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/utils/function/__init__.py
+-rw-r--r--   0        0        0      429 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/utils/function/_string.py
+-rw-r--r--   0        0        0      949 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/utils/io.py
+-rw-r--r--   0        0        0       56 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/utils/list/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/utils/list/_find.py
+-rw-r--r--   0        0        0       64 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/utils/mapping/__init__.py
+-rw-r--r--   0        0        0      620 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/utils/mapping/_subscriptable.py
+-rw-r--r--   0        0        0      414 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/utils/string.py
+-rw-r--r--   0        0        0      615 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/utils/subprocess.py
+-rw-r--r--   0        0        0       90 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/jtd_codebuild/values.py
+-rw-r--r--   0        0        0     1967 2024-04-30 21:23:10.391424 jtd_codebuild-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4803 1970-01-01 00:00:00.000000 jtd_codebuild-1.0.0/PKG-INFO
```

### Comparing `jtd_codebuild-0.8.0/LICENSE` & `jtd_codebuild-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jtd_codebuild-0.8.0/jtd_codebuild/codebuild.py` & `jtd_codebuild-1.0.0/jtd_codebuild/codebuild.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,87 @@
-import os
-import json
-import subprocess
-from typing import List
-from .bundle import bundle_schema
-from .config import get_config
-from .inheritance import resolve_inheritance
-from .utils import safe_open, wait_for_processes
-from .generators import (
-    JTDCodeGenerator,
-    JTDCodeGeneratorTypescriptTarget,
-    JTDCodeGeneratorPythonTarget,
-)
-
-
-def jtd_codebuild(cwd: str) -> None:
-    """Generate code from the JSON Type Definition files.
-
-    Args:
-        cwd: The current working directory.
-    """
-    # We use basename of cwd as the name of the package
-    # we're trying to generate a schema for
-    package_name = os.path.basename(cwd)
-
-    print(f"[jtd-codebuild] Start building: {package_name}")
-    config = get_config(cwd)
-
-    print("[jtd-codebuild] Bundling schema files...")
-    schema = bundle_schema(cwd)
-
-    print("[jtd-codebuild] Resolving inheritance...")
-    schema = resolve_inheritance(schema)
-
-    # Write a full schema file to output specified
-    # by the configuration file in json format
-    print("[jtd-codebuild] Writing full schema...")
-    output_path = os.path.join(cwd, config["output-schema-path"])
-    with safe_open(output_path, "w") as f:
-        json.dump(schema, f, indent=2)
-
-    print("[jtd-codebuild] Generating code...")
-    # Generate code from the full schema file
-    targets = config.get("targets", [])
-    processes: List[subprocess.Popen] = []
-    for target in targets:
-        generator: JTDCodeGenerator = None
-
-        target_language = target["language"]
-        if target_language == "typescript":
-            # Case: TypeScript
-            generator = JTDCodeGeneratorTypescriptTarget(cwd, output_path)
-        elif target_language == "python":
-            # Case: Python
-            generator = JTDCodeGeneratorPythonTarget(cwd, output_path)
+from os import getcwd
+from os.path import relpath
+from typing import Callable, Type
+from toolz import pipe
+from toolz.curried import map
+from .utils.fs import resolve
+from .utils.io import write_json
+from .bundler import Bundler
+from .inheritance import InheritanceResolver
+from .component import Component
+from .config.project import get_project_config
+from .config.project.model import Language, Target
+from .generators import JTDCodeGenerator
+from .generators.python import PythonJTDCodeGenerator
+from .generators.typescript import TypescriptJTDCodeGenerator
+from .generators.go import GoJTDCodeGenerator
+from .generators.java import JavaJTDCodeGenerator
+from .generators.ruby import RubyJTDCodeGenerator
+from .generators.rust import RustJTDCodeGenerator
+from .generators.csharp import CSharpJTDCodeGenerator
+
+GENERATORS: dict[Language, Type[JTDCodeGenerator]] = {
+    "python": PythonJTDCodeGenerator,
+    "typescript": TypescriptJTDCodeGenerator,
+    "go": GoJTDCodeGenerator,
+    "java": JavaJTDCodeGenerator,
+    "ruby": RubyJTDCodeGenerator,
+    "rust": RustJTDCodeGenerator,
+    "csharp": CSharpJTDCodeGenerator,
+}
+
+
+class Codebuild(Component):
+    def run(  # noqa: C901
+        self,
+        path: str,
+        cwd: str = getcwd(),
+    ):
+        """Generate code from the JSON Type Definition files.
+
+        Args:
+            path: The current working directory.
+        """
+        # Get the path of the target directory
+        target_path = resolve(cwd, path)
+        config = get_project_config(target_path)
+
+        self.logger.info(f"Start building: {path}")
+
+        self.logger.info("Bundling IDL files...")
+        bundler = Bundler(logger=self.logger)
+        inheritance = InheritanceResolver(logger=self.logger)
+        bundled_jtd_schema = pipe(
+            bundler.bundle(target_path, config),
+            inheritance.resolve,
+        )
+
+        schema_path = resolve(target_path, config.jtdBundlePath)
+        write_json(schema_path, bundled_jtd_schema)
+
+        self.logger.success(f"Wrote bundled IDL file at: {relpath(schema_path, cwd)}")
+
+        self.logger.info("Generating targets...")
+
+        context = {
+            "cwd": target_path,
+            "schema_path": schema_path,
+            "logger": self.logger,
+        }
+
+        def create_generator(target: Target) -> Callable[[], None]:
+            def generate() -> None:
+                generator = GENERATORS[target.language](**context)
+                generator.generate(target)
+
+            return generate
+
+        generators = pipe(config.targets, map(create_generator))
+        if config.targetProcessingStrategy == "serial":
+            for generator in generators:
+                generator()
         else:
-            # Default case
-            generator = JTDCodeGenerator(cwd, output_path)
+            from joblib import Parallel, delayed
 
-        processes.extend(generator.generate(target))
+            Parallel(n_jobs=-1)(delayed(generator)() for generator in generators)
 
-    # Wait for all processes to finish
-    wait_for_processes(processes)
-
-    print("[jtd-codebuild] Done!")
+        self.logger.success("Done!")
```

### Comparing `jtd_codebuild-0.8.0/jtd_codebuild/generators/generator.py` & `jtd_codebuild-1.0.0/jtd_codebuild/generators/_generator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,71 @@
-import os
+import abc
 import subprocess
-from typing import Dict, Any, AnyStr, List
-from ..utils import safe_mkdir
+from jtd_codebuild.component import Component
+from jtd_codebuild.logger import Logger
+from jtd_codebuild.config.project.model import Target
+from jtd_codebuild.utils.fs import safe_mkdir, resolve
+from jtd_codebuild.utils.subprocess import stream_logs
 
 
-class JTDCodeGenerator:
+class JTDCodeGenerator(Component, metaclass=abc.ABCMeta):
     """Generate code from the JSON Type Definition files.
 
     Attributes:
         cwd: The current working directory.
         schema_path: The path to the JSON Type Definition schema file.
     """
 
-    def __init__(self, cwd: str, schema_path: str):
-        """Initialize the JTDCodeGenerator.
-
-        Args:
-            cwd: The current working directory.
-            schema_path: The path to the JSON Type Definition schema file.
-        """
+    def __init__(
+        self,
+        cwd: str,
+        schema_path: str,
+        *,
+        logger: Logger | None = None,
+    ) -> None:
         self.cwd = cwd
         self.schema_path = schema_path
+        super().__init__(logger=logger)
 
     def _codegen_command(
         self,
-        schema_path: str,
-        output_dir: str,
-        target_language: str,
+        target: Target,
     ) -> str:
         """Generate code from a JSON Type Definition schema file.
 
         Args:
             schema_path: The path to the JSON Type Definition schema file.
             output_dir: The output directory.
             target_language: The target language.
 
         Returns:
             The command to generate code.
         """
+        schema_path = self.get_schema_path()
+        output_dir = self.get_target_path(target)
+        target_language = target.language
         return f"jtd-codegen {schema_path} --{target_language}-out {output_dir}"
 
-    def get_target_path(self, target: Dict[AnyStr, Any]) -> AnyStr:
-        """Get the target path.
-
-        Args:
-            target: Target configuration.
-
-        Returns:
-            The target path.
-        """
-        return os.path.join(self.cwd, target["path"])
-
-    def generate(
-        self,
-        target: Dict[AnyStr, Any],
-    ) -> List[subprocess.Popen]:
+    def generate(self, target: Target) -> None:
         """Generate code from the JSON Type Definition files.
 
         Args:
             target: Target configuration.
 
         Returns:
             A list of subprocesses created by the code generation.
         """
-        target_language = target["language"]
-        target_path = self.get_target_path(target)
-        safe_mkdir(target_path)
+        safe_mkdir(self.get_target_path(target))
         process = subprocess.Popen(
-            self._codegen_command(self.schema_path, target_path, target_language),
+            self._codegen_command(target),
             shell=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
-        return [process]
+        stream_logs(process, logger=self.logger, level="debug")
+        process.wait()
+
+    def get_schema_path(self) -> str:
+        return resolve(self.cwd, self.schema_path)
+
+    def get_target_path(self, target: Target) -> str:
+        return resolve(self.cwd, target.path)
```

### Comparing `jtd_codebuild-0.8.0/pyproject.toml` & `jtd_codebuild-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jtd-codebuild"
-version = "0.8.0"
+version = "1.0.0"
 description = "Tool for generating language specific schemas and interfaces code from JSON Type Definition IDL files in yaml format. Powered by jtd-codegen."
 classifiers = [
   'Development Status :: 5 - Production/Stable',
   'Intended Audience :: Developers',
   'Natural Language :: English',
   'Topic :: Software Development',
   'Topic :: Software Development :: Libraries :: Python Modules',
@@ -27,14 +27,19 @@
 include = "jtd_codebuild"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 pyyaml = "^6.0.1"
 click = "^8.1.7"
 case-converter = "^1.1.0"
+toolz = "^0.12.1"
+deepmerge = "^1.1.1"
+joblib = "^1.4.0"
+pydantic = "^2.7.1"
+colorama = "^0.4.6"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.1.0"
 black = "^23.10.1"
 poethepoet = "^0.24.4"
 
 [tool.poetry.group.test.dependencies]
```

