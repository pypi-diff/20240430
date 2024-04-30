# Comparing `tmp/streamlit_rec-0.0.3.tar.gz` & `tmp/streamlit_rec-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_rec-0.0.3.tar", last modified: Tue Apr 30 03:58:16 2024, max compression
+gzip compressed data, was "streamlit_rec-0.0.4.tar", last modified: Tue Apr 30 04:00:57 2024, max compression
```

## Comparing `streamlit_rec-0.0.3.tar` & `streamlit_rec-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:58:16.973737 streamlit_rec-0.0.3/
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     1063 2024-04-26 08:04:38.000000 streamlit_rec-0.0.3/LICENSE
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       49 2024-04-26 08:04:38.000000 streamlit_rec-0.0.3/MANIFEST.in
--rw-r--r--   0 bensonsung  (1002) bensonsung  (1002)     3424 2024-04-30 03:58:16.973737 streamlit_rec-0.0.3/PKG-INFO
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     3127 2024-04-30 03:57:52.000000 streamlit_rec-0.0.3/README.md
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       38 2024-04-30 03:58:16.973737 streamlit_rec-0.0.3/setup.cfg
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      670 2024-04-30 03:58:10.000000 streamlit_rec-0.0.3/setup.py
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:58:16.973737 streamlit_rec-0.0.3/streamlit_rec/
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       90 2024-04-30 03:19:08.000000 streamlit_rec-0.0.3/streamlit_rec/__init__.py
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:58:16.973737 streamlit_rec-0.0.3/streamlit_rec/frontend/
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:58:16.973737 streamlit_rec-0.0.3/streamlit_rec/frontend/build/
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      521 2024-04-30 02:03:50.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/asset-manifest.json
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)   197412 2024-04-30 02:03:47.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/bootstrap.min.css
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      500 2024-04-30 02:03:50.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/index.html
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:58:16.973737 streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:58:16.973737 streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)    19699 2024-04-30 02:03:50.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)    54687 2024-04-30 02:03:50.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js.map
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     5652 2024-04-30 02:03:50.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)    37989 2024-04-30 02:03:50.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js.map
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)   395798 2024-04-30 02:03:50.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     1693 2024-04-30 02:03:50.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.LICENSE.txt
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)  1407755 2024-04-30 02:03:50.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.map
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     1037 2024-04-30 02:55:07.000000 streamlit_rec-0.0.3/streamlit_rec/streamlit_rec.py
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:58:16.973737 streamlit_rec-0.0.3/streamlit_rec.egg-info/
--rw-r--r--   0 bensonsung  (1002) bensonsung  (1002)     3424 2024-04-30 03:58:16.000000 streamlit_rec-0.0.3/streamlit_rec.egg-info/PKG-INFO
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      851 2024-04-30 03:58:16.000000 streamlit_rec-0.0.3/streamlit_rec.egg-info/SOURCES.txt
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)        1 2024-04-30 03:58:16.000000 streamlit_rec-0.0.3/streamlit_rec.egg-info/dependency_links.txt
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       28 2024-04-30 03:58:16.000000 streamlit_rec-0.0.3/streamlit_rec.egg-info/requires.txt
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       14 2024-04-30 03:58:16.000000 streamlit_rec-0.0.3/streamlit_rec.egg-info/top_level.txt
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 04:00:57.683949 streamlit_rec-0.0.4/
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     1063 2024-04-26 08:04:38.000000 streamlit_rec-0.0.4/LICENSE
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       49 2024-04-26 08:04:38.000000 streamlit_rec-0.0.4/MANIFEST.in
+-rw-r--r--   0 bensonsung  (1002) bensonsung  (1002)     3424 2024-04-30 04:00:57.683949 streamlit_rec-0.0.4/PKG-INFO
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     3127 2024-04-30 03:59:37.000000 streamlit_rec-0.0.4/README.md
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       38 2024-04-30 04:00:57.683949 streamlit_rec-0.0.4/setup.cfg
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      670 2024-04-30 04:00:18.000000 streamlit_rec-0.0.4/setup.py
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 04:00:57.683949 streamlit_rec-0.0.4/streamlit_rec/
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       90 2024-04-30 03:19:08.000000 streamlit_rec-0.0.4/streamlit_rec/__init__.py
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 04:00:57.679949 streamlit_rec-0.0.4/streamlit_rec/frontend/
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 04:00:57.683949 streamlit_rec-0.0.4/streamlit_rec/frontend/build/
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      521 2024-04-30 02:03:50.000000 streamlit_rec-0.0.4/streamlit_rec/frontend/build/asset-manifest.json
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)   197412 2024-04-30 02:03:47.000000 streamlit_rec-0.0.4/streamlit_rec/frontend/build/bootstrap.min.css
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      500 2024-04-30 02:03:50.000000 streamlit_rec-0.0.4/streamlit_rec/frontend/build/index.html
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 04:00:57.679949 streamlit_rec-0.0.4/streamlit_rec/frontend/build/static/
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 04:00:57.683949 streamlit_rec-0.0.4/streamlit_rec/frontend/build/static/js/
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)    19699 2024-04-30 02:03:50.000000 streamlit_rec-0.0.4/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)    54687 2024-04-30 02:03:50.000000 streamlit_rec-0.0.4/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js.map
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     5652 2024-04-30 02:03:50.000000 streamlit_rec-0.0.4/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)    37989 2024-04-30 02:03:50.000000 streamlit_rec-0.0.4/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js.map
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)   395798 2024-04-30 02:03:50.000000 streamlit_rec-0.0.4/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     1693 2024-04-30 02:03:50.000000 streamlit_rec-0.0.4/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.LICENSE.txt
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)  1407755 2024-04-30 02:03:50.000000 streamlit_rec-0.0.4/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.map
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     1037 2024-04-30 02:55:07.000000 streamlit_rec-0.0.4/streamlit_rec/streamlit_rec.py
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 04:00:57.683949 streamlit_rec-0.0.4/streamlit_rec.egg-info/
+-rw-r--r--   0 bensonsung  (1002) bensonsung  (1002)     3424 2024-04-30 04:00:57.000000 streamlit_rec-0.0.4/streamlit_rec.egg-info/PKG-INFO
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      851 2024-04-30 04:00:57.000000 streamlit_rec-0.0.4/streamlit_rec.egg-info/SOURCES.txt
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)        1 2024-04-30 04:00:57.000000 streamlit_rec-0.0.4/streamlit_rec.egg-info/dependency_links.txt
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       28 2024-04-30 04:00:57.000000 streamlit_rec-0.0.4/streamlit_rec.egg-info/requires.txt
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       14 2024-04-30 04:00:57.000000 streamlit_rec-0.0.4/streamlit_rec.egg-info/top_level.txt
```

### Comparing `streamlit_rec-0.0.3/LICENSE` & `streamlit_rec-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.3/PKG-INFO` & `streamlit_rec-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_rec
-Version: 0.0.3
+Version: 0.0.4
 Summary: Audio recorder component for streamlit
 Home-page: 
 Author: Benson Sung
 Author-email: 
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -35,15 +35,15 @@
 
 On ubuntu/debian: `sudo apt update && sudo apt install ffmpeg`  
 On mac: `brew install ffmpeg`
 
 ### Usage:
 ```python
 import streamlit as st
-from audiorecorder import audiorecorder
+from streamlit_rec import audiorecorder
 
 st.title("Audio Recorder")
 audio = audiorecorder()
 
 if len(audio) > 0:
     # To play audio in frontend:
     st.audio(audio.export().read())
```

