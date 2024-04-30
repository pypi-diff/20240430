# Comparing `tmp/pyprojectlib-0.0.4.tar.gz` & `tmp/pyprojectlib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprojectlib-0.0.4.tar", last modified: Tue Apr 30 17:48:58 2024, max compression
+gzip compressed data, was "pyprojectlib-0.0.5.tar", last modified: Tue Apr 30 18:50:26 2024, max compression
```

## Comparing `pyprojectlib-0.0.4.tar` & `pyprojectlib-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 17:48:58.084734 pyprojectlib-0.0.4/
--rw-rw-rw-   0        0        0    35821 2023-08-08 21:22:00.000000 pyprojectlib-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     7341 2024-04-30 17:48:58.084734 pyprojectlib-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     6546 2024-04-30 16:24:22.000000 pyprojectlib-0.0.4/README.md
--rw-rw-rw-   0        0        0      952 2024-04-30 17:48:43.000000 pyprojectlib-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-30 17:48:58.084734 pyprojectlib-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-30 17:48:58.035751 pyprojectlib-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-30 17:48:58.058405 pyprojectlib-0.0.4/src/pyprojectlib/
--rw-rw-rw-   0        0        0    35821 2023-08-08 21:22:00.000000 pyprojectlib-0.0.4/src/pyprojectlib/LICENSE.template
--rw-rw-rw-   0        0        0     1455 2023-11-13 08:31:50.000000 pyprojectlib-0.0.4/src/pyprojectlib/README.template
--rw-rw-rw-   0        0        0     7657 2024-04-30 17:45:02.000000 pyprojectlib-0.0.4/src/pyprojectlib/__init__.py
--rw-rw-rw-   0        0        0     5556 2024-04-30 17:05:35.000000 pyprojectlib-0.0.4/src/pyprojectlib/cli.py
--rw-rw-rw-   0        0        0     1475 2024-04-30 15:25:10.000000 pyprojectlib-0.0.4/src/pyprojectlib/constants.py
--rw-rw-rw-   0        0        0     4824 2024-04-30 17:43:33.000000 pyprojectlib-0.0.4/src/pyprojectlib/helper.py
--rw-rw-rw-   0        0        0        0 2023-11-11 03:12:10.000000 pyprojectlib-0.0.4/src/pyprojectlib/py.typed
--rw-rw-rw-   0        0        0     8523 2024-04-30 17:47:15.000000 pyprojectlib-0.0.4/src/pyprojectlib/pypackage.py
--rw-rw-rw-   0        0        0     4321 2023-11-13 11:45:23.000000 pyprojectlib-0.0.4/src/pyprojectlib/pyproject.py
--rw-rw-rw-   0        0        0     8153 2024-04-30 16:25:28.000000 pyprojectlib-0.0.4/src/pyprojectlib/pyrepo.py
--rw-rw-rw-   0        0        0     1617 2023-11-13 05:08:24.000000 pyprojectlib-0.0.4/src/pyprojectlib/pyuser.py
-drwxrwxrwx   0        0        0        0 2024-04-30 17:48:58.082733 pyprojectlib-0.0.4/src/pyprojectlib.egg-info/
--rw-rw-rw-   0        0        0     7341 2024-04-30 17:48:58.000000 pyprojectlib-0.0.4/src/pyprojectlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      595 2024-04-30 17:48:58.000000 pyprojectlib-0.0.4/src/pyprojectlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 17:48:58.000000 pyprojectlib-0.0.4/src/pyprojectlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-30 17:48:58.000000 pyprojectlib-0.0.4/src/pyprojectlib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      123 2024-04-30 17:48:58.000000 pyprojectlib-0.0.4/src/pyprojectlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-30 17:48:58.000000 pyprojectlib-0.0.4/src/pyprojectlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 18:50:26.128693 pyprojectlib-0.0.5/
+-rw-rw-rw-   0        0        0    35821 2023-08-08 21:22:00.000000 pyprojectlib-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     7341 2024-04-30 18:50:26.127655 pyprojectlib-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6546 2024-04-30 16:24:22.000000 pyprojectlib-0.0.5/README.md
+-rw-rw-rw-   0        0        0      952 2024-04-30 18:50:09.000000 pyprojectlib-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-30 18:50:26.128693 pyprojectlib-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 18:50:26.075894 pyprojectlib-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-30 18:50:26.098164 pyprojectlib-0.0.5/src/pyprojectlib/
+-rw-rw-rw-   0        0        0    35821 2023-08-08 21:22:00.000000 pyprojectlib-0.0.5/src/pyprojectlib/LICENSE.template
+-rw-rw-rw-   0        0        0     1455 2023-11-13 08:31:50.000000 pyprojectlib-0.0.5/src/pyprojectlib/README.template
+-rw-rw-rw-   0        0        0     7657 2024-04-30 17:45:02.000000 pyprojectlib-0.0.5/src/pyprojectlib/__init__.py
+-rw-rw-rw-   0        0        0     5556 2024-04-30 17:05:35.000000 pyprojectlib-0.0.5/src/pyprojectlib/cli.py
+-rw-rw-rw-   0        0        0     1513 2024-04-30 17:55:48.000000 pyprojectlib-0.0.5/src/pyprojectlib/constants.py
+-rw-rw-rw-   0        0        0     4824 2024-04-30 17:43:33.000000 pyprojectlib-0.0.5/src/pyprojectlib/helper.py
+-rw-rw-rw-   0        0        0        0 2023-11-11 03:12:10.000000 pyprojectlib-0.0.5/src/pyprojectlib/py.typed
+-rw-rw-rw-   0        0        0     8594 2024-04-30 18:46:53.000000 pyprojectlib-0.0.5/src/pyprojectlib/pypackage.py
+-rw-rw-rw-   0        0        0     4321 2023-11-13 11:45:23.000000 pyprojectlib-0.0.5/src/pyprojectlib/pyproject.py
+-rw-rw-rw-   0        0        0     8153 2024-04-30 16:25:28.000000 pyprojectlib-0.0.5/src/pyprojectlib/pyrepo.py
+-rw-rw-rw-   0        0        0     1617 2023-11-13 05:08:24.000000 pyprojectlib-0.0.5/src/pyprojectlib/pyuser.py
+drwxrwxrwx   0        0        0        0 2024-04-30 18:50:26.125653 pyprojectlib-0.0.5/src/pyprojectlib.egg-info/
+-rw-rw-rw-   0        0        0     7341 2024-04-30 18:50:26.000000 pyprojectlib-0.0.5/src/pyprojectlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      595 2024-04-30 18:50:26.000000 pyprojectlib-0.0.5/src/pyprojectlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 18:50:26.000000 pyprojectlib-0.0.5/src/pyprojectlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-30 18:50:26.000000 pyprojectlib-0.0.5/src/pyprojectlib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      123 2024-04-30 18:50:26.000000 pyprojectlib-0.0.5/src/pyprojectlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-30 18:50:26.000000 pyprojectlib-0.0.5/src/pyprojectlib.egg-info/top_level.txt
```

### Comparing `pyprojectlib-0.0.4/LICENSE.txt` & `pyprojectlib-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyprojectlib-0.0.4/PKG-INFO` & `pyprojectlib-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprojectlib
-Version: 0.0.4
+Version: 0.0.5
 Author-email: Jason Krist <jkrist2696@gmail.com>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/jkrist2696/pyprojectlib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
