# Comparing `tmp/streamlit_rec-0.0.2.tar.gz` & `tmp/streamlit_rec-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_rec-0.0.2.tar", last modified: Tue Apr 30 03:24:26 2024, max compression
+gzip compressed data, was "streamlit_rec-0.0.3.tar", last modified: Tue Apr 30 03:58:16 2024, max compression
```

## Comparing `streamlit_rec-0.0.2.tar` & `streamlit_rec-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:24:26.897909 streamlit_rec-0.0.2/
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     1063 2024-04-26 08:04:38.000000 streamlit_rec-0.0.2/LICENSE
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       49 2024-04-26 08:04:38.000000 streamlit_rec-0.0.2/MANIFEST.in
--rw-r--r--   0 bensonsung  (1002) bensonsung  (1002)     3488 2024-04-30 03:24:26.897909 streamlit_rec-0.0.2/PKG-INFO
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     3192 2024-04-26 08:04:38.000000 streamlit_rec-0.0.2/README.md
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       38 2024-04-30 03:24:26.897909 streamlit_rec-0.0.2/setup.cfg
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      670 2024-04-30 03:24:13.000000 streamlit_rec-0.0.2/setup.py
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:24:26.897909 streamlit_rec-0.0.2/streamlit_rec/
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       90 2024-04-30 03:19:08.000000 streamlit_rec-0.0.2/streamlit_rec/__init__.py
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:24:26.897909 streamlit_rec-0.0.2/streamlit_rec/frontend/
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:24:26.897909 streamlit_rec-0.0.2/streamlit_rec/frontend/build/
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      521 2024-04-30 02:03:50.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/asset-manifest.json
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)   197412 2024-04-30 02:03:47.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/bootstrap.min.css
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      500 2024-04-30 02:03:50.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/index.html
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:24:26.897909 streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:24:26.897909 streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)    19699 2024-04-30 02:03:50.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)    54687 2024-04-30 02:03:50.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js.map
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     5652 2024-04-30 02:03:50.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)    37989 2024-04-30 02:03:50.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js.map
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)   395798 2024-04-30 02:03:50.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     1693 2024-04-30 02:03:50.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.LICENSE.txt
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)  1407755 2024-04-30 02:03:50.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.map
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     1037 2024-04-30 02:55:07.000000 streamlit_rec-0.0.2/streamlit_rec/streamlit_rec.py
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:24:26.897909 streamlit_rec-0.0.2/streamlit_rec.egg-info/
--rw-r--r--   0 bensonsung  (1002) bensonsung  (1002)     3488 2024-04-30 03:24:26.000000 streamlit_rec-0.0.2/streamlit_rec.egg-info/PKG-INFO
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      851 2024-04-30 03:24:26.000000 streamlit_rec-0.0.2/streamlit_rec.egg-info/SOURCES.txt
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)        1 2024-04-30 03:24:26.000000 streamlit_rec-0.0.2/streamlit_rec.egg-info/dependency_links.txt
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       28 2024-04-30 03:24:26.000000 streamlit_rec-0.0.2/streamlit_rec.egg-info/requires.txt
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       14 2024-04-30 03:24:26.000000 streamlit_rec-0.0.2/streamlit_rec.egg-info/top_level.txt
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:58:16.973737 streamlit_rec-0.0.3/
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     1063 2024-04-26 08:04:38.000000 streamlit_rec-0.0.3/LICENSE
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       49 2024-04-26 08:04:38.000000 streamlit_rec-0.0.3/MANIFEST.in
+-rw-r--r--   0 bensonsung  (1002) bensonsung  (1002)     3424 2024-04-30 03:58:16.973737 streamlit_rec-0.0.3/PKG-INFO
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     3127 2024-04-30 03:57:52.000000 streamlit_rec-0.0.3/README.md
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       38 2024-04-30 03:58:16.973737 streamlit_rec-0.0.3/setup.cfg
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      670 2024-04-30 03:58:10.000000 streamlit_rec-0.0.3/setup.py
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:58:16.973737 streamlit_rec-0.0.3/streamlit_rec/
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       90 2024-04-30 03:19:08.000000 streamlit_rec-0.0.3/streamlit_rec/__init__.py
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:58:16.973737 streamlit_rec-0.0.3/streamlit_rec/frontend/
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:58:16.973737 streamlit_rec-0.0.3/streamlit_rec/frontend/build/
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      521 2024-04-30 02:03:50.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/asset-manifest.json
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)   197412 2024-04-30 02:03:47.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/bootstrap.min.css
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      500 2024-04-30 02:03:50.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/index.html
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:58:16.973737 streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:58:16.973737 streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)    19699 2024-04-30 02:03:50.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)    54687 2024-04-30 02:03:50.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js.map
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     5652 2024-04-30 02:03:50.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)    37989 2024-04-30 02:03:50.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js.map
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)   395798 2024-04-30 02:03:50.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     1693 2024-04-30 02:03:50.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.LICENSE.txt
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)  1407755 2024-04-30 02:03:50.000000 streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.map
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     1037 2024-04-30 02:55:07.000000 streamlit_rec-0.0.3/streamlit_rec/streamlit_rec.py
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:58:16.973737 streamlit_rec-0.0.3/streamlit_rec.egg-info/
+-rw-r--r--   0 bensonsung  (1002) bensonsung  (1002)     3424 2024-04-30 03:58:16.000000 streamlit_rec-0.0.3/streamlit_rec.egg-info/PKG-INFO
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      851 2024-04-30 03:58:16.000000 streamlit_rec-0.0.3/streamlit_rec.egg-info/SOURCES.txt
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)        1 2024-04-30 03:58:16.000000 streamlit_rec-0.0.3/streamlit_rec.egg-info/dependency_links.txt
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       28 2024-04-30 03:58:16.000000 streamlit_rec-0.0.3/streamlit_rec.egg-info/requires.txt
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       14 2024-04-30 03:58:16.000000 streamlit_rec-0.0.3/streamlit_rec.egg-info/top_level.txt
```

### Comparing `streamlit_rec-0.0.2/LICENSE` & `streamlit_rec-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.2/PKG-INFO` & `streamlit_rec-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_rec
-Version: 0.0.2
+Version: 0.0.3
 Summary: Audio recorder component for streamlit
 Home-page: 
 Author: Benson Sung
 Author-email: 
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,43 +17,36 @@
 ### An audio Recorder for streamlit
 
 #### Description
 Audio recorder component for streamlit.  
 It creates a button to start the recording and takes three arguments: the start button text, the stop button text, and the pause button text.  
 If the pause button text is not specified, the pause button is not displayed.
 
