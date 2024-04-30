# Comparing `tmp/protokolo-2.1.3.tar.gz` & `tmp/protokolo-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protokolo-2.1.3.tar", max compression
+gzip compressed data, was "protokolo-2.1.4.tar", max compression
```

## Comparing `protokolo-2.1.3.tar` & `protokolo-2.1.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     3663 2024-04-27 22:50:04.816278 protokolo-2.1.3/CHANGELOG.md
-drwxr-xr-x   0        0        0        0 2023-10-19 20:10:58.496541 protokolo-2.1.3/LICENSES/
--rw-r--r--   0        0        0    18375 2023-10-19 20:10:58.496541 protokolo-2.1.3/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0        0        0     7048 2023-10-19 20:10:57.776495 protokolo-2.1.3/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0    34674 2023-10-19 20:10:58.188521 protokolo-2.1.3/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0        0        0     7095 2024-04-27 21:40:40.247205 protokolo-2.1.3/README.md
--rw-r--r--   0        0        0     2233 2024-04-27 21:40:40.251205 protokolo-2.1.3/_build.py
--rw-r--r--   0        0        0      758 2023-11-07 14:06:49.911908 protokolo-2.1.3/docs/Makefile
--rw-r--r--   0        0        0     2532 2024-04-27 22:46:04.274281 protokolo-2.1.3/docs/conf.py
--rw-r--r--   0        0        0      744 2024-04-27 21:40:40.251205 protokolo-2.1.3/docs/index.rst
--rw-r--r--   0        0        0      934 2023-11-07 14:07:09.073053 protokolo-2.1.3/docs/make.bat
--rw-r--r--   0        0        0      271 2024-04-27 21:40:40.251205 protokolo-2.1.3/docs/man/index.rst
--rw-r--r--   0        0        0     1638 2024-04-27 21:40:40.251205 protokolo-2.1.3/docs/man/protokolo-compile.rst
--rw-r--r--   0        0        0     2078 2024-04-27 21:40:40.251205 protokolo-2.1.3/docs/man/protokolo-init.rst
--rw-r--r--   0        0        0     1036 2024-04-27 21:40:40.251205 protokolo-2.1.3/docs/man/protokolo.rst
--rw-r--r--   0        0        0     7976 2024-04-27 21:40:40.251205 protokolo-2.1.3/docs/reference.md
--rw-r--r--   0        0        0     2944 2024-04-27 22:49:58.820225 protokolo-2.1.3/pyproject.toml
--rw-r--r--   0        0        0      177 2024-04-27 22:49:58.820225 protokolo-2.1.3/src/protokolo/__init__.py
--rw-r--r--   0        0        0      290 2024-04-27 21:40:40.255205 protokolo-2.1.3/src/protokolo/__main__.py
--rw-r--r--   0        0        0     4030 2024-04-27 21:40:40.255205 protokolo-2.1.3/src/protokolo/_formatter.py
--rw-r--r--   0        0        0     1424 2024-04-27 21:40:40.255205 protokolo-2.1.3/src/protokolo/_util.py
--rw-r--r--   0        0        0    10749 2024-04-27 21:40:40.255205 protokolo-2.1.3/src/protokolo/cli.py
--rw-r--r--   0        0        0    10420 2024-04-27 21:40:40.255205 protokolo-2.1.3/src/protokolo/compile.py
--rw-r--r--   0        0        0    12133 2024-04-27 21:40:40.255205 protokolo-2.1.3/src/protokolo/config.py
--rw-r--r--   0        0        0     3619 2024-04-27 21:40:40.259205 protokolo-2.1.3/src/protokolo/exceptions.py
--rw-r--r--   0        0        0     1099 2024-04-27 21:40:40.259205 protokolo-2.1.3/src/protokolo/i18n.py
--rw-r--r--   0        0        0     3785 2024-04-27 21:40:40.259205 protokolo-2.1.3/src/protokolo/initialise.py
--rw-r--r--   0        0        0        0 2023-10-21 21:28:23.558911 protokolo-2.1.3/src/protokolo/py.typed
--rw-r--r--   0        0        0     1520 2024-04-27 21:40:40.259205 protokolo-2.1.3/src/protokolo/replace.py
--rw-r--r--   0        0        0      903 2024-04-27 21:40:40.259205 protokolo-2.1.3/src/protokolo/types.py
--rw-r--r--   0        0        0     2263 2024-04-27 21:40:40.259205 protokolo-2.1.3/tests/conftest.py
--rw-r--r--   0        0        0    20548 2024-04-27 21:40:40.259205 protokolo-2.1.3/tests/test_cli.py
--rw-r--r--   0        0        0    15759 2024-04-27 21:40:40.259205 protokolo-2.1.3/tests/test_compile.py
--rw-r--r--   0        0        0    11400 2024-04-27 21:40:40.259205 protokolo-2.1.3/tests/test_config.py
--rw-r--r--   0        0        0     3592 2023-10-28 21:28:57.351824 protokolo-2.1.3/tests/test_exceptions.py
--rw-r--r--   0        0        0     6053 2024-04-27 21:40:40.259205 protokolo-2.1.3/tests/test_formatter.py
--rw-r--r--   0        0        0     3907 2024-04-27 21:40:40.259205 protokolo-2.1.3/tests/test_replace.py
--rw-r--r--   0        0        0     8065 1970-01-01 00:00:00.000000 protokolo-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4042 2024-04-30 17:50:27.423492 protokolo-2.1.4/CHANGELOG.md
+drwxr-xr-x   0        0        0        0 2024-04-07 16:16:03.003871 protokolo-2.1.4/LICENSES/
+-rw-r--r--   0        0        0    18375 2024-04-07 16:16:03.003871 protokolo-2.1.4/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0        0        0     7048 2024-04-07 16:16:03.003871 protokolo-2.1.4/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0    34674 2024-04-07 16:16:03.003871 protokolo-2.1.4/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0        0        0     7095 2024-04-30 15:55:26.799615 protokolo-2.1.4/README.md
+-rw-r--r--   0        0        0     2233 2024-04-30 15:55:26.799615 protokolo-2.1.4/_build.py
+-rw-r--r--   0        0        0      758 2024-04-07 16:16:03.003871 protokolo-2.1.4/docs/Makefile
+-rw-r--r--   0        0        0     2590 2024-04-30 16:37:24.775452 protokolo-2.1.4/docs/conf.py
+-rw-r--r--   0        0        0      744 2024-04-30 15:58:57.289471 protokolo-2.1.4/docs/index.rst
+-rw-r--r--   0        0        0      895 2024-04-07 16:16:03.003871 protokolo-2.1.4/docs/make.bat
+-rw-r--r--   0        0        0      271 2024-04-30 15:55:26.799615 protokolo-2.1.4/docs/man/index.rst
+-rw-r--r--   0        0        0     2274 2024-04-30 17:17:38.429193 protokolo-2.1.4/docs/man/protokolo-compile.rst
+-rw-r--r--   0        0        0     2067 2024-04-30 17:02:09.660093 protokolo-2.1.4/docs/man/protokolo-init.rst
+-rw-r--r--   0        0        0     1000 2024-04-30 16:49:29.603973 protokolo-2.1.4/docs/man/protokolo.rst
+-rw-r--r--   0        0        0     7989 2024-04-30 15:55:26.799615 protokolo-2.1.4/docs/reference.md
+-rw-r--r--   0        0        0     2945 2024-04-30 17:50:27.387491 protokolo-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0      177 2024-04-30 17:50:27.387491 protokolo-2.1.4/src/protokolo/__init__.py
+-rw-r--r--   0        0        0      290 2024-04-07 16:16:03.003871 protokolo-2.1.4/src/protokolo/__main__.py
+-rw-r--r--   0        0        0     4030 2024-04-30 15:55:26.799615 protokolo-2.1.4/src/protokolo/_formatter.py
+-rw-r--r--   0        0        0     1424 2024-04-30 16:05:12.017171 protokolo-2.1.4/src/protokolo/_util.py
+-rw-r--r--   0        0        0     9336 2024-04-30 17:31:59.790524 protokolo-2.1.4/src/protokolo/cli.py
+-rw-r--r--   0        0        0    10491 2024-04-30 16:36:14.614611 protokolo-2.1.4/src/protokolo/compile.py
+-rw-r--r--   0        0        0    12334 2024-04-30 16:37:40.039634 protokolo-2.1.4/src/protokolo/config.py
+-rw-r--r--   0        0        0     3619 2024-04-30 15:55:26.799615 protokolo-2.1.4/src/protokolo/exceptions.py
+-rw-r--r--   0        0        0     1099 2024-04-30 15:55:26.799615 protokolo-2.1.4/src/protokolo/i18n.py
+-rw-r--r--   0        0        0     3785 2024-04-30 15:55:26.799615 protokolo-2.1.4/src/protokolo/initialise.py
+-rw-r--r--   0        0        0        0 2024-04-07 16:16:03.003871 protokolo-2.1.4/src/protokolo/py.typed
+-rw-r--r--   0        0        0     1520 2024-04-30 15:55:26.799615 protokolo-2.1.4/src/protokolo/replace.py
+-rw-r--r--   0        0        0      903 2024-04-30 15:55:26.799615 protokolo-2.1.4/src/protokolo/types.py
+-rw-r--r--   0        0        0     2263 2024-04-30 15:55:26.799615 protokolo-2.1.4/tests/conftest.py
+-rw-r--r--   0        0        0    20548 2024-04-30 15:55:26.799615 protokolo-2.1.4/tests/test_cli.py
+-rw-r--r--   0        0        0    15759 2024-04-30 15:55:26.799615 protokolo-2.1.4/tests/test_compile.py
+-rw-r--r--   0        0        0    11400 2024-04-30 15:55:26.803615 protokolo-2.1.4/tests/test_config.py
+-rw-r--r--   0        0        0     3592 2024-04-07 16:16:03.003871 protokolo-2.1.4/tests/test_exceptions.py
+-rw-r--r--   0        0        0     6053 2024-04-30 15:55:26.803615 protokolo-2.1.4/tests/test_formatter.py
+-rw-r--r--   0        0        0     3907 2024-04-30 15:55:26.803615 protokolo-2.1.4/tests/test_replace.py
+-rw-r--r--   0        0        0     8065 1970-01-01 00:00:00.000000 protokolo-2.1.4/PKG-INFO
```

### Comparing `protokolo-2.1.3/CHANGELOG.md` & `protokolo-2.1.4/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,26 @@
 
 The versions follow [semantic versioning](https://semver.org) for the
 `protokolo` CLI command and its behaviour. There are no guarantees of stability
 for the `protokolo` Python library.
 
 <!-- protokolo-section-tag -->
 
+## 2.1.4 - 2024-04-30
+
+### Fixed
+
+- Changed the docs dependency for `sphinxcontrib-apidoc` from `^0.3.0` to
+  `>=0.3.0`.
+- Order of items in API documentation is now identical to how they are ordered
+  in the source code.
+- `protokolo compile --help` missed a paragraph. Instead of adding the
+  paragraph, a lot of `--help` text has been moved into the accompanying
+  manpages.
+
 ## 2.1.3 - 2024-04-28
 
 ### Fixed
 
 - Don't show change log in overview page in Sphinx. This bug was introduced in
   v2.1.0.
```

### Comparing `protokolo-2.1.3/LICENSES/CC-BY-SA-4.0.txt` & `protokolo-2.1.4/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/LICENSES/CC0-1.0.txt` & `protokolo-2.1.4/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/LICENSES/GPL-3.0-or-later.txt` & `protokolo-2.1.4/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/README.md` & `protokolo-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/_build.py` & `protokolo-2.1.4/_build.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/docs/Makefile` & `protokolo-2.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/docs/conf.py` & `protokolo-2.1.4/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "Protokolo"
-copyright = "2023, Carmen Bianca BAKKER"
+copyright = "2023 Carmen Bianca BAKKER"
 author = "Carmen Bianca BAKKER"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "myst_parser",
@@ -38,14 +38,17 @@
 
 # -- Extensions configuration ------------------------------------------------
 
 apidoc_module_dir = str(ROOT_DIR / "src/protokolo")
 # apidoc_output_dir = "api"
 # apidoc_excluded_paths = []
 apidoc_separate_modules = True
+apidoc_toc_file = False
+
+autodoc_member_order = "bysource"
 
 intersphinx_mapping = {"python": ("https://docs.python.org/3", None)}
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "furo"
```

### Comparing `protokolo-2.1.3/docs/index.rst` & `protokolo-2.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/docs/man/protokolo-compile.rst` & `protokolo-2.1.4/docs/man/protokolo-compile.rst`

 * *Files 13% similar despite different names*

```diff
@@ -5,23 +5,46 @@
 
 protokolo-compile
 =================
 
 Synopsis
 --------
 
-**protokolo compile** [*--help*] [*options*]
+**protokolo compile** [*options*]
 
 Description
 -----------
 
 :program:`protokolo compile` aggregates the contents of a change log directory
-into a new section in a change log file. The new section is inserted after the
-first line in the change log containing the text ``protokolo-section-tag``.
-Afterwards, the fragment files in the change log directory are deleted.
+into a new section in a change log file. Afterwards, the fragment files in the
+change log directory are deleted.
+
+A change log directory should contain a '.protokolo.toml' file that defines some
+attributes of the section. This is an example file::
+
+    [protokolo.section]
+    title = "${version} - ${date}"
+    level = 2
+
+When the section is compiled, its heading may look like this::
+
+    ## 1.0.0 - 2023-11-08
+
+The heading is followed by the contents of files in the section's directory, and
+subsections in subdirectories. If a section is empty (no change log fragments),
+it is not compiled.
+
+The change log file should contain the following comment, which is the location
+in the file after which the compiled section will be pasted::
+
+    <!-- protokolo-section-tag -->
+
+For more documentation and options, read the documentation at
+<https://protokolo.readthedocs.io>.
+
 
 Options with defaults
 ---------------------
 
 If the below options are not defined, they default to the corresponding options
 in the ``.protokolo.toml`` global configuration file if one exists, or otherwise
 their base defaults if they have one.
```

### Comparing `protokolo-2.1.3/docs/man/protokolo-init.rst` & `protokolo-2.1.4/docs/man/protokolo-init.rst`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 protokolo-init
 ==============
 
 Synopsis
 --------
 
-**protokolo init** [*--help*] [*options*]
+**protokolo init** [*options*]
 
 Description
 -----------
 
 :program:`protokolo init` sets up your project to be ready to use Protokolo
 using defaults recommended by `Keep a Changelog <https://keepachangelog.com>`_.
 It sets up three things:
```

### Comparing `protokolo-2.1.3/docs/man/protokolo.rst` & `protokolo-2.1.4/docs/man/protokolo.rst`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 protokolo
 =========
 
 Synopsis
 --------
 
-**protokolo** [*--help*] [*--version*] <command> [*options*] [*<args>*]
+**protokolo** [*options*] <command>
 
 Description
 -----------
 
 :program:`protokolo` allows you to maintain your change log fragments in
 separate files, and then finally aggregate them into a new section in CHANGELOG
 just before release.
```

### Comparing `protokolo-2.1.3/docs/reference.md` & `protokolo-2.1.4/docs/reference.md`

 * *Files 1% similar despite different names*

```diff
@@ -191,24 +191,26 @@
 does not end with a newline character, one is implicitly added during
 compilation.
 
 Fragments in the same section are sorted alphabetically by their file name. If
 you want to make sure that a fragment appears first or last, you can prefix the
 file name with something like `000_` or `zzz_` respectively.
 
+```{tip}
 Because of how the compilation works, you typically want to follow a few rules:
 
 - Do not start the fragment with a newline.
 - Do not include headings.
 - If the fragment represents a list item:
   - Start with a bullet, typically `- ` or `* `.
   - End the fragment with zero or one newline.
 - If the fragment represents a paragraph:
   - Adjust its file name to make it appear exactly where you want it to appear.
   - End the fragment with two newlines.
+```
 
 ## Compilation
 
 The main command of Protokolo is `protokolo compile`. It gathers all your change
 log fragment files and aggregates them into a new section in your change log
 file, after which the change log fragment files are deleted.
```

### Comparing `protokolo-2.1.3/pyproject.toml` & `protokolo-2.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 [tool.poetry]
 name = "protokolo"
-version = "2.1.3"
+version = "2.1.4"
 description = "Protokolo is a change log generator."
 authors = [
     "Carmen Bianca BAKKER <carmen@carmenbianca.eu>"
 ]
 maintainers = [
     "Carmen Bianca BAKKER <carmen@carmenbianca.eu>"
 ]
@@ -60,15 +60,15 @@
 reuse = "^3.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = ">=7.0.0"
-sphinxcontrib-apidoc = "^0.3.0"
+sphinxcontrib-apidoc = ">=0.3.0"
 myst-parser = "^2.0.0"
 furo = ">=2023.3.27"
 
 [tool.poetry.group.lsp]
 optional = true
 
 [tool.poetry.group.lsp.dependencies]
@@ -82,15 +82,15 @@
 script = "_build.py"
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [bumpver]
-current_version = "v2.1.3"
+current_version = "v2.1.4"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "Bump version: {old_version} → {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `protokolo-2.1.3/src/protokolo/_formatter.py` & `protokolo-2.1.4/src/protokolo/_formatter.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/src/protokolo/_util.py` & `protokolo-2.1.4/src/protokolo/_util.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/src/protokolo/cli.py` & `protokolo-2.1.4/src/protokolo/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmen@carmenbianca.eu>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
-"""Main entry of program."""
+"""Main entry of program.
+
+The autodoc documentation of this module is broken, but there is nothing in this
+module that you can't learn from typing ``protokolo --help``.
+"""
 
 import gettext
 import os
 import tomllib
-from inspect import cleandoc
 from io import TextIOWrapper
 from pathlib import Path
 
 import click
 from click.formatting import wrap_text
 
 from ._formatter import MARKUP_EXTENSION_MAPPING as _MARKUP_EXTENSION_MAPPING
@@ -65,15 +68,23 @@
         " along with this program. If not, see"
         " <https://www.gnu.org/licenses/>."
     )
     + "\n\n"
     + _("Written by Carmen Bianca BAKKER.")
 )
 
