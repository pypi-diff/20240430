# Comparing `tmp/wallpaper_factory-0.0.7.tar.gz` & `tmp/wallpaper_factory-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wallpaper_factory-0.0.7.tar", last modified: Tue Apr 30 13:48:56 2024, max compression
+gzip compressed data, was "wallpaper_factory-0.0.8.tar", last modified: Tue Apr 30 13:54:08 2024, max compression
```

## Comparing `wallpaper_factory-0.0.7.tar` & `wallpaper_factory-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:48:56.575783 wallpaper_factory-0.0.7/
--rw-r--r--   0 marlonkunz   (501) staff       (20)    35149 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.7/LICENSE
--rw-r--r--   0 marlonkunz   (501) staff       (20)     5820 2024-04-30 13:48:56.575530 wallpaper_factory-0.0.7/PKG-INFO
--rw-r--r--   0 marlonkunz   (501) staff       (20)     5645 2024-04-30 13:48:24.000000 wallpaper_factory-0.0.7/README.md
--rw-r--r--   0 marlonkunz   (501) staff       (20)       38 2024-04-30 13:48:56.575834 wallpaper_factory-0.0.7/setup.cfg
--rw-r--r--   0 marlonkunz   (501) staff       (20)      396 2024-04-30 13:48:51.000000 wallpaper_factory-0.0.7/setup.py
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:48:56.571529 wallpaper_factory-0.0.7/src/
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:48:56.573792 wallpaper_factory-0.0.7/src/wallpaper_factory/
--rw-r--r--   0 marlonkunz   (501) staff       (20)       61 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.7/src/wallpaper_factory/__init__.py
--rw-r--r--   0 marlonkunz   (501) staff       (20)     2378 2024-04-30 13:33:15.000000 wallpaper_factory-0.0.7/src/wallpaper_factory/available_palletes.py
--rw-r--r--   0 marlonkunz   (501) staff       (20)     3719 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.7/src/wallpaper_factory/main.py
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:48:56.575211 wallpaper_factory-0.0.7/src/wallpaper_factory.egg-info/
--rw-r--r--   0 marlonkunz   (501) staff       (20)     5820 2024-04-30 13:48:56.000000 wallpaper_factory-0.0.7/src/wallpaper_factory.egg-info/PKG-INFO
--rw-r--r--   0 marlonkunz   (501) staff       (20)      406 2024-04-30 13:48:56.000000 wallpaper_factory-0.0.7/src/wallpaper_factory.egg-info/SOURCES.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)        1 2024-04-30 13:48:56.000000 wallpaper_factory-0.0.7/src/wallpaper_factory.egg-info/dependency_links.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       74 2024-04-30 13:48:56.000000 wallpaper_factory-0.0.7/src/wallpaper_factory.egg-info/entry_points.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       21 2024-04-30 13:48:56.000000 wallpaper_factory-0.0.7/src/wallpaper_factory.egg-info/requires.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       18 2024-04-30 13:48:56.000000 wallpaper_factory-0.0.7/src/wallpaper_factory.egg-info/top_level.txt
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:54:08.180873 wallpaper_factory-0.0.8/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)    35149 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.8/LICENSE
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     5924 2024-04-30 13:54:08.180669 wallpaper_factory-0.0.8/PKG-INFO
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     5749 2024-04-30 13:53:35.000000 wallpaper_factory-0.0.8/README.md
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       38 2024-04-30 13:54:08.180916 wallpaper_factory-0.0.8/setup.cfg
+-rw-r--r--   0 marlonkunz   (501) staff       (20)      396 2024-04-30 13:53:58.000000 wallpaper_factory-0.0.8/setup.py
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:54:08.177848 wallpaper_factory-0.0.8/src/
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:54:08.179515 wallpaper_factory-0.0.8/src/wallpaper_factory/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       61 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.8/src/wallpaper_factory/__init__.py
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     2378 2024-04-30 13:33:15.000000 wallpaper_factory-0.0.8/src/wallpaper_factory/available_palletes.py
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     3719 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.8/src/wallpaper_factory/main.py
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:54:08.180443 wallpaper_factory-0.0.8/src/wallpaper_factory.egg-info/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     5924 2024-04-30 13:54:08.000000 wallpaper_factory-0.0.8/src/wallpaper_factory.egg-info/PKG-INFO
+-rw-r--r--   0 marlonkunz   (501) staff       (20)      406 2024-04-30 13:54:08.000000 wallpaper_factory-0.0.8/src/wallpaper_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)        1 2024-04-30 13:54:08.000000 wallpaper_factory-0.0.8/src/wallpaper_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       74 2024-04-30 13:54:08.000000 wallpaper_factory-0.0.8/src/wallpaper_factory.egg-info/entry_points.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       21 2024-04-30 13:54:08.000000 wallpaper_factory-0.0.8/src/wallpaper_factory.egg-info/requires.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       18 2024-04-30 13:54:08.000000 wallpaper_factory-0.0.8/src/wallpaper_factory.egg-info/top_level.txt
```

### Comparing `wallpaper_factory-0.0.7/LICENSE` & `wallpaper_factory-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wallpaper_factory-0.0.7/PKG-INFO` & `wallpaper_factory-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: wallpaper_factory
-Version: 0.0.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: opencv-python
-Requires-Dist: pillow
-
 # Wallpaper Factory
 
 ## Table of Content
 
 -   [Installation](#Installation)
 -   [Usage](#Usage)
 -   [Currently Available color schemes](#Currently-Available-color-schemes)
@@ -92,7 +84,9 @@
 
 ### Example Images
 
 | Original                                                                                                | Made By                                      | Link                          |
 | ------------------------------------------------------------------------------------------------------- | -------------------------------------------- | ----------------------------- |
 | ![Kaga(Azure Lane) 1920x1080 by voyager](https://w.wallhaven.cc/full/m9/wallhaven-m9e9m1.png)           | [voyager](https://wallhaven.cc/user/voyager) | https://wallhaven.cc/w/m9e9m1 |
 | ![Sparkle(Honkai: Star Rail) 1920x1080 by voyager](https://w.wallhaven.cc/full/1p/wallhaven-1pwxv1.png) | [voyager](https://wallhaven.cc/user/voyager) | https://wallhaven.cc/w/1pwxv1 |
+
+All images remain property of their original owners. Owners may request removal of images at any time.
```

### Comparing `wallpaper_factory-0.0.7/README.md` & `wallpaper_factory-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: wallpaper_factory
+Version: 0.0.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: opencv-python
+Requires-Dist: pillow
+
 # Wallpaper Factory
 
 ## Table of Content
 
 -   [Installation](#Installation)
 -   [Usage](#Usage)
 -   [Currently Available color schemes](#Currently-Available-color-schemes)
@@ -84,7 +92,9 @@
 
 ### Example Images
 
 | Original                                                                                                | Made By                                      | Link                          |
 | ------------------------------------------------------------------------------------------------------- | -------------------------------------------- | ----------------------------- |
 | ![Kaga(Azure Lane) 1920x1080 by voyager](https://w.wallhaven.cc/full/m9/wallhaven-m9e9m1.png)           | [voyager](https://wallhaven.cc/user/voyager) | https://wallhaven.cc/w/m9e9m1 |
 | ![Sparkle(Honkai: Star Rail) 1920x1080 by voyager](https://w.wallhaven.cc/full/1p/wallhaven-1pwxv1.png) | [voyager](https://wallhaven.cc/user/voyager) | https://wallhaven.cc/w/1pwxv1 |
+
+All images remain property of their original owners. Owners may request removal of images at any time.
```

### Comparing `wallpaper_factory-0.0.7/src/wallpaper_factory/available_palletes.py` & `wallpaper_factory-0.0.8/src/wallpaper_factory/available_palletes.py`

 * *Files identical despite different names*

### Comparing `wallpaper_factory-0.0.7/src/wallpaper_factory/main.py` & `wallpaper_factory-0.0.8/src/wallpaper_factory/main.py`

 * *Files identical despite different names*

### Comparing `wallpaper_factory-0.0.7/src/wallpaper_factory.egg-info/PKG-INFO` & `wallpaper_factory-0.0.8/src/wallpaper_factory.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wallpaper_factory
-Version: 0.0.7
+Version: 0.0.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
 Requires-Dist: pillow
 
 # Wallpaper Factory
 
@@ -92,7 +92,9 @@
 
 ### Example Images
 
 | Original                                                                                                | Made By                                      | Link                          |
 | ------------------------------------------------------------------------------------------------------- | -------------------------------------------- | ----------------------------- |
 | ![Kaga(Azure Lane) 1920x1080 by voyager](https://w.wallhaven.cc/full/m9/wallhaven-m9e9m1.png)           | [voyager](https://wallhaven.cc/user/voyager) | https://wallhaven.cc/w/m9e9m1 |
 | ![Sparkle(Honkai: Star Rail) 1920x1080 by voyager](https://w.wallhaven.cc/full/1p/wallhaven-1pwxv1.png) | [voyager](https://wallhaven.cc/user/voyager) | https://wallhaven.cc/w/1pwxv1 |
+
+All images remain property of their original owners. Owners may request removal of images at any time.
```

