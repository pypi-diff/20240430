# Comparing `tmp/rich_click-1.8.0.dev6.tar.gz` & `tmp/rich_click-1.8.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rich_click-1.8.0.dev6.tar", last modified: Sun Apr 14 16:03:03 2024, max compression
+gzip compressed data, was "rich_click-1.8.0.dev7.tar", last modified: Wed Apr 24 02:31:58 2024, max compression
```

## Comparing `rich_click-1.8.0.dev6.tar` & `rich_click-1.8.0.dev7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:03:03.852164 rich_click-1.8.0.dev6/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-04-14 16:03:03.852164 rich_click-1.8.0.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 16:03:03.852164 rich_click-1.8.0.dev6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:03:03.844164 rich_click-1.8.0.dev6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:03:03.848163 rich_click-1.8.0.dev6/src/rich_click/
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/_compat_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/rich_click.py
--rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/rich_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/rich_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/rich_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/rich_help_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/rich_help_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    31100 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/rich_help_rendering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/src/rich_click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:03:03.852164 rich_click-1.8.0.dev6/src/rich_click.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-04-14 16:03:03.000000 rich_click-1.8.0.dev6/src/rich_click.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-14 16:03:03.000000 rich_click-1.8.0.dev6/src/rich_click.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 16:03:03.000000 rich_click-1.8.0.dev6/src/rich_click.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-14 16:03:03.000000 rich_click-1.8.0.dev6/src/rich_click.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-14 16:03:03.000000 rich_click-1.8.0.dev6/src/rich_click.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-14 16:03:03.000000 rich_click-1.8.0.dev6/src/rich_click.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:03:03.848163 rich_click-1.8.0.dev6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/tests/test_exit_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-14 16:02:59.000000 rich_click-1.8.0.dev6/tests/test_rich_click_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:31:58.527460 rich_click-1.8.0.dev7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-04-24 02:31:58.527460 rich_click-1.8.0.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:31:58.527460 rich_click-1.8.0.dev7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:31:58.519460 rich_click-1.8.0.dev7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:31:58.523460 rich_click-1.8.0.dev7/src/rich_click/
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/_compat_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/rich_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/rich_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/rich_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/rich_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/rich_help_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/rich_help_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31100 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/rich_help_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/src/rich_click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:31:58.527460 rich_click-1.8.0.dev7/src/rich_click.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-04-24 02:31:58.000000 rich_click-1.8.0.dev7/src/rich_click.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-24 02:31:58.000000 rich_click-1.8.0.dev7/src/rich_click.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:31:58.000000 rich_click-1.8.0.dev7/src/rich_click.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 02:31:58.000000 rich_click-1.8.0.dev7/src/rich_click.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-24 02:31:58.000000 rich_click-1.8.0.dev7/src/rich_click.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 02:31:58.000000 rich_click-1.8.0.dev7/src/rich_click.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:31:58.527460 rich_click-1.8.0.dev7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/tests/test_exit_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-24 02:31:50.000000 rich_click-1.8.0.dev7/tests/test_rich_click_cli.py
```

### Comparing `rich_click-1.8.0.dev6/LICENSE` & `rich_click-1.8.0.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev6/PKG-INFO` & `rich_click-1.8.0.dev7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-click
-Version: 1.8.0.dev6
+Version: 1.8.0.dev7
 Summary: Format click help output nicely with rich
 Author-email: Phil Ewels <phil@ewels.co.uk>
 Maintainer-email: Phil Ewels <phil@ewels.co.uk>, Daniel Reeves <xdanielreeves@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Phil Ewels
         
@@ -51,23 +51,25 @@
 Requires-Dist: typing_extensions
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: packaging; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: rich-codex; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-setuptools; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: markdown_include; extra == "docs"
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-glightbox; extra == "docs"
-Requires-Dist: mkdocs-material; extra == "docs"
+Requires-Dist: mkdocs-material[imaging]~=9.5.18; extra == "docs"
 Requires-Dist: mkdocs-material-extensions; extra == "docs"
 Requires-Dist: mkdocstrings[python]; extra == "docs"
+Requires-Dist: rich-codex; extra == "docs"
 
 <p align="center">
     <picture>
         <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ewels/rich-click/main/docs/images/rich-click-logo-darkmode.png">
         <img alt="rich-click logo" src="https://raw.githubusercontent.com/ewels/rich-click/main/docs/images/rich-click-logo.png">
     </picture>
 </p>
```

### Comparing `rich_click-1.8.0.dev6/README.md` & `rich_click-1.8.0.dev7/README.md`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev6/pyproject.toml` & `rich_click-1.8.0.dev7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -32,24 +32,26 @@
 [project.optional-dependencies]
 dev = [
     "mypy",
     "packaging",
     "pre-commit",
     "pytest",
     "pytest-cov",
+    "rich-codex",
     "ruff",
     "types-setuptools",
 ]
 docs = [
     "markdown_include",
     "mkdocs",
     "mkdocs-glightbox",
-    "mkdocs-material",
+    "mkdocs-material[imaging]~=9.5.18",
     "mkdocs-material-extensions",
     "mkdocstrings[python]",
+    "rich-codex",
 ]
 [project.urls]
 Documentation = "https://github.com/ewels/rich-click"
 Homepage = "https://github.com/ewels/rich-click"
 Issues = "https://github.com/ewels/rich-click/issues"
 Repository = "https://github.com/ewels/rich-click"
 [project.scripts]
```

