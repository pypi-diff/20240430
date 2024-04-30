# Comparing `tmp/ocp_vscode-2.3.1.tar.gz` & `tmp/ocp_vscode-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_vscode-2.3.1.tar", last modified: Mon Apr 22 06:43:09 2024, max compression
+gzip compressed data, was "ocp_vscode-2.3.2.tar", last modified: Tue Apr 30 16:43:01 2024, max compression
```

## Comparing `ocp_vscode-2.3.1.tar` & `ocp_vscode-2.3.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-22 06:43:09.263153 ocp_vscode-2.3.1/
--rw-r--r--   0 bernhard   (501) staff       (20)    10938 2022-10-05 06:47:11.000000 ocp_vscode-2.3.1/LICENSE
--rw-r--r--   0 bernhard   (501) staff       (20)      959 2024-04-22 06:43:09.263078 ocp_vscode-2.3.1/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)    12982 2024-04-20 11:59:28.000000 ocp_vscode-2.3.1/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-22 06:43:09.261775 ocp_vscode-2.3.1/ocp_vscode/
--rw-r--r--   0 bernhard   (501) staff       (20)     1332 2024-04-20 15:35:45.000000 ocp_vscode-2.3.1/ocp_vscode/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     4972 2024-01-16 17:49:02.000000 ocp_vscode-2.3.1/ocp_vscode/animation.py
--rw-r--r--   0 bernhard   (501) staff       (20)    14216 2024-01-16 17:49:02.000000 ocp_vscode-2.3.1/ocp_vscode/backend.py
--rw-r--r--   0 bernhard   (501) staff       (20)    19453 2024-01-16 17:49:02.000000 ocp_vscode-2.3.1/ocp_vscode/build123d.py
--rw-r--r--   0 bernhard   (501) staff       (20)    19488 2024-01-16 17:49:02.000000 ocp_vscode-2.3.1/ocp_vscode/colors.py
--rw-r--r--   0 bernhard   (501) staff       (20)     8166 2024-04-20 15:33:55.000000 ocp_vscode-2.3.1/ocp_vscode/comms.py
--rw-r--r--   0 bernhard   (501) staff       (20)    16326 2024-04-16 20:13:23.000000 ocp_vscode-2.3.1/ocp_vscode/config.py
--rw-r--r--   0 bernhard   (501) staff       (20)    32313 2024-04-20 17:15:29.000000 ocp_vscode-2.3.1/ocp_vscode/show.py
--rw-r--r--   0 bernhard   (501) staff       (20)     5024 2024-01-16 17:49:02.000000 ocp_vscode-2.3.1/ocp_vscode/state.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-22 06:43:09.262883 ocp_vscode-2.3.1/ocp_vscode.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      959 2024-04-22 06:43:09.000000 ocp_vscode-2.3.1/ocp_vscode.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      479 2024-04-22 06:43:09.000000 ocp_vscode-2.3.1/ocp_vscode.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-04-22 06:43:09.000000 ocp_vscode-2.3.1/ocp_vscode.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-04-22 06:43:09.000000 ocp_vscode-2.3.1/ocp_vscode.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)       78 2024-04-22 06:43:09.000000 ocp_vscode-2.3.1/ocp_vscode.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       11 2024-04-22 06:43:09.000000 ocp_vscode-2.3.1/ocp_vscode.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)     1038 2024-04-22 06:43:09.263406 ocp_vscode-2.3.1/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1227 2024-04-20 12:06:41.000000 ocp_vscode-2.3.1/setup.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-22 06:43:09.262722 ocp_vscode-2.3.1/test/
--rw-r--r--   0 bernhard   (501) staff       (20)      401 2023-11-24 07:13:36.000000 ocp_vscode-2.3.1/test/test_for_backend.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1890 2023-11-24 07:13:36.000000 ocp_vscode-2.3.1/test/testextension.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-30 16:43:01.284750 ocp_vscode-2.3.2/
+-rw-r--r--   0 bernhard   (501) staff       (20)    10938 2022-10-05 06:47:11.000000 ocp_vscode-2.3.2/LICENSE
+-rw-r--r--   0 bernhard   (501) staff       (20)      953 2024-04-30 16:43:01.284638 ocp_vscode-2.3.2/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)    13294 2024-04-25 06:14:35.000000 ocp_vscode-2.3.2/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-30 16:43:01.282772 ocp_vscode-2.3.2/ocp_vscode/
+-rw-r--r--   0 bernhard   (501) staff       (20)     1332 2024-04-25 06:11:21.000000 ocp_vscode-2.3.2/ocp_vscode/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4972 2024-01-16 17:49:02.000000 ocp_vscode-2.3.2/ocp_vscode/animation.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    14216 2024-01-16 17:49:02.000000 ocp_vscode-2.3.2/ocp_vscode/backend.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    19453 2024-01-16 17:49:02.000000 ocp_vscode-2.3.2/ocp_vscode/build123d.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    19488 2024-01-16 17:49:02.000000 ocp_vscode-2.3.2/ocp_vscode/colors.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     8321 2024-04-25 16:56:31.000000 ocp_vscode-2.3.2/ocp_vscode/comms.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    16326 2024-04-16 20:13:23.000000 ocp_vscode-2.3.2/ocp_vscode/config.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     6498 2024-04-25 17:25:05.000000 ocp_vscode-2.3.2/ocp_vscode/daemonize.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    32313 2024-04-20 17:15:29.000000 ocp_vscode-2.3.2/ocp_vscode/show.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     5024 2024-01-16 17:49:02.000000 ocp_vscode-2.3.2/ocp_vscode/state.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-30 16:43:01.284340 ocp_vscode-2.3.2/ocp_vscode.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      953 2024-04-30 16:43:01.000000 ocp_vscode-2.3.2/ocp_vscode.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      503 2024-04-30 16:43:01.000000 ocp_vscode-2.3.2/ocp_vscode.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-04-30 16:43:01.000000 ocp_vscode-2.3.2/ocp_vscode.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-04-30 16:43:01.000000 ocp_vscode-2.3.2/ocp_vscode.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)       72 2024-04-30 16:43:01.000000 ocp_vscode-2.3.2/ocp_vscode.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       11 2024-04-30 16:43:01.000000 ocp_vscode-2.3.2/ocp_vscode.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)     1038 2024-04-30 16:43:01.285161 ocp_vscode-2.3.2/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1221 2024-04-25 16:53:47.000000 ocp_vscode-2.3.2/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-30 16:43:01.284111 ocp_vscode-2.3.2/test/
+-rw-r--r--   0 bernhard   (501) staff       (20)      401 2023-11-24 07:13:36.000000 ocp_vscode-2.3.2/test/test_for_backend.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1890 2023-11-24 07:13:36.000000 ocp_vscode-2.3.2/test/testextension.py
```

### Comparing `ocp_vscode-2.3.1/LICENSE` & `ocp_vscode-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.3.1/PKG-INFO` & `ocp_vscode-2.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_vscode
-Version: 2.3.1
+Version: 2.3.2
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
@@ -17,10 +17,10 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: ocp-tessellate<2.4.0,>=2.3.2
 Requires-Dist: requests
 Requires-Dist: ipykernel
 Requires-Dist: orjson
