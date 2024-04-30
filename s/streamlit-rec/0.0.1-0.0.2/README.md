# Comparing `tmp/streamlit-rec-0.0.1.tar.gz` & `tmp/streamlit_rec-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-rec-0.0.1.tar", last modified: Tue Apr 30 02:08:47 2024, max compression
+gzip compressed data, was "streamlit_rec-0.0.2.tar", last modified: Tue Apr 30 03:24:26 2024, max compression
```

## Comparing `streamlit-rec-0.0.1.tar` & `streamlit_rec-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 02:08:47.540437 streamlit-rec-0.0.1/
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     1063 2024-04-26 08:04:38.000000 streamlit-rec-0.0.1/LICENSE
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       49 2024-04-26 08:04:38.000000 streamlit-rec-0.0.1/MANIFEST.in
--rw-r--r--   0 bensonsung  (1002) bensonsung  (1002)     3488 2024-04-30 02:08:47.540437 streamlit-rec-0.0.1/PKG-INFO
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     3192 2024-04-26 08:04:38.000000 streamlit-rec-0.0.1/README.md
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 02:08:47.540437 streamlit-rec-0.0.1/audiorecorder/
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     1700 2024-04-30 02:00:20.000000 streamlit-rec-0.0.1/audiorecorder/__init__.py
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 02:08:47.540437 streamlit-rec-0.0.1/audiorecorder/frontend/
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 02:08:47.540437 streamlit-rec-0.0.1/audiorecorder/frontend/build/
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      521 2024-04-30 02:03:50.000000 streamlit-rec-0.0.1/audiorecorder/frontend/build/asset-manifest.json
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)   197412 2024-04-30 02:03:47.000000 streamlit-rec-0.0.1/audiorecorder/frontend/build/bootstrap.min.css
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      500 2024-04-30 02:03:50.000000 streamlit-rec-0.0.1/audiorecorder/frontend/build/index.html
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 02:08:47.540437 streamlit-rec-0.0.1/audiorecorder/frontend/build/static/
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 02:08:47.540437 streamlit-rec-0.0.1/audiorecorder/frontend/build/static/js/
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)    19699 2024-04-30 02:03:50.000000 streamlit-rec-0.0.1/audiorecorder/frontend/build/static/js/538.ed8de53c.chunk.js
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)    54687 2024-04-30 02:03:50.000000 streamlit-rec-0.0.1/audiorecorder/frontend/build/static/js/538.ed8de53c.chunk.js.map
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     5652 2024-04-30 02:03:50.000000 streamlit-rec-0.0.1/audiorecorder/frontend/build/static/js/850.047e6c02.chunk.js
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)    37989 2024-04-30 02:03:50.000000 streamlit-rec-0.0.1/audiorecorder/frontend/build/static/js/850.047e6c02.chunk.js.map
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)   395798 2024-04-30 02:03:50.000000 streamlit-rec-0.0.1/audiorecorder/frontend/build/static/js/main.c28cbcfe.js
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     1693 2024-04-30 02:03:50.000000 streamlit-rec-0.0.1/audiorecorder/frontend/build/static/js/main.c28cbcfe.js.LICENSE.txt
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)  1407755 2024-04-30 02:03:50.000000 streamlit-rec-0.0.1/audiorecorder/frontend/build/static/js/main.c28cbcfe.js.map
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       38 2024-04-30 02:08:47.540437 streamlit-rec-0.0.1/setup.cfg
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      567 2024-04-30 02:07:47.000000 streamlit-rec-0.0.1/setup.py
-drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 02:08:47.540437 streamlit-rec-0.0.1/streamlit_rec.egg-info/
--rw-r--r--   0 bensonsung  (1002) bensonsung  (1002)     3488 2024-04-30 02:08:47.000000 streamlit-rec-0.0.1/streamlit_rec.egg-info/PKG-INFO
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      820 2024-04-30 02:08:47.000000 streamlit-rec-0.0.1/streamlit_rec.egg-info/SOURCES.txt
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)        1 2024-04-30 02:08:47.000000 streamlit-rec-0.0.1/streamlit_rec.egg-info/dependency_links.txt
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       28 2024-04-30 02:08:47.000000 streamlit-rec-0.0.1/streamlit_rec.egg-info/requires.txt
--rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       14 2024-04-30 02:08:47.000000 streamlit-rec-0.0.1/streamlit_rec.egg-info/top_level.txt
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:24:26.897909 streamlit_rec-0.0.2/
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     1063 2024-04-26 08:04:38.000000 streamlit_rec-0.0.2/LICENSE
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       49 2024-04-26 08:04:38.000000 streamlit_rec-0.0.2/MANIFEST.in
+-rw-r--r--   0 bensonsung  (1002) bensonsung  (1002)     3488 2024-04-30 03:24:26.897909 streamlit_rec-0.0.2/PKG-INFO
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     3192 2024-04-26 08:04:38.000000 streamlit_rec-0.0.2/README.md
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       38 2024-04-30 03:24:26.897909 streamlit_rec-0.0.2/setup.cfg
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      670 2024-04-30 03:24:13.000000 streamlit_rec-0.0.2/setup.py
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:24:26.897909 streamlit_rec-0.0.2/streamlit_rec/
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       90 2024-04-30 03:19:08.000000 streamlit_rec-0.0.2/streamlit_rec/__init__.py
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:24:26.897909 streamlit_rec-0.0.2/streamlit_rec/frontend/
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:24:26.897909 streamlit_rec-0.0.2/streamlit_rec/frontend/build/
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      521 2024-04-30 02:03:50.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/asset-manifest.json
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)   197412 2024-04-30 02:03:47.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/bootstrap.min.css
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      500 2024-04-30 02:03:50.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/index.html
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:24:26.897909 streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:24:26.897909 streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)    19699 2024-04-30 02:03:50.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)    54687 2024-04-30 02:03:50.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js.map
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     5652 2024-04-30 02:03:50.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)    37989 2024-04-30 02:03:50.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js.map
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)   395798 2024-04-30 02:03:50.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     1693 2024-04-30 02:03:50.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.LICENSE.txt
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)  1407755 2024-04-30 02:03:50.000000 streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.map
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)     1037 2024-04-30 02:55:07.000000 streamlit_rec-0.0.2/streamlit_rec/streamlit_rec.py
+drwxrwxr-x   0 bensonsung  (1002) bensonsung  (1002)        0 2024-04-30 03:24:26.897909 streamlit_rec-0.0.2/streamlit_rec.egg-info/
+-rw-r--r--   0 bensonsung  (1002) bensonsung  (1002)     3488 2024-04-30 03:24:26.000000 streamlit_rec-0.0.2/streamlit_rec.egg-info/PKG-INFO
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)      851 2024-04-30 03:24:26.000000 streamlit_rec-0.0.2/streamlit_rec.egg-info/SOURCES.txt
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)        1 2024-04-30 03:24:26.000000 streamlit_rec-0.0.2/streamlit_rec.egg-info/dependency_links.txt
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       28 2024-04-30 03:24:26.000000 streamlit_rec-0.0.2/streamlit_rec.egg-info/requires.txt
+-rw-rw-r--   0 bensonsung  (1002) bensonsung  (1002)       14 2024-04-30 03:24:26.000000 streamlit_rec-0.0.2/streamlit_rec.egg-info/top_level.txt
```

### Comparing `streamlit-rec-0.0.1/LICENSE` & `streamlit_rec-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-rec-0.0.1/PKG-INFO` & `streamlit_rec-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: streamlit-rec
-Version: 0.0.1
+Name: streamlit_rec
+Version: 0.0.2
 Summary: Audio recorder component for streamlit
 Home-page: 
 Author: Benson Sung
 Author-email: 
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-rec-0.0.1/README.md` & `streamlit_rec-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-rec-0.0.1/audiorecorder/frontend/build/asset-manifest.json` & `streamlit_rec-0.0.2/streamlit_rec/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-rec-0.0.1/audiorecorder/frontend/build/bootstrap.min.css` & `streamlit_rec-0.0.2/streamlit_rec/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-rec-0.0.1/audiorecorder/frontend/build/static/js/538.ed8de53c.chunk.js` & `streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-rec-0.0.1/audiorecorder/frontend/build/static/js/538.ed8de53c.chunk.js.map` & `streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/538.ed8de53c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-rec-0.0.1/audiorecorder/frontend/build/static/js/850.047e6c02.chunk.js` & `streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-rec-0.0.1/audiorecorder/frontend/build/static/js/850.047e6c02.chunk.js.map` & `streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/850.047e6c02.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-rec-0.0.1/audiorecorder/frontend/build/static/js/main.c28cbcfe.js` & `streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js`

 * *Files identical despite different names*

### Comparing `streamlit-rec-0.0.1/audiorecorder/frontend/build/static/js/main.c28cbcfe.js.LICENSE.txt` & `streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-rec-0.0.1/audiorecorder/frontend/build/static/js/main.c28cbcfe.js.map` & `streamlit_rec-0.0.2/streamlit_rec/frontend/build/static/js/main.c28cbcfe.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-rec-0.0.1/streamlit_rec.egg-info/PKG-INFO` & `streamlit_rec-0.0.2/streamlit_rec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: streamlit-rec
-Version: 0.0.1
+Name: streamlit_rec
+Version: 0.0.2
 Summary: Audio recorder component for streamlit
 Home-page: 
 Author: Benson Sung
 Author-email: 
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

