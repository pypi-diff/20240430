# Comparing `tmp/mkdocs-git-revision-date-localized-plugin-1.2.4.tar.gz` & `tmp/mkdocs_git_revision_date_localized_plugin-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-git-revision-date-localized-plugin-1.2.4.tar", last modified: Sat Feb  3 08:11:12 2024, max compression
+gzip compressed data, was "mkdocs_git_revision_date_localized_plugin-1.2.5.tar", last modified: Tue Apr 30 21:22:05 2024, max compression
```

## Comparing `mkdocs-git-revision-date-localized-plugin-1.2.4.tar` & `mkdocs_git_revision_date_localized_plugin-1.2.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 08:11:12.543795 mkdocs-git-revision-date-localized-plugin-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-02-03 08:10:42.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-03 08:10:42.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-02-03 08:11:12.539795 mkdocs-git-revision-date-localized-plugin-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-02-03 08:10:42.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 08:11:12.539795 mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 08:10:42.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-02-03 08:10:42.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin/ci.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 08:11:12.539795 mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin/css/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-02-03 08:10:42.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin/css/timeago.css
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-02-03 08:10:42.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-02-03 08:10:42.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin/exclude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 08:11:12.539795 mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin/js/
--rw-r--r--   0 runner    (1001) docker     (127)    29575 2024-02-03 08:10:42.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin/js/timeago.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-03 08:10:42.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin/js/timeago_mkdocs_material.js
--rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-02-03 08:10:42.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-02-03 08:10:42.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 08:11:12.539795 mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-02-03 08:11:12.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-02-03 08:11:12.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 08:11:12.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-03 08:11:12.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-03 08:11:12.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-03 08:11:12.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-03 08:10:42.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-03 08:11:12.543795 mkdocs-git-revision-date-localized-plugin-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-02-03 08:10:42.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 08:11:12.539795 mkdocs-git-revision-date-localized-plugin-1.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    23576 2024-02-03 08:10:42.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/tests/test_builds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-02-03 08:10:42.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/tests/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-02-03 08:10:42.000000 mkdocs-git-revision-date-localized-plugin-1.2.4/tests/test_exclude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:22:05.158894 mkdocs_git_revision_date_localized_plugin-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-30 21:22:05.158894 mkdocs_git_revision_date_localized_plugin-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:22:05.154894 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/ci.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:22:05.154894 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/css/timeago.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/exclude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:22:05.158894 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    29575 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/js/timeago.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/js/timeago_mkdocs_material.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:22:05.158894 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-30 21:22:05.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-30 21:22:05.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 21:22:05.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-30 21:22:05.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-30 21:22:05.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-30 21:22:05.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 21:22:05.158894 mkdocs_git_revision_date_localized_plugin-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:22:05.158894 mkdocs_git_revision_date_localized_plugin-1.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    23576 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/tests/test_builds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/tests/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/tests/test_exclude.py
```

### Comparing `mkdocs-git-revision-date-localized-plugin-1.2.4/LICENSE` & `mkdocs_git_revision_date_localized_plugin-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-localized-plugin-1.2.4/PKG-INFO` & `mkdocs_git_revision_date_localized_plugin-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-git-revision-date-localized-plugin
-Version: 1.2.4
+Version: 1.2.5
 Summary: Mkdocs plugin that enables displaying the localized date of the last git modification of a markdown file.
 Home-page: https://github.com/timvink/mkdocs-git-revision-date-localized-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs git date timeago babel plugin
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: mkdocs-git-revision-date-localized-plugin Version:
-1.2.4 Summary: Mkdocs plugin that enables displaying the localized date of the
+1.2.5 Summary: Mkdocs plugin that enables displaying the localized date of the
 last git modification of a markdown file. Home-page: https://github.com/
 timvink/mkdocs-git-revision-date-localized-plugin Author: Tim Vink Author-
 email: vinktim@gmail.com License: MIT Keywords: mkdocs git date timeago babel
 plugin Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mkdocs-git-revision-date-localized-plugin-1.2.4/README.md` & `mkdocs_git_revision_date_localized_plugin-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin/ci.py` & `mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/ci.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin/dates.py` & `mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/dates.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin/exclude.py` & `mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/exclude.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin/js/timeago.min.js` & `mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/js/timeago.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin/js/timeago_mkdocs_material.js` & `mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/js/timeago_mkdocs_material.js`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin/plugin.py` & `mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 """
 MkDocs Plugin.
 
 https://www.mkdocs.org/
 https://github.com/timvink/mkdocs-git-revision-date-localized-plugin/
 """
-# standard lib
 import logging
 import re
 import os
 import time
 
-# 3rd party
+from mkdocs import __version__ as mkdocs_version
 from mkdocs.config import config_options
 from mkdocs.plugins import BasePlugin
 from mkdocs.structure.nav import Page
 from mkdocs.utils import copy_file
 from mkdocs.exceptions import ConfigurationError
 
-# package modules
 from mkdocs_git_revision_date_localized_plugin.util import Util
 from mkdocs_git_revision_date_localized_plugin.exclude import exclude
 
 from typing import Any, Dict
 from collections import OrderedDict
 
 HERE = os.path.dirname(os.path.abspath(__file__))
 
-
 class GitRevisionDateLocalizedPlugin(BasePlugin):
     """
     Mkdocs plugin to add revision date from Git.
 
     See https://www.mkdocs.org/user-guide/plugins
     """
 
@@ -75,15 +72,15 @@
 
         # Get locale from plugin configuration
         plugin_locale = self.config.get("locale", None)
 
         # theme locale
         if "theme" in config and "locale" in config.get("theme"):
             custom_theme = config.get("theme")
-            theme_locale = custom_theme._vars.get("locale")
+            theme_locale = custom_theme.locale if mkdocs_version >= "1.6.0" else custom_theme._vars.get("locale")
             logging.debug(
                 "Locale '%s' extracted from the custom theme: '%s'"
                 % (theme_locale, custom_theme.name)
             )
         elif "theme" in config and "language" in config.get("theme"):
             custom_theme = config.get("theme")
             theme_locale = custom_theme._vars.get("language")
```

