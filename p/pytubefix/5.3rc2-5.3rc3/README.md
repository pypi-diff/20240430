# Comparing `tmp/pytubefix-5.3rc2.tar.gz` & `tmp/pytubefix-5.3rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytubefix-5.3rc2.tar", last modified: Tue Apr 30 00:41:11 2024, max compression
+gzip compressed data, was "pytubefix-5.3rc3.tar", last modified: Tue Apr 30 00:45:26 2024, max compression
```

## Comparing `pytubefix-5.3rc2.tar` & `pytubefix-5.3rc3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:41:11.301142 pytubefix-5.3rc2/
--rw-rw-r--   0 juan      (1000) juan      (1000)     1101 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/LICENSE
--rw-rw-r--   0 juan      (1000) juan      (1000)       18 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/MANIFEST.in
--rw-r--r--   0 juan      (1000) juan      (1000)     4342 2024-04-30 00:41:11.301142 pytubefix-5.3rc2/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)     3010 2024-04-30 00:39:00.000000 pytubefix-5.3rc2/README.md
--rw-rw-r--   0 juan      (1000) juan      (1000)     1524 2024-04-30 00:37:27.000000 pytubefix-5.3rc2/pyproject.toml
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:41:11.293141 pytubefix-5.3rc2/pytubefix/
--rw-rw-r--   0 juan      (1000) juan      (1000)      614 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    20118 2024-04-30 00:31:55.000000 pytubefix-5.3rc2/pytubefix/__main__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     6595 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/captions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1358 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/chapters.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     5645 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/cipher.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    17032 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/cli.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      786 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/colors.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:41:11.297141 pytubefix-5.3rc2/pytubefix/contrib/
--rw-rw-r--   0 juan      (1000) juan      (1000)        0 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/contrib/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    19995 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/contrib/channel.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    14600 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/contrib/playlist.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    11072 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/contrib/search.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     4115 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/exceptions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    18319 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/extract.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     9944 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/helpers.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    17902 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/innertube.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     4311 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/itags.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    41663 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/jsinterp.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1483 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/metadata.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      478 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/monostate.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     5960 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/parser.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    14289 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/query.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     8817 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/request.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    14818 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/pytubefix/streams.py
--rw-rw-r--   0 juan      (1000) juan      (1000)       75 2024-04-30 00:37:53.000000 pytubefix-5.3rc2/pytubefix/version.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:41:11.297141 pytubefix-5.3rc2/pytubefix.egg-info/
--rw-r--r--   0 juan      (1000) juan      (1000)     4342 2024-04-30 00:41:11.000000 pytubefix-5.3rc2/pytubefix.egg-info/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)     1029 2024-04-30 00:41:11.000000 pytubefix-5.3rc2/pytubefix.egg-info/SOURCES.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-04-30 00:41:11.000000 pytubefix-5.3rc2/pytubefix.egg-info/dependency_links.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       49 2024-04-30 00:41:11.000000 pytubefix-5.3rc2/pytubefix.egg-info/entry_points.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       10 2024-04-30 00:41:11.000000 pytubefix-5.3rc2/pytubefix.egg-info/top_level.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-04-30 00:41:11.301142 pytubefix-5.3rc2/setup.cfg
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:41:11.297141 pytubefix-5.3rc2/tests/
--rw-rw-r--   0 juan      (1000) juan      (1000)     6579 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/tests/test_captions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1360 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/tests/test_cipher.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    18009 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/tests/test_cli.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     3626 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/tests/test_exceptions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     2963 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/tests/test_extract.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     5060 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/tests/test_helpers.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      279 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/tests/test_itags.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1939 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/tests/test_main.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      501 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/tests/test_metadata.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1412 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/tests/test_parser.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     6172 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/tests/test_query.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1882 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/tests/test_request.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    13661 2024-04-30 00:29:57.000000 pytubefix-5.3rc2/tests/test_streams.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:45:26.140663 pytubefix-5.3rc3/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1101 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/LICENSE
+-rw-rw-r--   0 juan      (1000) juan      (1000)       18 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/MANIFEST.in
+-rw-r--r--   0 juan      (1000) juan      (1000)     4342 2024-04-30 00:45:26.136663 pytubefix-5.3rc3/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3010 2024-04-30 00:39:00.000000 pytubefix-5.3rc3/README.md
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1524 2024-04-30 00:41:41.000000 pytubefix-5.3rc3/pyproject.toml
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:45:26.124663 pytubefix-5.3rc3/pytubefix/
+-rw-rw-r--   0 juan      (1000) juan      (1000)      614 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    20118 2024-04-30 00:31:55.000000 pytubefix-5.3rc3/pytubefix/__main__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6595 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/captions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1358 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/chapters.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5645 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/cipher.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    17032 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/cli.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      786 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/colors.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:45:26.132663 pytubefix-5.3rc3/pytubefix/contrib/
+-rw-rw-r--   0 juan      (1000) juan      (1000)        0 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/contrib/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    19995 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/contrib/channel.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14600 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/contrib/playlist.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    11072 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/contrib/search.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     4115 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/exceptions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    18319 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/extract.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     9944 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/helpers.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    17902 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/innertube.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     4311 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/itags.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    41663 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/jsinterp.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1483 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/metadata.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      478 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/monostate.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5960 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/parser.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14289 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/query.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     8817 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/request.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14818 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/pytubefix/streams.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)       75 2024-04-30 00:42:00.000000 pytubefix-5.3rc3/pytubefix/version.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:45:26.136663 pytubefix-5.3rc3/pytubefix.egg-info/
+-rw-r--r--   0 juan      (1000) juan      (1000)     4342 2024-04-30 00:45:26.000000 pytubefix-5.3rc3/pytubefix.egg-info/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1029 2024-04-30 00:45:26.000000 pytubefix-5.3rc3/pytubefix.egg-info/SOURCES.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-04-30 00:45:26.000000 pytubefix-5.3rc3/pytubefix.egg-info/dependency_links.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       49 2024-04-30 00:45:26.000000 pytubefix-5.3rc3/pytubefix.egg-info/entry_points.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       10 2024-04-30 00:45:26.000000 pytubefix-5.3rc3/pytubefix.egg-info/top_level.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-04-30 00:45:26.140663 pytubefix-5.3rc3/setup.cfg
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:45:26.136663 pytubefix-5.3rc3/tests/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6579 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_captions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1360 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_cipher.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    18009 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_cli.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3626 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_exceptions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2963 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_extract.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5060 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_helpers.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      279 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_itags.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1939 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_main.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      501 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_metadata.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1412 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_parser.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6172 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_query.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1882 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_request.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    13661 2024-04-30 00:29:57.000000 pytubefix-5.3rc3/tests/test_streams.py
```

### Comparing `pytubefix-5.3rc2/LICENSE` & `pytubefix-5.3rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/PKG-INFO` & `pytubefix-5.3rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubefix
-Version: 5.3rc2
+Version: 5.3rc3
 Summary: Python3 library for downloading YouTube Videos.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: MIT license
 Project-URL: Homepage, https://github.com/juanbindez/pytubefix
 Project-URL: Bug Reports, https://github.com/juanbindez/pytubefix/issues
 Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytubefix Version: 5.3rc2 Summary: Python3 library
