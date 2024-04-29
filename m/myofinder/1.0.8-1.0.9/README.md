# Comparing `tmp/myofinder-1.0.8.tar.gz` & `tmp/myofinder-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myofinder-1.0.8.tar", last modified: Thu Apr 25 21:50:22 2024, max compression
+gzip compressed data, was "myofinder-1.0.9.tar", last modified: Mon Apr 29 22:29:14 2024, max compression
```

## Comparing `myofinder-1.0.8.tar` & `myofinder-1.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 21:50:22.156554 myofinder-1.0.8/
--rw-rw-r--   0 root         (0) root         (0)    35149 2023-07-18 11:52:57.000000 myofinder-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)    44871 2024-04-25 21:50:22.156554 myofinder-1.0.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2687 2023-07-18 11:52:57.000000 myofinder-1.0.8/README.md
--rw-rw-r--   0 root         (0) root         (0)     1889 2024-04-25 20:59:11.000000 myofinder-1.0.8/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)      104 2023-09-11 14:15:14.000000 myofinder-1.0.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 21:50:22.156554 myofinder-1.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 21:50:22.148553 myofinder-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 21:50:22.152554 myofinder-1.0.8/src/myofinder/
--rw-rw-r--   0 root         (0) root         (0)       90 2023-12-25 13:40:07.000000 myofinder-1.0.8/src/myofinder/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4158 2024-03-19 22:13:01.000000 myofinder-1.0.8/src/myofinder/__main__.py
--rw-rw-r--   0 root         (0) root         (0)       39 2024-04-25 20:52:42.000000 myofinder-1.0.8/src/myofinder/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 21:50:22.152554 myofinder-1.0.8/src/myofinder/app_images/
--rw-rw-r--   0 root         (0) root         (0)   211262 2023-07-18 11:52:57.000000 myofinder-1.0.8/src/myofinder/app_images/project_icon.ico
--rw-rw-r--   0 root         (0) root         (0)   147234 2023-07-18 11:52:57.000000 myofinder-1.0.8/src/myofinder/app_images/project_icon.png
--rw-rw-r--   0 root         (0) root         (0)  2234620 2023-07-18 11:52:57.000000 myofinder-1.0.8/src/myofinder/app_images/splash_background.png
--rw-rw-r--   0 root         (0) root         (0)    27756 2023-12-25 13:40:07.000000 myofinder-1.0.8/src/myofinder/files_table.py
--rw-rw-r--   0 root         (0) root         (0)    34451 2023-12-25 13:40:07.000000 myofinder-1.0.8/src/myofinder/image_canvas.py
--rw-rw-r--   0 root         (0) root         (0)    10485 2023-12-25 13:40:07.000000 myofinder-1.0.8/src/myofinder/image_segmentation.py
--rw-rw-r--   0 root         (0) root         (0)    43359 2024-04-25 09:16:16.000000 myofinder-1.0.8/src/myofinder/main_window.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 21:50:22.152554 myofinder-1.0.8/src/myofinder/tools/
--rw-rw-r--   0 root         (0) root         (0)      401 2023-12-25 13:40:07.000000 myofinder-1.0.8/src/myofinder/tools/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3114 2023-07-18 11:52:57.000000 myofinder-1.0.8/src/myofinder/tools/_check_image.py
--rw-rw-r--   0 root         (0) root         (0)     1995 2023-12-25 13:40:07.000000 myofinder-1.0.8/src/myofinder/tools/_check_project_name.py
--rw-rw-r--   0 root         (0) root         (0)     1790 2023-12-25 13:40:07.000000 myofinder-1.0.8/src/myofinder/tools/save_popup.py
--rw-rw-r--   0 root         (0) root         (0)     9201 2023-12-25 13:40:07.000000 myofinder-1.0.8/src/myofinder/tools/settings_window.py
--rw-rw-r--   0 root         (0) root         (0)     4243 2023-12-25 13:40:07.000000 myofinder-1.0.8/src/myofinder/tools/splash_window.py
--rw-rw-r--   0 root         (0) root         (0)    21064 2023-12-25 13:40:07.000000 myofinder-1.0.8/src/myofinder/tools/structure_classes.py
--rw-rw-r--   0 root         (0) root         (0)     3441 2023-12-25 13:40:07.000000 myofinder-1.0.8/src/myofinder/tools/warning_window.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 21:50:22.152554 myofinder-1.0.8/src/myofinder.egg-info/
--rw-r--r--   0 root         (0) root         (0)    44871 2024-04-25 21:50:22.000000 myofinder-1.0.8/src/myofinder.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      869 2024-04-25 21:50:22.000000 myofinder-1.0.8/src/myofinder.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2024-04-25 21:50:22.000000 myofinder-1.0.8/src/myofinder.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)      104 2024-04-25 21:50:22.000000 myofinder-1.0.8/src/myofinder.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       10 2024-04-25 21:50:22.000000 myofinder-1.0.8/src/myofinder.egg-info/top_level.txt
+drwxrwxr-x   0 weis      (1000) weis      (1000)        0 2024-04-29 22:29:14.200982 myofinder-1.0.9/
+-rw-rw-r--   0 weis      (1000) weis      (1000)    35149 2023-07-18 11:52:57.000000 myofinder-1.0.9/LICENSE
+-rw-r--r--   0 weis      (1000) weis      (1000)    44871 2024-04-29 22:29:14.200982 myofinder-1.0.9/PKG-INFO
+-rw-rw-r--   0 weis      (1000) weis      (1000)     2687 2023-07-18 11:52:57.000000 myofinder-1.0.9/README.md
+-rw-rw-r--   0 weis      (1000) weis      (1000)     1889 2024-04-29 21:55:55.000000 myofinder-1.0.9/pyproject.toml
+-rw-rw-r--   0 weis      (1000) weis      (1000)      104 2023-09-11 14:15:14.000000 myofinder-1.0.9/requirements.txt
+-rw-rw-r--   0 weis      (1000) weis      (1000)       38 2024-04-29 22:29:14.200982 myofinder-1.0.9/setup.cfg
+drwxrwxr-x   0 weis      (1000) weis      (1000)        0 2024-04-29 22:29:14.188982 myofinder-1.0.9/src/
+drwxrwxr-x   0 weis      (1000) weis      (1000)        0 2024-04-29 22:29:14.192982 myofinder-1.0.9/src/myofinder/
+-rw-rw-r--   0 weis      (1000) weis      (1000)       90 2023-12-25 13:40:07.000000 myofinder-1.0.9/src/myofinder/__init__.py
+-rw-rw-r--   0 weis      (1000) weis      (1000)     4158 2024-03-19 22:13:01.000000 myofinder-1.0.9/src/myofinder/__main__.py
+-rw-rw-r--   0 weis      (1000) weis      (1000)       39 2024-04-29 21:55:55.000000 myofinder-1.0.9/src/myofinder/__version__.py
+drwxrwxr-x   0 weis      (1000) weis      (1000)        0 2024-04-29 22:29:14.196982 myofinder-1.0.9/src/myofinder/app_images/
+-rw-rw-r--   0 weis      (1000) weis      (1000)   211262 2023-07-18 11:52:57.000000 myofinder-1.0.9/src/myofinder/app_images/project_icon.ico
+-rw-rw-r--   0 weis      (1000) weis      (1000)   147234 2023-07-18 11:52:57.000000 myofinder-1.0.9/src/myofinder/app_images/project_icon.png
+-rw-rw-r--   0 weis      (1000) weis      (1000)  2234620 2023-07-18 11:52:57.000000 myofinder-1.0.9/src/myofinder/app_images/splash_background.png
+-rw-rw-r--   0 weis      (1000) weis      (1000)    27756 2023-12-25 13:40:07.000000 myofinder-1.0.9/src/myofinder/files_table.py
+-rw-rw-r--   0 weis      (1000) weis      (1000)    34451 2023-12-25 13:40:07.000000 myofinder-1.0.9/src/myofinder/image_canvas.py
+-rw-rw-r--   0 weis      (1000) weis      (1000)    10485 2023-12-25 13:40:07.000000 myofinder-1.0.9/src/myofinder/image_segmentation.py
+-rw-rw-r--   0 weis      (1000) weis      (1000)    43359 2024-04-25 09:16:16.000000 myofinder-1.0.9/src/myofinder/main_window.py
+drwxrwxr-x   0 weis      (1000) weis      (1000)        0 2024-04-29 22:29:14.200982 myofinder-1.0.9/src/myofinder/tools/
+-rw-rw-r--   0 weis      (1000) weis      (1000)      401 2023-12-25 13:40:07.000000 myofinder-1.0.9/src/myofinder/tools/__init__.py
+-rw-rw-r--   0 weis      (1000) weis      (1000)     3114 2023-07-18 11:52:57.000000 myofinder-1.0.9/src/myofinder/tools/_check_image.py
+-rw-rw-r--   0 weis      (1000) weis      (1000)     1995 2023-12-25 13:40:07.000000 myofinder-1.0.9/src/myofinder/tools/_check_project_name.py
+-rw-rw-r--   0 weis      (1000) weis      (1000)     1790 2023-12-25 13:40:07.000000 myofinder-1.0.9/src/myofinder/tools/save_popup.py
+-rw-rw-r--   0 weis      (1000) weis      (1000)     9201 2023-12-25 13:40:07.000000 myofinder-1.0.9/src/myofinder/tools/settings_window.py
+-rw-rw-r--   0 weis      (1000) weis      (1000)     4243 2023-12-25 13:40:07.000000 myofinder-1.0.9/src/myofinder/tools/splash_window.py
+-rw-rw-r--   0 weis      (1000) weis      (1000)    21064 2023-12-25 13:40:07.000000 myofinder-1.0.9/src/myofinder/tools/structure_classes.py
+-rw-rw-r--   0 weis      (1000) weis      (1000)     3441 2023-12-25 13:40:07.000000 myofinder-1.0.9/src/myofinder/tools/warning_window.py
+drwxrwxr-x   0 weis      (1000) weis      (1000)        0 2024-04-29 22:29:14.200982 myofinder-1.0.9/src/myofinder.egg-info/
+-rw-r--r--   0 weis      (1000) weis      (1000)    44871 2024-04-29 22:29:14.000000 myofinder-1.0.9/src/myofinder.egg-info/PKG-INFO
+-rw-rw-r--   0 weis      (1000) weis      (1000)      869 2024-04-29 22:29:14.000000 myofinder-1.0.9/src/myofinder.egg-info/SOURCES.txt
+-rw-rw-r--   0 weis      (1000) weis      (1000)        1 2024-04-29 22:29:14.000000 myofinder-1.0.9/src/myofinder.egg-info/dependency_links.txt
+-rw-rw-r--   0 weis      (1000) weis      (1000)      104 2024-04-29 22:29:14.000000 myofinder-1.0.9/src/myofinder.egg-info/requires.txt
+-rw-rw-r--   0 weis      (1000) weis      (1000)       10 2024-04-29 22:29:14.000000 myofinder-1.0.9/src/myofinder.egg-info/top_level.txt
```

### Comparing `myofinder-1.0.8/LICENSE` & `myofinder-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `myofinder-1.0.8/PKG-INFO` & `myofinder-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myofinder
-Version: 1.0.8
+Version: 1.0.9
 Summary: Automatic calculation of the fusion index by AI segmentation
 Author-email: Tissue Engineering Lab <antoine.weisrock@kuleuven.be>
 Maintainer-email: Antoine Weisrock <antoine.weisrock@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `myofinder-1.0.8/README.md` & `myofinder-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `myofinder-1.0.8/pyproject.toml` & `myofinder-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "myofinder"
 dynamic = ["readme", "dependencies"]
-version = "1.0.8"
+version = "1.0.9"
 description = "Automatic calculation of the fusion index by AI segmentation"
 license = {file = "LICENSE"}
 keywords = ["segmentation", "fusion index", "automation", "muscle culture"]
 requires-python = ">=3.7,<3.11"
 authors = [{name = "Tissue Engineering Lab", email = "antoine.weisrock@kuleuven.be"}]
 maintainers = [{name = "Antoine Weisrock", email = "antoine.weisrock@gmail.com"}]
 classifiers = [
```