```

### Comparing `pyprojectlib-0.0.4/README.md` & `pyprojectlib-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyprojectlib-0.0.4/pyproject.toml` & `pyprojectlib-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     'Operating System :: Microsoft :: Windows',
     'Operating System :: Unix',
 ]
 
 name = "pyprojectlib"
-version = "0.0.4"
+version = "0.0.5"
 authors = [{ name = "Jason Krist", email = "jkrist2696@gmail.com" }]
 description = ""
 requires-python = ">=3.6"
 dependencies = ["cleandoc>=0.0.13","GitPython>=3.1.40","pipreqs>=0.4.13","pytest>=7.4.3","build","twine","tomli","tomli-w","types-requests","types-setuptools"]
 [tool.setuptools.package-data]
 pyprojectlib = ["*.typed", "*.template"]
 [project.scripts]
```

### Comparing `pyprojectlib-0.0.4/src/pyprojectlib/LICENSE.template` & `pyprojectlib-0.0.5/src/pyprojectlib/LICENSE.template`

 * *Files identical despite different names*

### Comparing `pyprojectlib-0.0.4/src/pyprojectlib/README.template` & `pyprojectlib-0.0.5/src/pyprojectlib/README.template`

 * *Files identical despite different names*

### Comparing `pyprojectlib-0.0.4/src/pyprojectlib/__init__.py` & `pyprojectlib-0.0.5/src/pyprojectlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyprojectlib-0.0.4/src/pyprojectlib/cli.py` & `pyprojectlib-0.0.5/src/pyprojectlib/cli.py`

 * *Files identical despite different names*

### Comparing `pyprojectlib-0.0.4/src/pyprojectlib/constants.py` & `pyprojectlib-0.0.5/src/pyprojectlib/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,8 +61,10 @@
     "docs/conf.txt",  # "src/proj/__pycache__
     "test/__pycache__",
     "test/.mypy_cache/",
     "test/docs",
     "test/examples",
     "test/cleandoc_log.txt",
     "src/*.egg-info/",
