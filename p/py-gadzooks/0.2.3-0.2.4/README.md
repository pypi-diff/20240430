# Comparing `tmp/py_gadzooks-0.2.3.tar.gz` & `tmp/py_gadzooks-0.2.4.tar.gz`

## Comparing `py_gadzooks-0.2.3.tar` & `py_gadzooks-0.2.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 py_gadzooks-0.2.3/gadzooks/__init__.py
--rw-r--r--   0        0        0     7987 2020-02-02 00:00:00.000000 py_gadzooks-0.2.3/gadzooks/check_version.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 py_gadzooks-0.2.3/gadzooks/loc_summarize.py
--rwxr-xr-x   0        0        0     1122 2020-02-02 00:00:00.000000 py_gadzooks-0.2.3/gadzooks/main.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 py_gadzooks-0.2.3/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 py_gadzooks-0.2.3/LICENSE
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 py_gadzooks-0.2.3/README.md
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 py_gadzooks-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 py_gadzooks-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 py_gadzooks-0.2.4/gadzooks/__init__.py
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 py_gadzooks-0.2.4/gadzooks/build_docs.py
+-rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 py_gadzooks-0.2.4/gadzooks/check_version.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 py_gadzooks-0.2.4/gadzooks/loc_summarize.py
+-rwxr-xr-x   0        0        0     1385 2020-02-02 00:00:00.000000 py_gadzooks-0.2.4/gadzooks/main.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 py_gadzooks-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 py_gadzooks-0.2.4/LICENSE
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 py_gadzooks-0.2.4/README.md
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 py_gadzooks-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 py_gadzooks-0.2.4/PKG-INFO
```

### Comparing `py_gadzooks-0.2.3/gadzooks/__init__.py` & `py_gadzooks-0.2.4/gadzooks/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from argparse import ArgumentParser, Namespace
 import sys
-from typing import ClassVar
+from typing import ClassVar, Optional
 
 
-__version__ = '0.2.3'
+__version__ = '0.2.4'
 
 
 def error(msg: str) -> None:
     """Prints an error message and exits the program with return code 1."""
     print(f'ERROR: {msg}', file=sys.stderr)
     sys.exit(1)
 
@@ -20,9 +20,9 @@
     """Configures a subcommand for the main executable."""
 
     @classmethod
     def configure_parser(cls, parser: ArgumentParser) -> None:
         """Configures an argument parser."""
 
     @classmethod
-    def main(cls, args: Namespace) -> None:
+    def main(cls, args: Namespace, extra_args: Optional[list[str]] = None) -> None:
         """Runs the main logic of the subcommand, given parsed arguments."""
```

### Comparing `py_gadzooks-0.2.3/gadzooks/check_version.py` & `py_gadzooks-0.2.4/gadzooks/check_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,31 +34,31 @@
             return (tag, 0)
         # otherwise, string contains number of commits past the tag
         assert full_tag.startswith(tag)
         n = int(full_tag.removeprefix(tag).lstrip('-').split('-')[0])
         return (tag, n)
     return None
 
-def check_tag_version() -> Optional[tuple[str, int]]:
+def check_tag_version() -> Optional[str]:
     """Checks that the latest tag is a valid version (for now, other tags are not allowed).
-    Returns the version as a string, or None if there is no tag."""
+    If a valid tag exists, returns the version; otherwise, issues a warning and returns None."""
     result = get_latest_tag()
     if result:
         (latest_tag, n) = result
         if n == 0:
             msg = 'current commit'
         elif n == 1:
             msg = '1 commit ago'
         else:
             msg = f'{n} commits ago'
         print(f'Latest tag:           {latest_tag} ({msg})')
         tag_version = latest_tag.lstrip('v')
         if VERSION_REGEX.match(tag_version):
             print(f'Tag version:          {tag_version}')
-            return (tag_version, n)
+            return tag_version
         warning(f'tag {latest_tag!r} is not a valid version')
     else:
         warning('no tags exist')
     return None
 
 def get_pkg_version(path: Path) -> Optional[str]:
     """Finds the first occurrence of a version string in the given file.