### Comparing `myofinder-1.0.8/src/myofinder/__main__.py` & `myofinder-1.0.9/src/myofinder/__main__.py`

 * *Files identical despite different names*

### Comparing `myofinder-1.0.8/src/myofinder/app_images/project_icon.ico` & `myofinder-1.0.9/src/myofinder/app_images/project_icon.ico`

 * *Files identical despite different names*

### Comparing `myofinder-1.0.8/src/myofinder/app_images/project_icon.png` & `myofinder-1.0.9/src/myofinder/app_images/project_icon.png`

 * *Files identical despite different names*

### Comparing `myofinder-1.0.8/src/myofinder/app_images/splash_background.png` & `myofinder-1.0.9/src/myofinder/app_images/splash_background.png`

 * *Files identical despite different names*

### Comparing `myofinder-1.0.8/src/myofinder/files_table.py` & `myofinder-1.0.9/src/myofinder/files_table.py`

 * *Files identical despite different names*

### Comparing `myofinder-1.0.8/src/myofinder/image_canvas.py` & `myofinder-1.0.9/src/myofinder/image_canvas.py`

 * *Files identical despite different names*

### Comparing `myofinder-1.0.8/src/myofinder/image_segmentation.py` & `myofinder-1.0.9/src/myofinder/image_segmentation.py`

 * *Files identical despite different names*