### Comparing `mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin/util.py` & `mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/util.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin.egg-info/PKG-INFO` & `mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-git-revision-date-localized-plugin
-Version: 1.2.4
+Version: 1.2.5
 Summary: Mkdocs plugin that enables displaying the localized date of the last git modification of a markdown file.
 Home-page: https://github.com/timvink/mkdocs-git-revision-date-localized-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs git date timeago babel plugin
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: mkdocs-git-revision-date-localized-plugin Version:
-1.2.4 Summary: Mkdocs plugin that enables displaying the localized date of the
+1.2.5 Summary: Mkdocs plugin that enables displaying the localized date of the
 last git modification of a markdown file. Home-page: https://github.com/
 timvink/mkdocs-git-revision-date-localized-plugin Author: Tim Vink Author-
 email: vinktim@gmail.com License: MIT Keywords: mkdocs git date timeago babel
 plugin Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mkdocs-git-revision-date-localized-plugin-1.2.4/mkdocs_git_revision_date_localized_plugin.egg-info/SOURCES.txt` & `mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-localized-plugin-1.2.4/setup.py` & `mkdocs_git_revision_date_localized_plugin-1.2.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 DEPENDENCIES = file.readlines()
 file.close()
 
 del file
 
 setup(
     name="mkdocs-git-revision-date-localized-plugin",
-    version="1.2.4",
+    version="1.2.5",
     description="Mkdocs plugin that enables displaying the localized date of the last git modification of a markdown file.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     keywords="mkdocs git date timeago babel plugin",
     url="https://github.com/timvink/mkdocs-git-revision-date-localized-plugin",
     author="Tim Vink",
     author_email="vinktim@gmail.com",
```

### Comparing `mkdocs-git-revision-date-localized-plugin-1.2.4/tests/test_builds.py` & `mkdocs_git_revision_date_localized_plugin-1.2.5/tests/test_builds.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-localized-plugin-1.2.4/tests/test_dates.py` & `mkdocs_git_revision_date_localized_plugin-1.2.5/tests/test_dates.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-localized-plugin-1.2.4/tests/test_exclude.py` & `mkdocs_git_revision_date_localized_plugin-1.2.5/tests/test_exclude.py`

 * *Files identical despite different names*

