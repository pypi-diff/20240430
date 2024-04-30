# Comparing `tmp/star_dresden_gs_lib-0.1.2.tar.gz` & `tmp/star_dresden_gs_lib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "star_dresden_gs_lib-0.1.2.tar", last modified: Wed Mar 20 20:20:53 2024, max compression
+gzip compressed data, was "star_dresden_gs_lib-0.2.0.tar", last modified: Tue Apr 30 17:57:14 2024, max compression
```

## Comparing `star_dresden_gs_lib-0.1.2.tar` & `star_dresden_gs_lib-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxrwxrwx   0 sners03   (1000) sners03   (1000)        0 2024-03-20 20:20:53.831028 star_dresden_gs_lib-0.1.2/
--rwxrwxrwx   0 sners03   (1000) sners03   (1000)     1098 2024-03-18 18:54:01.000000 star_dresden_gs_lib-0.1.2/LICENSE.txt
--rwxrwxrwx   0 sners03   (1000) sners03   (1000)     2080 2024-03-20 20:20:53.823024 star_dresden_gs_lib-0.1.2/PKG-INFO
--rwxrwxrwx   0 sners03   (1000) sners03   (1000)     1503 2024-03-20 16:48:30.000000 star_dresden_gs_lib-0.1.2/README.md
--rwxrwxrwx   0 sners03   (1000) sners03   (1000)      637 2024-03-20 20:20:05.000000 star_dresden_gs_lib-0.1.2/pyproject.toml
--rwxrwxrwx   0 sners03   (1000) sners03   (1000)       78 2024-03-20 20:20:53.842050 star_dresden_gs_lib-0.1.2/setup.cfg
--rwxrwxrwx   0 sners03   (1000) sners03   (1000)     2584 2024-03-20 20:20:05.000000 star_dresden_gs_lib-0.1.2/setup.py
-drwxrwxrwx   0 sners03   (1000) sners03   (1000)        0 2024-03-20 20:20:52.907096 star_dresden_gs_lib-0.1.2/src/
-drwxrwxrwx   0 sners03   (1000) sners03   (1000)        0 2024-03-20 20:20:53.186885 star_dresden_gs_lib-0.1.2/src/star_dresden_gs_lib/
--rwxrwxrwx   0 sners03   (1000) sners03   (1000)       34 2024-03-20 16:41:42.000000 star_dresden_gs_lib-0.1.2/src/star_dresden_gs_lib/__init__.py
-drwxrwxrwx   0 sners03   (1000) sners03   (1000)        0 2024-03-20 20:20:53.566020 star_dresden_gs_lib-0.1.2/src/star_dresden_gs_lib/components/
--rwxrwxrwx   0 sners03   (1000) sners03   (1000)       22 2024-03-20 16:29:39.000000 star_dresden_gs_lib-0.1.2/src/star_dresden_gs_lib/components/__init__.py
--rwxrwxrwx   0 sners03   (1000) sners03   (1000)     8060 2024-03-20 20:19:50.000000 star_dresden_gs_lib-0.1.2/src/star_dresden_gs_lib/components/getter.py
--rwxrwxrwx   0 sners03   (1000) sners03   (1000)     1568 2024-03-20 17:09:10.000000 star_dresden_gs_lib-0.1.2/src/star_dresden_gs_lib/components/setter.py
--rwxrwxrwx   0 sners03   (1000) sners03   (1000)       93 2024-03-18 18:54:01.000000 star_dresden_gs_lib-0.1.2/src/star_dresden_gs_lib/main.py
-drwxrwxrwx   0 sners03   (1000) sners03   (1000)        0 2024-03-20 20:20:53.695024 star_dresden_gs_lib-0.1.2/src/star_dresden_gs_lib/tools/
--rwxrwxrwx   0 sners03   (1000) sners03   (1000)        0 2024-03-20 17:02:24.000000 star_dresden_gs_lib-0.1.2/src/star_dresden_gs_lib/tools/__init__.py
--rwxrwxrwx   0 sners03   (1000) sners03   (1000)      361 2024-03-20 17:03:45.000000 star_dresden_gs_lib-0.1.2/src/star_dresden_gs_lib/tools/async_tools.py
-drwxrwxrwx   0 sners03   (1000) sners03   (1000)        0 2024-03-20 20:20:53.804024 star_dresden_gs_lib-0.1.2/src/star_dresden_gs_lib.egg-info/
--rwxrwxrwx   0 sners03   (1000) sners03   (1000)     2080 2024-03-20 20:20:52.000000 star_dresden_gs_lib-0.1.2/src/star_dresden_gs_lib.egg-info/PKG-INFO
--rwxrwxrwx   0 sners03   (1000) sners03   (1000)      555 2024-03-20 20:20:52.000000 star_dresden_gs_lib-0.1.2/src/star_dresden_gs_lib.egg-info/SOURCES.txt
--rwxrwxrwx   0 sners03   (1000) sners03   (1000)        1 2024-03-20 20:20:52.000000 star_dresden_gs_lib-0.1.2/src/star_dresden_gs_lib.egg-info/dependency_links.txt
--rwxrwxrwx   0 sners03   (1000) sners03   (1000)       20 2024-03-20 20:20:52.000000 star_dresden_gs_lib-0.1.2/src/star_dresden_gs_lib.egg-info/top_level.txt
-drwxrwxrwx   0 sners03   (1000) sners03   (1000)        0 2024-03-20 20:20:53.754023 star_dresden_gs_lib-0.1.2/tests/
--rwxrwxrwx   0 sners03   (1000) sners03   (1000)     1242 2024-03-20 16:29:39.000000 star_dresden_gs_lib-0.1.2/tests/testWindow.py
+drwxrwxrwx   0 sners03   (1000) sners03   (1000)        0 2024-04-30 17:57:13.989310 star_dresden_gs_lib-0.2.0/
+-rwxrwxrwx   0 sners03   (1000) sners03   (1000)     1098 2024-03-18 18:54:01.000000 star_dresden_gs_lib-0.2.0/LICENSE.txt
+-rwxrwxrwx   0 sners03   (1000) sners03   (1000)     2078 2024-04-30 17:57:13.982308 star_dresden_gs_lib-0.2.0/PKG-INFO
+-rwxrwxrwx   0 sners03   (1000) sners03   (1000)     1503 2024-03-20 16:48:30.000000 star_dresden_gs_lib-0.2.0/README.md
+-rwxrwxrwx   0 sners03   (1000) sners03   (1000)      635 2024-04-30 17:55:53.000000 star_dresden_gs_lib-0.2.0/pyproject.toml
+-rwxrwxrwx   0 sners03   (1000) sners03   (1000)       78 2024-04-30 17:57:13.999297 star_dresden_gs_lib-0.2.0/setup.cfg
+-rwxrwxrwx   0 sners03   (1000) sners03   (1000)     2584 2024-04-30 17:55:30.000000 star_dresden_gs_lib-0.2.0/setup.py
+drwxrwxrwx   0 sners03   (1000) sners03   (1000)        0 2024-04-30 17:57:13.109121 star_dresden_gs_lib-0.2.0/src/
+drwxrwxrwx   0 sners03   (1000) sners03   (1000)        0 2024-04-30 17:57:13.386292 star_dresden_gs_lib-0.2.0/src/star_dresden_gs_lib/
+-rwxrwxrwx   0 sners03   (1000) sners03   (1000)       34 2024-03-20 16:41:42.000000 star_dresden_gs_lib-0.2.0/src/star_dresden_gs_lib/__init__.py
+drwxrwxrwx   0 sners03   (1000) sners03   (1000)        0 2024-04-30 17:57:13.855291 star_dresden_gs_lib-0.2.0/src/star_dresden_gs_lib/components/
+-rwxrwxrwx   0 sners03   (1000) sners03   (1000)       22 2024-03-20 16:29:39.000000 star_dresden_gs_lib-0.2.0/src/star_dresden_gs_lib/components/__init__.py
+-rwxrwxrwx   0 sners03   (1000) sners03   (1000)     3962 2024-04-30 17:14:56.000000 star_dresden_gs_lib-0.2.0/src/star_dresden_gs_lib/components/getter.py
+-rwxrwxrwx   0 sners03   (1000) sners03   (1000)     1897 2024-04-30 17:55:19.000000 star_dresden_gs_lib-0.2.0/src/star_dresden_gs_lib/components/logs.py
+-rwxrwxrwx   0 sners03   (1000) sners03   (1000)     1624 2024-04-30 17:19:03.000000 star_dresden_gs_lib-0.2.0/src/star_dresden_gs_lib/components/setter.py
+-rwxrwxrwx   0 sners03   (1000) sners03   (1000)       93 2024-03-18 18:54:01.000000 star_dresden_gs_lib-0.2.0/src/star_dresden_gs_lib/main.py
+drwxrwxrwx   0 sners03   (1000) sners03   (1000)        0 2024-04-30 17:57:13.964296 star_dresden_gs_lib-0.2.0/src/star_dresden_gs_lib.egg-info/
+-rwxrwxrwx   0 sners03   (1000) sners03   (1000)     2078 2024-04-30 17:57:12.000000 star_dresden_gs_lib-0.2.0/src/star_dresden_gs_lib.egg-info/PKG-INFO
+-rwxrwxrwx   0 sners03   (1000) sners03   (1000)      511 2024-04-30 17:57:13.000000 star_dresden_gs_lib-0.2.0/src/star_dresden_gs_lib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sners03   (1000) sners03   (1000)        1 2024-04-30 17:57:12.000000 star_dresden_gs_lib-0.2.0/src/star_dresden_gs_lib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sners03   (1000) sners03   (1000)       20 2024-04-30 17:57:12.000000 star_dresden_gs_lib-0.2.0/src/star_dresden_gs_lib.egg-info/top_level.txt
+drwxrwxrwx   0 sners03   (1000) sners03   (1000)        0 2024-04-30 17:57:13.909299 star_dresden_gs_lib-0.2.0/tests/
+-rwxrwxrwx   0 sners03   (1000) sners03   (1000)     1213 2024-04-30 17:43:10.000000 star_dresden_gs_lib-0.2.0/tests/testWindow.py
```

### Comparing `star_dresden_gs_lib-0.1.2/LICENSE.txt` & `star_dresden_gs_lib-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `star_dresden_gs_lib-0.1.2/PKG-INFO` & `star_dresden_gs_lib-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: star_dresden_gs_lib
-Version: 0.1.2
-Summary: A framework for creating a groundstation with grpc and tkinter
+Version: 0.2.0
+Summary: A framework for creating a groundstation with grpc and PyQt6
 Home-page: https://www.star-dresden.de
 Author: STAR Dresden e.V.
 Author-email: Lars Reiche <sners03coding@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `star_dresden_gs_lib-0.1.2/README.md` & `star_dresden_gs_lib-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `star_dresden_gs_lib-0.1.2/pyproject.toml` & `star_dresden_gs_lib-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "star_dresden_gs_lib"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="Lars Reiche", email="sners03coding@gmail.com" },
 ]
-description = "A framework for creating a groundstation with grpc and tkinter"
+description = "A framework for creating a groundstation with grpc and PyQt6"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `star_dresden_gs_lib-0.1.2/setup.py` & `star_dresden_gs_lib-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="star_dresden_gs_lib",  # Required
-    version="0.1.2",  # Required
+    version="0.2.0",  # Required
     description="A Library for creating a Groundstation using PyQt6",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown", 
     url="https://www.star-dresden.de",  # Optional, Gitlab adress if open source
     author="STAR Dresden e.V.",  # Optional
     author_email="info@star-dresden.de",  # Optional
     # For a list of valid classifiers, see https://pypi.org/classifiers/
