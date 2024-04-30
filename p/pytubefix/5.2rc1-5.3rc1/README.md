# Comparing `tmp/pytubefix-5.2rc1.tar.gz` & `tmp/pytubefix-5.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytubefix-5.2rc1.tar", last modified: Sat Apr 27 03:05:55 2024, max compression
+gzip compressed data, was "pytubefix-5.3rc1.tar", last modified: Tue Apr 30 00:36:03 2024, max compression
```

## Comparing `pytubefix-5.2rc1.tar` & `pytubefix-5.3rc1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-27 03:05:55.167881 pytubefix-5.2rc1/
--rw-rw-r--   0 juan      (1000) juan      (1000)     1101 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/LICENSE
--rw-rw-r--   0 juan      (1000) juan      (1000)       18 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/MANIFEST.in
--rw-r--r--   0 juan      (1000) juan      (1000)     4390 2024-04-27 03:05:55.163881 pytubefix-5.2rc1/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)     3058 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/README.md
--rw-rw-r--   0 juan      (1000) juan      (1000)     1524 2024-04-27 03:01:59.000000 pytubefix-5.2rc1/pyproject.toml
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-27 03:05:55.159881 pytubefix-5.2rc1/pytubefix/
--rw-rw-r--   0 juan      (1000) juan      (1000)      614 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    20108 2024-04-27 03:00:33.000000 pytubefix-5.2rc1/pytubefix/__main__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     6595 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/captions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1358 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/chapters.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     5645 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/cipher.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    17032 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/cli.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      786 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/colors.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-27 03:05:55.159881 pytubefix-5.2rc1/pytubefix/contrib/
--rw-rw-r--   0 juan      (1000) juan      (1000)        0 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/contrib/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    19995 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/contrib/channel.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    14600 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/contrib/playlist.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    11072 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/contrib/search.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     4115 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/exceptions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    18319 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/extract.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     9944 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/helpers.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    17902 2024-04-27 03:00:33.000000 pytubefix-5.2rc1/pytubefix/innertube.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     4311 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/itags.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    41663 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/jsinterp.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1483 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/metadata.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      478 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/monostate.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     5960 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/parser.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    14289 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/query.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     8817 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/request.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    14818 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/pytubefix/streams.py
--rw-rw-r--   0 juan      (1000) juan      (1000)       75 2024-04-27 03:04:59.000000 pytubefix-5.2rc1/pytubefix/version.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-27 03:05:55.163881 pytubefix-5.2rc1/pytubefix.egg-info/
--rw-r--r--   0 juan      (1000) juan      (1000)     4390 2024-04-27 03:05:55.000000 pytubefix-5.2rc1/pytubefix.egg-info/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)     1029 2024-04-27 03:05:55.000000 pytubefix-5.2rc1/pytubefix.egg-info/SOURCES.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-04-27 03:05:55.000000 pytubefix-5.2rc1/pytubefix.egg-info/dependency_links.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       49 2024-04-27 03:05:55.000000 pytubefix-5.2rc1/pytubefix.egg-info/entry_points.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       10 2024-04-27 03:05:55.000000 pytubefix-5.2rc1/pytubefix.egg-info/top_level.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-04-27 03:05:55.167881 pytubefix-5.2rc1/setup.cfg
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-27 03:05:55.163881 pytubefix-5.2rc1/tests/
--rw-rw-r--   0 juan      (1000) juan      (1000)     6579 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/tests/test_captions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1360 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/tests/test_cipher.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    18009 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/tests/test_cli.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     3626 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/tests/test_exceptions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     2963 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/tests/test_extract.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     5060 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/tests/test_helpers.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      279 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/tests/test_itags.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1939 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/tests/test_main.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      501 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/tests/test_metadata.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1412 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/tests/test_parser.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     6172 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/tests/test_query.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1882 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/tests/test_request.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    13661 2024-04-27 02:56:57.000000 pytubefix-5.2rc1/tests/test_streams.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:36:03.407103 pytubefix-5.3rc1/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1101 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/LICENSE
+-rw-rw-r--   0 juan      (1000) juan      (1000)       18 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/MANIFEST.in
+-rw-r--r--   0 juan      (1000) juan      (1000)     4388 2024-04-30 00:36:03.407103 pytubefix-5.3rc1/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3056 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/README.md
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1524 2024-04-30 00:33:40.000000 pytubefix-5.3rc1/pyproject.toml
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:36:03.403103 pytubefix-5.3rc1/pytubefix/
+-rw-rw-r--   0 juan      (1000) juan      (1000)      614 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    20118 2024-04-30 00:31:55.000000 pytubefix-5.3rc1/pytubefix/__main__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6595 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/captions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1358 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/chapters.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5645 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/cipher.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    17032 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/cli.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      786 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/colors.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:36:03.403103 pytubefix-5.3rc1/pytubefix/contrib/
+-rw-rw-r--   0 juan      (1000) juan      (1000)        0 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/contrib/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    19995 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/contrib/channel.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14600 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/contrib/playlist.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    11072 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/contrib/search.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     4115 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/exceptions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    18319 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/extract.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     9944 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/helpers.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    17902 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/innertube.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     4311 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/itags.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    41663 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/jsinterp.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1483 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/metadata.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      478 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/monostate.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5960 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/parser.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14289 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/query.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     8817 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/request.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14818 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/pytubefix/streams.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)       75 2024-04-30 00:33:20.000000 pytubefix-5.3rc1/pytubefix/version.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:36:03.407103 pytubefix-5.3rc1/pytubefix.egg-info/
+-rw-r--r--   0 juan      (1000) juan      (1000)     4388 2024-04-30 00:36:03.000000 pytubefix-5.3rc1/pytubefix.egg-info/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1029 2024-04-30 00:36:03.000000 pytubefix-5.3rc1/pytubefix.egg-info/SOURCES.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-04-30 00:36:03.000000 pytubefix-5.3rc1/pytubefix.egg-info/dependency_links.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       49 2024-04-30 00:36:03.000000 pytubefix-5.3rc1/pytubefix.egg-info/entry_points.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       10 2024-04-30 00:36:03.000000 pytubefix-5.3rc1/pytubefix.egg-info/top_level.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-04-30 00:36:03.407103 pytubefix-5.3rc1/setup.cfg
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-30 00:36:03.407103 pytubefix-5.3rc1/tests/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6579 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/tests/test_captions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1360 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/tests/test_cipher.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    18009 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/tests/test_cli.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3626 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/tests/test_exceptions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2963 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/tests/test_extract.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5060 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/tests/test_helpers.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      279 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/tests/test_itags.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1939 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/tests/test_main.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      501 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/tests/test_metadata.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1412 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/tests/test_parser.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6172 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/tests/test_query.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1882 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/tests/test_request.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    13661 2024-04-30 00:29:57.000000 pytubefix-5.3rc1/tests/test_streams.py
```

### Comparing `pytubefix-5.2rc1/LICENSE` & `pytubefix-5.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/PKG-INFO` & `pytubefix-5.3rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubefix
-Version: 5.2rc1
+Version: 5.3rc1
 Summary: Python3 library for downloading YouTube Videos.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: MIT license
 Project-URL: Homepage, https://github.com/juanbindez/pytubefix
 Project-URL: Bug Reports, https://github.com/juanbindez/pytubefix/issues
 Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream
