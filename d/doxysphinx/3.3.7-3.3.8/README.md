# Comparing `tmp/doxysphinx-3.3.7.tar.gz` & `tmp/doxysphinx-3.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doxysphinx-3.3.7.tar", max compression
+gzip compressed data, was "doxysphinx-3.3.8.tar", max compression
```

## Comparing `doxysphinx-3.3.7.tar` & `doxysphinx-3.3.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1078 2023-10-20 10:35:53.123446 doxysphinx-3.3.7/LICENSE.md
--rw-r--r--   0        0        0     2602 2023-10-20 10:35:53.123446 doxysphinx-3.3.7/README.md
--rw-r--r--   0        0        0      926 2023-10-20 10:35:53.139446 doxysphinx-3.3.7/doxysphinx/__init__.py
--rw-r--r--   0        0        0      608 2023-10-20 10:35:53.139446 doxysphinx-3.3.7/doxysphinx/__main__.py
--rw-r--r--   0        0        0     8173 2023-10-20 10:35:53.139446 doxysphinx-3.3.7/doxysphinx/cli.py
--rw-r--r--   0        0        0    13391 2023-10-20 10:35:53.139446 doxysphinx-3.3.7/doxysphinx/doxygen.py
--rw-r--r--   0        0        0    21996 2023-10-20 10:35:53.139446 doxysphinx-3.3.7/doxysphinx/html_parser.py
--rw-r--r--   0        0        0     9102 2023-10-20 10:35:53.139446 doxysphinx-3.3.7/doxysphinx/process.py
--rw-r--r--   0        0        0     5925 2023-10-20 10:35:53.139446 doxysphinx-3.3.7/doxysphinx/resources/custom.scss
--rw-r--r--   0        0        0        0 2023-10-20 10:35:53.139446 doxysphinx-3.3.7/doxysphinx/resources/toc_template.html.j2
--rw-r--r--   0        0        0    11663 2023-10-20 10:35:53.139446 doxysphinx-3.3.7/doxysphinx/resources.py
--rw-r--r--   0        0        0     2943 2023-10-20 10:35:53.139446 doxysphinx-3.3.7/doxysphinx/sphinx.py
--rw-r--r--   0        0        0    11504 2023-10-20 10:35:53.139446 doxysphinx-3.3.7/doxysphinx/toc.py
--rw-r--r--   0        0        0      527 2023-10-20 10:35:53.139446 doxysphinx-3.3.7/doxysphinx/utils/__init__.py
--rw-r--r--   0        0        0     2282 2023-10-20 10:35:53.139446 doxysphinx-3.3.7/doxysphinx/utils/contexts.py
--rw-r--r--   0        0        0     1156 2023-10-20 10:35:53.139446 doxysphinx-3.3.7/doxysphinx/utils/exceptions.py
--rw-r--r--   0        0        0     6235 2023-10-20 10:35:53.139446 doxysphinx-3.3.7/doxysphinx/utils/files.py
--rw-r--r--   0        0        0     1757 2023-10-20 10:35:53.139446 doxysphinx-3.3.7/doxysphinx/utils/iterators.py
--rw-r--r--   0        0        0     1431 2023-10-20 10:35:53.139446 doxysphinx-3.3.7/doxysphinx/utils/pathlib_fix.py
--rw-r--r--   0        0        0      924 2023-10-20 10:35:53.139446 doxysphinx-3.3.7/doxysphinx/utils/rst.py
--rw-r--r--   0        0        0    12187 2023-10-20 10:35:53.139446 doxysphinx-3.3.7/doxysphinx/writer.py
--rw-r--r--   0        0        0     4182 2023-10-20 10:35:53.143446 doxysphinx-3.3.7/pyproject.toml
--rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 doxysphinx-3.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-30 06:04:56.527233 doxysphinx-3.3.8/LICENSE.md
+-rw-r--r--   0        0        0     1440 2024-04-30 06:04:56.527233 doxysphinx-3.3.8/NOTICE.md
+-rw-r--r--   0        0        0     2602 2024-04-30 06:04:56.527233 doxysphinx-3.3.8/README.md
+-rw-r--r--   0        0        0      926 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/doxysphinx/__init__.py
+-rw-r--r--   0        0        0      608 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/doxysphinx/__main__.py
+-rw-r--r--   0        0        0     8173 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/doxysphinx/cli.py
+-rw-r--r--   0        0        0    13391 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/doxysphinx/doxygen.py
+-rw-r--r--   0        0        0    21996 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/doxysphinx/html_parser.py
+-rw-r--r--   0        0        0     9102 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/doxysphinx/process.py
+-rw-r--r--   0        0        0     5925 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/doxysphinx/resources/custom.scss
+-rw-r--r--   0        0        0        0 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/doxysphinx/resources/toc_template.html.j2
+-rw-r--r--   0        0        0    11663 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/doxysphinx/resources.py
+-rw-r--r--   0        0        0     2943 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/doxysphinx/sphinx.py
+-rw-r--r--   0        0        0    11504 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/doxysphinx/toc.py
+-rw-r--r--   0        0        0      527 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/doxysphinx/utils/__init__.py
+-rw-r--r--   0        0        0     2282 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/doxysphinx/utils/contexts.py
+-rw-r--r--   0        0        0     1156 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/doxysphinx/utils/exceptions.py
+-rw-r--r--   0        0        0     6235 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/doxysphinx/utils/files.py
+-rw-r--r--   0        0        0     1757 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/doxysphinx/utils/iterators.py
+-rw-r--r--   0        0        0     1431 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/doxysphinx/utils/pathlib_fix.py
+-rw-r--r--   0        0        0      924 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/doxysphinx/utils/rst.py
+-rw-r--r--   0        0        0    12187 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/doxysphinx/writer.py
+-rw-r--r--   0        0        0     4292 2024-04-30 06:04:56.543233 doxysphinx-3.3.8/pyproject.toml
+-rw-r--r--   0        0        0     4294 1970-01-01 00:00:00.000000 doxysphinx-3.3.8/PKG-INFO
```

### Comparing `doxysphinx-3.3.7/LICENSE.md` & `doxysphinx-3.3.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/README.md` & `doxysphinx-3.3.8/README.md`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/doxysphinx/__init__.py` & `doxysphinx-3.3.8/doxysphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/doxysphinx/__main__.py` & `doxysphinx-3.3.8/doxysphinx/__main__.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/doxysphinx/cli.py` & `doxysphinx-3.3.8/doxysphinx/cli.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/doxysphinx/doxygen.py` & `doxysphinx-3.3.8/doxysphinx/doxygen.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/doxysphinx/html_parser.py` & `doxysphinx-3.3.8/doxysphinx/html_parser.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/doxysphinx/process.py` & `doxysphinx-3.3.8/doxysphinx/process.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/doxysphinx/resources/custom.scss` & `doxysphinx-3.3.8/doxysphinx/resources/custom.scss`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/doxysphinx/resources.py` & `doxysphinx-3.3.8/doxysphinx/resources.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/doxysphinx/sphinx.py` & `doxysphinx-3.3.8/doxysphinx/sphinx.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/doxysphinx/toc.py` & `doxysphinx-3.3.8/doxysphinx/toc.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/doxysphinx/utils/__init__.py` & `doxysphinx-3.3.8/doxysphinx/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/doxysphinx/utils/contexts.py` & `doxysphinx-3.3.8/doxysphinx/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/doxysphinx/utils/exceptions.py` & `doxysphinx-3.3.8/doxysphinx/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/doxysphinx/utils/files.py` & `doxysphinx-3.3.8/doxysphinx/utils/files.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/doxysphinx/utils/iterators.py` & `doxysphinx-3.3.8/doxysphinx/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/doxysphinx/utils/pathlib_fix.py` & `doxysphinx-3.3.8/doxysphinx/utils/pathlib_fix.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/doxysphinx/utils/rst.py` & `doxysphinx-3.3.8/doxysphinx/utils/rst.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/doxysphinx/writer.py` & `doxysphinx-3.3.8/doxysphinx/writer.py`

 * *Files identical despite different names*

### Comparing `doxysphinx-3.3.7/pyproject.toml` & `doxysphinx-3.3.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ##
 ##  Author(s):
 ##  - Markus Braun, :em engineering methods AG (contracted by Robert Bosch GmbH)
 ## =====================================================================================
 
 [tool.poetry]
 name = "doxysphinx"