-#### Parameters
-The signature of the component is:
-```python
-audiorecorder(start_prompt="Start recording", stop_prompt="Stop recording", pause_prompt="", key=None):
-```
-The prompt parameters are self-explanatory, and the optionnal `key` parameter is used internally by streamlit to properly distinguish multiple audiorecorders on the page.
-
 #### Return value
 The component's return value is a [pydub](https://github.com/jiaaro/pydub/) [`AudioSegment`](https://github.com/jiaaro/pydub/blob/master/API.markdown#audiosegment).  
 All `AudioSegment` methods are available, in particular you can:
 - Play the audio in the frontend with `st.audio(audio.export().read())`
 - Save the audio to a file with `audio.export("audio.wav", format="wav")`
 
 ### Installation:
 ```bash
-pip install streamlit-audiorecorder
+pip install streamlit_rec
 ```
 Note: This package uses ffmpeg, so it should be installed for this audiorecorder to work properly.
 
 On ubuntu/debian: `sudo apt update && sudo apt install ffmpeg`  
 On mac: `brew install ffmpeg`
 
 ### Usage:
 ```python
 import streamlit as st
 from audiorecorder import audiorecorder
 
 st.title("Audio Recorder")
-audio = audiorecorder("Click to record", "Click to stop recording")
+audio = audiorecorder()
 
 if len(audio) > 0:
     # To play audio in frontend:
     st.audio(audio.export().read())  
 
     # To save audio to a file, use pydub export method:
     audio.export("audio.wav", format="wav")
@@ -76,8 +69,20 @@
 
 > As an API that may involve significant privacy concerns, getUserMedia()'s specification lays out a wide array of privacy and security requirements that browsers are obligated to meet.
 > 
 > getUserMedia() is a powerful feature that can only be used in secure contexts; in insecure contexts, navigator.mediaDevices is undefined, preventing access to getUserMedia(). A secure context is, in short, a page loaded using HTTPS or the file:/// URL scheme, or a page loaded from localhost.
 
 **Solution**: Serve your website using HTTPS. If you are serving your website locally, make sure to access it using `localhost`, not an IP address.
 
+Just solved this problem.
 
+1.Generate temporary SSL authentication
+```console
+openssl genrsa 2048 > host.key
+chmod 400 host.key
+openssl req -new -x509 -nodes -sha256 -days 365 -key host.key -out host.cert
+```
+
+2.streamlit run with https
+```console
+streamlit run xx.py --server.sslCertFile host.cert --server.sslKeyFile=host.key
+```
```

