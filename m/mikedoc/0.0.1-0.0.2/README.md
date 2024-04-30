# Comparing `tmp/mikedoc-0.0.1.tar.gz` & `tmp/mikedoc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mikedoc-0.0.1.tar", last modified: Thu Apr 18 18:24:47 2024, max compression
+gzip compressed data, was "dist/mikedoc-0.0.2.tar", last modified: Tue Apr 30 20:01:49 2024, max compression
```

## Comparing `mikedoc-0.0.1.tar` & `mikedoc-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-18 18:24:47.259318 mikedoc-0.0.1/
--rw-rw-r--   0 alex      (1002) alex      (1003)     1076 2024-03-16 21:20:24.000000 mikedoc-0.0.1/LICENSE
--rw-rw-r--   0 alex      (1002) alex      (1003)       69 2024-03-16 21:20:36.000000 mikedoc-0.0.1/MANIFEST.in
--rw-rw-r--   0 alex      (1002) alex      (1003)      573 2024-04-18 18:24:47.259318 mikedoc-0.0.1/PKG-INFO
--rw-rw-r--   0 alex      (1002) alex      (1003)       14 2024-04-18 18:22:33.000000 mikedoc-0.0.1/README.md
--rw-rw-r--   0 alex      (1002) alex      (1003)        5 2024-03-16 21:20:36.000000 mikedoc-0.0.1/VERSION
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-18 18:24:47.211318 mikedoc-0.0.1/mikedoc/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2024-04-18 18:23:47.000000 mikedoc-0.0.1/mikedoc/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2024-04-18 18:23:47.000000 mikedoc-0.0.1/mikedoc/__main__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-18 18:24:47.239318 mikedoc-0.0.1/mikedoc.egg-info/
--rw-r--r--   0 alex      (1002) alex      (1003)      573 2024-04-18 18:24:47.000000 mikedoc-0.0.1/mikedoc.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1002) alex      (1003)      537 2024-04-18 18:24:47.000000 mikedoc-0.0.1/mikedoc.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2024-04-18 18:24:47.000000 mikedoc-0.0.1/mikedoc.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)       51 2024-04-18 18:24:47.000000 mikedoc-0.0.1/mikedoc.egg-info/entry_points.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2024-03-16 21:21:59.000000 mikedoc-0.0.1/mikedoc.egg-info/not-zip-safe
--rw-rw-r--   0 alex      (1002) alex      (1003)        5 2024-04-18 18:24:47.000000 mikedoc-0.0.1/mikedoc.egg-info/requires.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)       14 2024-04-18 18:24:47.000000 mikedoc-0.0.1/mikedoc.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)      100 2024-03-16 21:20:36.000000 mikedoc-0.0.1/pyproject.toml
--rw-rw-r--   0 alex      (1002) alex      (1003)      764 2024-04-18 18:24:47.259318 mikedoc-0.0.1/setup.cfg
--rw-rw-r--   0 alex      (1002) alex      (1003)      100 2024-03-16 21:20:36.000000 mikedoc-0.0.1/setup.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-18 18:24:47.239318 mikedoc-0.0.1/tests/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2024-03-16 21:20:36.000000 mikedoc-0.0.1/tests/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-18 18:24:47.239318 mikedoc-0.0.1/tests/project/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2024-04-04 10:29:33.000000 mikedoc-0.0.1/tests/project/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2024-04-04 10:29:47.000000 mikedoc-0.0.1/tests/project/__main__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-18 18:24:47.243318 mikedoc-0.0.1/tests/project/package1/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2024-04-04 10:30:04.000000 mikedoc-0.0.1/tests/project/package1/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      129 2024-04-04 10:36:24.000000 mikedoc-0.0.1/tests/project/package1/module1.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-18 18:24:47.255318 mikedoc-0.0.1/tests/project/package2/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2024-04-04 10:30:55.000000 mikedoc-0.0.1/tests/project/package2/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2024-04-04 10:31:14.000000 mikedoc-0.0.1/tests/project/package2/module2.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:01:49.858580 mikedoc-0.0.2/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1076 2024-03-16 21:20:24.000000 mikedoc-0.0.2/LICENSE
+-rw-rw-r--   0 alex      (1002) alex      (1003)       69 2024-03-16 21:20:36.000000 mikedoc-0.0.2/MANIFEST.in
+-rw-rw-r--   0 alex      (1002) alex      (1003)    12947 2024-04-30 20:01:49.858580 mikedoc-0.0.2/PKG-INFO
+-rw-rw-r--   0 alex      (1002) alex      (1003)    12343 2024-04-30 19:17:30.000000 mikedoc-0.0.2/README.md
+-rw-rw-r--   0 alex      (1002) alex      (1003)        5 2024-04-18 18:24:47.000000 mikedoc-0.0.2/VERSION
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:01:49.806578 mikedoc-0.0.2/mikedoc/
+-rw-rw-r--   0 alex      (1002) alex      (1003)      373 2024-04-30 20:00:04.000000 mikedoc-0.0.2/mikedoc/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)      172 2024-04-30 10:04:19.000000 mikedoc-0.0.2/mikedoc/__main__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:01:49.858580 mikedoc-0.0.2/mikedoc/browser/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     9079 2024-04-30 20:00:04.000000 mikedoc-0.0.2/mikedoc/browser/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:01:49.858580 mikedoc-0.0.2/mikedoc/builder/
+-rw-rw-r--   0 alex      (1002) alex      (1003)    33338 2024-04-30 20:00:04.000000 mikedoc-0.0.2/mikedoc/builder/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:01:49.858580 mikedoc-0.0.2/mikedoc/cli/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     3885 2024-04-30 20:00:04.000000 mikedoc-0.0.2/mikedoc/cli/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:01:49.858580 mikedoc-0.0.2/mikedoc/errors/
+-rw-rw-r--   0 alex      (1002) alex      (1003)       34 2024-03-30 14:51:17.000000 mikedoc-0.0.2/mikedoc/errors/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:01:49.858580 mikedoc-0.0.2/mikedoc/misc/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     7417 2024-04-30 20:00:04.000000 mikedoc-0.0.2/mikedoc/misc/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:01:49.858580 mikedoc-0.0.2/mikedoc/templates/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     3238 2024-04-30 10:04:19.000000 mikedoc-0.0.2/mikedoc/templates/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:01:49.858580 mikedoc-0.0.2/mikedoc.egg-info/
+-rw-r--r--   0 alex      (1002) alex      (1003)    12947 2024-04-30 20:01:49.000000 mikedoc-0.0.2/mikedoc.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1002) alex      (1003)      509 2024-04-30 20:01:49.000000 mikedoc-0.0.2/mikedoc.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2024-04-30 20:01:49.000000 mikedoc-0.0.2/mikedoc.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)       51 2024-04-30 20:01:49.000000 mikedoc-0.0.2/mikedoc.egg-info/entry_points.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2024-03-16 21:21:59.000000 mikedoc-0.0.2/mikedoc.egg-info/not-zip-safe
+-rw-rw-r--   0 alex      (1002) alex      (1003)       14 2024-04-30 20:01:49.000000 mikedoc-0.0.2/mikedoc.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)       14 2024-04-30 20:01:49.000000 mikedoc-0.0.2/mikedoc.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)      100 2024-03-16 21:20:36.000000 mikedoc-0.0.2/pyproject.toml
+-rw-rw-r--   0 alex      (1002) alex      (1003)      819 2024-04-30 20:01:49.858580 mikedoc-0.0.2/setup.cfg
+-rw-rw-r--   0 alex      (1002) alex      (1003)      100 2024-03-16 21:20:36.000000 mikedoc-0.0.2/setup.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:01:49.858580 mikedoc-0.0.2/tests/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2024-03-16 21:20:36.000000 mikedoc-0.0.2/tests/__init__.py
```

### Comparing `mikedoc-0.0.1/LICENSE` & `mikedoc-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mikedoc-0.0.1/setup.cfg` & `mikedoc-0.0.2/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = mikedoc
 version = file: VERSION
 url = https://pyrustic.github.com
 author = Pyrustic Evangelist
 author_email = rusticalex@yahoo.com
 maintainer = Pyrustic Evangelist
 maintainer_email = rusticalex@yahoo.com
-description = Secret
+description = Neat docstring format for generating API references
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 keywords = 
 	docs
 	docstring
 	documentation
@@ -23,14 +23,15 @@
 [options]
 python_requires = >=3.5
 packages = find:
 include_package_data = true
 zip_safe = false
 install_requires = 
 	braq
+	paradict
 
 [options.entry_points]
 console_scripts = 
 	mikedoc = mikedoc.__main__:main
 
 [egg_info]
 tag_build =
```