@@ -68,15 +68,14 @@
     regex = re.compile(r'\_*version\_*\s*=\s*[\'\"]?(' + VERSION_PATTERN + ')')
     if (match := regex.search(contents)):
         return match.group(1)
     return None
 
 def check_pkg_version(version_path: Path) -> str:
     """Checks that the version of the Python package is a valid version string.
-    If check_tag=True, also requires this version to match the tag version.
     Returns the package version."""
     pkg_version = get_pkg_version(version_path)
     if pkg_version is None:
         error(f'no package version found in {version_path}')
     assert isinstance(pkg_version, str)
     print(f'Package version:      {pkg_version}')
     if not VERSION_REGEX.match(pkg_version):
@@ -131,43 +130,38 @@
     if has_pattern:
         print(f'Changelog line:       {line}')
     elif strict:
         error(f'{changelog} may not be up-to-date, does not contain a line matching:\n\t{pattern}')
 
 
 class CheckVersion(Subcommand):
-    """check version consistency in a Python project"""
+    """check version consistency"""
 
     @classmethod
     def configure_parser(cls, parser: ArgumentParser) -> None:
         parser.add_argument('--pkg-name', help='name of the Python package')
         parser.add_argument('--dist-name', help='name of the PyPI distribution')
         parser.add_argument('--version-path', type=Path, help='path to file containing current version')
+        parser.add_argument('--check-tag', action='store_true', help='check that the latest tag is a valid version')
         parser.add_argument('--check-dist', action='store_true', help='check version of latest built wheel')
         parser.add_argument('--dist-dir', help='directory where package wheels are built')
         parser.add_argument('--changelog', help='changelog file')
         parser.add_argument('--changelog-version-regex', default='{version}', help='pattern to match to find version in changelog file ("{version}" within the pattern marks the target version')
 
     @classmethod
-    def main(cls, args: Namespace) -> None:
+    def main(cls, args: Namespace, extra_args: Optional[list[str]] = None) -> None:
         # by default, assume root directory name matches the package name
         pkg_name = args.pkg_name or Path.cwd().name.replace('-', '_')
         # by default, assume the package directory is a subdirectory with the package name
         version_path = args.version_path or Path(pkg_name) / '__init__.py'
         pkg_version = check_pkg_version(version_path)
-        result = check_tag_version()
-        if result is None:
-            tag_version = None
-            tag_is_current = False
-        else:
-            (tag_version, n) = result
-            tag_is_current = (n == 0)
-        if tag_is_current:
+        tag_version = check_tag_version()
+        if args.check_tag:
             check_pkg_tag_consistency(pkg_version, tag_version)
         if args.check_dist or args.dist_dir:
             dist_dir = args.dist_dir or 'dist'
             dist_name = args.dist_name or pkg_name
             built_version = show_latest_built_version(dist_name, dist_dir)
             if tag_version:
                 check_built_tag_consistency(built_version, tag_version, dist_dir)
         if args.changelog:
-            check_changelog_version(pkg_version, args.changelog, args.changelog_version_regex, strict=tag_is_current)
+            check_changelog_version(pkg_version, args.changelog, args.changelog_version_regex, strict=args.check_tag)
```

### Comparing `py_gadzooks-0.2.3/gadzooks/loc_summarize.py` & `py_gadzooks-0.2.4/gadzooks/loc_summarize.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from argparse import ArgumentParser, Namespace
 import glob
 import itertools
 import subprocess
+from typing import Optional
 
 from gadzooks import Subcommand
 
 
 class LinesOfCodeSummarize(Subcommand):
-    """summarize lines of code in a Python project"""
+    """summarize lines of code"""
 
     @classmethod
     def configure_parser(cls, parser: ArgumentParser) -> None:
         parser.add_argument('source_files', nargs='*', help='Python files to check')
 
     @classmethod