### Comparing `streamlit_rec-0.0.2/README.md` & `streamlit_rec-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -4,43 +4,36 @@
 ### An audio Recorder for streamlit
 
 #### Description
 Audio recorder component for streamlit.  
 It creates a button to start the recording and takes three arguments: the start button text, the stop button text, and the pause button text.  
 If the pause button text is not specified, the pause button is not displayed.
 
-#### Parameters
-The signature of the component is:
-```python
-audiorecorder(start_prompt="Start recording", stop_prompt="Stop recording", pause_prompt="", key=None):
-```
-The prompt parameters are self-explanatory, and the optionnal `key` parameter is used internally by streamlit to properly distinguish multiple audiorecorders on the page.
-
 #### Return value
 The component's return value is a [pydub](https://github.com/jiaaro/pydub/) [`AudioSegment`](https://github.com/jiaaro/pydub/blob/master/API.markdown#audiosegment).  
 All `AudioSegment` methods are available, in particular you can:
 - Play the audio in the frontend with `st.audio(audio.export().read())`
 - Save the audio to a file with `audio.export("audio.wav", format="wav")`
 
 ### Installation:
 ```bash
-pip install streamlit-audiorecorder
+pip install streamlit_rec
 ```
 Note: This package uses ffmpeg, so it should be installed for this audiorecorder to work properly.
 
 On ubuntu/debian: `sudo apt update && sudo apt install ffmpeg`  
 On mac: `brew install ffmpeg`
 
 ### Usage:
 ```python
 import streamlit as st
 from audiorecorder import audiorecorder
 
 st.title("Audio Recorder")
-audio = audiorecorder("Click to record", "Click to stop recording")
+audio = audiorecorder()
 
 if len(audio) > 0:
     # To play audio in frontend:
     st.audio(audio.export().read())  
 
     # To save audio to a file, use pydub export method:
     audio.export("audio.wav", format="wav")
@@ -63,8 +56,20 @@
 
 > As an API that may involve significant privacy concerns, getUserMedia()'s specification lays out a wide array of privacy and security requirements that browsers are obligated to meet.
 > 
 > getUserMedia() is a powerful feature that can only be used in secure contexts; in insecure contexts, navigator.mediaDevices is undefined, preventing access to getUserMedia(). A secure context is, in short, a page loaded using HTTPS or the file:/// URL scheme, or a page loaded from localhost.
 
 **Solution**: Serve your website using HTTPS. If you are serving your website locally, make sure to access it using `localhost`, not an IP address.
 
+Just solved this problem.
+
+1.Generate temporary SSL authentication
+```console
+openssl genrsa 2048 > host.key
+chmod 400 host.key
+openssl req -new -x509 -nodes -sha256 -days 365 -key host.key -out host.cert
+```
 
+2.streamlit run with https
+```console
+streamlit run xx.py --server.sslCertFile host.cert --server.sslKeyFile=host.key
+```
```

