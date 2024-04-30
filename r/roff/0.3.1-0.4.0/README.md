# Comparing `tmp/roff-0.3.1.tar.gz` & `tmp/roff-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roff-0.3.1.tar", last modified: Mon Apr 29 10:45:35 2024, max compression
+gzip compressed data, was "roff-0.4.0.tar", last modified: Tue Apr 30 13:55:41 2024, max compression
```

## Comparing `roff-0.3.1.tar` & `roff-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-29 10:45:35.169957 roff-0.3.1/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1072 2024-04-21 09:37:21.000000 roff-0.3.1/LICENSE
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3370 2024-04-29 10:45:35.169957 roff-0.3.1/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1673 2024-04-28 12:23:56.000000 roff-0.3.1/README.md
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-29 10:45:35.169957 roff-0.3.1/docs/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1645 2024-04-29 10:43:42.000000 roff-0.3.1/docs/roff.1
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2857 2024-04-29 10:43:48.000000 roff-0.3.1/docs/roff.5
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2024-04-21 09:38:29.000000 roff-0.3.1/pyproject.toml
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2024-04-29 10:45:35.169957 roff-0.3.1/setup.cfg
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2155 2024-04-25 15:15:31.000000 roff-0.3.1/setup.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-29 10:45:35.169957 roff-0.3.1/src/
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-29 10:45:35.169957 roff-0.3.1/src/roff/
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-29 10:45:35.169957 roff-0.3.1/src/roff/__cli__/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      104 2024-04-23 17:04:15.000000 roff-0.3.1/src/roff/__cli__/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      446 2024-04-25 15:15:31.000000 roff-0.3.1/src/roff/__cli__/convert.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1036 2024-04-27 11:45:13.000000 roff-0.3.1/src/roff/__cli__/template.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      713 2024-04-23 17:04:15.000000 roff-0.3.1/src/roff/__cli__/util.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1508 2024-04-29 10:43:13.000000 roff-0.3.1/src/roff/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1601 2024-04-23 20:27:06.000000 roff-0.3.1/src/roff/__main__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2641 2024-04-25 15:15:31.000000 roff-0.3.1/src/roff/_images.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2303 2024-04-27 11:04:01.000000 roff-0.3.1/src/roff/_markdown.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      213 2024-04-26 19:43:17.000000 roff-0.3.1/src/roff/_util.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)    11069 2024-04-29 10:42:32.000000 roff-0.3.1/src/roff/convert.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-29 10:45:35.169957 roff-0.3.1/src/roff.egg-info/
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3370 2024-04-29 10:45:35.000000 roff-0.3.1/src/roff.egg-info/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      492 2024-04-29 10:45:35.000000 roff-0.3.1/src/roff.egg-info/SOURCES.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2024-04-29 10:45:35.000000 roff-0.3.1/src/roff.egg-info/dependency_links.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       44 2024-04-29 10:45:35.000000 roff-0.3.1/src/roff.egg-info/entry_points.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       94 2024-04-29 10:45:35.000000 roff-0.3.1/src/roff.egg-info/requires.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        5 2024-04-29 10:45:35.000000 roff-0.3.1/src/roff.egg-info/top_level.txt
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-30 13:55:41.570971 roff-0.4.0/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1072 2024-04-23 10:39:23.000000 roff-0.4.0/LICENSE
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3370 2024-04-30 13:55:41.570971 roff-0.4.0/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1673 2024-04-30 12:20:39.000000 roff-0.4.0/README.md
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-30 13:55:41.566971 roff-0.4.0/docs/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1755 2024-04-27 11:59:02.000000 roff-0.4.0/docs/roff.1
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2948 2024-04-30 13:51:21.000000 roff-0.4.0/docs/roff.5
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2024-04-23 10:39:23.000000 roff-0.4.0/pyproject.toml
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2024-04-30 13:55:41.570971 roff-0.4.0/setup.cfg
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2155 2024-04-25 12:26:07.000000 roff-0.4.0/setup.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-30 13:55:41.566971 roff-0.4.0/src/
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-30 13:55:41.566971 roff-0.4.0/src/roff/
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-30 13:55:41.570971 roff-0.4.0/src/roff/__cli__/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      114 2024-04-30 13:02:33.000000 roff-0.4.0/src/roff/__cli__/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      446 2024-04-25 12:31:14.000000 roff-0.4.0/src/roff/__cli__/convert.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1036 2024-04-27 11:58:51.000000 roff-0.4.0/src/roff/__cli__/template.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      403 2024-04-30 13:06:47.000000 roff-0.4.0/src/roff/__cli__/tree.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      747 2024-04-30 13:14:13.000000 roff-0.4.0/src/roff/__cli__/util.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1508 2024-04-30 13:54:58.000000 roff-0.4.0/src/roff/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2112 2024-04-30 13:13:29.000000 roff-0.4.0/src/roff/__main__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2641 2024-04-25 14:11:43.000000 roff-0.4.0/src/roff/_images.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2303 2024-04-27 11:58:51.000000 roff-0.4.0/src/roff/_markdown.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      853 2024-04-30 13:53:23.000000 roff-0.4.0/src/roff/_util.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)    10969 2024-04-30 13:04:33.000000 roff-0.4.0/src/roff/convert.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-30 13:55:41.570971 roff-0.4.0/src/roff.egg-info/
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3370 2024-04-30 13:55:41.000000 roff-0.4.0/src/roff.egg-info/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      517 2024-04-30 13:55:41.000000 roff-0.4.0/src/roff.egg-info/SOURCES.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2024-04-30 13:55:41.000000 roff-0.4.0/src/roff.egg-info/dependency_links.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       44 2024-04-30 13:55:41.000000 roff-0.4.0/src/roff.egg-info/entry_points.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       94 2024-04-30 13:55:41.000000 roff-0.4.0/src/roff.egg-info/requires.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        5 2024-04-30 13:55:41.000000 roff-0.4.0/src/roff.egg-info/top_level.txt
```

### Comparing `roff-0.3.1/LICENSE` & `roff-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `roff-0.3.1/PKG-INFO` & `roff-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roff
-Version: 0.3.1
+Version: 0.4.0
 Summary: python-based cli to convert markdown to the roff (man-pages) format
 Home-page: https://github.com/utility-toolbox/roff
 Author: PlayerG9
 License: MIT
 Project-URL: Organisation Github, https://github.com/utility-toolbox
 Project-URL: Homepage, https://github.com/utility-toolbox/roff/
 Project-URL: Bug Tracker, https://github.com/utility-toolbox/roff/issues
```