```

### Comparing `star_dresden_gs_lib-0.1.2/src/star_dresden_gs_lib/components/setter.py` & `star_dresden_gs_lib-0.2.0/src/star_dresden_gs_lib/components/setter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Callable
 
 from PyQt6 import QtWidgets
 
 
 class SetterWidget(QtWidgets.QWidget):
 
-    def __init__(self, name: str, endpoint: Callable, button: QtWidgets.QPushButton = QtWidgets.QPushButton('None'),
-                 text: QtWidgets.QLabel = QtWidgets.QLabel('None'), execute_func: Callable = None, *args, **kwargs):
+    def __init__(self, name: str, endpoint: Callable, button: QtWidgets.QPushButton = None,
+                 text: QtWidgets.QLabel = None, execute_func: Callable = None, *args, **kwargs):
         """
 
         :param name: the name of the Widget
         :param endpoint: a Callable function for either the Endpoint
         :param button_pos: (optional)
         :param text_pos: (optional)
         :param execute_func: (optional) a custom function for the button press
@@ -19,28 +19,25 @@
         """
         super().__init__(*args, **kwargs)
         self.layout = QtWidgets.QGridLayout()
         self.setLayout(self.layout)
         self.name = name
         self._endpoint = endpoint
 
-        self.button = button
+        self.button = button if button is not None else QtWidgets.QPushButton('None')
         self.button.setObjectName(name)
         # self.input_field = QtWidgets.QLineEdit
