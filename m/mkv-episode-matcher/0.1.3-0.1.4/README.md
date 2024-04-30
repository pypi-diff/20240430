# Comparing `tmp/mkv_episode_matcher-0.1.3.tar.gz` & `tmp/mkv_episode_matcher-0.1.4.tar.gz`

## Comparing `mkv_episode_matcher-0.1.3.tar` & `mkv_episode_matcher-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/.coverage.DESKTOP-NTJ52LL.19040.XkHNEbEx
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/.coverage.DESKTOP-NTJ52LL.24340.XjsBEKWx
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/.gitattributes
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/.gitmodules
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkdocs.yml
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/.vscode/settings.json
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/docs/index.md
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/.gitattributes
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/__init__.py
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/__main__.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/config.py
--rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/episode_matcher.py
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/mkv_to_srt.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/requirements.txt
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/tmdb_client.py
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/utils.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/libraries/pgs2srt/.git
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/libraries/pgs2srt/.gitignore
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/libraries/pgs2srt/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/libraries/pgs2srt/__init__.py
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/libraries/pgs2srt/imagemaker.py
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/libraries/pgs2srt/pgs2srt.py
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/libraries/pgs2srt/pgsreader.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/libraries/pgs2srt/requirements.txt
--rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/libraries/pgs2srt/Libraries/SubZero/SubZero.py
--rw-r--r--   0        0        0     9957 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/libraries/pgs2srt/Libraries/SubZero/post_processing.py
--rw-r--r--   0        0        0   676829 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/mkv_episode_matcher/libraries/pgs2srt/Libraries/SubZero/dictionaries/data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/.gitignore
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/README.md
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/.coverage.DESKTOP-NTJ52LL.19040.XkHNEbEx
+-rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/.coverage.DESKTOP-NTJ52LL.24340.XjsBEKWx
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/.gitattributes
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/.gitmodules
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkdocs.yml
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/.vscode/settings.json
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/docs/index.md
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/.gitattributes
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/__init__.py
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/__main__.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/config.py
+-rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/episode_matcher.py
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/mkv_to_srt.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/requirements.txt
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/tmdb_client.py
+-rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/utils.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/libraries/pgs2srt/.git
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/libraries/pgs2srt/.gitignore
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/libraries/pgs2srt/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/libraries/pgs2srt/__init__.py
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/libraries/pgs2srt/imagemaker.py
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/libraries/pgs2srt/pgs2srt.py
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/libraries/pgs2srt/pgsreader.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/libraries/pgs2srt/requirements.txt
+-rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/libraries/pgs2srt/Libraries/SubZero/SubZero.py
+-rw-r--r--   0        0        0     9957 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/libraries/pgs2srt/Libraries/SubZero/post_processing.py
+-rw-r--r--   0        0        0   676829 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/mkv_episode_matcher/libraries/pgs2srt/Libraries/SubZero/dictionaries/data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/.gitignore
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/README.md
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 mkv_episode_matcher-0.1.4/PKG-INFO
```

### Comparing `mkv_episode_matcher-0.1.3/.coverage.DESKTOP-NTJ52LL.19040.XkHNEbEx` & `mkv_episode_matcher-0.1.4/.coverage.DESKTOP-NTJ52LL.19040.XkHNEbEx`

 * *Files identical despite different names*

### Comparing `mkv_episode_matcher-0.1.3/.coverage.DESKTOP-NTJ52LL.24340.XjsBEKWx` & `mkv_episode_matcher-0.1.4/.coverage.DESKTOP-NTJ52LL.24340.XjsBEKWx`

 * *Files identical despite different names*

### Comparing `mkv_episode_matcher-0.1.3/.github/workflows/ci.yml` & `mkv_episode_matcher-0.1.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `mkv_episode_matcher-0.1.3/mkv_episode_matcher/__main__.py` & `mkv_episode_matcher-0.1.4/mkv_episode_matcher/__main__.py`

 * *Files identical despite different names*

### Comparing `mkv_episode_matcher-0.1.3/mkv_episode_matcher/config.py` & `mkv_episode_matcher-0.1.4/mkv_episode_matcher/config.py`

 * *Files identical despite different names*

### Comparing `mkv_episode_matcher-0.1.3/mkv_episode_matcher/episode_matcher.py` & `mkv_episode_matcher-0.1.4/mkv_episode_matcher/episode_matcher.py`

 * *Files identical despite different names*

