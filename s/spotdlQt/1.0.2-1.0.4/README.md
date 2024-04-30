# Comparing `tmp/spotdlqt-1.0.2.tar.gz` & `tmp/spotdlqt-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotdlqt-1.0.2.tar", last modified: Tue Apr 23 19:25:45 2024, max compression
+gzip compressed data, was "spotdlqt-1.0.4.tar", last modified: Tue Apr 30 03:04:12 2024, max compression
```

## Comparing `spotdlqt-1.0.2.tar` & `spotdlqt-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:25:45.301698 spotdlqt-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:25:45.301698 spotdlqt-1.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-23 19:24:18.000000 spotdlqt-1.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:25:45.301698 spotdlqt-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-23 19:24:18.000000 spotdlqt-1.0.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-23 19:24:18.000000 spotdlqt-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 19:24:18.000000 spotdlqt-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-23 19:25:45.301698 spotdlqt-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-23 19:24:18.000000 spotdlqt-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-23 19:24:18.000000 spotdlqt-1.0.2/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-23 19:24:18.000000 spotdlqt-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 19:24:18.000000 spotdlqt-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    28952 2024-04-23 19:24:18.000000 spotdlqt-1.0.2/screenshot1.png
--rw-r--r--   0 runner    (1001) docker     (127)    46212 2024-04-23 19:24:18.000000 spotdlqt-1.0.2/screenshot2.png
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:25:45.301698 spotdlqt-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:25:45.297698 spotdlqt-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:25:45.301698 spotdlqt-1.0.2/src/spotdlQt/
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-23 19:24:18.000000 spotdlqt-1.0.2/src/spotdlQt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:25:45.301698 spotdlqt-1.0.2/src/spotdlQt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-23 19:25:45.000000 spotdlqt-1.0.2/src/spotdlQt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-23 19:25:45.000000 spotdlqt-1.0.2/src/spotdlQt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:25:45.000000 spotdlqt-1.0.2/src/spotdlQt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 19:25:45.000000 spotdlqt-1.0.2/src/spotdlQt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 19:25:45.000000 spotdlqt-1.0.2/src/spotdlQt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 19:25:45.000000 spotdlqt-1.0.2/src/spotdlQt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:04:12.890852 spotdlqt-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:04:12.886852 spotdlqt-1.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-30 03:04:08.000000 spotdlqt-1.0.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:04:12.886852 spotdlqt-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-30 03:04:08.000000 spotdlqt-1.0.4/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-30 03:04:08.000000 spotdlqt-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 03:04:08.000000 spotdlqt-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-30 03:04:12.890852 spotdlqt-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-30 03:04:08.000000 spotdlqt-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-30 03:04:08.000000 spotdlqt-1.0.4/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-30 03:04:08.000000 spotdlqt-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 03:04:08.000000 spotdlqt-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    28952 2024-04-30 03:04:08.000000 spotdlqt-1.0.4/screenshot1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46212 2024-04-30 03:04:08.000000 spotdlqt-1.0.4/screenshot2.png
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 03:04:12.890852 spotdlqt-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:04:12.886852 spotdlqt-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:04:12.886852 spotdlqt-1.0.4/src/spotdlQt/
+-rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-04-30 03:04:08.000000 spotdlqt-1.0.4/src/spotdlQt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 03:04:12.890852 spotdlqt-1.0.4/src/spotdlQt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-30 03:04:12.000000 spotdlqt-1.0.4/src/spotdlQt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-30 03:04:12.000000 spotdlqt-1.0.4/src/spotdlQt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 03:04:12.000000 spotdlqt-1.0.4/src/spotdlQt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 03:04:12.000000 spotdlqt-1.0.4/src/spotdlQt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 03:04:12.000000 spotdlqt-1.0.4/src/spotdlQt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 03:04:12.000000 spotdlqt-1.0.4/src/spotdlQt.egg-info/top_level.txt
```

### Comparing `spotdlqt-1.0.2/.github/dependabot.yml` & `spotdlqt-1.0.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `spotdlqt-1.0.2/.github/workflows/pypi-publish.yml` & `spotdlqt-1.0.4/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `spotdlqt-1.0.2/.gitignore` & `spotdlqt-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `spotdlqt-1.0.2/LICENSE` & `spotdlqt-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spotdlqt-1.0.2/PKG-INFO` & `spotdlqt-1.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: spotdlQt
-Version: 1.0.2
+Version: 1.0.4
 Summary: A small gui for spotdl using qt written in python
 Author-email: Magi3r <magier.mit.f3erball@gmail.com>
 Project-URL: Repository, https://github.com/Magi3r/spotdlQt
 Project-URL: Issues, https://github.com/Magi3r/spotdlQt/issues
 Keywords: spotdl,qt6,downloader,music
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyqt6==6.6.1
+Requires-Dist: pyqt6==6.7.0
 Requires-Dist: spotdl==4.2.5
 
 # spotdlQt
 A very simple gui application for spotdl to download music.
 
 Written in python using [spotdl](https://github.com/spotDL/spotify-downloader) and [pyqt6](https://pypi.org/project/PyQt6/).
```

### Comparing `spotdlqt-1.0.2/icon.svg` & `spotdlqt-1.0.4/icon.svg`

 * *Files identical despite different names*

### Comparing `spotdlqt-1.0.2/pyproject.toml` & `spotdlqt-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["pyqt6==6.6.1", "spotdl==4.2.5"]
+dependencies = ["pyqt6==6.7.0", "spotdl==4.2.5"]
 keywords = ["spotdl", "qt6", "downloader", "music"]
 
 [project.gui-scripts]
 spotdlQt = "spotdlQt.app:main"
 
 [project.urls]
 Repository = "https://github.com/Magi3r/spotdlQt"
```

### Comparing `spotdlqt-1.0.2/screenshot1.png` & `spotdlqt-1.0.4/screenshot1.png`

 * *Files identical despite different names*

### Comparing `spotdlqt-1.0.2/screenshot2.png` & `spotdlqt-1.0.4/screenshot2.png`

 * *Files identical despite different names*

### Comparing `spotdlqt-1.0.2/src/spotdlQt/app.py` & `spotdlqt-1.0.4/src/spotdlQt/app.py`

 * *Files identical despite different names*

### Comparing `spotdlqt-1.0.2/src/spotdlQt.egg-info/PKG-INFO` & `spotdlqt-1.0.4/src/spotdlQt.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: spotdlQt
-Version: 1.0.2
+Version: 1.0.4
 Summary: A small gui for spotdl using qt written in python
 Author-email: Magi3r <magier.mit.f3erball@gmail.com>
 Project-URL: Repository, https://github.com/Magi3r/spotdlQt
 Project-URL: Issues, https://github.com/Magi3r/spotdlQt/issues
 Keywords: spotdl,qt6,downloader,music
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyqt6==6.6.1
+Requires-Dist: pyqt6==6.7.0
 Requires-Dist: spotdl==4.2.5
 
 # spotdlQt
 A very simple gui application for spotdl to download music.
 
 Written in python using [spotdl](https://github.com/spotDL/spotify-downloader) and [pyqt6](https://pypi.org/project/PyQt6/).
```

