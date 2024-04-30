# Comparing `tmp/mkdocs-rss-plugin-1.8.0.tar.gz` & `tmp/mkdocs-rss-plugin-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-rss-plugin-1.8.0.tar", last modified: Mon Jul 24 17:11:15 2023, max compression
+gzip compressed data, was "mkdocs-rss-plugin-1.9.0.tar", last modified: Thu Dec  7 15:47:04 2023, max compression
```

## Comparing `mkdocs-rss-plugin-1.8.0.tar` & `mkdocs-rss-plugin-1.9.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:11:15.331236 mkdocs-rss-plugin-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-07-24 17:11:15.331236 mkdocs-rss-plugin-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:11:15.327236 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/customtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:11:15.331236 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/git_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/git_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/git_manager/ci.py
--rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:11:15.331236 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/templates/rss.xml.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/timezoner_pre39.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/timezoner_py39.py
--rw-r--r--   0 runner    (1001) docker     (123)    25752 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:11:15.327236 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-07-24 17:11:15.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-24 17:11:15.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:11:15.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 17:11:15.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-24 17:11:15.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 17:11:15.000000 mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-24 17:11:15.331236 mkdocs-rss-plugin-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-24 17:10:54.000000 mkdocs-rss-plugin-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:11:15.331236 mkdocs-rss-plugin-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21020 2023-07-24 17:10:55.000000 mkdocs-rss-plugin-1.8.0/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-24 17:10:55.000000 mkdocs-rss-plugin-1.8.0/tests/test_build_no_git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-24 17:10:55.000000 mkdocs-rss-plugin-1.8.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-24 17:10:55.000000 mkdocs-rss-plugin-1.8.0/tests/test_rss_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-24 17:10:55.000000 mkdocs-rss-plugin-1.8.0/tests/test_timezoner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:47:04.225861 mkdocs-rss-plugin-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2023-12-07 15:47:04.225861 mkdocs-rss-plugin-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:47:04.217861 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:47:04.221861 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/git_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/git_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/git_manager/ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13407 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:47:04.221861 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/templates/rss.xml.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/timezoner_pre39.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/timezoner_py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26874 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:47:04.221861 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2023-12-07 15:47:04.000000 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2023-12-07 15:47:04.000000 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 15:47:04.000000 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-07 15:47:04.000000 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2023-12-07 15:47:04.000000 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-07 15:47:04.000000 mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2023-12-07 15:47:04.225861 mkdocs-rss-plugin-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:47:04.221861 mkdocs-rss-plugin-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    23158 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/tests/test_build_no_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/tests/test_rss_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2023-12-07 15:46:48.000000 mkdocs-rss-plugin-1.9.0/tests/test_timezoner.py
```

### Comparing `mkdocs-rss-plugin-1.8.0/LICENSE` & `mkdocs-rss-plugin-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.8.0/PKG-INFO` & `mkdocs-rss-plugin-1.9.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.1
-Name: mkdocs-rss-plugin
-Version: 1.8.0
-Summary: MkDocs plugin which generates a static RSS feed using git log and page.meta.
-Author: Julien Moura
-Author-email: dev@ingeoveritas.com
-License: MIT
-Project-URL: Docs, https://guts.github.io/mkdocs-rss-plugin/
-Project-URL: Bug Reports, https://github.com/Guts/mkdocs-rss-plugin/issues/
-Project-URL: Source, https://github.com/Guts/mkdocs-rss-plugin/
-Keywords: mkdocs rss git plugin
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Documentation
-Classifier: Topic :: Text Processing :: Markup :: Markdown
-Requires-Python: >=3.8, <4
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: doc
-License-File: LICENSE
-
 # MkDocs RSS plugin
 
 [![PyPi version badge](https://badgen.net/pypi/v/mkdocs-rss-plugin)](https://pypi.org/project/mkdocs-rss-plugin/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mkdocs-rss-plugin)](https://pypi.org/project/mkdocs-rss-plugin/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-rss-plugin)](https://pypi.org/project/mkdocs-rss-plugin/)
 
 [![codecov](https://codecov.io/gh/Guts/mkdocs-rss-plugin/branch/main/graph/badge.svg?token=A0XPLKiwiW)](https://codecov.io/gh/Guts/mkdocs-rss-plugin)
@@ -93,34 +63,49 @@
 
 Following initiative from the author of Material for MkDocs, this plugin provides its own JSON schema to validate configuration: [source](https://github.com/Guts/mkdocs-rss-plugin/blob/main/docs/schema.json) - [documentation](https://guts.github.io/mkdocs-rss-plugin/schema.json).
 
 ## Development
 
 Clone the repository:
 
-```bash
+```sh
 # install development dependencies
 python -m pip install -U -r requirements/development.txt
 # alternatively: pip install -e .[dev]
 
 # install project as editable
 python -m pip install -e .
 
 # install git hooks
 pre-commit install
+```
+
+Then follow the [contribution guidelines](CONTRIBUTING.md).
+
+### Run the tests
+
+```sh
+# install development dependencies
+python -m pip install -U -r requirements/testing.txt
+# alternatively: pip install -e .[test]
 
 # run tests
 pytest
+```
+
+### Build the documentation
 
+```sh
 # install dependencies for documentation
 python -m pip install -U -r requirements/documentation.txt
 # alternatively: pip install -e .[doc]
-```
 
-Then follow the [contribution guidelines](CONTRIBUTING.md).
+# build the documentation
+mkdocs build
+```
 
-## Release workflow
+### Release workflow
 
 1. Fill the `CHANGELOG.md`
 1. Change the version number in `__about__.py`
 1. Apply a git tag with the relevant version: `git tag -a 0.3.0 {git commit hash} -m "New awesome feature"`
 1. Push tag to main branch: `git push origin 0.3.0`
```

### Comparing `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/__about__.py` & `mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/__about__.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,14 +36,14 @@
 __summary__ = (
     "MkDocs plugin which generates a static RSS feed using git log and page.meta."
 )
 __title__ = "MkDocs RSS plugin"
 __title_clean__ = "".join(e for e in __title__ if e.isalnum())
 __uri__ = "https://github.com/Guts/mkdocs-rss-plugin/"
 
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 __version_info__ = tuple(
     [
         int(num) if num.isdigit() else num
         for num in __version__.replace("-", ".", 1).split(".")
     ]
 )
```

### Comparing `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/customtypes.py` & `mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! python3  # noqa: E265
 
 # ############################################################################
 # ########## Libraries #############
 # ##################################
 
-# standard library
+# standard
 from datetime import datetime
 from pathlib import Path
 from typing import NamedTuple
 
 
 # ############################################################################
 # ########## Classes ###############
```

### Comparing `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/git_manager/ci.py` & `mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/git_manager/ci.py`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/plugin.py` & `mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,76 +7,62 @@
 # standard library
 import logging
 from copy import deepcopy
 from datetime import datetime
 from email.utils import formatdate
 from pathlib import Path
 from re import compile
+from typing import Optional
 
 # 3rd party
 from jinja2 import Environment, FileSystemLoader, select_autoescape
 from mkdocs.config import config_options
 from mkdocs.exceptions import PluginError
 from mkdocs.plugins import BasePlugin
 from mkdocs.structure.pages import Page
 from mkdocs.utils import get_build_timestamp
 
 # package modules
-from .__about__ import __title__, __uri__, __version__
-from .customtypes import PageInformation
-from .util import Util
+from mkdocs_rss_plugin.__about__ import __title__, __uri__, __version__
+from mkdocs_rss_plugin.config import RssPluginConfig
+from mkdocs_rss_plugin.constants import (
+    DEFAULT_TEMPLATE_FILENAME,
+    DEFAULT_TEMPLATE_FOLDER,
+    OUTPUT_FEED_CREATED,
+    OUTPUT_FEED_UPDATED,
+)
+from mkdocs_rss_plugin.models import PageInformation
+from mkdocs_rss_plugin.util import Util
 
 # ############################################################################
 # ########## Globals #############
 # ################################
-
-DEFAULT_TEMPLATE_FOLDER = Path(__file__).parent / "templates"
-DEFAULT_TEMPLATE_FILENAME = DEFAULT_TEMPLATE_FOLDER / "rss.xml.jinja2"
-OUTPUT_FEED_CREATED = "feed_rss_created.xml"
-OUTPUT_FEED_UPDATED = "feed_rss_updated.xml"
-
 logger = logging.getLogger("mkdocs.mkdocs_rss_plugin")
 
 
 # ############################################################################
 # ########## Classes ###############
 # ##################################
 
 
-class GitRssPlugin(BasePlugin):
+class GitRssPlugin(BasePlugin[RssPluginConfig]):
     """Main class for MkDocs plugin."""
 
-    config_scheme = (
-        ("abstract_chars_count", config_options.Type(int, default=160)),
-        ("abstract_delimiter", config_options.Type(str, default="<!-- more -->")),
-        ("categories", config_options.Type(list, default=None)),
-        ("comments_path", config_options.Type(str, default=None)),
-        ("date_from_meta", config_options.Type(dict, default=None)),
-        ("enabled", config_options.Type(bool, default=True)),
-        ("feed_ttl", config_options.Type(int, default=1440)),
-        ("image", config_options.Type(str, default=None)),
-        ("length", config_options.Type(int, default=20)),
-        ("match_path", config_options.Type(str, default=".*")),
-        ("pretty_print", config_options.Type(bool, default=False)),
-        ("url_parameters", config_options.Type(dict, default=None)),
-        ("use_git", config_options.Type(bool, default=True)),
-    )
-
     def __init__(self):
         """Instanciation."""
         # dates source
         self.src_date_created = self.src_date_updated = "git"
-        self.meta_datetime_format = None
-        self.meta_default_timezone = "UTC"
-        self.meta_default_time = None
+        self.meta_datetime_format: Optional[str] = None
+        self.meta_default_timezone: str = "UTC"
+        self.meta_default_time: Optional[str] = None
         # pages storage
-        self.pages_to_filter = []
+        self.pages_to_filter: list = []
         # prepare output feeds
-        self.feed_created = dict
-        self.feed_updated = dict
+        self.feed_created: dict = {}
+        self.feed_updated: dict = {}
 
     def on_config(self, config: config_options.Config) -> dict:
         """The config event is the first event called on build and
         is run immediately after the user configuration is loaded and validated.
         Any alterations to the config should be made here.
         https://www.mkdocs.org/user-guide/plugins/#on_config
 
@@ -86,79 +72,75 @@
         :raises FileExistsError: if the template for the RSS feed is not found
 
         :return: plugin configuration object
         :rtype: dict
         """
 
         # Skip if disabled
-        if not self.config.get("enabled"):
+        if not self.config.enabled:
             return config
 
         # instanciate plugin tooling
-        self.util = Util(use_git=self.config.get("use_git", True))
+        self.util = Util(use_git=self.config.use_git)
 
         # check template dirs
         if not Path(DEFAULT_TEMPLATE_FILENAME).is_file():
             raise FileExistsError(DEFAULT_TEMPLATE_FILENAME)
         self.tpl_file = Path(DEFAULT_TEMPLATE_FILENAME)
         self.tpl_folder = DEFAULT_TEMPLATE_FOLDER
 
         # start a feed dictionary using global config vars
         base_feed = {
-            "author": config.get("site_author", None),
+            "author": config.site_author or None,
             "buildDate": formatdate(get_build_timestamp()),
-            "copyright": config.get("copyright", None),
-            "description": config.get("site_description", None),
+            "copyright": config.copyright,
+            "description": config.site_description,
             "entries": [],
             "generator": f"{__title__} - v{__version__}",
             "html_url": self.util.get_site_url(config),
             "language": self.util.guess_locale(config),
             "pubDate": formatdate(get_build_timestamp()),
-            "repo_url": config.get("repo_url", config.get("site_url", None)),
-            "title": config.get("site_name", None),
-            "ttl": self.config.get("feed_ttl", None),
+            "repo_url": config.repo_url,
+            "title": config.site_name,
+            "ttl": self.config.feed_ttl,
         }
 
         # feed image
-        if self.config.get("image"):
-            base_feed["logo_url"] = self.config.get("image")
+        if self.config.image:
+            base_feed["logo_url"] = self.config.image
 
         # pattern to match pages included in output
-        self.match_path_pattern = compile(self.config.get("match_path"))
+        self.match_path_pattern = compile(self.config.match_path)
 
         # date handling
-        if self.config.get("date_from_meta") is not None:
-            self.src_date_created = self.config.get("date_from_meta").get(
-                "as_creation", False
-            )
-            self.src_date_updated = self.config.get("date_from_meta").get(
-                "as_update", False
-            )
-            self.meta_datetime_format = self.config.get("date_from_meta").get(
+        if self.config.date_from_meta is not None:
+            self.src_date_created = self.config.date_from_meta.get("as_creation", False)
+            self.src_date_updated = self.config.date_from_meta.get("as_update", False)
+            self.meta_datetime_format = self.config.date_from_meta.get(
                 "datetime_format", "%Y-%m-%d %H:%M"
             )
-            self.meta_default_timezone = self.config.get("date_from_meta").get(
+            self.meta_default_timezone = self.config.date_from_meta.get(
                 "default_timezone", "UTC"
             )
-            self.meta_default_time = self.config.get("date_from_meta").get(
+            self.meta_default_time = self.config.date_from_meta.get(
                 "default_time", None
             )
             if self.meta_default_time:
                 try:
                     self.meta_default_time = datetime.strptime(
                         self.meta_default_time, "%H:%M"
                     )
                 except ValueError as err:
                     raise PluginError(
                         "[rss-plugin] Config error: `date_from_meta.default_time` value "
                         f"'{self.meta_default_time}' format doesn't match the expected "
                         f"format %H:%M. Trace: {err}"
                     )
 
-            if self.config.get("use_git", True):
+            if self.config.use_git:
                 logger.debug(
                     "[rss-plugin] Dates will be retrieved FIRSTLY from page meta (yaml "
                     "frontmatter). The git log will be used as fallback."
                 )
             else:
                 logger.debug(
                     "[rss-plugin] Dates will be retrieved ONLY from page meta (yaml "
@@ -211,15 +193,15 @@
         :type files: [type]
 
         :return: HTML rendered from Markdown source as string
         :rtype: str
         """
 
         # Skip if disabled
-        if not self.config.get("enabled"):
+        if not self.config.enabled:
             return
 
         # skip pages that don't match the config var match_path
         if not self.match_path_pattern.match(page.file.src_path):
             return
 
         # skip pages with draft=true
@@ -234,49 +216,51 @@
             source_date_update=self.src_date_updated,
             meta_datetime_format=self.meta_datetime_format,
             meta_default_timezone=self.meta_default_timezone,
             meta_default_time=self.meta_default_time,
         )
 
         # handle custom URL parameters
-        if self.config.get("url_parameters"):
+        if self.config.url_parameters:
             page_url_full = self.util.build_url(
                 base_url=page.canonical_url,
                 path="",
-                args_dict=self.config.get("url_parameters"),
+                args_dict=self.config.url_parameters,
             )
         else:
             page_url_full = page.canonical_url
 
         # handle URL comment path
-        if self.config.get("comments_path"):
+        if self.config.comments_path:
             page_url_comments = self.util.build_url(
                 base_url=page.canonical_url,
-                path=self.config.get("comments_path"),
+                path=self.config.comments_path,
             )
         else:
             page_url_comments = None
 
         # append to list to be filtered later
         self.pages_to_filter.append(
             PageInformation(
                 abs_path=Path(page.file.abs_src_path),
                 authors=self.util.get_authors_from_meta(in_page=page),
                 categories=self.util.get_categories_from_meta(
-                    in_page=page, categories_labels=self.config.get("categories")
+                    in_page=page, categories_labels=self.config.categories
                 ),
                 created=page_dates[0],
                 description=self.util.get_description_or_abstract(
                     in_page=page,
-                    chars_count=self.config.get("abstract_chars_count"),
-                    abstract_delimiter=self.config.get("abstract_delimiter"),
+                    chars_count=self.config.abstract_chars_count,
+                    abstract_delimiter=self.config.abstract_delimiter,
                 ),
                 guid=page.canonical_url,
                 image=self.util.get_image(
-                    in_page=page, base_url=config.get("site_url", __uri__)
+                    in_page=page,
+                    # below let it as old dict get method to handle custom fallback value
+                    base_url=config.get("site_url", __uri__),
                 ),
                 title=page.title,
                 updated=page_dates[1],
                 url_comments=page_url_comments,
                 url_full=page_url_full,
             )
         )
@@ -289,39 +273,39 @@
         :param config: global configuration object
         :type config: config_options.Config
         :return: global configuration object
         :rtype: dict
         """
 
         # Skip if disabled
-        if not self.config.get("enabled"):
+        if not self.config.enabled:
             return
 
         # pretty print or not
-        pretty_print = self.config.get("pretty_print", False)
+        pretty_print = self.config.pretty_print
 
         # output filepaths
-        out_feed_created = Path(config.get("site_dir")) / OUTPUT_FEED_CREATED
-        out_feed_updated = Path(config.get("site_dir")) / OUTPUT_FEED_UPDATED
+        out_feed_created = Path(config.site_dir).joinpath(OUTPUT_FEED_CREATED)
+        out_feed_updated = Path(config.site_dir).joinpath(OUTPUT_FEED_UPDATED)
 
         # created items
         self.feed_created.get("entries").extend(
             self.util.filter_pages(
                 pages=self.pages_to_filter,
                 attribute="created",
-                length=self.config.get("length", 20),
+                length=self.config.length,
             )
         )
 
         # updated items
         self.feed_updated.get("entries").extend(
             self.util.filter_pages(
                 pages=self.pages_to_filter,
                 attribute="updated",
-                length=self.config.get("length", 20),
+                length=self.config.length,
             )
         )
 
         # write feeds according to the pretty print option
         if pretty_print:
             # load Jinja environment and template
             env = Environment(
```

### Comparing `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/templates/rss.xml.jinja2` & `mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/templates/rss.xml.jinja2`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/timezoner_pre39.py` & `mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/timezoner_pre39.py`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/timezoner_py39.py` & `mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/timezoner_py39.py`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin/util.py` & `mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,32 +21,27 @@
 import markdown
 from git import GitCommandError, GitCommandNotFound, InvalidGitRepositoryError, Repo
 from mkdocs.config.config_options import Config
 from mkdocs.structure.pages import Page
 from mkdocs.utils import get_build_datetime
 
 # package
-from mkdocs_rss_plugin import __about__
+from mkdocs_rss_plugin.constants import REMOTE_REQUEST_HEADERS
 from mkdocs_rss_plugin.git_manager.ci import CiHandler
 
 # conditional imports
 if sys.version_info < (3, 9):
     from mkdocs_rss_plugin.timezoner_pre39 import set_datetime_zoneinfo
 else:
     from mkdocs_rss_plugin.timezoner_py39 import set_datetime_zoneinfo
 
 # ############################################################################
 # ########## Globals #############
 # ################################
 
-REMOTE_REQUEST_HEADERS = {
-    "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8",
-    "User-Agent": f"{__about__.__title__}/{__about__.__version__}",
-}
-
 logger = logging.getLogger("mkdocs.mkdocs_rss_plugin")
 
 
 # ############################################################################
 # ########## Classes #############
 # ################################
 
@@ -586,15 +581,15 @@
         :type mkdocs_config: Config
 
         :return: site url
         :rtype: str or None
         """
         # this method exists because the following line returns an empty string instead of \
         # None (because the key alwayus exists)
-        defined_site_url = mkdocs_config.get("site_url", None)
+        defined_site_url = mkdocs_config.site_url
 
         # cases
         if defined_site_url is None or not len(defined_site_url):
             # in case of mkdocs's behavior change
             site_url = None
         else:
             site_url = defined_site_url
@@ -613,24 +608,56 @@
 
         :return: language code
         :rtype: str or None
         """
         # MkDocs locale settings - might be added in future mkdocs versions
         # see: https://github.com/timvink/mkdocs-git-revision-date-localized-plugin/issues/24
         if mkdocs_config.get("locale"):
+            logger.warning(
+                DeprecationWarning(
+                    "[rss-plugin] Mkdocs does not support locale option at the "
+                    "configuration root but under theme sub-configuration. It won't be "
+                    "supported anymore by the plugin in the next version."
+                )
+            )
             return mkdocs_config.get("locale")
 
-        # Some themes implement a locale or a language setting
-        if "theme" in mkdocs_config and "locale" in mkdocs_config.get("theme"):
-            locale = mkdocs_config.get("theme")._vars.get("locale")
-            return f"{locale.language}-{locale.territory}"
-        elif "theme" in mkdocs_config and "language" in mkdocs_config.get("theme"):
-            return mkdocs_config.get("theme")._vars.get("language")
-        else:
-            return None
+        # Some themes implement a locale or a language settings
+        if "theme" in mkdocs_config:
+            if (
+                mkdocs_config.theme.name == "material"
+                and "language" in mkdocs_config.theme
+            ):
+                # TODO: remove custom behavior when Material theme switches to locale
+                # see: https://github.com/squidfunk/mkdocs-material/discussions/6453
+                logger.debug(
+                    "[rss plugin] Language detected in Material theme "
+                    f"('{mkdocs_config.theme.name}') settings: "
+                    f"{mkdocs_config.theme.get('language')}"
+                )
+                return mkdocs_config.theme.get("language")
+
+            elif "locale" in mkdocs_config.theme:
+                locale = mkdocs_config.theme.locale
+                logger.debug(
+                    "[rss plugin] Locale detected in theme "
+                    f"('{mkdocs_config.theme.name}') settings: {locale=}"
+                )
+                return (
+                    f"{locale.language}-{locale.territory}"
+                    if locale.territory
+                    else f"{locale.language}"
+                )
+            else:
+                logger.debug(
+                    "[rss plugin] Nor locale or language detected in theme settings "
+                    f"('{mkdocs_config.theme.name}')."
+                )
+
+        return None
 
     @staticmethod
     def filter_pages(pages: list, attribute: str, length: int) -> list:
         """Filter and return pages into a friendly RSS structure.
 
         :param pages: pages to filter
         :type pages: list
```

### Comparing `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin.egg-info/PKG-INFO` & `mkdocs-rss-plugin-1.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-rss-plugin
-Version: 1.8.0
+Version: 1.9.0
 Summary: MkDocs plugin which generates a static RSS feed using git log and page.meta.
 Author: Julien Moura
 Author-email: dev@ingeoveritas.com
 License: MIT
 Project-URL: Docs, https://guts.github.io/mkdocs-rss-plugin/
 Project-URL: Bug Reports, https://github.com/Guts/mkdocs-rss-plugin/issues/
 Project-URL: Source, https://github.com/Guts/mkdocs-rss-plugin/
@@ -12,25 +12,46 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Documentation
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: GitPython<3.2,>=3.1
+Requires-Dist: mkdocs<2,>=1.4
+Requires-Dist: pytz==2022.*; python_version < "3.9"
+Requires-Dist: tzdata==2023.*; python_version >= "3.9" and sys_platform == "win32"
 Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: flake8<7,>=6; extra == "dev"
+Requires-Dist: flake8-bugbear>=23.12; extra == "dev"
+Requires-Dist: flake8-builtins>=2.1; extra == "dev"
+Requires-Dist: flake8-eradicate>=1; extra == "dev"
+Requires-Dist: flake8-isort>=6; extra == "dev"
+Requires-Dist: pre-commit<4,>=3; extra == "dev"
 Provides-Extra: doc
-License-File: LICENSE
+Requires-Dist: mkdocs-bootswatch<2,>=1; extra == "doc"
+Requires-Dist: mkdocs-minify-plugin==0.7.*; extra == "doc"
+Requires-Dist: pygments<3,>=2.5; extra == "doc"
+Requires-Dist: pymdown-extensions<11,>=10; extra == "doc"
+Provides-Extra: test
+Requires-Dist: feedparser<6.1,>=6.0; extra == "test"
+Requires-Dist: mkdocs-material>=9; extra == "test"
+Requires-Dist: pytest-cov<4.2,>=4; extra == "test"
+Requires-Dist: validator-collection<1.6,>=1.5; extra == "test"
 
 # MkDocs RSS plugin
 
 [![PyPi version badge](https://badgen.net/pypi/v/mkdocs-rss-plugin)](https://pypi.org/project/mkdocs-rss-plugin/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mkdocs-rss-plugin)](https://pypi.org/project/mkdocs-rss-plugin/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-rss-plugin)](https://pypi.org/project/mkdocs-rss-plugin/)
 
@@ -93,34 +114,49 @@
 
 Following initiative from the author of Material for MkDocs, this plugin provides its own JSON schema to validate configuration: [source](https://github.com/Guts/mkdocs-rss-plugin/blob/main/docs/schema.json) - [documentation](https://guts.github.io/mkdocs-rss-plugin/schema.json).
 
 ## Development
 
 Clone the repository:
 
-```bash
+```sh
 # install development dependencies
 python -m pip install -U -r requirements/development.txt
 # alternatively: pip install -e .[dev]
 
 # install project as editable
 python -m pip install -e .
 
 # install git hooks
 pre-commit install
+```
+
+Then follow the [contribution guidelines](CONTRIBUTING.md).
+
+### Run the tests
+
+```sh
+# install development dependencies
+python -m pip install -U -r requirements/testing.txt
+# alternatively: pip install -e .[test]
 
 # run tests
 pytest
+```
+
+### Build the documentation
 
+```sh
 # install dependencies for documentation
 python -m pip install -U -r requirements/documentation.txt
 # alternatively: pip install -e .[doc]
-```
 
-Then follow the [contribution guidelines](CONTRIBUTING.md).
+# build the documentation
+mkdocs build
+```
 
-## Release workflow
+### Release workflow
 
 1. Fill the `CHANGELOG.md`
 1. Change the version number in `__about__.py`
 1. Apply a git tag with the relevant version: `git tag -a 0.3.0 {git commit hash} -m "New awesome feature"`
 1. Push tag to main branch: `git push origin 0.3.0`
```

### Comparing `mkdocs-rss-plugin-1.8.0/mkdocs_rss_plugin.egg-info/SOURCES.txt` & `mkdocs-rss-plugin-1.9.0/mkdocs_rss_plugin.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 mkdocs_rss_plugin/__about__.py
 mkdocs_rss_plugin/__init__.py
-mkdocs_rss_plugin/customtypes.py
+mkdocs_rss_plugin/config.py
+mkdocs_rss_plugin/constants.py
+mkdocs_rss_plugin/models.py
 mkdocs_rss_plugin/plugin.py
 mkdocs_rss_plugin/timezoner_pre39.py
 mkdocs_rss_plugin/timezoner_py39.py
 mkdocs_rss_plugin/util.py
 mkdocs_rss_plugin.egg-info/PKG-INFO
 mkdocs_rss_plugin.egg-info/SOURCES.txt
 mkdocs_rss_plugin.egg-info/dependency_links.txt
```

### Comparing `mkdocs-rss-plugin-1.8.0/setup.cfg` & `mkdocs-rss-plugin-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.8.0/tests/test_build.py` & `mkdocs-rss-plugin-1.9.0/tests/test_build.py`

 * *Files 3% similar despite different names*

```diff
@@ -326,20 +326,20 @@
                     "Page without meta with short text",
                     "Blog sample",
                 ):
                     self.assertGreaterEqual(
                         len(feed_item.description), 150, feed_item.title
                     )
 
-    def test_simple_build_lang_with_territory(self):
+    def test_simple_build_locale_with_territory(self):
         with tempfile.TemporaryDirectory() as tmpdirname:
             cli_result = self.build_docs_setup(
                 testproject_path="docs",
                 mkdocs_yml_filepath=Path(
-                    "tests/fixtures/mkdocs_lang_with_territory.yml"
+                    "tests/fixtures/mkdocs_locale_with_territory.yml"
                 ),
                 output_path=tmpdirname,
                 strict=True,
             )
 
             if cli_result.exception is not None:
                 e = cli_result.exception
@@ -352,14 +352,66 @@
             feed_parsed = feedparser.parse(Path(tmpdirname) / "feed_rss_created.xml")
             self.assertEqual(feed_parsed.feed.get("language"), "en-US")
 
             # updated items
             feed_parsed = feedparser.parse(Path(tmpdirname) / "feed_rss_updated.xml")
             self.assertEqual(feed_parsed.feed.get("language"), "en-US")
 
+    def test_simple_build_locale_without_territory(self):
+        with tempfile.TemporaryDirectory() as tmpdirname:
+            cli_result = self.build_docs_setup(
+                testproject_path="docs",
+                mkdocs_yml_filepath=Path(
+                    "tests/fixtures/mkdocs_locale_without_territory.yml"
+                ),
+                output_path=tmpdirname,
+                strict=True,
+            )
+
+            if cli_result.exception is not None:
+                e = cli_result.exception
+                logger.debug(format_exception(type(e), e, e.__traceback__))
+
+            self.assertEqual(cli_result.exit_code, 0)
+            self.assertIsNone(cli_result.exception)
+
+            # created items
+            feed_parsed = feedparser.parse(Path(tmpdirname) / "feed_rss_created.xml")
+            self.assertEqual(feed_parsed.feed.get("language"), "fr")
+
+            # updated items
+            feed_parsed = feedparser.parse(Path(tmpdirname) / "feed_rss_updated.xml")
+            self.assertEqual(feed_parsed.feed.get("language"), "fr")
+
+    def test_simple_build_language_specific_material(self):
+        with tempfile.TemporaryDirectory() as tmpdirname:
+            cli_result = self.build_docs_setup(
+                testproject_path="docs",
+                mkdocs_yml_filepath=Path(
+                    "tests/fixtures/mkdocs_language_specific_material.yml"
+                ),
+                output_path=tmpdirname,
+                strict=True,
+            )
+
+            if cli_result.exception is not None:
+                e = cli_result.exception
+                logger.debug(format_exception(type(e), e, e.__traceback__))
+
+            self.assertEqual(cli_result.exit_code, 0)
+            self.assertIsNone(cli_result.exception)
+
+            # created items
+            feed_parsed = feedparser.parse(Path(tmpdirname) / "feed_rss_created.xml")
+            self.assertEqual(feed_parsed.feed.get("language"), "fr")
+
+            # updated items
+            feed_parsed = feedparser.parse(Path(tmpdirname) / "feed_rss_updated.xml")
+            self.assertEqual(feed_parsed.feed.get("language"), "fr")
+
     def test_simple_build_pretty_print_enabled(self):
         with tempfile.TemporaryDirectory() as tmpdirname:
             cli_result = self.build_docs_setup(
                 testproject_path="docs",
                 mkdocs_yml_filepath=Path(
                     "tests/fixtures/mkdocs_pretty_print_enabled.yml"
                 ),
```

### Comparing `mkdocs-rss-plugin-1.8.0/tests/test_build_no_git.py` & `mkdocs-rss-plugin-1.9.0/tests/test_build_no_git.py`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.8.0/tests/test_config.py` & `mkdocs-rss-plugin-1.9.0/tests/test_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,16 +13,19 @@
 # ########## Libraries #############
 # ##################################
 
 # Standard library
 import unittest
 from pathlib import Path
 
+# 3rd party
 from mkdocs.config.base import Config
 
+from mkdocs_rss_plugin.config import RssPluginConfig
+
 # plugin target
 from mkdocs_rss_plugin.plugin import GitRssPlugin
 
 # test suite
 from tests.base import BaseTest
 
 
@@ -61,23 +64,25 @@
             "categories": None,
             "comments_path": None,
             "date_from_meta": None,
             "enabled": True,
             "feed_ttl": 1440,
             "image": None,
             "length": 20,
-            "pretty_print": False,
             "match_path": ".*",
+            "pretty_print": False,
             "url_parameters": None,
             "use_git": True,
         }
 
         # load
         plugin = GitRssPlugin()
         errors, warnings = plugin.load_config({})
+        self.assertIsInstance(plugin.config, RssPluginConfig)
+        self.assertIsInstance(plugin.config, Config)
         self.assertEqual(plugin.config, expected)
         self.assertEqual(errors, [])
         self.assertEqual(warnings, [])
 
     def test_plugin_config_image(self):
         # reference
         expected = {
@@ -86,26 +91,28 @@
             "categories": None,
             "comments_path": None,
             "date_from_meta": None,
             "enabled": True,
             "feed_ttl": 1440,
             "image": self.feed_image,
             "length": 20,
-            "pretty_print": False,
             "match_path": ".*",
+            "pretty_print": False,
             "url_parameters": None,
             "use_git": True,
         }
 
         # custom config
         custom_cfg = {"image": self.feed_image}
 
         # load
         plugin = GitRssPlugin()
         errors, warnings = plugin.load_config(custom_cfg)
+        self.assertIsInstance(plugin.config, RssPluginConfig)
+        self.assertIsInstance(plugin.config, Config)
         self.assertEqual(plugin.config, expected)
         self.assertEqual(errors, [])
         self.assertEqual(warnings, [])
 
     def test_plugin_config_through_mkdocs(self):
         for config_filepath in self.config_files:
             plg_cfg = self.get_plugin_config_from_mkdocs(config_filepath, "rss")
```

### Comparing `mkdocs-rss-plugin-1.8.0/tests/test_rss_util.py` & `mkdocs-rss-plugin-1.9.0/tests/test_rss_util.py`

 * *Files identical despite different names*

### Comparing `mkdocs-rss-plugin-1.8.0/tests/test_timezoner.py` & `mkdocs-rss-plugin-1.9.0/tests/test_timezoner.py`

 * *Files identical despite different names*

