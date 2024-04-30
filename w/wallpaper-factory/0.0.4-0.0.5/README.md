# Comparing `tmp/wallpaper_factory-0.0.4.tar.gz` & `tmp/wallpaper_factory-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wallpaper_factory-0.0.4.tar", last modified: Tue Apr 30 13:18:33 2024, max compression
+gzip compressed data, was "wallpaper_factory-0.0.5.tar", last modified: Tue Apr 30 13:37:24 2024, max compression
```

## Comparing `wallpaper_factory-0.0.4.tar` & `wallpaper_factory-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:18:33.201351 wallpaper_factory-0.0.4/
--rw-r--r--   0 marlonkunz   (501) staff       (20)    35149 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.4/LICENSE
--rw-r--r--   0 marlonkunz   (501) staff       (20)     4306 2024-04-30 13:18:33.201161 wallpaper_factory-0.0.4/PKG-INFO
--rw-r--r--   0 marlonkunz   (501) staff       (20)     4131 2024-04-30 13:18:06.000000 wallpaper_factory-0.0.4/README.md
--rw-r--r--   0 marlonkunz   (501) staff       (20)       38 2024-04-30 13:18:33.201396 wallpaper_factory-0.0.4/setup.cfg
--rw-r--r--   0 marlonkunz   (501) staff       (20)      396 2024-04-30 13:18:25.000000 wallpaper_factory-0.0.4/setup.py
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:18:33.198537 wallpaper_factory-0.0.4/src/
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:18:33.199983 wallpaper_factory-0.0.4/src/wallpaper_factory/
--rw-r--r--   0 marlonkunz   (501) staff       (20)       61 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.4/src/wallpaper_factory/__init__.py
--rw-r--r--   0 marlonkunz   (501) staff       (20)     1564 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.4/src/wallpaper_factory/available_palletes.py
--rw-r--r--   0 marlonkunz   (501) staff       (20)     3719 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.4/src/wallpaper_factory/main.py
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:18:33.200928 wallpaper_factory-0.0.4/src/wallpaper_factory.egg-info/
--rw-r--r--   0 marlonkunz   (501) staff       (20)     4306 2024-04-30 13:18:33.000000 wallpaper_factory-0.0.4/src/wallpaper_factory.egg-info/PKG-INFO
--rw-r--r--   0 marlonkunz   (501) staff       (20)      406 2024-04-30 13:18:33.000000 wallpaper_factory-0.0.4/src/wallpaper_factory.egg-info/SOURCES.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)        1 2024-04-30 13:18:33.000000 wallpaper_factory-0.0.4/src/wallpaper_factory.egg-info/dependency_links.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       74 2024-04-30 13:18:33.000000 wallpaper_factory-0.0.4/src/wallpaper_factory.egg-info/entry_points.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       21 2024-04-30 13:18:33.000000 wallpaper_factory-0.0.4/src/wallpaper_factory.egg-info/requires.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       18 2024-04-30 13:18:33.000000 wallpaper_factory-0.0.4/src/wallpaper_factory.egg-info/top_level.txt
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:37:24.360388 wallpaper_factory-0.0.5/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)    35149 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.5/LICENSE
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     5005 2024-04-30 13:37:24.360196 wallpaper_factory-0.0.5/PKG-INFO
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     4830 2024-04-30 13:36:35.000000 wallpaper_factory-0.0.5/README.md
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       38 2024-04-30 13:37:24.360430 wallpaper_factory-0.0.5/setup.cfg
+-rw-r--r--   0 marlonkunz   (501) staff       (20)      396 2024-04-30 13:37:09.000000 wallpaper_factory-0.0.5/setup.py
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:37:24.357213 wallpaper_factory-0.0.5/src/
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:37:24.358957 wallpaper_factory-0.0.5/src/wallpaper_factory/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       61 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.5/src/wallpaper_factory/__init__.py
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     2378 2024-04-30 13:33:15.000000 wallpaper_factory-0.0.5/src/wallpaper_factory/available_palletes.py
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     3719 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.5/src/wallpaper_factory/main.py
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:37:24.359963 wallpaper_factory-0.0.5/src/wallpaper_factory.egg-info/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     5005 2024-04-30 13:37:24.000000 wallpaper_factory-0.0.5/src/wallpaper_factory.egg-info/PKG-INFO
+-rw-r--r--   0 marlonkunz   (501) staff       (20)      406 2024-04-30 13:37:24.000000 wallpaper_factory-0.0.5/src/wallpaper_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)        1 2024-04-30 13:37:24.000000 wallpaper_factory-0.0.5/src/wallpaper_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       74 2024-04-30 13:37:24.000000 wallpaper_factory-0.0.5/src/wallpaper_factory.egg-info/entry_points.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       21 2024-04-30 13:37:24.000000 wallpaper_factory-0.0.5/src/wallpaper_factory.egg-info/requires.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       18 2024-04-30 13:37:24.000000 wallpaper_factory-0.0.5/src/wallpaper_factory.egg-info/top_level.txt
```

### Comparing `wallpaper_factory-0.0.4/LICENSE` & `wallpaper_factory-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wallpaper_factory-0.0.4/PKG-INFO` & `wallpaper_factory-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wallpaper_factory
-Version: 0.0.4
+Version: 0.0.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
 Requires-Dist: pillow
 
 # Wallpaper Factory
 
