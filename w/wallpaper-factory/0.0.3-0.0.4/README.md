# Comparing `tmp/wallpaper_factory-0.0.3.tar.gz` & `tmp/wallpaper_factory-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wallpaper_factory-0.0.3.tar", last modified: Tue Apr 30 13:16:14 2024, max compression
+gzip compressed data, was "wallpaper_factory-0.0.4.tar", last modified: Tue Apr 30 13:18:33 2024, max compression
```

## Comparing `wallpaper_factory-0.0.3.tar` & `wallpaper_factory-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:16:14.382939 wallpaper_factory-0.0.3/
--rw-r--r--   0 marlonkunz   (501) staff       (20)    35149 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.3/LICENSE
--rw-r--r--   0 marlonkunz   (501) staff       (20)     4241 2024-04-30 13:16:14.382740 wallpaper_factory-0.0.3/PKG-INFO
--rw-r--r--   0 marlonkunz   (501) staff       (20)     4066 2024-04-30 13:14:58.000000 wallpaper_factory-0.0.3/README.md
--rw-r--r--   0 marlonkunz   (501) staff       (20)       38 2024-04-30 13:16:14.382981 wallpaper_factory-0.0.3/setup.cfg
--rw-r--r--   0 marlonkunz   (501) staff       (20)      396 2024-04-30 13:16:06.000000 wallpaper_factory-0.0.3/setup.py
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:16:14.379716 wallpaper_factory-0.0.3/src/
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:16:14.381530 wallpaper_factory-0.0.3/src/wallpaper_factory/
--rw-r--r--   0 marlonkunz   (501) staff       (20)       61 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.3/src/wallpaper_factory/__init__.py
--rw-r--r--   0 marlonkunz   (501) staff       (20)     1564 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.3/src/wallpaper_factory/available_palletes.py
--rw-r--r--   0 marlonkunz   (501) staff       (20)     3719 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.3/src/wallpaper_factory/main.py
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:16:14.382508 wallpaper_factory-0.0.3/src/wallpaper_factory.egg-info/
--rw-r--r--   0 marlonkunz   (501) staff       (20)     4241 2024-04-30 13:16:14.000000 wallpaper_factory-0.0.3/src/wallpaper_factory.egg-info/PKG-INFO
--rw-r--r--   0 marlonkunz   (501) staff       (20)      406 2024-04-30 13:16:14.000000 wallpaper_factory-0.0.3/src/wallpaper_factory.egg-info/SOURCES.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)        1 2024-04-30 13:16:14.000000 wallpaper_factory-0.0.3/src/wallpaper_factory.egg-info/dependency_links.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       74 2024-04-30 13:16:14.000000 wallpaper_factory-0.0.3/src/wallpaper_factory.egg-info/entry_points.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       21 2024-04-30 13:16:14.000000 wallpaper_factory-0.0.3/src/wallpaper_factory.egg-info/requires.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       18 2024-04-30 13:16:14.000000 wallpaper_factory-0.0.3/src/wallpaper_factory.egg-info/top_level.txt
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:18:33.201351 wallpaper_factory-0.0.4/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)    35149 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.4/LICENSE
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     4306 2024-04-30 13:18:33.201161 wallpaper_factory-0.0.4/PKG-INFO
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     4131 2024-04-30 13:18:06.000000 wallpaper_factory-0.0.4/README.md
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       38 2024-04-30 13:18:33.201396 wallpaper_factory-0.0.4/setup.cfg
+-rw-r--r--   0 marlonkunz   (501) staff       (20)      396 2024-04-30 13:18:25.000000 wallpaper_factory-0.0.4/setup.py
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:18:33.198537 wallpaper_factory-0.0.4/src/
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:18:33.199983 wallpaper_factory-0.0.4/src/wallpaper_factory/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       61 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.4/src/wallpaper_factory/__init__.py
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     1564 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.4/src/wallpaper_factory/available_palletes.py
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     3719 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.4/src/wallpaper_factory/main.py
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:18:33.200928 wallpaper_factory-0.0.4/src/wallpaper_factory.egg-info/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     4306 2024-04-30 13:18:33.000000 wallpaper_factory-0.0.4/src/wallpaper_factory.egg-info/PKG-INFO
+-rw-r--r--   0 marlonkunz   (501) staff       (20)      406 2024-04-30 13:18:33.000000 wallpaper_factory-0.0.4/src/wallpaper_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)        1 2024-04-30 13:18:33.000000 wallpaper_factory-0.0.4/src/wallpaper_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       74 2024-04-30 13:18:33.000000 wallpaper_factory-0.0.4/src/wallpaper_factory.egg-info/entry_points.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       21 2024-04-30 13:18:33.000000 wallpaper_factory-0.0.4/src/wallpaper_factory.egg-info/requires.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       18 2024-04-30 13:18:33.000000 wallpaper_factory-0.0.4/src/wallpaper_factory.egg-info/top_level.txt
```

### Comparing `wallpaper_factory-0.0.3/LICENSE` & `wallpaper_factory-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wallpaper_factory-0.0.3/PKG-INFO` & `wallpaper_factory-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wallpaper_factory
-Version: 0.0.3
+Version: 0.0.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
 Requires-Dist: pillow
 
 # Wallpaper Factory
 
