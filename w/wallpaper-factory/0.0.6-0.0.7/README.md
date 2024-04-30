# Comparing `tmp/wallpaper_factory-0.0.6.tar.gz` & `tmp/wallpaper_factory-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wallpaper_factory-0.0.6.tar", last modified: Tue Apr 30 13:44:26 2024, max compression
+gzip compressed data, was "wallpaper_factory-0.0.7.tar", last modified: Tue Apr 30 13:48:56 2024, max compression
```

## Comparing `wallpaper_factory-0.0.6.tar` & `wallpaper_factory-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:44:26.606368 wallpaper_factory-0.0.6/
--rw-r--r--   0 marlonkunz   (501) staff       (20)    35149 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.6/LICENSE
--rw-r--r--   0 marlonkunz   (501) staff       (20)     5603 2024-04-30 13:44:26.606155 wallpaper_factory-0.0.6/PKG-INFO
--rw-r--r--   0 marlonkunz   (501) staff       (20)     5428 2024-04-30 13:44:07.000000 wallpaper_factory-0.0.6/README.md
--rw-r--r--   0 marlonkunz   (501) staff       (20)       38 2024-04-30 13:44:26.606411 wallpaper_factory-0.0.6/setup.cfg
--rw-r--r--   0 marlonkunz   (501) staff       (20)      396 2024-04-30 13:44:14.000000 wallpaper_factory-0.0.6/setup.py
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:44:26.603276 wallpaper_factory-0.0.6/src/
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:44:26.604942 wallpaper_factory-0.0.6/src/wallpaper_factory/
--rw-r--r--   0 marlonkunz   (501) staff       (20)       61 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.6/src/wallpaper_factory/__init__.py
--rw-r--r--   0 marlonkunz   (501) staff       (20)     2378 2024-04-30 13:33:15.000000 wallpaper_factory-0.0.6/src/wallpaper_factory/available_palletes.py
--rw-r--r--   0 marlonkunz   (501) staff       (20)     3719 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.6/src/wallpaper_factory/main.py
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:44:26.605921 wallpaper_factory-0.0.6/src/wallpaper_factory.egg-info/
--rw-r--r--   0 marlonkunz   (501) staff       (20)     5603 2024-04-30 13:44:26.000000 wallpaper_factory-0.0.6/src/wallpaper_factory.egg-info/PKG-INFO
--rw-r--r--   0 marlonkunz   (501) staff       (20)      406 2024-04-30 13:44:26.000000 wallpaper_factory-0.0.6/src/wallpaper_factory.egg-info/SOURCES.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)        1 2024-04-30 13:44:26.000000 wallpaper_factory-0.0.6/src/wallpaper_factory.egg-info/dependency_links.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       74 2024-04-30 13:44:26.000000 wallpaper_factory-0.0.6/src/wallpaper_factory.egg-info/entry_points.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       21 2024-04-30 13:44:26.000000 wallpaper_factory-0.0.6/src/wallpaper_factory.egg-info/requires.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       18 2024-04-30 13:44:26.000000 wallpaper_factory-0.0.6/src/wallpaper_factory.egg-info/top_level.txt
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:48:56.575783 wallpaper_factory-0.0.7/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)    35149 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.7/LICENSE
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     5820 2024-04-30 13:48:56.575530 wallpaper_factory-0.0.7/PKG-INFO
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     5645 2024-04-30 13:48:24.000000 wallpaper_factory-0.0.7/README.md
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       38 2024-04-30 13:48:56.575834 wallpaper_factory-0.0.7/setup.cfg
+-rw-r--r--   0 marlonkunz   (501) staff       (20)      396 2024-04-30 13:48:51.000000 wallpaper_factory-0.0.7/setup.py
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:48:56.571529 wallpaper_factory-0.0.7/src/
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:48:56.573792 wallpaper_factory-0.0.7/src/wallpaper_factory/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       61 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.7/src/wallpaper_factory/__init__.py
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     2378 2024-04-30 13:33:15.000000 wallpaper_factory-0.0.7/src/wallpaper_factory/available_palletes.py
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     3719 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.7/src/wallpaper_factory/main.py
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:48:56.575211 wallpaper_factory-0.0.7/src/wallpaper_factory.egg-info/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     5820 2024-04-30 13:48:56.000000 wallpaper_factory-0.0.7/src/wallpaper_factory.egg-info/PKG-INFO
+-rw-r--r--   0 marlonkunz   (501) staff       (20)      406 2024-04-30 13:48:56.000000 wallpaper_factory-0.0.7/src/wallpaper_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)        1 2024-04-30 13:48:56.000000 wallpaper_factory-0.0.7/src/wallpaper_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       74 2024-04-30 13:48:56.000000 wallpaper_factory-0.0.7/src/wallpaper_factory.egg-info/entry_points.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       21 2024-04-30 13:48:56.000000 wallpaper_factory-0.0.7/src/wallpaper_factory.egg-info/requires.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       18 2024-04-30 13:48:56.000000 wallpaper_factory-0.0.7/src/wallpaper_factory.egg-info/top_level.txt
```

### Comparing `wallpaper_factory-0.0.6/LICENSE` & `wallpaper_factory-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wallpaper_factory-0.0.6/PKG-INFO` & `wallpaper_factory-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wallpaper_factory
-Version: 0.0.6
+Version: 0.0.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
 Requires-Dist: pillow
 
 # Wallpaper Factory
 