### Comparing `roff-0.3.1/README.md` & `roff-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `roff-0.3.1/docs/roff.5` & `roff-0.4.0/docs/roff.5`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 .\" generated with roff/v0.3.1
 .\" https://pypi.org/project/roff/0.3.1
 .\" https://github.com/utility-toolbox/roff/
 .\"
-.TH "ROFF" "5" "29 April 2024" "github.com/utility-toolbox/roff"
+.TH "ROFF" "5" "30 April 2024" "github.com/utility-toolbox/roff"
 .SH "NAME"
-\fBroff\fP • python-based cli to convert markdown to the roff (man-pages) format
+\fBroff\fP • python\[em]based cli to convert markdown to the roff (man\[em]pages) format
 .SH "DESCRIPTION"
-see roff(1) for more information about the CLI\.
-This document is about the \.md file-specification
+see roff(1) for more information about the CLI.
+This document is about the .md file\[em]specification
 .sp
 .RS 2
-Use \fBroff\fP \fItemplate\fP \fIcommand\fP.\fI1\fP.\fImd\fP to get a template as a starting point\.
+Use \fBroff\fP \fItemplate\fP \fIcommand\fP.\fI1\fP.\fImd\fP to get a template as a starting point.
 .RE
 .sp
+\fBhello\fP \fB\-\-key\fP \fI\[dq]value\\\[dq]\fP\fIworth\fP" \fIstuff\fP
 .SH "FILES"