### Comparing `mkv_episode_matcher-0.1.3/mkv_episode_matcher/mkv_to_srt.py` & `mkv_episode_matcher-0.1.4/mkv_episode_matcher/mkv_to_srt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 import os
 import subprocess
 import sys
 
 # Get the absolute path of the parent directory of the current script.
 parent_dir = os.path.dirname(os.path.abspath(__file__))
-
-# Add the parent directory to the Python path.
-sys.path.append(parent_dir)
-# Add the 'libraries' directory to the Python path.
-sys.path.append(os.path.join(parent_dir, "libraries"))
-# Add the 'libraries' directory to the Python path.
-sys.path.append(os.path.join(parent_dir, "..", "libraries", "pgs2srt"))
+# Add the 'pgs2srt' directory to the Python path.
+sys.path.append(os.path.join(parent_dir, "libraries", "pgs2srt"))
 import re
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime, timedelta
 
 import pytesseract
 from imagemaker import make_image
 from loguru import logger
```

### Comparing `mkv_episode_matcher-0.1.3/mkv_episode_matcher/tmdb_client.py` & `mkv_episode_matcher-0.1.4/mkv_episode_matcher/tmdb_client.py`

 * *Files identical despite different names*

### Comparing `mkv_episode_matcher-0.1.3/mkv_episode_matcher/utils.py` & `mkv_episode_matcher-0.1.4/mkv_episode_matcher/utils.py`

 * *Files identical despite different names*

### Comparing `mkv_episode_matcher-0.1.3/mkv_episode_matcher/libraries/pgs2srt/README.md` & `mkv_episode_matcher-0.1.4/mkv_episode_matcher/libraries/pgs2srt/README.md`

 * *Files identical despite different names*

### Comparing `mkv_episode_matcher-0.1.3/mkv_episode_matcher/libraries/pgs2srt/imagemaker.py` & `mkv_episode_matcher-0.1.4/mkv_episode_matcher/libraries/pgs2srt/imagemaker.py`

 * *Files identical despite different names*

### Comparing `mkv_episode_matcher-0.1.3/mkv_episode_matcher/libraries/pgs2srt/pgs2srt.py` & `mkv_episode_matcher-0.1.4/mkv_episode_matcher/libraries/pgs2srt/pgs2srt.py`

 * *Files identical despite different names*

### Comparing `mkv_episode_matcher-0.1.3/mkv_episode_matcher/libraries/pgs2srt/pgsreader.py` & `mkv_episode_matcher-0.1.4/mkv_episode_matcher/libraries/pgs2srt/pgsreader.py`

 * *Files identical despite different names*

### Comparing `mkv_episode_matcher-0.1.3/mkv_episode_matcher/libraries/pgs2srt/Libraries/SubZero/SubZero.py` & `mkv_episode_matcher-0.1.4/mkv_episode_matcher/libraries/pgs2srt/Libraries/SubZero/SubZero.py`

 * *Files identical despite different names*

### Comparing `mkv_episode_matcher-0.1.3/mkv_episode_matcher/libraries/pgs2srt/Libraries/SubZero/post_processing.py` & `mkv_episode_matcher-0.1.4/mkv_episode_matcher/libraries/pgs2srt/Libraries/SubZero/post_processing.py`

 * *Files identical despite different names*

### Comparing `mkv_episode_matcher-0.1.3/mkv_episode_matcher/libraries/pgs2srt/Libraries/SubZero/dictionaries/data.py` & `mkv_episode_matcher-0.1.4/mkv_episode_matcher/libraries/pgs2srt/Libraries/SubZero/dictionaries/data.py`

 * *Files identical despite different names*

### Comparing `mkv_episode_matcher-0.1.3/README.md` & `mkv_episode_matcher-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mkv_episode_matcher-0.1.3/pyproject.toml` & `mkv_episode_matcher-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mkv_episode_matcher-0.1.3/PKG-INFO` & `mkv_episode_matcher-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mkv-episode-matcher
-Version: 0.1.3
+Version: 0.1.4
 Summary: The MKV Episode Matcher is a tool for identifying TV series episodes from MKV files and renaming the files accordingly.
 Project-URL: Documentation, https://github.com/Jsakkos/mkv-episode-matcher#readme
 Project-URL: Issues, https://github.com/Jsakkos/mkv-episode-matcher/issues
 Project-URL: Source, https://github.com/Jsakkos/mkv-episode-matcher
 Author-email: Jsakkos <jonathansakkos@protonmail.com>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