@@ -88,10 +88,11 @@
 | palette       | ![palette](https://user-images.githubusercontent.com/58662350/214382352-cd7a4f63-e6ef-4575-82c0-a8b72aa37c0c.png)                                                                                                             |
 | example image | ![./assets/everforest_dark_medium/everforest_dark_medium_wallhaven-1pwxv1.png](https://raw.githubusercontent.com/TheBaum123/wallpaper-factory/main/assets/everforest_dark_medium/everforest_dark_medium_wallhaven-1pwxv1.png) |
 
 ## Attributions
 
 ### Example Images
 
-| Original                                                                                      | Made By                                      | Link                          |
-| --------------------------------------------------------------------------------------------- | -------------------------------------------- | ----------------------------- |
-| ![Kaga(Azure Lane) 1920x1080 by voyager](https://w.wallhaven.cc/full/m9/wallhaven-m9e9m1.png) | [voyager](https://wallhaven.cc/user/voyager) | https://wallhaven.cc/w/m9e9m1 |
+| Original                                                                                                | Made By                                      | Link                          |
+| ------------------------------------------------------------------------------------------------------- | -------------------------------------------- | ----------------------------- |
+| ![Kaga(Azure Lane) 1920x1080 by voyager](https://w.wallhaven.cc/full/m9/wallhaven-m9e9m1.png)           | [voyager](https://wallhaven.cc/user/voyager) | https://wallhaven.cc/w/m9e9m1 |
+| ![Sparkle(Honkai: Star Rail) 1920x1080 by voyager](https://w.wallhaven.cc/full/1p/wallhaven-1pwxv1.png) | [voyager](https://wallhaven.cc/user/voyager) | https://wallhaven.cc/w/1pwxv1 |
```

### Comparing `wallpaper_factory-0.0.6/README.md` & `wallpaper_factory-0.0.7/src/wallpaper_factory.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: wallpaper_factory
+Version: 0.0.7
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
@@ -80,10 +88,11 @@
 | palette       | ![palette](https://user-images.githubusercontent.com/58662350/214382352-cd7a4f63-e6ef-4575-82c0-a8b72aa37c0c.png)                                                                                                             |
 | example image | ![./assets/everforest_dark_medium/everforest_dark_medium_wallhaven-1pwxv1.png](https://raw.githubusercontent.com/TheBaum123/wallpaper-factory/main/assets/everforest_dark_medium/everforest_dark_medium_wallhaven-1pwxv1.png) |
 
 ## Attributions
 
 ### Example Images
 
-| Original                                                                                      | Made By                                      | Link                          |
-| --------------------------------------------------------------------------------------------- | -------------------------------------------- | ----------------------------- |
-| ![Kaga(Azure Lane) 1920x1080 by voyager](https://w.wallhaven.cc/full/m9/wallhaven-m9e9m1.png) | [voyager](https://wallhaven.cc/user/voyager) | https://wallhaven.cc/w/m9e9m1 |
+| Original                                                                                                | Made By                                      | Link                          |
+| ------------------------------------------------------------------------------------------------------- | -------------------------------------------- | ----------------------------- |
+| ![Kaga(Azure Lane) 1920x1080 by voyager](https://w.wallhaven.cc/full/m9/wallhaven-m9e9m1.png)           | [voyager](https://wallhaven.cc/user/voyager) | https://wallhaven.cc/w/m9e9m1 |
+| ![Sparkle(Honkai: Star Rail) 1920x1080 by voyager](https://w.wallhaven.cc/full/1p/wallhaven-1pwxv1.png) | [voyager](https://wallhaven.cc/user/voyager) | https://wallhaven.cc/w/1pwxv1 |
```

### Comparing `wallpaper_factory-0.0.6/src/wallpaper_factory/available_palletes.py` & `wallpaper_factory-0.0.7/src/wallpaper_factory/available_palletes.py`

 * *Files identical despite different names*

### Comparing `wallpaper_factory-0.0.6/src/wallpaper_factory/main.py` & `wallpaper_factory-0.0.7/src/wallpaper_factory/main.py`

 * *Files identical despite different names*

### Comparing `wallpaper_factory-0.0.6/src/wallpaper_factory.egg-info/PKG-INFO` & `wallpaper_factory-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: wallpaper_factory
-Version: 0.0.6
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
@@ -88,10 +80,11 @@
 | palette       | ![palette](https://user-images.githubusercontent.com/58662350/214382352-cd7a4f63-e6ef-4575-82c0-a8b72aa37c0c.png)                                                                                                             |
 | example image | ![./assets/everforest_dark_medium/everforest_dark_medium_wallhaven-1pwxv1.png](https://raw.githubusercontent.com/TheBaum123/wallpaper-factory/main/assets/everforest_dark_medium/everforest_dark_medium_wallhaven-1pwxv1.png) |
 
 ## Attributions
 
 ### Example Images
 
-| Original                                                                                      | Made By                                      | Link                          |
-| --------------------------------------------------------------------------------------------- | -------------------------------------------- | ----------------------------- |
-| ![Kaga(Azure Lane) 1920x1080 by voyager](https://w.wallhaven.cc/full/m9/wallhaven-m9e9m1.png) | [voyager](https://wallhaven.cc/user/voyager) | https://wallhaven.cc/w/m9e9m1 |
+| Original                                                                                                | Made By                                      | Link                          |
+| ------------------------------------------------------------------------------------------------------- | -------------------------------------------- | ----------------------------- |
+| ![Kaga(Azure Lane) 1920x1080 by voyager](https://w.wallhaven.cc/full/m9/wallhaven-m9e9m1.png)           | [voyager](https://wallhaven.cc/user/voyager) | https://wallhaven.cc/w/m9e9m1 |
+| ![Sparkle(Honkai: Star Rail) 1920x1080 by voyager](https://w.wallhaven.cc/full/1p/wallhaven-1pwxv1.png) | [voyager](https://wallhaven.cc/user/voyager) | https://wallhaven.cc/w/1pwxv1 |
```