@@ -61,19 +61,19 @@
 
 if you chose to generate a denoised version of the image as well.
 
 ## Currently Available color schemes
 
 ### Gruvbox
 
-| made by       | [morhetz](https://github.com/morhetz)                                                                                                                                        |
-| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| repository    | [gruvbox](https://github.com/morhetz/gruvbox)                                                                                                                                |
-| palette       | ![palette](https://camo.githubusercontent.com/72015eab40bd7a696e2802810d7519480d51a2fba75f0f873dc23b990eb860f8/687474703a2f2f692e696d6775722e636f6d2f776136363678672e706e67) |
-| example image | ![./assets/gruvbox/gruvbox_dark_medium_wallhaven-m9e9m1.png](./assets/gruvbox/gruvbox_dark_medium_wallhaven-m9e9m1.png)                                                      |
+| made by       | [morhetz](https://github.com/morhetz)                                                                                                                                                     |
+| ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| repository    | [gruvbox](https://github.com/morhetz/gruvbox)                                                                                                                                             |
+| palette       | ![palette](https://camo.githubusercontent.com/72015eab40bd7a696e2802810d7519480d51a2fba75f0f873dc23b990eb860f8/687474703a2f2f692e696d6775722e636f6d2f776136363678672e706e67)              |
+| example image | ![./assets/gruvbox/gruvbox_dark_medium_wallhaven-m9e9m1.png](https://raw.githubusercontent.com/TheBaum123/wallpaper-factory/main/assets/gruvbox/gruvbox_dark_medium_wallhaven-m9e9m1.png) |
 
 ### rose pine moon
 
 | made by       | [?Rosé Pine?](https://rosepinetheme.com/)                                                            |
 | ------------- | ---------------------------------------------------------------------------------------------------- |
 | repository    | [rose-pine-theme](https://github.com/rose-pine/rose-pine-theme)                                      |
 | palette       | ![palette](https://raw.githubusercontent.com/rose-pine/rose-pine-theme/main/assets/palette-moon.png) |
```

### Comparing `wallpaper_factory-0.0.3/README.md` & `wallpaper_factory-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,19 +53,19 @@
 
 if you chose to generate a denoised version of the image as well.
 
 ## Currently Available color schemes
 
 ### Gruvbox
 
-| made by       | [morhetz](https://github.com/morhetz)                                                                                                                                        |
-| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| repository    | [gruvbox](https://github.com/morhetz/gruvbox)                                                                                                                                |
-| palette       | ![palette](https://camo.githubusercontent.com/72015eab40bd7a696e2802810d7519480d51a2fba75f0f873dc23b990eb860f8/687474703a2f2f692e696d6775722e636f6d2f776136363678672e706e67) |
-| example image | ![./assets/gruvbox/gruvbox_dark_medium_wallhaven-m9e9m1.png](./assets/gruvbox/gruvbox_dark_medium_wallhaven-m9e9m1.png)                                                      |
+| made by       | [morhetz](https://github.com/morhetz)                                                                                                                                                     |
+| ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| repository    | [gruvbox](https://github.com/morhetz/gruvbox)                                                                                                                                             |
+| palette       | ![palette](https://camo.githubusercontent.com/72015eab40bd7a696e2802810d7519480d51a2fba75f0f873dc23b990eb860f8/687474703a2f2f692e696d6775722e636f6d2f776136363678672e706e67)              |
+| example image | ![./assets/gruvbox/gruvbox_dark_medium_wallhaven-m9e9m1.png](https://raw.githubusercontent.com/TheBaum123/wallpaper-factory/main/assets/gruvbox/gruvbox_dark_medium_wallhaven-m9e9m1.png) |
 
 ### rose pine moon
 
 | made by       | [?Rosé Pine?](https://rosepinetheme.com/)                                                            |
 | ------------- | ---------------------------------------------------------------------------------------------------- |
 | repository    | [rose-pine-theme](https://github.com/rose-pine/rose-pine-theme)                                      |
 | palette       | ![palette](https://raw.githubusercontent.com/rose-pine/rose-pine-theme/main/assets/palette-moon.png) |
```

### Comparing `wallpaper_factory-0.0.3/src/wallpaper_factory/available_palletes.py` & `wallpaper_factory-0.0.4/src/wallpaper_factory/available_palletes.py`

 * *Files identical despite different names*

### Comparing `wallpaper_factory-0.0.3/src/wallpaper_factory/main.py` & `wallpaper_factory-0.0.4/src/wallpaper_factory/main.py`

 * *Files identical despite different names*

### Comparing `wallpaper_factory-0.0.3/src/wallpaper_factory.egg-info/PKG-INFO` & `wallpaper_factory-0.0.4/src/wallpaper_factory.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wallpaper_factory
-Version: 0.0.3
+Version: 0.0.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
 Requires-Dist: pillow
 
 # Wallpaper Factory
 
@@ -61,19 +61,19 @@
 
 if you chose to generate a denoised version of the image as well.
 
 ## Currently Available color schemes
 
 ### Gruvbox
 
-| made by       | [morhetz](https://github.com/morhetz)                                                                                                                                        |
-| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| repository    | [gruvbox](https://github.com/morhetz/gruvbox)                                                                                                                                |
-| palette       | ![palette](https://camo.githubusercontent.com/72015eab40bd7a696e2802810d7519480d51a2fba75f0f873dc23b990eb860f8/687474703a2f2f692e696d6775722e636f6d2f776136363678672e706e67) |
-| example image | ![./assets/gruvbox/gruvbox_dark_medium_wallhaven-m9e9m1.png](./assets/gruvbox/gruvbox_dark_medium_wallhaven-m9e9m1.png)                                                      |
+| made by       | [morhetz](https://github.com/morhetz)                                                                                                                                                     |
+| ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| repository    | [gruvbox](https://github.com/morhetz/gruvbox)                                                                                                                                             |
+| palette       | ![palette](https://camo.githubusercontent.com/72015eab40bd7a696e2802810d7519480d51a2fba75f0f873dc23b990eb860f8/687474703a2f2f692e696d6775722e636f6d2f776136363678672e706e67)              |
+| example image | ![./assets/gruvbox/gruvbox_dark_medium_wallhaven-m9e9m1.png](https://raw.githubusercontent.com/TheBaum123/wallpaper-factory/main/assets/gruvbox/gruvbox_dark_medium_wallhaven-m9e9m1.png) |
 
 ### rose pine moon
 
 | made by       | [?Rosé Pine?](https://rosepinetheme.com/)                                                            |
 | ------------- | ---------------------------------------------------------------------------------------------------- |
 | repository    | [rose-pine-theme](https://github.com/rose-pine/rose-pine-theme)                                      |
 | palette       | ![palette](https://raw.githubusercontent.com/rose-pine/rose-pine-theme/main/assets/palette-moon.png) |
```