### Comparing `myofinder-1.0.8/src/myofinder/main_window.py` & `myofinder-1.0.9/src/myofinder/main_window.py`

 * *Files identical despite different names*

### Comparing `myofinder-1.0.8/src/myofinder/tools/_check_image.py` & `myofinder-1.0.9/src/myofinder/tools/_check_image.py`

 * *Files identical despite different names*

### Comparing `myofinder-1.0.8/src/myofinder/tools/_check_project_name.py` & `myofinder-1.0.9/src/myofinder/tools/_check_project_name.py`

 * *Files identical despite different names*

### Comparing `myofinder-1.0.8/src/myofinder/tools/save_popup.py` & `myofinder-1.0.9/src/myofinder/tools/save_popup.py`

 * *Files identical despite different names*

### Comparing `myofinder-1.0.8/src/myofinder/tools/settings_window.py` & `myofinder-1.0.9/src/myofinder/tools/settings_window.py`

 * *Files identical despite different names*

### Comparing `myofinder-1.0.8/src/myofinder/tools/splash_window.py` & `myofinder-1.0.9/src/myofinder/tools/splash_window.py`

 * *Files identical despite different names*

### Comparing `myofinder-1.0.8/src/myofinder/tools/structure_classes.py` & `myofinder-1.0.9/src/myofinder/tools/structure_classes.py`

 * *Files identical despite different names*

### Comparing `myofinder-1.0.8/src/myofinder/tools/warning_window.py` & `myofinder-1.0.9/src/myofinder/tools/warning_window.py`

 * *Files identical despite different names*

### Comparing `myofinder-1.0.8/src/myofinder.egg-info/PKG-INFO` & `myofinder-1.0.9/src/myofinder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myofinder
-Version: 1.0.8
+Version: 1.0.9
 Summary: Automatic calculation of the fusion index by AI segmentation
 Author-email: Tissue Engineering Lab <antoine.weisrock@kuleuven.be>
 Maintainer-email: Antoine Weisrock <antoine.weisrock@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `myofinder-1.0.8/src/myofinder.egg-info/SOURCES.txt` & `myofinder-1.0.9/src/myofinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