+    "src/*/__pycache/",
+    "old/",
 ]
```

### Comparing `pyprojectlib-0.0.4/src/pyprojectlib/helper.py` & `pyprojectlib-0.0.5/src/pyprojectlib/helper.py`

 * *Files identical despite different names*

### Comparing `pyprojectlib-0.0.4/src/pyprojectlib/pypackage.py` & `pyprojectlib-0.0.5/src/pyprojectlib/pypackage.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,16 @@
         elif len(pyversion) > 0:
             pyversion_check(pyversion)
             toml_str += f'requires-python = ">={pyversion}"\n'
         toml_str += f"dependencies = [{depstr}]\n"
         # toml_str += '[tool.setuptools.packages.find]\nwhere = ["src"]\n'
         # toml_str += f'exclude = ["*.__pycache__"]\n'
         toml_str += "[tool.setuptools.package-data]\n"
-        filetypes_list = [ft[1:] if ft[0] == "." else ft for ft in filetypes.split(",")]
+        filetypes_list = [ft for ft in filetypes.split(",") if len(ft) > 0]
+        filetypes_list = [ft[1:] if ft[0] == "." else ft for ft in filetypes_list]
         filetypes_str = '", "*.'.join(["typed"] + filetypes_list)
         toml_str += f'{self.name} = ["*.{filetypes_str}"]\n'
         # toml_str += "[tool.setuptools.exclude-package-data]\n"
         # toml_str += f'{self.name} = ["__pycache__/*", "__pycache__"]\n'
         if len(self.cli.strip()) > 0:
             toml_str += "[project.scripts]\n"
             toml_str += f"{self.cli}\n"
```

### Comparing `pyprojectlib-0.0.4/src/pyprojectlib/pyproject.py` & `pyprojectlib-0.0.5/src/pyprojectlib/pyproject.py`

 * *Files identical despite different names*

### Comparing `pyprojectlib-0.0.4/src/pyprojectlib/pyrepo.py` & `pyprojectlib-0.0.5/src/pyprojectlib/pyrepo.py`

 * *Files identical despite different names*

### Comparing `pyprojectlib-0.0.4/src/pyprojectlib/pyuser.py` & `pyprojectlib-0.0.5/src/pyprojectlib/pyuser.py`

 * *Files identical despite different names*

### Comparing `pyprojectlib-0.0.4/src/pyprojectlib.egg-info/PKG-INFO` & `pyprojectlib-0.0.5/src/pyprojectlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprojectlib
-Version: 0.0.4
+Version: 0.0.5
 Author-email: Jason Krist <jkrist2696@gmail.com>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/jkrist2696/pyprojectlib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
```

### Comparing `pyprojectlib-0.0.4/src/pyprojectlib.egg-info/SOURCES.txt` & `pyprojectlib-0.0.5/src/pyprojectlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