-_MAIN_HELP = _("Protokolo is a change log generator.")
+_MAIN_HELP = (
+    _("Protokolo is a change log generator.")
+    + "\n\n"
+    + _(
+        "Protokolo allows you to maintain your change log fragments in"
+        " separate files, and then finally aggregate them into a new section in"
+        " CHANGELOG just before release."
+    )
+)
 
 
 @click.group(name="protokolo", help=_MAIN_HELP)
 @click.version_option(
     package_name="protokolo",
     message=wrap_text(_VERSION_TEXT, preserve_paragraphs=True),
 )
@@ -102,56 +113,18 @@
             ctx.default_map["init"] = {
                 "changelog": config.changelog,
                 "markup": config.markup,
                 "directory": config.directory,
             }
 
 
-_COMPILE_HELP = (
-    _(
-        "Aggregate all change log fragments into a change log file. The"
-        " fragments are gathered from a change log directory, and subsequently"
-        " deleted."
-    )
-    + "\n\n"
-    + _(
-        "A change log directory should contain a '.protokolo.toml' file that"
-        " defines some attributes of the section. This is an example file:"
-    )
-    + "\n\n"
-    + cleandoc(
-        """
-        \b
-        [protokolo.section]
-        title = "${version} - ${date}"
-        level = 2
-        """
-    )
-    + "\n\n"
-    + _("When the section is compiled, it looks a little like this:")
-    + "\n\n"
-    + "## 1.0.0 - 2023-11-08"
-    + "\n\n"
-    + _(
-        "The heading is followed by the contents of files in the section's"
-        " directory. If a section is empty (no change log fragments), it is not"
-        " compiled."
-    )
-    + "\n\n"
-    + cleandoc(
-        """
-        \b
-        <!-- protokolo-section-tag -->
-        """
-    )
-    + "\n\n"
-    + _(
-        "For more documentation and options, read the documentation at"
-        " <https://protokolo.readthedocs.io>."
-    )
+_COMPILE_HELP = _(
+    "Aggregate all change log fragments into a change log file. The"
+    " fragments are gathered from a change log directory, and subsequently"
+    " deleted."
 )
 
 
 @main.command(name="compile", help=_COMPILE_HELP)
 @click.option(
     "--changelog",
     "-c",
@@ -264,41 +237,16 @@
         _delete_fragments(section)
 
 
 _INIT_HELP = (
     _(
         "Set up your project to be ready to use Protokolo. It creates a change"
         " log file, a change log directory with subsections that match the Keep"
-        " a Changelog recommendations, .protokolo.toml files with metadata for"
-        " those (sub)sections, and a root .protokolo.toml file with defaults"
-        " for subsequent Protokolo commands. Assuming defaults, the end result"
-        " looks like this:"
-    )
-    + "\n\n"
-    + cleandoc(
-        """
-        \b
-        .
-        ├── changelog.d
-        │   ├── added
-        │   │   └── .protokolo.toml
-        │   ├── changed
-        │   │   └── .protokolo.toml
-        │   ├── deprecated
-        │   │   └── .protokolo.toml
-        │   ├── fixed
-        │   │   └── .protokolo.toml
-        │   ├── removed
-        │   │   └── .protokolo.toml
-        │   ├── security
-        │   │   └── .protokolo.toml
-        │   └── .protokolo.toml
-        ├── CHANGELOG.md
-        └── .protokolo.toml
-        """
+        " a Changelog recommendations, and a root .protokolo.toml file with"
+        " defaults for subsequent Protokolo commands."
     )
     + "\n\n"
     + _(
         "Files that already exist are never overwritten, except the root"
         " .protokolo.toml file, which is always (re-)generated."
     )
 )
@@ -350,10 +298,10 @@
         raise click.UsageError(str(error)) from error
 
 
 def _delete_fragments(section: Section) -> None:
     """Delete :class:`.compile.Fragment`s' source files recursively."""
     for fragment in section.fragments:
         if fragment.source:
-            fragment.source.unlink(missing_ok=True)
+            Path(fragment.source).unlink(missing_ok=True)
     for subsection in section.subsections:
         _delete_fragments(subsection)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `protokolo-2.1.3/src/protokolo/compile.py` & `protokolo-2.1.4/src/protokolo/compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import errno
 import tomllib
 from io import StringIO
 from itertools import chain
 from operator import attrgetter
 from os import strerror
-from pathlib import Path
+from pathlib import Path, PurePath
 from typing import Iterator, Self, cast
 
 import attrs as attrs_
 from attrs.converters import optional
 
 from ._formatter import MARKUP_EXTENSION_MAPPING as _MARKUP_EXTENSION_MAPPING
 from ._formatter import MARKUP_FORMATTER_MAPPING as _MARKUP_FORMATTER_MAPPING
@@ -32,15 +32,17 @@
 
 
 @attrs_.define(frozen=True)
 class Fragment:
     """A fragment, analogous to a file."""
 
     text: str
-    source: Path | None = attrs_.field(default=None, converter=optional(Path))
+    source: PurePath | None = attrs_.field(
+        default=None, converter=optional(PurePath)
+    )
 
     def compile(self) -> str:
         """Compile the fragment. For the time being, this just means adding a
         newline at the end if one does not exist.
         """
         if not self.text.endswith("\n"):
             return f"{self.text}\n"
@@ -49,15 +51,17 @@
 
 @attrs_.define(eq=False)
 class Section:
     """A section, analogous to a directory."""
 
     attrs: SectionAttributes = attrs_.field(factory=SectionAttributes)
     markup: SupportedMarkup = "markdown"
-    source: Path | None = attrs_.field(default=None, converter=optional(Path))
+    source: PurePath | None = attrs_.field(
+        default=None, converter=optional(PurePath)
+    )
 
     fragments: set[Fragment] = attrs_.field(factory=set, init=False)
     subsections: set[Self] = attrs_.field(factory=set, init=False)
 
     @classmethod
     def from_directory(
         cls,
@@ -251,15 +255,16 @@
         """
         with_source = {
             fragment
             for fragment in self.fragments
             if fragment.source is not None
         }
         source_sorted = sorted(
-            with_source, key=lambda fragment: cast(Path, fragment.source).name
+            with_source,
+            key=lambda fragment: cast(PurePath, fragment.source).name,
         )
         alphabetical_sorted = sorted(
             self.fragments - with_source, key=attrgetter("text")
         )
         return chain(source_sorted, alphabetical_sorted)
 
     def sorted_subsections(self) -> Iterator[Self]:
```

### Comparing `protokolo-2.1.3/src/protokolo/config.py` & `protokolo-2.1.4/src/protokolo/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 from .types import StrPath, TOMLValue, TOMLValueType
 
 
 def parse_toml(
     toml: str | IO[bytes],
     section: Sequence[str] | None = None,
 ) -> dict[str, Any]:
-    """
+    """Parse a string representing a TOML file, and return a dictionary
+    representing the defined section.
+
     Args:
         toml: A TOML string or binary file object.
         sections: A list of nested sections, for example
             ``["protokolo", "section"]`` to return the values of
             ``[protokolo.section]``
 
     Raises:
@@ -54,15 +56,18 @@
         return nested_itemgetter(*section)(values)
     except KeyError:
         return {}
 
 
 @attrs.define
 class TOMLConfig:
-    """A utility class to hold data parsed from a TOML file."""
+    """A utility class to hold data parsed from a TOML file.
+
+    Immediately after object instantiation, :meth:`validate` is called.
+    """
 
     _values: dict[str, TOMLValue] = attrs.field(factory=dict)
     source: str | None = attrs.field(converter=str, default=None)
 
     def __attrs_post_init__(self) -> None:
         self._values = deepcopy(self._values)
         # Can't use validator on the attribute itself because the validation
@@ -107,15 +112,16 @@
 
     def validate(self) -> None:
         """Verify that all keys contain valid TOML types. This is automatically
         run on object instantiation.
 
         Raises:
             DictTypeError: value isn't an expected/supported type.
-            DictTypeListError: if a list contains elements other than a dict.
+            DictTypeListError: if a list contains elements that aren't
+                supported.
         """
         self._validate(cast(dict[str, Any], self._values))
 
     def _validate(self, values: dict[str, Any]) -> None:
         for name, value in values.items():
             # Use typed annotations to expect a very specific type. If not,
             # allow any valid TOML type.
```

### Comparing `protokolo-2.1.3/src/protokolo/exceptions.py` & `protokolo-2.1.4/src/protokolo/exceptions.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/src/protokolo/i18n.py` & `protokolo-2.1.4/src/protokolo/i18n.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/src/protokolo/initialise.py` & `protokolo-2.1.4/src/protokolo/initialise.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/src/protokolo/replace.py` & `protokolo-2.1.4/src/protokolo/replace.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/src/protokolo/types.py` & `protokolo-2.1.4/src/protokolo/types.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/tests/conftest.py` & `protokolo-2.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/tests/test_cli.py` & `protokolo-2.1.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/tests/test_compile.py` & `protokolo-2.1.4/tests/test_compile.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/tests/test_config.py` & `protokolo-2.1.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/tests/test_exceptions.py` & `protokolo-2.1.4/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/tests/test_formatter.py` & `protokolo-2.1.4/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/tests/test_replace.py` & `protokolo-2.1.4/tests/test_replace.py`

 * *Files identical despite different names*

### Comparing `protokolo-2.1.3/PKG-INFO` & `protokolo-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protokolo
-Version: 2.1.3
+Version: 2.1.4
 Summary: Protokolo is a change log generator.
 Home-page: https://codeberg.org/carmenbianca/protokolo
 License: GPL-3.0-or-later
 Keywords: changelog,history,news
 Author: Carmen Bianca BAKKER
 Author-email: carmen@carmenbianca.eu
 Maintainer: Carmen Bianca BAKKER
```

