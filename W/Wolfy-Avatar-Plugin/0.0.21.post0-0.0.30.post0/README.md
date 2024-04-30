# Comparing `tmp/Wolfy-Avatar-Plugin-0.0.21.post0.tar.gz` & `tmp/wolfy_avatar_plugin-0.0.30.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Wolfy-Avatar-Plugin-0.0.21.post0.tar", last modified: Fri Mar 29 17:53:22 2024, max compression
+gzip compressed data, was "wolfy_avatar_plugin-0.0.30.post0.tar", last modified: Tue Apr 30 08:54:07 2024, max compression
```

## Comparing `Wolfy-Avatar-Plugin-0.0.21.post0.tar` & `wolfy_avatar_plugin-0.0.30.post0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 sparkypenguin  (1000) sparkypenguin  (1000)        0 2024-03-29 17:53:22.128997 Wolfy-Avatar-Plugin-0.0.21.post0/
--rw-r--r--   0 sparkypenguin  (1000) sparkypenguin  (1000)     1867 2024-03-29 17:53:22.128997 Wolfy-Avatar-Plugin-0.0.21.post0/PKG-INFO
--rw-r--r--   0 sparkypenguin  (1000) sparkypenguin  (1000)     1237 2024-03-29 16:57:53.000000 Wolfy-Avatar-Plugin-0.0.21.post0/README.md
-drwxr-xr-x   0 sparkypenguin  (1000) sparkypenguin  (1000)        0 2024-03-29 17:53:22.128997 Wolfy-Avatar-Plugin-0.0.21.post0/Wolfy_Avatar_Plugin.egg-info/
--rw-r--r--   0 sparkypenguin  (1000) sparkypenguin  (1000)     1867 2024-03-29 17:53:22.000000 Wolfy-Avatar-Plugin-0.0.21.post0/Wolfy_Avatar_Plugin.egg-info/PKG-INFO
--rw-r--r--   0 sparkypenguin  (1000) sparkypenguin  (1000)      196 2024-03-29 17:53:22.000000 Wolfy-Avatar-Plugin-0.0.21.post0/Wolfy_Avatar_Plugin.egg-info/SOURCES.txt
--rw-r--r--   0 sparkypenguin  (1000) sparkypenguin  (1000)        1 2024-03-29 17:53:22.000000 Wolfy-Avatar-Plugin-0.0.21.post0/Wolfy_Avatar_Plugin.egg-info/dependency_links.txt
--rw-r--r--   0 sparkypenguin  (1000) sparkypenguin  (1000)        1 2024-03-29 17:53:22.000000 Wolfy-Avatar-Plugin-0.0.21.post0/Wolfy_Avatar_Plugin.egg-info/top_level.txt
--rw-r--r--   0 sparkypenguin  (1000) sparkypenguin  (1000)     1203 2024-03-29 17:39:37.000000 Wolfy-Avatar-Plugin-0.0.21.post0/pyproject.toml
--rw-r--r--   0 sparkypenguin  (1000) sparkypenguin  (1000)       38 2024-03-29 17:53:22.128997 Wolfy-Avatar-Plugin-0.0.21.post0/setup.cfg
+drwxr-xr-x   0 sparkypenguin  (1000) sparkypenguin  (1000)        0 2024-04-30 08:54:07.165573 wolfy_avatar_plugin-0.0.30.post0/
+-rw-r--r--   0 sparkypenguin  (1000) sparkypenguin  (1000)     1867 2024-04-30 08:54:07.165573 wolfy_avatar_plugin-0.0.30.post0/PKG-INFO
+-rw-r--r--   0 sparkypenguin  (1000) sparkypenguin  (1000)     1237 2024-03-29 16:57:53.000000 wolfy_avatar_plugin-0.0.30.post0/README.md
+drwxr-xr-x   0 sparkypenguin  (1000) sparkypenguin  (1000)        0 2024-04-30 08:54:07.165573 wolfy_avatar_plugin-0.0.30.post0/Wolfy_Avatar_Plugin.egg-info/
+-rw-r--r--   0 sparkypenguin  (1000) sparkypenguin  (1000)     1867 2024-04-30 08:54:07.000000 wolfy_avatar_plugin-0.0.30.post0/Wolfy_Avatar_Plugin.egg-info/PKG-INFO
+-rw-r--r--   0 sparkypenguin  (1000) sparkypenguin  (1000)      196 2024-04-30 08:54:07.000000 wolfy_avatar_plugin-0.0.30.post0/Wolfy_Avatar_Plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 sparkypenguin  (1000) sparkypenguin  (1000)        1 2024-04-30 08:54:07.000000 wolfy_avatar_plugin-0.0.30.post0/Wolfy_Avatar_Plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 sparkypenguin  (1000) sparkypenguin  (1000)        1 2024-04-30 08:54:07.000000 wolfy_avatar_plugin-0.0.30.post0/Wolfy_Avatar_Plugin.egg-info/top_level.txt
+-rw-r--r--   0 sparkypenguin  (1000) sparkypenguin  (1000)     1203 2024-03-29 17:39:37.000000 wolfy_avatar_plugin-0.0.30.post0/pyproject.toml
+-rw-r--r--   0 sparkypenguin  (1000) sparkypenguin  (1000)       38 2024-04-30 08:54:07.165573 wolfy_avatar_plugin-0.0.30.post0/setup.cfg
```

### Comparing `Wolfy-Avatar-Plugin-0.0.21.post0/PKG-INFO` & `wolfy_avatar_plugin-0.0.30.post0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Wolfy-Avatar-Plugin
-Version: 0.0.21.post0
+Version: 0.0.30.post0
 Summary: Small virtual character plugin to track mouse and keyboard inputs.
 Author-email: Sparky <sparks29032@gmail.com>
 Maintainer-email: Sparky <sparks29032@gmail.com>
 Project-URL: Homepage, https://github.com/Sparks29032/Character_Plugin
 Project-URL: Issues, https://github.com/Sparks29032/Character_Plugin/issues
 Keywords: obs-compatible
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `Wolfy-Avatar-Plugin-0.0.21.post0/README.md` & `wolfy_avatar_plugin-0.0.30.post0/README.md`

 * *Files identical despite different names*

### Comparing `Wolfy-Avatar-Plugin-0.0.21.post0/Wolfy_Avatar_Plugin.egg-info/PKG-INFO` & `wolfy_avatar_plugin-0.0.30.post0/Wolfy_Avatar_Plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Wolfy-Avatar-Plugin
-Version: 0.0.21.post0
+Version: 0.0.30.post0
 Summary: Small virtual character plugin to track mouse and keyboard inputs.
 Author-email: Sparky <sparks29032@gmail.com>
 Maintainer-email: Sparky <sparks29032@gmail.com>
 Project-URL: Homepage, https://github.com/Sparks29032/Character_Plugin
 Project-URL: Issues, https://github.com/Sparks29032/Character_Plugin/issues
 Keywords: obs-compatible
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `Wolfy-Avatar-Plugin-0.0.21.post0/pyproject.toml` & `wolfy_avatar_plugin-0.0.30.post0/pyproject.toml`

 * *Files identical despite different names*