### Comparing `rich_click-1.8.0.dev6/src/rich_click/__init__.py` & `rich_click-1.8.0.dev7/src/rich_click/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 rich-click is a minimal Python module to combine the efforts of the excellent packages 'rich' and 'click'.
 
 The intention is to provide attractive help output from Click, formatted with Rich, with minimal
 customisation required.
 """
 
-__version__ = "1.8.0dev6"
+__version__ = "1.8.0dev7"
 
 # Import the entire click API here.
 # We need to manually import these instead of `from click import *` to force
 # mypy to recognize a few type annotation overrides for the rich_click decorators.
 from click.core import Argument as Argument
 from click.core import Command as Command
 from click.core import CommandCollection as CommandCollection
```

### Comparing `rich_click-1.8.0.dev6/src/rich_click/cli.py` & `rich_click-1.8.0.dev7/src/rich_click/cli.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev6/src/rich_click/decorators.py` & `rich_click-1.8.0.dev7/src/rich_click/decorators.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev6/src/rich_click/patch.py` & `rich_click-1.8.0.dev7/src/rich_click/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 def rich_group(*args, **kwargs):  # type: ignore[no-untyped-def]
     kwargs.setdefault("cls", _PatchedRichGroup)
     return _rich_group(*args, **kwargs)
 
 
 def patch(rich_config: Optional[RichHelpConfiguration] = None) -> None:
-    """Patch Click internals to use Rich-Click types."""
+    """Patch Click internals to use rich-click types."""
     rich_click.rich_command.OVERRIDES_GUARD = True
     click.group = rich_group
     click.command = rich_command
     click.Group = _PatchedRichGroup  # type: ignore[misc]
     click.Command = _PatchedRichCommand  # type: ignore[misc]
     click.CommandCollection = _PatchedRichCommandCollection  # type: ignore[misc]
     if "MultiCommand" in dir(click):
```

### Comparing `rich_click-1.8.0.dev6/src/rich_click/rich_click.py` & `rich_click-1.8.0.dev7/src/rich_click/rich_click.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev6/src/rich_click/rich_command.py` & `rich_click-1.8.0.dev7/src/rich_click/rich_command.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev6/src/rich_click/rich_context.py` & `rich_click-1.8.0.dev7/src/rich_click/rich_context.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev6/src/rich_click/rich_help_configuration.py` & `rich_click-1.8.0.dev7/src/rich_click/rich_help_configuration.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev6/src/rich_click/rich_help_formatter.py` & `rich_click-1.8.0.dev7/src/rich_click/rich_help_formatter.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev6/src/rich_click/rich_help_rendering.py` & `rich_click-1.8.0.dev7/src/rich_click/rich_help_rendering.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev6/src/rich_click/utils.py` & `rich_click-1.8.0.dev7/src/rich_click/utils.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev6/src/rich_click.egg-info/PKG-INFO` & `rich_click-1.8.0.dev7/src/rich_click.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-click
-Version: 1.8.0.dev6
+Version: 1.8.0.dev7
 Summary: Format click help output nicely with rich
 Author-email: Phil Ewels <phil@ewels.co.uk>
 Maintainer-email: Phil Ewels <phil@ewels.co.uk>, Daniel Reeves <xdanielreeves@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Phil Ewels
         
@@ -51,23 +51,25 @@
 Requires-Dist: typing_extensions
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: packaging; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: rich-codex; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-setuptools; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: markdown_include; extra == "docs"
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-glightbox; extra == "docs"
-Requires-Dist: mkdocs-material; extra == "docs"
+Requires-Dist: mkdocs-material[imaging]~=9.5.18; extra == "docs"
 Requires-Dist: mkdocs-material-extensions; extra == "docs"
 Requires-Dist: mkdocstrings[python]; extra == "docs"
+Requires-Dist: rich-codex; extra == "docs"
 
 <p align="center">
     <picture>
         <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ewels/rich-click/main/docs/images/rich-click-logo-darkmode.png">
         <img alt="rich-click logo" src="https://raw.githubusercontent.com/ewels/rich-click/main/docs/images/rich-click-logo.png">
     </picture>
 </p>
```

### Comparing `rich_click-1.8.0.dev6/src/rich_click.egg-info/SOURCES.txt` & `rich_click-1.8.0.dev7/src/rich_click.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev6/tests/test_config.py` & `rich_click-1.8.0.dev7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev6/tests/test_exit_code.py` & `rich_click-1.8.0.dev7/tests/test_exit_code.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev6/tests/test_help.py` & `rich_click-1.8.0.dev7/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.0.dev6/tests/test_rich_click_cli.py` & `rich_click-1.8.0.dev7/tests/test_rich_click_cli.py`

 * *Files identical despite different names*

