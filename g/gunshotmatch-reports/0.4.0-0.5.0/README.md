# Comparing `tmp/gunshotmatch_reports-0.4.0.tar.gz` & `tmp/gunshotmatch_reports-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gunshotmatch_reports-0.4.0.tar", last modified: Thu Feb 15 13:47:55 2024, max compression
+gzip compressed data, was "gunshotmatch_reports-0.5.0.tar", last modified: Tue Apr 30 14:35:11 2024, max compression
```

## Comparing `gunshotmatch_reports-0.4.0.tar` & `gunshotmatch_reports-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-02-15 13:47:55.411838 gunshotmatch_reports-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-02-15 13:47:55.419838 gunshotmatch_reports-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-02-15 13:47:55.415838 gunshotmatch_reports-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-15 13:47:55.415838 gunshotmatch_reports-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-02-15 13:47:55.419838 gunshotmatch_reports-0.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-02-15 13:47:27.419857 gunshotmatch_reports-0.4.0/gunshotmatch_reports/chromatogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-02-15 13:47:27.419857 gunshotmatch_reports-0.4.0/gunshotmatch_reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-02-15 13:47:27.419857 gunshotmatch_reports-0.4.0/gunshotmatch_reports/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-02-15 13:47:27.419857 gunshotmatch_reports-0.4.0/gunshotmatch_reports/peaks.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 13:47:27.419857 gunshotmatch_reports-0.4.0/gunshotmatch_reports/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-30 14:35:11.768609 gunshotmatch_reports-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-30 14:35:11.772609 gunshotmatch_reports-0.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-04-30 14:35:11.772609 gunshotmatch_reports-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-30 14:35:11.772609 gunshotmatch_reports-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-30 14:35:11.772609 gunshotmatch_reports-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-30 14:34:46.620318 gunshotmatch_reports-0.5.0/gunshotmatch_reports/chromatogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-30 14:34:46.620318 gunshotmatch_reports-0.5.0/gunshotmatch_reports/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-30 14:34:46.620318 gunshotmatch_reports-0.5.0/gunshotmatch_reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:34:46.620318 gunshotmatch_reports-0.5.0/gunshotmatch_reports/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-30 14:34:46.620318 gunshotmatch_reports-0.5.0/gunshotmatch_reports/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-04-30 14:34:46.620318 gunshotmatch_reports-0.5.0/gunshotmatch_reports/peaks.py
```

### Comparing `gunshotmatch_reports-0.4.0/LICENSE` & `gunshotmatch_reports-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gunshotmatch_reports-0.4.0/PKG-INFO` & `gunshotmatch_reports-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.2
 Name: gunshotmatch-reports
-Version: 0.4.0
+Version: 0.5.0
 Summary: PDF Report Generation for GunShotMatch.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Home-page: https://github.com/GunShotMatch/gunshotmatch-reports
 Project-URL: Issue Tracker, https://github.com/GunShotMatch/gunshotmatch-reports/issues
 Project-URL: Source Code, https://github.com/GunShotMatch/gunshotmatch-reports
 Project-URL: Documentation, https://gunshotmatch-reports.readthedocs.io/en/latest
@@ -117,15 +117,15 @@
 .. |license| image:: https://img.shields.io/github/license/GunShotMatch/gunshotmatch-reports
 	:target: https://github.com/GunShotMatch/gunshotmatch-reports/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/GunShotMatch/gunshotmatch-reports
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-reports/v0.4.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-reports/v0.5.0
 	:target: https://github.com/GunShotMatch/gunshotmatch-reports/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/GunShotMatch/gunshotmatch-reports
 	:target: https://github.com/GunShotMatch/gunshotmatch-reports/commit/master
 	:alt: GitHub last commit
```

### Comparing `gunshotmatch_reports-0.4.0/pyproject.toml` & `gunshotmatch_reports-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "gunshotmatch-reports"
-version = "0.4.0"
+version = "0.5.0"
 description = "PDF Report Generation for GunShotMatch."
 readme = "README.rst"
 keywords = []
 dynamic = []
 dependencies = [
     "domdf-python-tools>=3.8.0.post2",
     "libgunshotmatch>=0.5.0",
@@ -28,22 +28,21 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Typing :: Typed",
 ]
 requires-python = ">=3.8"
 