+Metadata-Version: 2.1 Name: pytubefix Version: 5.3rc3 Summary: Python3 library
 for downloading YouTube Videos. Author-email: Juan Bindez
 gmail.com> License: MIT license Project-URL: Homepage, https://github.com/
 juanbindez/pytubefix Project-URL: Bug Reports, https://github.com/juanbindez/
 pytubefix/issues Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytubefix-5.3rc2/README.md` & `pytubefix-5.3rc3/README.md`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pyproject.toml` & `pytubefix-5.3rc3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytubefix"
-version = "5.3-rc2"
+version = "5.3-rc3"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python3 library for downloading YouTube Videos."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT license"}
```

### Comparing `pytubefix-5.3rc2/pytubefix/__init__.py` & `pytubefix-5.3rc3/pytubefix/__init__.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/__main__.py` & `pytubefix-5.3rc3/pytubefix/__main__.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/captions.py` & `pytubefix-5.3rc3/pytubefix/captions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/chapters.py` & `pytubefix-5.3rc3/pytubefix/chapters.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/cipher.py` & `pytubefix-5.3rc3/pytubefix/cipher.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/cli.py` & `pytubefix-5.3rc3/pytubefix/cli.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/colors.py` & `pytubefix-5.3rc3/pytubefix/colors.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/contrib/channel.py` & `pytubefix-5.3rc3/pytubefix/contrib/channel.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/contrib/playlist.py` & `pytubefix-5.3rc3/pytubefix/contrib/playlist.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/contrib/search.py` & `pytubefix-5.3rc3/pytubefix/contrib/search.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/exceptions.py` & `pytubefix-5.3rc3/pytubefix/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/extract.py` & `pytubefix-5.3rc3/pytubefix/extract.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/helpers.py` & `pytubefix-5.3rc3/pytubefix/helpers.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/innertube.py` & `pytubefix-5.3rc3/pytubefix/innertube.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/itags.py` & `pytubefix-5.3rc3/pytubefix/itags.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/jsinterp.py` & `pytubefix-5.3rc3/pytubefix/jsinterp.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/metadata.py` & `pytubefix-5.3rc3/pytubefix/metadata.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/parser.py` & `pytubefix-5.3rc3/pytubefix/parser.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/query.py` & `pytubefix-5.3rc3/pytubefix/query.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/request.py` & `pytubefix-5.3rc3/pytubefix/request.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix/streams.py` & `pytubefix-5.3rc3/pytubefix/streams.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/pytubefix.egg-info/PKG-INFO` & `pytubefix-5.3rc3/pytubefix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubefix
-Version: 5.3rc2
+Version: 5.3rc3
 Summary: Python3 library for downloading YouTube Videos.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: MIT license
 Project-URL: Homepage, https://github.com/juanbindez/pytubefix
 Project-URL: Bug Reports, https://github.com/juanbindez/pytubefix/issues
 Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytubefix Version: 5.3rc2 Summary: Python3 library