-Input files should follow the naming convention of \fI[command].[area].md\fP (e\.g\. \fIroff.1.md\fP)
-Output files should follow the naming convention of \fI[command].[area]\fP (e\.g\. \fIroff.1\fP)
+Input files should follow the naming convention of \fI[command].[area].md\fP (e.g. \fIroff.1.md\fP)
+Output files should follow the naming convention of \fI[command].[area]\fP (e.g. \fIroff.1\fP)
 .SH "ELEMENTS"
 .SS "Document Head"
 The Document head should have the following structure and is required in the document
 .sp
 .RS 2
 .EX
 \fI
@@ -116,15 +117,15 @@
 \fI
 .br
 > You can simply add blockquotes by starting a line with `>`
 \fP
 .EE
 .RE
 .sp
-.SS "Code-Blocks"
+.SS "Code\[em]Blocks"
 .sp
 .RS 2
 .EX
 \fI
 .br
 ```
 .br
@@ -211,15 +212,15 @@
 .br
 shows a help message and exists
 \fP
 .EE
 .RE
 .sp
 .SH "BUGS"
-https://github\.com/utility-toolbox/roff/issues
+https://github.com/utility\[em]toolbox/roff/issues
 .SH "AUTHOR"
-https://github\.com/PlayerG9
+https://github.com/PlayerG9
 .SH "SEE ALSO"
 .SS "Organisation"
-https://github\.com/utility-toolbox
+https://github.com/utility\[em]toolbox
 .SS "Repository"
-https://github\.com/utility-toolbox/roff
+https://github.com/utility\[em]toolbox/roff
```

### Comparing `roff-0.3.1/setup.py` & `roff-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `roff-0.3.1/src/roff/__cli__/template.py` & `roff-0.4.0/src/roff/__cli__/template.py`

 * *Files identical despite different names*

### Comparing `roff-0.3.1/src/roff/__cli__/util.py` & `roff-0.4.0/src/roff/__cli__/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 
 class ActionListManpageAreas(ap.Action):
     def __init__(self, option_strings, dest, help=None, metavar=None):
         super().__init__(option_strings=option_strings, nargs=0, help=help, metavar=metavar,
                          dest=ap.SUPPRESS, default=ap.SUPPRESS)
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, parser: ap.ArgumentParser, *args, **kwargs):
         print("1. general commands")
         print("2. system calls")
         print("3. library functions")
         print("4. special files")
         print("5. file formats and conventions")
         print("6. games and screensavers")
         print("7. miscellanea")
         print("8. system administration commands and daemons")
-        exit(0)
+        parser.exit(0)
```

### Comparing `roff-0.3.1/src/roff/__init__.py` & `roff-0.4.0/src/roff/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 __copyright__ = "Copyright 2024, utility-toolbox"
 __credits__ = ["PlayerG9"]
 __license__ = "MIT"
 __maintainer__ = "PlayerG9"
 __email__ = None
 __status__ = "Prototype"  # Prototype, Development, Production
 __description__ = "python-based cli to convert markdown to the roff (man-pages) format"
-__version_info__ = (0, 3, 1)
+__version_info__ = (0, 4, 0)
 __version__ = '.'.join(str(_) for _ in __version_info__)