-    def main(cls, args: Namespace) -> None:
+    def main(cls, args: Namespace, extra_args: Optional[list] = None) -> None:
         paths = list(itertools.chain.from_iterable(map(glob.glob, args.source_files)))
         if not paths:
             print('No source files to check')
             return
         cmd = ['radon', 'raw'] + list(paths) + ['-s']
         lines = subprocess.check_output(cmd, text=True).splitlines()
         num_files = sum(not line.startswith(' ') for line in lines) - 1
```

### Comparing `py_gadzooks-0.2.3/LICENSE` & `py_gadzooks-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.3/README.md` & `py_gadzooks-0.2.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 
 A collection of code maintenance tools for Python projects. These are especially useful as [pre-commit](https://pre-commit.com) hooks.
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
-    - [Check version consistency](#check-version)
     - [Lines of code summary](#loc-summarize)
+    - [Check version consistency](#check-version)
+    - [Build documentation](#build-docs)
 
 ## Installation
 
 ```text
 pip install py-gadzooks
 ```
 
@@ -28,23 +29,52 @@
 
 Once installed, `gadzooks` will be available as a command-line executable.
 
 Different tools can be called as subcommands, which are as follows:
 
 | Subcommand | Description |
 | ---------- | ----------- |
+| `build-docs` | Build project documentation |
 | `check-version` | Check version consistency |
 | `loc-summarize` | Summarize lines of code |
 
 To view the help and options for a particular subcommand, do:
 
 ```text
 gadzooks <SUBCOMMAND> --help
 ```
 
+### `loc-summarize`
+
+Computes various lines-of-code metrics such as LOC (lines of code), LLOC (logical lines of code), and SLOC (source lines of code). Uses the [`radon`](https://radon.readthedocs.io/en/latest/) tool to do this.
+
+The input argument is a path or list of paths to look for Python source files.
+
+Example:
+
+```text
+gadzooks loc-summarize .
+```
+
+Output:
+
+```text
+Checked 4 source file(s)
+
+LINE STATS
+----------
+LOC:             244
+LLOC:            198
+SLOC:            182
+Comments:          6
+Single comments:  15
+Multi:            10
+Blank:            37
+```
+
 ### `check-version`
 
 Versions may appear in multiple locations within a project, including:
 
 - A source file such as `__init__.py` or `__version__.py`
 - Git tag
 - Locally built wheels
@@ -58,46 +88,38 @@
 A valid Git tag may be a version string, optionally prefixed with `v`, for example, `v3.7.1`.
 
 | Option | Description | Default |
 | ------ | ----------- | ------- |
 | `--pkg-name PKG_NAME` | Name of package | Current directory |
 | `--dist-name DIST_NAME` | Name of PyPI distribution | `<PKG_NAME>` |
 | `--version-path VERSION_PATH` | Path to file where package version is defined | `<PKG_NAME>/__init__.py` |
+| `--check-tag` | Check that latest tag is valid | |
 | `--check-dist` | Check version of latest built wheel | |
 | `--dist-dir DIST_DIR` | Directory where wheels are built | `dist` |
 | `--changelog CHANGELOG` | Changelog file | |
 | `--changelog-version-regex` | Pattern to match to find version in changelog file (`{version}` within the pattern marks the target version) | `{version}` |
 
-### `loc-summarize`
+### `build-docs`
 
-Computes various lines-of-code metrics such as LOC (lines of code), LLOC (logical lines of code), and SLOC (source lines of code). Uses the [`radon`](https://radon.readthedocs.io/en/latest/) tool to do this.
+Runs a command to build docs within your project.
 
-The input argument is a path or list of paths to look for Python source files.
+A typical pattern is to build documentation from template files such as Markdown, then save them out as HTML. Often this is done external to source control via some CI process which builds and deploys docs to a website. However, in some cases you may want to commit the built documentation to your Git repo. This is an easy step to forget, so `gadzooks` let you make the action into a `pre-commit` hook.
 
-Example:
+Example usage:
 
 ```text
-gadzooks loc-summarize .
+gadzooks build-docs --src-docs docs -- make docs
 ```
 
-Output:
-
-```text
-Checked 4 source file(s)
+The `--src-docs` option lets you specify which files are the source docs to be built. `gadzooks` will first check if any of these files has changed since the last time the docs were built (by means of a saved checksum file). If none has changed, it will do nothing. Otherwise, it will call the command following the final `--` (in the example above, `make docs`).
 
-LINE STATS
-----------
-LOC:             244
-LLOC:            198
-SLOC:            182
-Comments:          6
-Single comments:  15
-Multi:            10
-Blank:            37
-```
+| Option | Description | Default |
+| ------ | ----------- | ------- |
+| `--src-docs SRC_DOCS` | Files or directories containing source docs |  |
+| `--checksum-file CHECKSUM_FILE` | File where SHA-1 checksum is stored | `.doc-checksum` |
 
 ## Pre-commit hooks
 
 You can set up individual `gadzooks` subcommands to run as [pre-commit](https://pre-commit.com) hooks by configuring your `.pre-commit-config.yaml` file to point to this [Github repo](https://github.com/jeremander/gadzooks), specifying your desired subcommand by `id`, along with the command-line arguments.
 
 You should also set `pass_filenames` to `false` to avoid passing filenames as command-line arguments by default, and `verbose` to `true` so that `gadzooks` output will be visible.
 
@@ -107,17 +129,18 @@
 - repo: https://github.com/jeremander/gadzooks
   rev: v0.2.0
   hooks:
     - id: loc-summarize
       args: ['.']
       pass_filenames: false
       verbose: true
+      # before pushing, require the git tag match the package version
     - id: check-version
-      args: []
+      args: ['--check-tag']
       pass_filenames: false
       verbose: true
-      stages: [commit, push]
+      stages: [push]
 ```
 
 ## License
 
 `gadzooks` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `py_gadzooks-0.2.3/pyproject.toml` & `py_gadzooks-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.3/PKG-INFO` & `py_gadzooks-0.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: py-gadzooks
-Version: 0.2.3
+Version: 0.2.4
 Summary: A collection of code maintenance tools for Python projects, intended to be used within git hooks.
 Project-URL: Documentation, https://github.com/jeremander/gadzooks#readme
 Project-URL: Issues, https://github.com/jeremander/gadzooks/issues
 Project-URL: Source, https://github.com/jeremander/gadzooks
 Author-email: Jeremy Silver <jeremys@nessiness.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -24,16 +24,17 @@
 
 A collection of code maintenance tools for Python projects. These are especially useful as [pre-commit](https://pre-commit.com) hooks.
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
-    - [Check version consistency](#check-version)
     - [Lines of code summary](#loc-summarize)
+    - [Check version consistency](#check-version)
+    - [Build documentation](#build-docs)
 
 ## Installation
 
 ```text
 pip install py-gadzooks
 ```
 
@@ -43,23 +44,52 @@
 
 Once installed, `gadzooks` will be available as a command-line executable.
 
 Different tools can be called as subcommands, which are as follows:
 
 | Subcommand | Description |
 | ---------- | ----------- |
+| `build-docs` | Build project documentation |
 | `check-version` | Check version consistency |
 | `loc-summarize` | Summarize lines of code |
 
 To view the help and options for a particular subcommand, do:
 
 ```text
 gadzooks <SUBCOMMAND> --help
 ```
 
+### `loc-summarize`
+
+Computes various lines-of-code metrics such as LOC (lines of code), LLOC (logical lines of code), and SLOC (source lines of code). Uses the [`radon`](https://radon.readthedocs.io/en/latest/) tool to do this.
+
+The input argument is a path or list of paths to look for Python source files.
+
+Example:
+
+```text
+gadzooks loc-summarize .
+```
+
+Output:
+
+```text
+Checked 4 source file(s)
+
+LINE STATS
+----------
+LOC:             244
+LLOC:            198
+SLOC:            182
+Comments:          6
+Single comments:  15
+Multi:            10
+Blank:            37
+```
+
 ### `check-version`
 
 Versions may appear in multiple locations within a project, including:
 
 - A source file such as `__init__.py` or `__version__.py`
 - Git tag
 - Locally built wheels
@@ -73,46 +103,38 @@
 A valid Git tag may be a version string, optionally prefixed with `v`, for example, `v3.7.1`.
 
 | Option | Description | Default |
 | ------ | ----------- | ------- |
 | `--pkg-name PKG_NAME` | Name of package | Current directory |
 | `--dist-name DIST_NAME` | Name of PyPI distribution | `<PKG_NAME>` |
 | `--version-path VERSION_PATH` | Path to file where package version is defined | `<PKG_NAME>/__init__.py` |
+| `--check-tag` | Check that latest tag is valid | |
 | `--check-dist` | Check version of latest built wheel | |
 | `--dist-dir DIST_DIR` | Directory where wheels are built | `dist` |
 | `--changelog CHANGELOG` | Changelog file | |
 | `--changelog-version-regex` | Pattern to match to find version in changelog file (`{version}` within the pattern marks the target version) | `{version}` |
 
-### `loc-summarize`
+### `build-docs`
 
-Computes various lines-of-code metrics such as LOC (lines of code), LLOC (logical lines of code), and SLOC (source lines of code). Uses the [`radon`](https://radon.readthedocs.io/en/latest/) tool to do this.
+Runs a command to build docs within your project.
 
-The input argument is a path or list of paths to look for Python source files.
+A typical pattern is to build documentation from template files such as Markdown, then save them out as HTML. Often this is done external to source control via some CI process which builds and deploys docs to a website. However, in some cases you may want to commit the built documentation to your Git repo. This is an easy step to forget, so `gadzooks` let you make the action into a `pre-commit` hook.
 
-Example:
+Example usage:
 
 ```text
-gadzooks loc-summarize .
+gadzooks build-docs --src-docs docs -- make docs
 ```
 
-Output:
-
-```text
-Checked 4 source file(s)
+The `--src-docs` option lets you specify which files are the source docs to be built. `gadzooks` will first check if any of these files has changed since the last time the docs were built (by means of a saved checksum file). If none has changed, it will do nothing. Otherwise, it will call the command following the final `--` (in the example above, `make docs`).
 
-LINE STATS
-----------
-LOC:             244
-LLOC:            198
-SLOC:            182
-Comments:          6
-Single comments:  15
-Multi:            10
-Blank:            37
-```
+| Option | Description | Default |
+| ------ | ----------- | ------- |
+| `--src-docs SRC_DOCS` | Files or directories containing source docs |  |
+| `--checksum-file CHECKSUM_FILE` | File where SHA-1 checksum is stored | `.doc-checksum` |
 
 ## Pre-commit hooks
 
 You can set up individual `gadzooks` subcommands to run as [pre-commit](https://pre-commit.com) hooks by configuring your `.pre-commit-config.yaml` file to point to this [Github repo](https://github.com/jeremander/gadzooks), specifying your desired subcommand by `id`, along with the command-line arguments.
 
 You should also set `pass_filenames` to `false` to avoid passing filenames as command-line arguments by default, and `verbose` to `true` so that `gadzooks` output will be visible.
 
@@ -122,17 +144,18 @@
 - repo: https://github.com/jeremander/gadzooks
   rev: v0.2.0
   hooks:
     - id: loc-summarize
       args: ['.']
       pass_filenames: false
       verbose: true
+      # before pushing, require the git tag match the package version
     - id: check-version
-      args: []
+      args: ['--check-tag']
       pass_filenames: false
       verbose: true
-      stages: [commit, push]
+      stages: [push]
 ```
 
 ## License
 
 `gadzooks` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