-version = "3.3.7"
+version = "3.3.8"
 description = "Integrates doxygen html documentation with sphinx."
 authors = [
     "Nirmal Sasidharan <nirmal.sasidharan@de.bosch.com>",
     "Markus Braun <markus.braun@em.ag>",
     "Aniket Salve <aniketdilip.salve@bosch.com>",
 ]
 maintainers = ["Nirmal Sasidharan <nirmal.sasidharan@de.bosch.com>"]
@@ -32,23 +32,24 @@
     "Topic :: Text Processing :: Markup :: reStructuredText",
     "Topic :: Documentation :: Sphinx",
     "Topic :: Documentation",
 ]
 packages = [{ include = "doxysphinx" }]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.9,<3.13"
 lxml = "^4.9.2"
 colorama = { version = "^0.4.6", platform = "windows" }
 click = "^8.1.3"
 click-log = "^0.4.0"
 pyparsing = "^3.0.9"
 mpire = "^2.6.0"
 pyjson5 = "^1.6.2"
 libsass = "^0.22.0"
+numpy = "^1.26.4"                                       # Adding this version of numpy to support python 3.12
 
 [tool.poetry.group.sphinx.dependencies]
 sphinx = "<7"
 pillow = "^10.0.1"
 sphinx-rtd-theme = "^1.3.0"
 sphinx-needs = "^1.3.0"
 sphinxcontrib-plantuml = "^0.26"
@@ -80,15 +81,15 @@
 commitizen = "^2.42.1"
 
 [tool.poetry.scripts]
 doxysphinx = "doxysphinx.cli:cli"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "3.3.7"
+version = "3.3.8"
 tag_format = "v$version"
 version_files = ["pyproject.toml:^version"]
 bump_message = """chore(release): release $current_version → $new_version by commitizen [skip-ci]
 
 Signed-off-by: github-actions <actions@github.com>
 """
```

### Comparing `doxysphinx-3.3.7/PKG-INFO` & `doxysphinx-3.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: doxysphinx
-Version: 3.3.7
+Version: 3.3.8
 Summary: Integrates doxygen html documentation with sphinx.
 Home-page: https://github.com/boschglobal/doxysphinx
 License: MIT
 Keywords: DaC,docs-as-code,doxygen,sphinx
 Author: Nirmal Sasidharan
 Author-email: nirmal.sasidharan@de.bosch.com
 Maintainer: Nirmal Sasidharan
 Maintainer-email: nirmal.sasidharan@de.bosch.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: Framework :: Sphinx :: Extension
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Pre-processors
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: reStructuredText
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-log (>=0.4.0,<0.5.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0) ; sys_platform == "windows"
 Requires-Dist: libsass (>=0.22.0,<0.23.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: mpire (>=2.6.0,<3.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pyjson5 (>=1.6.2,<2.0.0)
 Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
 Project-URL: Documentation, https://boschglobal.github.io/doxysphinx/
 Project-URL: Repository, https://github.com/boschglobal/doxysphinx
 Description-Content-Type: text/markdown
 
 <!--
```