```

### Comparing `roff-0.3.1/src/roff/__main__.py` & `roff-0.4.0/src/roff/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from . import __version__, __cli__
 
 
 parser = ap.ArgumentParser(prog='roff', formatter_class=ap.ArgumentDefaultsHelpFormatter, description=__doc__)
 parser.set_defaults(__cmd__=parser.print_help)
 parser.add_argument('-v', '--version', action='version', version='{}'.format(__version__))
 parser.add_argument('--list-areas', action=__cli__.util.ActionListManpageAreas,
-                    help="Lists the manpage-areas")
+                    help="Lists the manpage-areas and exit")
 subparsers = parser.add_subparsers()
 
 
 convert_parser = subparsers.add_parser('convert',
                                        help="Converts markdown files to roff files")
 convert_parser.set_defaults(__cmd__=__cli__.convert.__cmd__)
 convert_parser.add_argument('source',
@@ -28,14 +28,24 @@
 template_parser.set_defaults(__cmd__=__cli__.template.__cmd__)
 template_parser.add_argument('-y', '--yes', action='store_true',
                              help="Overwrite file if it exists")
 template_parser.add_argument('dest',
                              help="Target file that should be generated")
 
 
+tree_parser = subparsers.add_parser('tree',
+                                    help="Shows the parsed tree-structure of a markdown document."
+                                         " (For debugging purposes)")
+tree_parser.set_defaults(__cmd__=__cli__.tree.__cmd__)
+tree_parser.add_argument('--show-text', action=ap.BooleanOptionalAction,
+                         help="Show text in the tree")
+tree_parser.add_argument('source',
+                         help="Markdown file that should be parsed")
+
+
 def main():
     args = vars(parser.parse_args())
     cmd = args.pop('__cmd__')
     cmd(**args)
 
 
 if __name__ == '__main__':
```

### Comparing `roff-0.3.1/src/roff/_images.py` & `roff-0.4.0/src/roff/_images.py`

 * *Files identical despite different names*

### Comparing `roff-0.3.1/src/roff/_markdown.py` & `roff-0.4.0/src/roff/_markdown.py`

 * *Files identical despite different names*

### Comparing `roff-0.3.1/src/roff/convert.py` & `roff-0.4.0/src/roff/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import warnings
 import typing as t
 from pathlib import Path
 import markdown_it.tree
 from . import __version__
 from ._util import *
 from ._images import render_image
-from ._markdown import markdown_plugin_command
 
 
 __all__ = ['convert', 'Converter']
 
 
 def convert(fp: t.Union[str, os.PathLike]) -> str:
     r"""
@@ -43,16 +42,15 @@
         self._stream = io.StringIO()
         self._had_head = False
         self._fp = Path(fp).absolute()
         self._root = self._fp.parent
 
         self.manpage_area = 1  # default. should be overwritten while parsing
 
-        parser = markdown_it.MarkdownIt()
-        parser.use(markdown_plugin_command)
+        parser = get_parser()
 
         with open(self._fp, 'r') as file:
             source = file.read()
 
         tokens = parser.parse(src=source)
         root_node = markdown_it.tree.SyntaxTreeNode(tokens=tokens, create_root=True)
 
@@ -139,18 +137,18 @@
                     return f'[\\fB{escape(argkey)}\\fP]'
             argument = match.group()
             if argument.startswith("-"):
                 return f'\\fB{escape(argument)}\\fP'
             else:
                 return f'\\fI{escape(argument)}\\fP'
 
-        patterns_re = re.compile(r'^(?P<head>\w[\w-]*)'  # ^command
-                                 r'|\[(?P<argkey>--?\w[\w-]*)(?: (?P<argvalue>\w[\w-]*))?]'  # [--key value]
+        patterns_re = re.compile(r'^(?P<head>\w[\w\-]*)'  # ^command
+                                 r'|\[(?P<argkey>--?\w[\w-]*)(?: (?P<argvalue>\w[\w\-]*))?]'  # [--key value]
                                  r'|(?P<quote>[\"\']).*?(?P=quote)'  # "longer text's"
-                                 r'|(-{0,2}\w[\w-]*)')  # other stuff
+                                 r'|(-{0,2}\w[\w\-]*)')  # other stuff
 
         return patterns_re.sub(repl, command)
 
     def _parse_h1(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
         from datetime import date
 
         if self._had_head:
```

### Comparing `roff-0.3.1/src/roff.egg-info/PKG-INFO` & `roff-0.4.0/src/roff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roff
-Version: 0.3.1
+Version: 0.4.0
 Summary: python-based cli to convert markdown to the roff (man-pages) format
 Home-page: https://github.com/utility-toolbox/roff
 Author: PlayerG9
 License: MIT
 Project-URL: Organisation Github, https://github.com/utility-toolbox
 Project-URL: Homepage, https://github.com/utility-toolbox/roff/
 Project-URL: Bug Tracker, https://github.com/utility-toolbox/roff/issues
```