-Requires-Dist: websockets<11.1,>=11.0
+Requires-Dist: websockets>=12.0
 
 An extension to show OCP cad CAD objects (CadQuery, build123d) in VS Code via threejs
```

### Comparing `ocp_vscode-2.3.1/README.md` & `ocp_vscode-2.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 -   To use OCP CAD Viewer, start VS Code from the commandline in the Python environment you want to use or select the right Python interpreter in VS Code first. **OCP CAD Viewer depends on VS Code using the right Python interpreter** (i.e. mamba / conda / pyenv / poetry / ... environment).
 -   For VSCodium, the extension is not available in the VS code market place. You need to download the the vsix file from the [release folder](https://github.com/bernhard-42/vscode-ocp-cad-viewer/releases) and install it manually.
 -   Currently, on a Silicon Mac (ARM CPU), _OCP_ and _CadQuery_ can only be installed via `mamba`, see 3. below.
 
 ### Installation
 
-1. Open the VS Code Marketplace, and search and install _OCP CAD Viewer 2.2.1_.
+1. Open the VS Code Marketplace, and search and install _OCP CAD Viewer 2.3.2_.
 
     Afterwards the OCP viewer is available in the VS Code sidebar:
 
     ![](screenshots/ocp_icon.png)
 
 2. Clicking on it shows the OCP CAD Viewer UI with the viewer manager and the library manager:
 
@@ -198,22 +198,26 @@
 ```bash
 NATIVE_TESSELLATOR=0 OCP_VSCODE_PYTEST=1 pytest -v -s pytests/
 NATIVE_TESSELLATOR=1 OCP_VSCODE_PYTEST=1 pytest -v -s pytests/
 ```
 
 ## Changes
 
+v2.3.2
+- Fix regression that Python script hang in threading before exit ([#73](https://github.com/bernhard-42/vscode-ocp-cad-viewer/issues/60))
+
 v2.3.1
 - Add latest ocp-tessellate to fixed regression with handling instances
 - Make native default if ocp-addons exists
 
 v2.3.0
-- Add newest ocp-tessellate to allow using native tessellator from ocp_addons
-- Fine tune communication to ensure the memory view of buffers will be passed through to javascript for performance
-- Use of the new protocol v3 of three-cad-viewer
+Fine tune communication to ensure the memory view of buffers will be passed through to javascript for performance (*)
+Use of the new protocol v3 of three-cad-viewer
+Fix show_all regressions https://github.com/bernhard-42/vscode-ocp-cad-viewer/issues/71. It should also properly catch exceptions now to not interrupt viausl debugging
+Add newest ocp-tessellate to allow using native tessellator from ocp_addons
 
 v2.2.2
 - Fix regression in measure tools
 
 v2.2.1
 -   Fix: Wrong back material color for faces
 -   Improve parameters of Imageface
```

### Comparing `ocp_vscode-2.3.1/ocp_vscode/__init__.py` & `ocp_vscode-2.3.2/ocp_vscode/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "2.3.1"
+__version__ = "2.3.2"
 
 import os
 
 from .show import *
 from .config import *
 from .comms import *
```

### Comparing `ocp_vscode-2.3.1/ocp_vscode/animation.py` & `ocp_vscode-2.3.2/ocp_vscode/animation.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.3.1/ocp_vscode/backend.py` & `ocp_vscode-2.3.2/ocp_vscode/backend.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.3.1/ocp_vscode/build123d.py` & `ocp_vscode-2.3.2/ocp_vscode/build123d.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.3.1/ocp_vscode/colors.py` & `ocp_vscode-2.3.2/ocp_vscode/colors.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.3.1/ocp_vscode/comms.py` & `ocp_vscode-2.3.2/ocp_vscode/comms.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 import enum
 import json
 import os
 import socket
 
 from pathlib import Path
 
-from websockets.sync.client import connect
+# TODO:
+# As soon as websockets 12.1 is released, replace with
+#   "from websockets.sync.client import connect"
+from .daemonize import connect
 
 import orjson
 from ocp_tessellate.utils import Timer
 from ocp_tessellate.ocp_utils import (
     is_topods_shape,
     is_toploc_location,
     serialize,
@@ -30,15 +33,15 @@
 except:  # pylint: disable=bare-except
     JCONSOLE = False
 
 CMD_URL = "ws://127.0.0.1"
 CMD_PORT = 3939
 
 INIT_DONE = False
-
+WS = None
 
 #
 # Send data to the viewer
 #
 
 
 class MessageType(enum.IntEnum):
@@ -106,14 +109,16 @@
     global CMD_PORT, INIT_DONE  # pylint: disable=global-statement
     CMD_PORT = port
     INIT_DONE = True
 
 
 def _send(data, message_type, port=None, timeit=False):
     """Send data to the viewer"""
+    global WS
+
     if port is None:
         if not INIT_DONE:
             find_and_set_port()
             set_connection_file()
         port = CMD_PORT
     try:
         with Timer(timeit, "", "json dumps", 1):
@@ -128,21 +133,22 @@
                 j = b"B:" + j
             elif message_type == MessageType.BACKEND_RESPONSE:
                 j = b"R:" + j
             elif message_type == MessageType.CONFIG:
                 j = b"S:" + j
 
         with Timer(timeit, "", f"websocket send {len(j)/1024/1024:.3f} MB", 1):
-            ws = connect(f"{CMD_URL}:{port}")
-            ws.send(j)
+            if WS is None:
+                WS = connect(f"{CMD_URL}:{port}")
+            WS.send(j)
 
             result = None
             if message_type == MessageType.COMMAND:
                 try:
-                    result = json.loads(ws.recv())
+                    result = json.loads(WS.recv())
                 except Exception as ex:  # pylint: disable=broad-except
                     print(ex)
 
             # try:
             #     ws.close()
             # except Exception as ex:  # pylint: disable=bare-except
             #     pass
```

### Comparing `ocp_vscode-2.3.1/ocp_vscode/config.py` & `ocp_vscode-2.3.2/ocp_vscode/config.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.3.1/ocp_vscode/show.py` & `ocp_vscode-2.3.2/ocp_vscode/show.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.3.1/ocp_vscode/state.py` & `ocp_vscode-2.3.2/ocp_vscode/state.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-2.3.1/ocp_vscode.egg-info/PKG-INFO` & `ocp_vscode-2.3.2/ocp_vscode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_vscode
-Version: 2.3.1
+Version: 2.3.2
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
@@ -17,10 +17,10 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: ocp-tessellate<2.4.0,>=2.3.2
 Requires-Dist: requests
 Requires-Dist: ipykernel
 Requires-Dist: orjson
-Requires-Dist: websockets<11.1,>=11.0
+Requires-Dist: websockets>=12.0
 
 An extension to show OCP cad CAD objects (CadQuery, build123d) in VS Code via threejs
```

### Comparing `ocp_vscode-2.3.1/setup.cfg` & `ocp_vscode-2.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.3.1
+current_version = 2.3.2
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_vscode-2.3.1/setup.py` & `ocp_vscode-2.3.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup_args = {
     "name": "ocp_vscode",
-    "version": "2.3.1",
+    "version": "2.3.2",
     "description": "OCP CAD Viewer for VSCode",
     "long_description": "An extension to show OCP cad CAD objects (CadQuery, build123d) in VS Code via threejs",
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": [
         "ocp-tessellate>=2.3.2,<2.4.0",
         "requests",
         "ipykernel",
         "orjson",
-        "websockets>=11.0,<11.1",
+        "websockets>=12.0",
     ],
     "packages": find_packages(),
     "zip_safe": False,
     "author": "Bernhard Walter",
     "author_email": "b_walter@arcor.de",
     "url": "https://github.com/bernhard-42/vscode-ocp-cad-viewer",
     "keywords": ["vscode", "widgets", "CAD", "cadquery"],
```

### Comparing `ocp_vscode-2.3.1/test/testextension.py` & `ocp_vscode-2.3.2/test/testextension.py`

 * *Files identical despite different names*

