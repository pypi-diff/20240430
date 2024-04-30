# Comparing `tmp/wallpaper_factory-0.0.2.tar.gz` & `tmp/wallpaper_factory-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wallpaper_factory-0.0.2.tar", last modified: Tue Apr 30 12:30:05 2024, max compression
+gzip compressed data, was "wallpaper_factory-0.0.3.tar", last modified: Tue Apr 30 13:16:14 2024, max compression
```

## Comparing `wallpaper_factory-0.0.2.tar` & `wallpaper_factory-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 12:30:05.789355 wallpaper_factory-0.0.2/
--rw-r--r--   0 marlonkunz   (501) staff       (20)    35149 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.2/LICENSE
--rw-r--r--   0 marlonkunz   (501) staff       (20)     1730 2024-04-30 12:30:05.789172 wallpaper_factory-0.0.2/PKG-INFO
--rw-r--r--   0 marlonkunz   (501) staff       (20)     1555 2024-04-30 12:24:00.000000 wallpaper_factory-0.0.2/README.md
--rw-r--r--   0 marlonkunz   (501) staff       (20)       38 2024-04-30 12:30:05.789397 wallpaper_factory-0.0.2/setup.cfg
--rw-r--r--   0 marlonkunz   (501) staff       (20)      396 2024-04-30 12:30:01.000000 wallpaper_factory-0.0.2/setup.py
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 12:30:05.786624 wallpaper_factory-0.0.2/src/
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 12:30:05.788064 wallpaper_factory-0.0.2/src/wallpaper_factory/
--rw-r--r--   0 marlonkunz   (501) staff       (20)       61 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.2/src/wallpaper_factory/__init__.py
--rw-r--r--   0 marlonkunz   (501) staff       (20)     1564 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.2/src/wallpaper_factory/available_palletes.py
--rw-r--r--   0 marlonkunz   (501) staff       (20)     3719 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.2/src/wallpaper_factory/main.py
-drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 12:30:05.788956 wallpaper_factory-0.0.2/src/wallpaper_factory.egg-info/
--rw-r--r--   0 marlonkunz   (501) staff       (20)     1730 2024-04-30 12:30:05.000000 wallpaper_factory-0.0.2/src/wallpaper_factory.egg-info/PKG-INFO
--rw-r--r--   0 marlonkunz   (501) staff       (20)      406 2024-04-30 12:30:05.000000 wallpaper_factory-0.0.2/src/wallpaper_factory.egg-info/SOURCES.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)        1 2024-04-30 12:30:05.000000 wallpaper_factory-0.0.2/src/wallpaper_factory.egg-info/dependency_links.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       74 2024-04-30 12:30:05.000000 wallpaper_factory-0.0.2/src/wallpaper_factory.egg-info/entry_points.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       21 2024-04-30 12:30:05.000000 wallpaper_factory-0.0.2/src/wallpaper_factory.egg-info/requires.txt
--rw-r--r--   0 marlonkunz   (501) staff       (20)       18 2024-04-30 12:30:05.000000 wallpaper_factory-0.0.2/src/wallpaper_factory.egg-info/top_level.txt
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:16:14.382939 wallpaper_factory-0.0.3/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)    35149 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.3/LICENSE
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     4241 2024-04-30 13:16:14.382740 wallpaper_factory-0.0.3/PKG-INFO
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     4066 2024-04-30 13:14:58.000000 wallpaper_factory-0.0.3/README.md
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       38 2024-04-30 13:16:14.382981 wallpaper_factory-0.0.3/setup.cfg
+-rw-r--r--   0 marlonkunz   (501) staff       (20)      396 2024-04-30 13:16:06.000000 wallpaper_factory-0.0.3/setup.py
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:16:14.379716 wallpaper_factory-0.0.3/src/
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:16:14.381530 wallpaper_factory-0.0.3/src/wallpaper_factory/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       61 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.3/src/wallpaper_factory/__init__.py
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     1564 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.3/src/wallpaper_factory/available_palletes.py
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     3719 2024-04-30 12:02:22.000000 wallpaper_factory-0.0.3/src/wallpaper_factory/main.py
+drwxr-xr-x   0 marlonkunz   (501) staff       (20)        0 2024-04-30 13:16:14.382508 wallpaper_factory-0.0.3/src/wallpaper_factory.egg-info/
+-rw-r--r--   0 marlonkunz   (501) staff       (20)     4241 2024-04-30 13:16:14.000000 wallpaper_factory-0.0.3/src/wallpaper_factory.egg-info/PKG-INFO
+-rw-r--r--   0 marlonkunz   (501) staff       (20)      406 2024-04-30 13:16:14.000000 wallpaper_factory-0.0.3/src/wallpaper_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)        1 2024-04-30 13:16:14.000000 wallpaper_factory-0.0.3/src/wallpaper_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       74 2024-04-30 13:16:14.000000 wallpaper_factory-0.0.3/src/wallpaper_factory.egg-info/entry_points.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       21 2024-04-30 13:16:14.000000 wallpaper_factory-0.0.3/src/wallpaper_factory.egg-info/requires.txt
+-rw-r--r--   0 marlonkunz   (501) staff       (20)       18 2024-04-30 13:16:14.000000 wallpaper_factory-0.0.3/src/wallpaper_factory.egg-info/top_level.txt
```

### Comparing `wallpaper_factory-0.0.2/LICENSE` & `wallpaper_factory-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wallpaper_factory-0.0.2/src/wallpaper_factory/available_palletes.py` & `wallpaper_factory-0.0.3/src/wallpaper_factory/available_palletes.py`

 * *Files identical despite different names*

### Comparing `wallpaper_factory-0.0.2/src/wallpaper_factory/main.py` & `wallpaper_factory-0.0.3/src/wallpaper_factory/main.py`

 * *Files identical despite different names*

