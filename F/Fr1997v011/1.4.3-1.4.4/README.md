# Comparing `tmp/Fr1997v011-1.4.3.tar.gz` & `tmp/Fr1997v011-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.4.3.tar", last modified: Mon Apr 29 17:06:07 2024, max compression
+gzip compressed data, was "Fr1997v011-1.4.4.tar", last modified: Mon Apr 29 18:50:03 2024, max compression
```

## Comparing `Fr1997v011-1.4.3.tar` & `Fr1997v011-1.4.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 17:06:07.375366 Fr1997v011-1.4.3/
-drwxrwxrwx   0        0        0        0 2024-04-29 17:06:07.365354 Fr1997v011-1.4.3/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-04-29 17:06:07.000000 Fr1997v011-1.4.3/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-29 17:06:07.000000 Fr1997v011-1.4.3/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 17:06:07.000000 Fr1997v011-1.4.3/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-29 17:06:07.000000 Fr1997v011-1.4.3/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-04-29 17:06:07.000000 Fr1997v011-1.4.3/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.4.3/LICENSE
--rw-rw-rw-   0        0        0      182 2024-04-29 17:06:07.373367 Fr1997v011-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-04-29 09:24:56.000000 Fr1997v011-1.4.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 17:06:07.367360 Fr1997v011-1.4.3/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.4.3/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 17:06:07.370366 Fr1997v011-1.4.3/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.4.3/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   173742 2024-04-29 09:28:37.000000 Fr1997v011-1.4.3/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-04-29 17:06:07.372366 Fr1997v011-1.4.3/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.4.3/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-29 17:06:07.375366 Fr1997v011-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-04-29 09:24:52.000000 Fr1997v011-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:50:03.791046 Fr1997v011-1.4.4/
+drwxrwxrwx   0        0        0        0 2024-04-29 18:50:03.774978 Fr1997v011-1.4.4/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-29 18:50:03.000000 Fr1997v011-1.4.4/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-04-29 18:50:03.000000 Fr1997v011-1.4.4/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 18:50:03.000000 Fr1997v011-1.4.4/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-29 18:50:03.000000 Fr1997v011-1.4.4/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-04-29 18:50:03.000000 Fr1997v011-1.4.4/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.4.4/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-04-29 18:50:03.789042 Fr1997v011-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-04-29 09:24:56.000000 Fr1997v011-1.4.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 18:50:03.777005 Fr1997v011-1.4.4/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.4.4/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:50:03.783010 Fr1997v011-1.4.4/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.4.4/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   173742 2024-04-29 09:28:37.000000 Fr1997v011-1.4.4/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:50:03.786516 Fr1997v011-1.4.4/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.4.4/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-29 18:50:03.791046 Fr1997v011-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-04-29 18:50:00.000000 Fr1997v011-1.4.4/setup.py
```

### Comparing `Fr1997v011-1.4.3/LICENSE` & `Fr1997v011-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.4.3/README.md` & `Fr1997v011-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.4.3/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.4.4/fr1997_mode/mode_func/all_func.py`

 * *Files identical despite different names*