-        self.text = text
+        self.text = text if text is not None else QtWidgets.QLabel('None')
 
         # noinspection PyUnresolvedReferences
         # self.textbox.textChanged.connect(self.textbox_text_changed)
         self.button.clicked.connect(self.__execute if execute_func is None else execute_func)
 
         self.layout.addWidget(self.button, 0, 1)
         self.layout.addWidget(self.text, 0, 0)
         self.layout.addWidget(self.text, 0, 2)
 
-
     def __change_text(self, value):
         self.text.setText(f"{self.name}: {value}")
 
     def __execute(self):
         value = self._endpoint()
-
-
```

### Comparing `star_dresden_gs_lib-0.1.2/src/star_dresden_gs_lib.egg-info/PKG-INFO` & `star_dresden_gs_lib-0.2.0/src/star_dresden_gs_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: star_dresden_gs_lib
-Version: 0.1.2
-Summary: A framework for creating a groundstation with grpc and tkinter
+Version: 0.2.0
+Summary: A framework for creating a groundstation with grpc and PyQt6
 Home-page: https://www.star-dresden.de
 Author: STAR Dresden e.V.
 Author-email: Lars Reiche <sners03coding@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `star_dresden_gs_lib-0.1.2/tests/testWindow.py` & `star_dresden_gs_lib-0.2.0/tests/testWindow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
-from random import random
+from random import randint
 
-from PyQt6.uic.properties import QtWidgets
+from PyQt6 import QtWidgets
 
 from star_dresden_gs_lib.components.getter import GetterWidget
 
 
 class MainWindow(QtWidgets.QMainWindow):
     count = 0
 
@@ -20,26 +20,27 @@
 
     def init_gui(self):
         self.window = QtWidgets.QWidget()
         self.layout = QtWidgets.QGridLayout()
         self.setCentralWidget(self.window)
         self.window.setLayout(self.layout)
 
-        self.echotext_widget = GetterWidget("alpha", self.add1, button_pos=(5, 7), text_pos=(9,9))
+        self.echotext_widget = GetterWidget("alpha", self.add1)
         self.echotext_widget2 = GetterWidget("beta", self.rand_num)
 
         self.layout.addWidget(self.echotext_widget, 0, 0)
         self.layout.addWidget(self.echotext_widget2, 1, 1)
 
     def add1(self):
         self.count += 1
+        print(self.count)
         return self.count
 
     def rand_num(self):
-        return random.randint(0, 200)
+        return randint(0, 200)
 
 
 if __name__ == '__main__':
     app = QtWidgets.QApplication([])
 
     win = MainWindow()
     win.show()
```