### Comparing `streamlit_rec-0.0.2/setup.py` & `streamlit_rec-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="streamlit_rec",
-    version="0.0.2",
+    version="0.0.3",
     author="Benson Sung",
     author_email="",
     description="Audio recorder component for streamlit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_rec-0.0.2/streamlit_rec/frontend/build/asset-manifest.json` & `streamlit_rec-0.0.3/streamlit_rec/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.2/streamlit_rec/frontend/build/bootstrap.min.css` & `streamlit_rec-0.0.3/streamlit_rec/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js` & `streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js.map` & `streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js` & `streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js.map` & `streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js` & `streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.LICENSE.txt` & `streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.map` & `streamlit_rec-0.0.3/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.2/streamlit_rec/streamlit_rec.py` & `streamlit_rec-0.0.3/streamlit_rec/streamlit_rec.py`

 * *Files identical despite different names*

### Comparing `streamlit_rec-0.0.2/streamlit_rec.egg-info/PKG-INFO` & `streamlit_rec-0.0.3/streamlit_rec.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_rec
-Version: 0.0.2
+Version: 0.0.3
 Summary: Audio recorder component for streamlit
 Home-page: 
 Author: Benson Sung
 Author-email: 
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,43 +17,36 @@
 ### An audio Recorder for streamlit
 
 #### Description
 Audio recorder component for streamlit.  
 It creates a button to start the recording and takes three arguments: the start button text, the stop button text, and the pause button text.  
 If the pause button text is not specified, the pause button is not displayed.
 
-#### Parameters
-The signature of the component is:
-```python
-audiorecorder(start_prompt="Start recording", stop_prompt="Stop recording", pause_prompt="", key=None):
-```
-The prompt parameters are self-explanatory, and the optionnal `key` parameter is used internally by streamlit to properly distinguish multiple audiorecorders on the page.
-
 #### Return value
 The component's return value is a [pydub](https://github.com/jiaaro/pydub/) [`AudioSegment`](https://github.com/jiaaro/pydub/blob/master/API.markdown#audiosegment).  
 All `AudioSegment` methods are available, in particular you can:
 - Play the audio in the frontend with `st.audio(audio.export().read())`
 - Save the audio to a file with `audio.export("audio.wav", format="wav")`
 
 ### Installation:
 ```bash
-pip install streamlit-audiorecorder
+pip install streamlit_rec
 ```
 Note: This package uses ffmpeg, so it should be installed for this audiorecorder to work properly.
 
 On ubuntu/debian: `sudo apt update && sudo apt install ffmpeg`  
 On mac: `brew install ffmpeg`
 
 ### Usage:
 ```python
 import streamlit as st
 from audiorecorder import audiorecorder
 
 st.title("Audio Recorder")
-audio = audiorecorder("Click to record", "Click to stop recording")
+audio = audiorecorder()
 
 if len(audio) > 0:
     # To play audio in frontend:
     st.audio(audio.export().read())  
 
     # To save audio to a file, use pydub export method:
     audio.export("audio.wav", format="wav")
@@ -76,8 +69,20 @@
 
 > As an API that may involve significant privacy concerns, getUserMedia()'s specification lays out a wide array of privacy and security requirements that browsers are obligated to meet.
 > 
 > getUserMedia() is a powerful feature that can only be used in secure contexts; in insecure contexts, navigator.mediaDevices is undefined, preventing access to getUserMedia(). A secure context is, in short, a page loaded using HTTPS or the file:/// URL scheme, or a page loaded from localhost.
 
 **Solution**: Serve your website using HTTPS. If you are serving your website locally, make sure to access it using `localhost`, not an IP address.
 
+Just solved this problem.
 
+1.Generate temporary SSL authentication
+```console
+openssl genrsa 2048 > host.key
+chmod 400 host.key
+openssl req -new -x509 -nodes -sha256 -days 365 -key host.key -out host.cert
+```
+
+2.streamlit run with https
+```console
+streamlit run xx.py --server.sslCertFile host.cert --server.sslKeyFile=host.key
+```
```

### Comparing `streamlit_rec-0.0.2/streamlit_rec.egg-info/SOURCES.txt` & `streamlit_rec-0.0.3/streamlit_rec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