@@ -75,14 +75,22 @@
 
 | made by       | [?Rosé Pine?](https://rosepinetheme.com/)                                                            |
 | ------------- | ---------------------------------------------------------------------------------------------------- |
 | repository    | [rose-pine-theme](https://github.com/rose-pine/rose-pine-theme)                                      |
 | palette       | ![palette](https://raw.githubusercontent.com/rose-pine/rose-pine-theme/main/assets/palette-moon.png) |
 | example image | waiting for consent to distribute                                                                    |
 
+### everforest medium dark
+
+| made by       | [sainnhe](https://github.com/sainnhe)                                                                             |
+| ------------- | ----------------------------------------------------------------------------------------------------------------- |
+| repository    | [everforest](https://github.com/sainnhe/everforest)                                                               |
+| palette       | ![palette](https://user-images.githubusercontent.com/58662350/214382352-cd7a4f63-e6ef-4575-82c0-a8b72aa37c0c.png) |
+| example image | TODO                                                                                                              |
+
 ## Attributions
 
 ### Example Images
 
 | Original                                                                                      | Made By                                      | Link                          |
 | --------------------------------------------------------------------------------------------- | -------------------------------------------- | ----------------------------- |
 | ![Kaga(Azure Lane) 1920x1080 by voyager](https://w.wallhaven.cc/full/m9/wallhaven-m9e9m1.png) | [voyager](https://wallhaven.cc/user/voyager) | https://wallhaven.cc/w/m9e9m1 |
```

### Comparing `wallpaper_factory-0.0.4/README.md` & `wallpaper_factory-0.0.5/src/wallpaper_factory.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: wallpaper_factory
+Version: 0.0.5
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
@@ -67,14 +75,22 @@
 
 | made by       | [?Rosé Pine?](https://rosepinetheme.com/)                                                            |
 | ------------- | ---------------------------------------------------------------------------------------------------- |
 | repository    | [rose-pine-theme](https://github.com/rose-pine/rose-pine-theme)                                      |
 | palette       | ![palette](https://raw.githubusercontent.com/rose-pine/rose-pine-theme/main/assets/palette-moon.png) |
 | example image | waiting for consent to distribute                                                                    |
 
+### everforest medium dark
+
+| made by       | [sainnhe](https://github.com/sainnhe)                                                                             |
+| ------------- | ----------------------------------------------------------------------------------------------------------------- |
+| repository    | [everforest](https://github.com/sainnhe/everforest)                                                               |
+| palette       | ![palette](https://user-images.githubusercontent.com/58662350/214382352-cd7a4f63-e6ef-4575-82c0-a8b72aa37c0c.png) |
+| example image | TODO                                                                                                              |
+
 ## Attributions
 
 ### Example Images
 
 | Original                                                                                      | Made By                                      | Link                          |
 | --------------------------------------------------------------------------------------------- | -------------------------------------------- | ----------------------------- |
 | ![Kaga(Azure Lane) 1920x1080 by voyager](https://w.wallhaven.cc/full/m9/wallhaven-m9e9m1.png) | [voyager](https://wallhaven.cc/user/voyager) | https://wallhaven.cc/w/m9e9m1 |
```

### Comparing `wallpaper_factory-0.0.4/src/wallpaper_factory/available_palletes.py` & `wallpaper_factory-0.0.5/src/wallpaper_factory/available_palletes.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,8 +48,36 @@
             (156, 207, 216, 255),
             (196, 167, 231, 255),
             (42, 40, 62, 255),
             (68, 65, 90, 255),
             (86, 82, 110, 255),
         ],
     ],
+    [
+        "everforest_dark_medium",
+        [
+            (35, 42, 46, 255),
+            (45, 53, 59, 255),
+            (52, 63, 68, 255),
+            (45, 72, 77, 255),
+            (71, 82, 88, 255),
+            (79, 88, 94, 255),
+            (86, 99, 95, 255),
+            (84, 58, 72, 255),
+            (81, 64, 69, 255),
+            (77, 76, 67, 255),
+            (66, 80, 71, 255),
+            (58, 81, 93, 255),
+            (230, 126, 128, 255),
+            (230, 152, 117, 255),
+            (219, 188, 127, 255),
+            (167, 192, 128, 255),
+            (127, 187, 179, 255),
+            (131, 192, 146, 255),
+            (214, 153, 182, 255),
+            (211, 198, 170, 255),
+            (122, 132, 120, 255),
+            (133, 146, 137, 255),
+            (157, 169, 160, 255),
+        ],
+    ],
 ]
```

### Comparing `wallpaper_factory-0.0.4/src/wallpaper_factory/main.py` & `wallpaper_factory-0.0.5/src/wallpaper_factory/main.py`

 * *Files identical despite different names*

### Comparing `wallpaper_factory-0.0.4/src/wallpaper_factory.egg-info/PKG-INFO` & `wallpaper_factory-0.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: wallpaper_factory
-Version: 0.0.4
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
@@ -75,14 +67,22 @@
 
 | made by       | [?Rosé Pine?](https://rosepinetheme.com/)                                                            |
 | ------------- | ---------------------------------------------------------------------------------------------------- |
 | repository    | [rose-pine-theme](https://github.com/rose-pine/rose-pine-theme)                                      |
 | palette       | ![palette](https://raw.githubusercontent.com/rose-pine/rose-pine-theme/main/assets/palette-moon.png) |
 | example image | waiting for consent to distribute                                                                    |
 
+### everforest medium dark
+
+| made by       | [sainnhe](https://github.com/sainnhe)                                                                             |
+| ------------- | ----------------------------------------------------------------------------------------------------------------- |
+| repository    | [everforest](https://github.com/sainnhe/everforest)                                                               |
+| palette       | ![palette](https://user-images.githubusercontent.com/58662350/214382352-cd7a4f63-e6ef-4575-82c0-a8b72aa37c0c.png) |
+| example image | TODO                                                                                                              |
+
 ## Attributions
 
 ### Example Images
 
 | Original                                                                                      | Made By                                      | Link                          |
 | --------------------------------------------------------------------------------------------- | -------------------------------------------- | ----------------------------- |
 | ![Kaga(Azure Lane) 1920x1080 by voyager](https://w.wallhaven.cc/full/m9/wallhaven-m9e9m1.png) | [voyager](https://wallhaven.cc/user/voyager) | https://wallhaven.cc/w/m9e9m1 |
```

