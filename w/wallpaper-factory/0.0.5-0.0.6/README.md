# Comparing `tmp/wallpaper_factory-0.0.5.tar.gz` & `tmp/wallpaper_factory-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wallpaper_factory-0.0.5.tar", last modified: Tue Apr 30 13:37:24 2024, max compression
+gzip compressed data, was "wallpaper_factory-0.0.6.tar", last modified: Tue Apr 30 13:44:26 2024, max compression
```

## Comparing `wallpaper_factory-0.0.5.tar` & `wallpaper_factory-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:37:24.360388 wallpaper_factory-0.0.5/
--rw-r--r--   0 marlonkunz   (501) staff       (20)    35149 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.5/LICENSE
--rw-r--r--   0 marlonkunz   (501) staff       (20)     5005 2024-04-30 13:37:24.360196 wallpaper_factory-0.0.5/PKG-INFO
--rw-r--r--   0 marlonkunz   (501) staff       (20)     4830 2024-04-30 13:36:35.000000 wallpaper_factory-0.0.5/README.md
--rw-r--r--   0 marlonkunz   (501) staff       (20)       38 2024-04-30 13:37:24.360430 wallpaper_factory-0.0.5/setup.cfg
--rw-r--r--   0 marlonkunz   (501) staff       (20)      396 2024-04-30 13:37:09.000000 wallpaper_factory-0.0.5/setup.py
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:37:24.357213 wallpaper_factory-0.0.5/src/
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:37:24.358957 wallpaper_factory-0.0.5/src/wallpaper_factory/
--rw-r--r--   0 marlonkunz   (501) staff       (20)       61 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.5/src/wallpaper_factory/__init__.py
--rw-r--r--   0 marlonkunz   (501) staff       (20)     2378 2024-04-30 13:33:15.000000 wallpaper_factory-0.0.5/src/wallpaper_factory/available_palletes.py
--rw-r--r--   0 marlonkunz   (501) staff       (20)     3719 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.5/src/wallpaper_factory/main.py
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:37:24.359963 wallpaper_factory-0.0.5/src/wallpaper_factory.egg-info/
--rw-r--r--   0 marlonkunz   (501) staff       (20)     5005 2024-04-30 13:37:24.000000 wallpaper_factory-0.0.5/src/wallpaper_factory.egg-info/PKG-INFO
--rw-r--r--   0 marlonkunz   (501) staff       (20)      406 2024-04-30 13:37:24.000000 wallpaper_factory-0.0.5/src/wallpaper_factory.egg-info/SOURCES.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)        1 2024-04-30 13:37:24.000000 wallpaper_factory-0.0.5/src/wallpaper_factory.egg-info/dependency_links.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       74 2024-04-30 13:37:24.000000 wallpaper_factory-0.0.5/src/wallpaper_factory.egg-info/entry_points.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       21 2024-04-30 13:37:24.000000 wallpaper_factory-0.0.5/src/wallpaper_factory.egg-info/requires.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       18 2024-04-30 13:37:24.000000 wallpaper_factory-0.0.5/src/wallpaper_factory.egg-info/top_level.txt
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:44:26.606368 wallpaper_factory-0.0.6/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)    35149 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.6/LICENSE
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     5603 2024-04-30 13:44:26.606155 wallpaper_factory-0.0.6/PKG-INFO
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     5428 2024-04-30 13:44:07.000000 wallpaper_factory-0.0.6/README.md
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       38 2024-04-30 13:44:26.606411 wallpaper_factory-0.0.6/setup.cfg
+-rw-r--r--   0 marlonkunz   (501) staff       (20)      396 2024-04-30 13:44:14.000000 wallpaper_factory-0.0.6/setup.py
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:44:26.603276 wallpaper_factory-0.0.6/src/
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:44:26.604942 wallpaper_factory-0.0.6/src/wallpaper_factory/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       61 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.6/src/wallpaper_factory/__init__.py
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     2378 2024-04-30 13:33:15.000000 wallpaper_factory-0.0.6/src/wallpaper_factory/available_palletes.py
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     3719 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.6/src/wallpaper_factory/main.py
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:44:26.605921 wallpaper_factory-0.0.6/src/wallpaper_factory.egg-info/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     5603 2024-04-30 13:44:26.000000 wallpaper_factory-0.0.6/src/wallpaper_factory.egg-info/PKG-INFO
+-rw-r--r--   0 marlonkunz   (501) staff       (20)      406 2024-04-30 13:44:26.000000 wallpaper_factory-0.0.6/src/wallpaper_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)        1 2024-04-30 13:44:26.000000 wallpaper_factory-0.0.6/src/wallpaper_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       74 2024-04-30 13:44:26.000000 wallpaper_factory-0.0.6/src/wallpaper_factory.egg-info/entry_points.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       21 2024-04-30 13:44:26.000000 wallpaper_factory-0.0.6/src/wallpaper_factory.egg-info/requires.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       18 2024-04-30 13:44:26.000000 wallpaper_factory-0.0.6/src/wallpaper_factory.egg-info/top_level.txt
```

### Comparing `wallpaper_factory-0.0.5/LICENSE` & `wallpaper_factory-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wallpaper_factory-0.0.5/PKG-INFO` & `wallpaper_factory-0.0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: wallpaper_factory
-Version: 0.0.5
+Version: 0.0.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
 Requires-Dist: pillow
 
 # Wallpaper Factory
 
 ## Table of Content
 
 -   [Installation](#Installation)
 -   [Usage](#Usage)
 -   [Currently Available color schemes](#Currently-Available-color-schemes)
     -   [Gruvbox](#Gruvbox)
     -   [rose pine moon](#rose-pine-moon)
+    -   [everforest medium dark](#everforest-medium-dark)
 -   [Attributions](#Attributions)
     -   [Example Images](#Example-Images)
 
 ## Installation
 
 You can install this package / cli utility by running `pip install wallpaper-factory`.
 
@@ -77,19 +78,19 @@
 | ------------- | ---------------------------------------------------------------------------------------------------- |
 | repository    | [rose-pine-theme](https://github.com/rose-pine/rose-pine-theme)                                      |
 | palette       | ![palette](https://raw.githubusercontent.com/rose-pine/rose-pine-theme/main/assets/palette-moon.png) |
 | example image | waiting for consent to distribute                                                                    |
 
 ### everforest medium dark
 
-| made by       | [sainnhe](https://github.com/sainnhe)                                                                             |
-| ------------- | ----------------------------------------------------------------------------------------------------------------- |
-| repository    | [everforest](https://github.com/sainnhe/everforest)                                                               |
-| palette       | ![palette](https://user-images.githubusercontent.com/58662350/214382352-cd7a4f63-e6ef-4575-82c0-a8b72aa37c0c.png) |
-| example image | TODO                                                                                                              |
+| made by       | [sainnhe](https://github.com/sainnhe)                                                                                                                                                                                         |
+| ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| repository    | [everforest](https://github.com/sainnhe/everforest)                                                                                                                                                                           |
+| palette       | ![palette](https://user-images.githubusercontent.com/58662350/214382352-cd7a4f63-e6ef-4575-82c0-a8b72aa37c0c.png)                                                                                                             |
+| example image | ![./assets/everforest_dark_medium/everforest_dark_medium_wallhaven-1pwxv1.png](https://raw.githubusercontent.com/TheBaum123/wallpaper-factory/main/assets/everforest_dark_medium/everforest_dark_medium_wallhaven-1pwxv1.png) |
 
 ## Attributions
 
 ### Example Images
 
 | Original                                                                                      | Made By                                      | Link                          |
 | --------------------------------------------------------------------------------------------- | -------------------------------------------- | ----------------------------- |
```

### Comparing `wallpaper_factory-0.0.5/README.md` & `wallpaper_factory-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 ## Table of Content
 
 -   [Installation](#Installation)
 -   [Usage](#Usage)
 -   [Currently Available color schemes](#Currently-Available-color-schemes)
     -   [Gruvbox](#Gruvbox)
     -   [rose pine moon](#rose-pine-moon)
+    -   [everforest medium dark](#everforest-medium-dark)
 -   [Attributions](#Attributions)
     -   [Example Images](#Example-Images)
 
 ## Installation
 
 You can install this package / cli utility by running `pip install wallpaper-factory`.
 
@@ -69,19 +70,19 @@
 | ------------- | ---------------------------------------------------------------------------------------------------- |
 | repository    | [rose-pine-theme](https://github.com/rose-pine/rose-pine-theme)                                      |
 | palette       | ![palette](https://raw.githubusercontent.com/rose-pine/rose-pine-theme/main/assets/palette-moon.png) |
 | example image | waiting for consent to distribute                                                                    |
 
 ### everforest medium dark
 
-| made by       | [sainnhe](https://github.com/sainnhe)                                                                             |
-| ------------- | ----------------------------------------------------------------------------------------------------------------- |
-| repository    | [everforest](https://github.com/sainnhe/everforest)                                                               |
-| palette       | ![palette](https://user-images.githubusercontent.com/58662350/214382352-cd7a4f63-e6ef-4575-82c0-a8b72aa37c0c.png) |
-| example image | TODO                                                                                                              |
+| made by       | [sainnhe](https://github.com/sainnhe)                                                                                                                                                                                         |
+| ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| repository    | [everforest](https://github.com/sainnhe/everforest)                                                                                                                                                                           |
+| palette       | ![palette](https://user-images.githubusercontent.com/58662350/214382352-cd7a4f63-e6ef-4575-82c0-a8b72aa37c0c.png)                                                                                                             |
+| example image | ![./assets/everforest_dark_medium/everforest_dark_medium_wallhaven-1pwxv1.png](https://raw.githubusercontent.com/TheBaum123/wallpaper-factory/main/assets/everforest_dark_medium/everforest_dark_medium_wallhaven-1pwxv1.png) |
 
 ## Attributions
 
 ### Example Images
 
 | Original                                                                                      | Made By                                      | Link                          |
 | --------------------------------------------------------------------------------------------- | -------------------------------------------- | ----------------------------- |
```

### Comparing `wallpaper_factory-0.0.5/src/wallpaper_factory/available_palletes.py` & `wallpaper_factory-0.0.6/src/wallpaper_factory/available_palletes.py`

 * *Files identical despite different names*

### Comparing `wallpaper_factory-0.0.5/src/wallpaper_factory/main.py` & `wallpaper_factory-0.0.6/src/wallpaper_factory/main.py`

 * *Files identical despite different names*

### Comparing `wallpaper_factory-0.0.5/src/wallpaper_factory.egg-info/PKG-INFO` & `wallpaper_factory-0.0.6/src/wallpaper_factory.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: wallpaper_factory
-Version: 0.0.5
+Version: 0.0.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
 Requires-Dist: pillow
 
 # Wallpaper Factory
 
 ## Table of Content
 
 -   [Installation](#Installation)
 -   [Usage](#Usage)
 -   [Currently Available color schemes](#Currently-Available-color-schemes)
     -   [Gruvbox](#Gruvbox)
     -   [rose pine moon](#rose-pine-moon)
+    -   [everforest medium dark](#everforest-medium-dark)
 -   [Attributions](#Attributions)
     -   [Example Images](#Example-Images)
 
 ## Installation
 
 You can install this package / cli utility by running `pip install wallpaper-factory`.
 
@@ -77,19 +78,19 @@
 | ------------- | ---------------------------------------------------------------------------------------------------- |
 | repository    | [rose-pine-theme](https://github.com/rose-pine/rose-pine-theme)                                      |
 | palette       | ![palette](https://raw.githubusercontent.com/rose-pine/rose-pine-theme/main/assets/palette-moon.png) |
 | example image | waiting for consent to distribute                                                                    |
 
 ### everforest medium dark
 
-| made by       | [sainnhe](https://github.com/sainnhe)                                                                             |
-| ------------- | ----------------------------------------------------------------------------------------------------------------- |
-| repository    | [everforest](https://github.com/sainnhe/everforest)                                                               |
-| palette       | ![palette](https://user-images.githubusercontent.com/58662350/214382352-cd7a4f63-e6ef-4575-82c0-a8b72aa37c0c.png) |
-| example image | TODO                                                                                                              |
+| made by       | [sainnhe](https://github.com/sainnhe)                                                                                                                                                                                         |
+| ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| repository    | [everforest](https://github.com/sainnhe/everforest)                                                                                                                                                                           |
+| palette       | ![palette](https://user-images.githubusercontent.com/58662350/214382352-cd7a4f63-e6ef-4575-82c0-a8b72aa37c0c.png)                                                                                                             |
+| example image | ![./assets/everforest_dark_medium/everforest_dark_medium_wallhaven-1pwxv1.png](https://raw.githubusercontent.com/TheBaum123/wallpaper-factory/main/assets/everforest_dark_medium/everforest_dark_medium_wallhaven-1pwxv1.png) |
 
 ## Attributions
 
 ### Example Images
 
 | Original                                                                                      | Made By                                      | Link                          |
 | --------------------------------------------------------------------------------------------- | -------------------------------------------- | ----------------------------- |
```