@@ -37,20 +37,20 @@
 ![GitHub Tag](https://img.shields.io/github/v/tag/JuanBindez/pytubefix?include_prereleases)
 <a href="https://pypi.org/project/pytubefix/"><img src="https://img.shields.io/pypi/v/pytubefix" /></a>
 
 
 ## A pytube fork with additional features and fixes.
 
 ----------
-## install:
+## install
 
     pip install pytubefix
 
 
-## Quickstart:
+## Quickstart
 
 #### mp4 video download highest resolution:
 
 ```python
 
 from pytubefix import YouTube
 from pytubefix.cli import on_progress
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytubefix Version: 5.2rc1 Summary: Python3 library
+Metadata-Version: 2.1 Name: pytubefix Version: 5.3rc1 Summary: Python3 library
 for downloading YouTube Videos. Author-email: Juan Bindez
 gmail.com> License: MIT license Project-URL: Homepage, https://github.com/
 juanbindez/pytubefix Project-URL: Bug Reports, https://github.com/juanbindez/
 pytubefix/issues Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
@@ -16,16 +16,16 @@
 Development :: Libraries :: Python Modules Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities Requires-Python: >=3.7 Description-Content-Type:
 text/markdown License-File: LICENSE # pytubefix ![PyPI - Downloads](https://
 img.shields.io/pypi/dm/pytubefix) ![PyPI - License](https://img.shields.io/
 pypi/l/pytubefix) ![Read the Docs](https://img.shields.io/readthedocs/
 pytubefix) ![GitHub Tag](https://img.shields.io/github/v/tag/JuanBindez/
 pytubefix?include_prereleases) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_p_y_t_u_b_e_f_i_x_]## A
-pytube fork with additional features and fixes. ---------- ## install: pip
-install pytubefix ## Quickstart: #### mp4 video download highest resolution:
+pytube fork with additional features and fixes. ---------- ## install pip
+install pytubefix ## Quickstart #### mp4 video download highest resolution:
 ```python from pytubefix import YouTube from pytubefix.cli import on_progress
 url = input("url >") yt = YouTube(url, on_progress_callback = on_progress)
 print(yt.title) ys = yt.streams.get_highest_resolution() ys.download() ``` ####
 If you want to save in .mp3 just pass the mp3=True parameter (MPEG-4 AAC audio
 codec): ```python from pytubefix import YouTube from pytubefix.cli import
 on_progress url = input("url >") yt = YouTube(url, on_progress_callback =
 on_progress) print(yt.title) ys = yt.streams.get_audio_only() ys.download
```

### Comparing `pytubefix-5.2rc1/README.md` & `pytubefix-5.3rc1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 ![GitHub Tag](https://img.shields.io/github/v/tag/JuanBindez/pytubefix?include_prereleases)
 <a href="https://pypi.org/project/pytubefix/"><img src="https://img.shields.io/pypi/v/pytubefix" /></a>
 
 
 ## A pytube fork with additional features and fixes.
 
 ----------
-## install:
+## install
 
     pip install pytubefix
 
 
-## Quickstart:
+## Quickstart
 
 #### mp4 video download highest resolution:
 
 ```python
 
 from pytubefix import YouTube
 from pytubefix.cli import on_progress
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # pytubefix ![PyPI - Downloads](https://img.shields.io/pypi/dm/pytubefix) !
 [PyPI - License](https://img.shields.io/pypi/l/pytubefix) ![Read the Docs]
 (https://img.shields.io/readthedocs/pytubefix) ![GitHub Tag](https://
 img.shields.io/github/v/tag/JuanBindez/pytubefix?include_prereleases) _[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_p_y_t_u_b_e_f_i_x_]## A pytube fork with additional features and
-fixes. ---------- ## install: pip install pytubefix ## Quickstart: #### mp4
-video download highest resolution: ```python from pytubefix import YouTube from
+fixes. ---------- ## install pip install pytubefix ## Quickstart #### mp4 video
+download highest resolution: ```python from pytubefix import YouTube from
 pytubefix.cli import on_progress url = input("url >") yt = YouTube(url,
 on_progress_callback = on_progress) print(yt.title) ys =
 yt.streams.get_highest_resolution() ys.download() ``` #### If you want to save
 in .mp3 just pass the mp3=True parameter (MPEG-4 AAC audio codec): ```python
 from pytubefix import YouTube from pytubefix.cli import on_progress url = input
 ("url >") yt = YouTube(url, on_progress_callback = on_progress) print(yt.title)
 ys = yt.streams.get_audio_only() ys.download(mp3=True) # pass the parameter
```

### Comparing `pytubefix-5.2rc1/pyproject.toml` & `pytubefix-5.3rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytubefix"
-version = "5.2-rc1"
+version = "5.3-rc1"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python3 library for downloading YouTube Videos."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT license"}
```

### Comparing `pytubefix-5.2rc1/pytubefix/__init__.py` & `pytubefix-5.3rc1/pytubefix/__init__.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix/__main__.py` & `pytubefix-5.3rc1/pytubefix/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     def __init__(
             self,
             url: str,
             client: str = 'ANDROID_TESTSUITE',
             on_progress_callback: Optional[Callable[[Any, bytes, int], None]] = None,
             on_complete_callback: Optional[Callable[[Any, Optional[str]], None]] = None,
-            proxies: Dict[str, str] = None,
+            proxies: Optional[Dict[str, str]] = None,
             use_oauth: bool = False,
             allow_oauth_cache: bool = True
     ):
         """Construct a :class:`YouTube <YouTube>`.
 
         :param str url:
             A valid YouTube watch URL.
```

### Comparing `pytubefix-5.2rc1/pytubefix/captions.py` & `pytubefix-5.3rc1/pytubefix/captions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix/chapters.py` & `pytubefix-5.3rc1/pytubefix/chapters.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix/cipher.py` & `pytubefix-5.3rc1/pytubefix/cipher.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix/cli.py` & `pytubefix-5.3rc1/pytubefix/cli.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix/colors.py` & `pytubefix-5.3rc1/pytubefix/colors.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix/contrib/channel.py` & `pytubefix-5.3rc1/pytubefix/contrib/channel.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix/contrib/playlist.py` & `pytubefix-5.3rc1/pytubefix/contrib/playlist.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix/contrib/search.py` & `pytubefix-5.3rc1/pytubefix/contrib/search.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix/exceptions.py` & `pytubefix-5.3rc1/pytubefix/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix/extract.py` & `pytubefix-5.3rc1/pytubefix/extract.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix/helpers.py` & `pytubefix-5.3rc1/pytubefix/helpers.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix/innertube.py` & `pytubefix-5.3rc1/pytubefix/innertube.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix/itags.py` & `pytubefix-5.3rc1/pytubefix/itags.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix/jsinterp.py` & `pytubefix-5.3rc1/pytubefix/jsinterp.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix/metadata.py` & `pytubefix-5.3rc1/pytubefix/metadata.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix/parser.py` & `pytubefix-5.3rc1/pytubefix/parser.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix/query.py` & `pytubefix-5.3rc1/pytubefix/query.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix/request.py` & `pytubefix-5.3rc1/pytubefix/request.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix/streams.py` & `pytubefix-5.3rc1/pytubefix/streams.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/pytubefix.egg-info/PKG-INFO` & `pytubefix-5.3rc1/pytubefix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubefix
-Version: 5.2rc1
+Version: 5.3rc1
 Summary: Python3 library for downloading YouTube Videos.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: MIT license
 Project-URL: Homepage, https://github.com/juanbindez/pytubefix
 Project-URL: Bug Reports, https://github.com/juanbindez/pytubefix/issues
 Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream
@@ -37,20 +37,20 @@
 ![GitHub Tag](https://img.shields.io/github/v/tag/JuanBindez/pytubefix?include_prereleases)
 <a href="https://pypi.org/project/pytubefix/"><img src="https://img.shields.io/pypi/v/pytubefix" /></a>
 
 
 ## A pytube fork with additional features and fixes.
 
 ----------
-## install:
+## install
 
     pip install pytubefix
 
 
-## Quickstart:
+## Quickstart
 
 #### mp4 video download highest resolution:
 
 ```python
 
 from pytubefix import YouTube
 from pytubefix.cli import on_progress
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytubefix Version: 5.2rc1 Summary: Python3 library
+Metadata-Version: 2.1 Name: pytubefix Version: 5.3rc1 Summary: Python3 library
 for downloading YouTube Videos. Author-email: Juan Bindez
 gmail.com> License: MIT license Project-URL: Homepage, https://github.com/
 juanbindez/pytubefix Project-URL: Bug Reports, https://github.com/juanbindez/
 pytubefix/issues Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
@@ -16,16 +16,16 @@
 Development :: Libraries :: Python Modules Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities Requires-Python: >=3.7 Description-Content-Type:
 text/markdown License-File: LICENSE # pytubefix ![PyPI - Downloads](https://
 img.shields.io/pypi/dm/pytubefix) ![PyPI - License](https://img.shields.io/
 pypi/l/pytubefix) ![Read the Docs](https://img.shields.io/readthedocs/
 pytubefix) ![GitHub Tag](https://img.shields.io/github/v/tag/JuanBindez/
 pytubefix?include_prereleases) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_p_y_t_u_b_e_f_i_x_]## A
-pytube fork with additional features and fixes. ---------- ## install: pip
-install pytubefix ## Quickstart: #### mp4 video download highest resolution:
+pytube fork with additional features and fixes. ---------- ## install pip
+install pytubefix ## Quickstart #### mp4 video download highest resolution:
 ```python from pytubefix import YouTube from pytubefix.cli import on_progress
 url = input("url >") yt = YouTube(url, on_progress_callback = on_progress)
 print(yt.title) ys = yt.streams.get_highest_resolution() ys.download() ``` ####
 If you want to save in .mp3 just pass the mp3=True parameter (MPEG-4 AAC audio
 codec): ```python from pytubefix import YouTube from pytubefix.cli import
 on_progress url = input("url >") yt = YouTube(url, on_progress_callback =
 on_progress) print(yt.title) ys = yt.streams.get_audio_only() ys.download
```

### Comparing `pytubefix-5.2rc1/pytubefix.egg-info/SOURCES.txt` & `pytubefix-5.3rc1/pytubefix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/tests/test_captions.py` & `pytubefix-5.3rc1/tests/test_captions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/tests/test_cipher.py` & `pytubefix-5.3rc1/tests/test_cipher.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/tests/test_cli.py` & `pytubefix-5.3rc1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/tests/test_exceptions.py` & `pytubefix-5.3rc1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/tests/test_extract.py` & `pytubefix-5.3rc1/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/tests/test_helpers.py` & `pytubefix-5.3rc1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/tests/test_main.py` & `pytubefix-5.3rc1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/tests/test_parser.py` & `pytubefix-5.3rc1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/tests/test_query.py` & `pytubefix-5.3rc1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/tests/test_request.py` & `pytubefix-5.3rc1/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.2rc1/tests/test_streams.py` & `pytubefix-5.3rc1/tests/test_streams.py`

 * *Files identical despite different names*