+[project.license]
+file = "LICENSE"
+
 [[project.authors]]
 name = "Dominic Davis-Foster"
 email = "dominic@davis-foster.co.uk"
 
-
-[project.license]
-file = "LICENSE"
-
 [project.urls]
 Homepage = "https://github.com/GunShotMatch/gunshotmatch-reports"
 "Issue Tracker" = "https://github.com/GunShotMatch/gunshotmatch-reports/issues"
 "Source Code" = "https://github.com/GunShotMatch/gunshotmatch-reports"
 Documentation = "https://gunshotmatch-reports.readthedocs.io/en/latest"
 
 [tool.whey]
@@ -69,14 +68,24 @@
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
 directives = [ "code-block",]
 
+[tool.snippet-fmt.languages.python]
+reformat = true
+
+[tool.snippet-fmt.languages.TOML]
+reformat = true
+
+[tool.snippet-fmt.languages.ini]
+
+[tool.snippet-fmt.languages.json]
+
 [tool.sphinx-pyproject]
 github_username = "GunShotMatch"
 github_repository = "gunshotmatch-reports"
 author = "Dominic Davis-Foster"
 project = "gunshotmatch-reports"
 copyright = "2020-2024 Dominic Davis-Foster"
 language = "en"
@@ -90,24 +99,22 @@
     "sphinxcontrib.toctree_plus",
     "sphinx_toolbox.tweaks.latex_layout",
     "sphinx_toolbox.tweaks.latex_toc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinxcontrib.extras_require",
     "sphinx.ext.todo",
-    "sphinxemoji.sphinxemoji",
     "notfound.extension",
     "sphinx_copybutton",
     "sphinxcontrib.default_values",
     "sphinx_debuginfo",
     "sphinx_licenseinfo",
     "seed_intersphinx_mapping",
     "html_section",
 ]
-sphinxemoji_style = "twemoji"
 gitstamp_fmt = "%d %b %Y"
 templates_path = [ "_templates",]
 html_static_path = [ "_static",]
 source_suffix = ".rst"
 master_doc = "index"
 suppress_warnings = [ "image.nonlocal_uri",]
 pygments_style = "default"
@@ -154,17 +161,7 @@
 
 [tool.dependency-dash."requirements.txt"]
 order = 10
 
 [tool.dependency-dash."doc-source/requirements.txt"]
 order = 30
 include = false
-
-[tool.snippet-fmt.languages.python]
-reformat = true
-
-[tool.snippet-fmt.languages.TOML]
-reformat = true
-
-[tool.snippet-fmt.languages.ini]
-
-[tool.snippet-fmt.languages.json]
```

### Comparing `gunshotmatch_reports-0.4.0/README.rst` & `gunshotmatch_reports-0.5.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 .. |license| image:: https://img.shields.io/github/license/GunShotMatch/gunshotmatch-reports
 	:target: https://github.com/GunShotMatch/gunshotmatch-reports/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/GunShotMatch/gunshotmatch-reports
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-reports/v0.4.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/GunShotMatch/gunshotmatch-reports/v0.5.0
 	:target: https://github.com/GunShotMatch/gunshotmatch-reports/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/GunShotMatch/gunshotmatch-reports
 	:target: https://github.com/GunShotMatch/gunshotmatch-reports/commit/master
 	:alt: GitHub last commit
```

### Comparing `gunshotmatch_reports-0.4.0/gunshotmatch_reports/chromatogram.py` & `gunshotmatch_reports-0.5.0/gunshotmatch_reports/chromatogram.py`

 * *Files identical despite different names*

### Comparing `gunshotmatch_reports-0.4.0/gunshotmatch_reports/__init__.py` & `gunshotmatch_reports-0.5.0/gunshotmatch_reports/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020-2024 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.4.0"
+__version__: str = "0.5.0"
 __email__: str = "dominic@davis-foster.co.uk"
```

### Comparing `gunshotmatch_reports-0.4.0/gunshotmatch_reports/utils.py` & `gunshotmatch_reports-0.5.0/gunshotmatch_reports/utils.py`

 * *Files identical despite different names*

### Comparing `gunshotmatch_reports-0.4.0/gunshotmatch_reports/peaks.py` & `gunshotmatch_reports-0.5.0/gunshotmatch_reports/peaks.py`

 * *Files identical despite different names*