### Comparing `streamlit_rec-0.0.3/README.md` & `streamlit_rec-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 On ubuntu/debian: `sudo apt update && sudo apt install ffmpeg`  
 On mac: `brew install ffmpeg`
 
 ### Usage:
 ```python
 import streamlit as st
-from audiorecorder import audiorecorder
+from streamlit_rec import audiorecorder
 
 st.title("Audio Recorder")
 audio = audiorecorder()
 
 if len(audio) > 0:
     # To play audio in frontend:
     st.audio(audio.export().read())
```

### Comparing `streamlit_rec-0.0.3/setup.py` & `streamlit_rec-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="streamlit_rec",
-    version="0.0.3",
+    version="0.0.4",
     author="Benson Sung",
     author_email="",
     description="Audio recorder component for streamlit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_rec-0.0.3/streamlit_rec/frontend/build/asset-manifest.json` & `streamlit_rec-0.0.4/streamlit_rec/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.3/streamlit_rec/frontend/build/bootstrap.min.css` & `streamlit_rec-0.0.4/streamlit_rec/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js` & `streamlit_rec-0.0.4/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js.map` & `streamlit_rec-0.0.4/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js` & `streamlit_rec-0.0.4/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js.map` & `streamlit_rec-0.0.4/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js` & `streamlit_rec-0.0.4/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.LICENSE.txt` & `streamlit_rec-0.0.4/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.map` & `streamlit_rec-0.0.4/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.3/streamlit_rec/streamlit_rec.py` & `streamlit_rec-0.0.4/streamlit_rec/streamlit_rec.py`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.3/streamlit_rec.egg-info/PKG-INFO` & `streamlit_rec-0.0.4/streamlit_rec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_rec
-Version: 0.0.3
+Version: 0.0.4
 Summary: Audio recorder component for streamlit
 Home-page: 
 Author: Benson Sung
 Author-email: 
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -35,15 +35,15 @@
 
 On ubuntu/debian: `sudo apt update && sudo apt install ffmpeg`  
 On mac: `brew install ffmpeg`
 
 ### Usage:
 ```python
 import streamlit as st
-from audiorecorder import audiorecorder
+from streamlit_rec import audiorecorder
 
 st.title("Audio Recorder")
 audio = audiorecorder()
 
 if len(audio) > 0:
     # To play audio in frontend:
     st.audio(audio.export().read())
```

### Comparing `streamlit_rec-0.0.3/streamlit_rec.egg-info/SOURCES.txt` & `streamlit_rec-0.0.4/streamlit_rec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