+Metadata-Version: 2.1 Name: pytubefix Version: 5.3rc3 Summary: Python3 library
 for downloading YouTube Videos. Author-email: Juan Bindez
 gmail.com> License: MIT license Project-URL: Homepage, https://github.com/
 juanbindez/pytubefix Project-URL: Bug Reports, https://github.com/juanbindez/
 pytubefix/issues Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytubefix-5.3rc2/pytubefix.egg-info/SOURCES.txt` & `pytubefix-5.3rc3/pytubefix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/tests/test_captions.py` & `pytubefix-5.3rc3/tests/test_captions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/tests/test_cipher.py` & `pytubefix-5.3rc3/tests/test_cipher.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/tests/test_cli.py` & `pytubefix-5.3rc3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/tests/test_exceptions.py` & `pytubefix-5.3rc3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/tests/test_extract.py` & `pytubefix-5.3rc3/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/tests/test_helpers.py` & `pytubefix-5.3rc3/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/tests/test_main.py` & `pytubefix-5.3rc3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/tests/test_parser.py` & `pytubefix-5.3rc3/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/tests/test_query.py` & `pytubefix-5.3rc3/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/tests/test_request.py` & `pytubefix-5.3rc3/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.3rc2/tests/test_streams.py` & `pytubefix-5.3rc3/tests/test_streams.py`

 * *Files identical despite different names*

