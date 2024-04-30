# Comparing `tmp/python_coding_playground-1.1.tar.gz` & `tmp/python_coding_playground-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_coding_playground-1.1.tar", last modified: Tue Apr 30 17:03:02 2024, max compression
+gzip compressed data, was "python_coding_playground-1.2.tar", last modified: Tue Apr 30 17:28:50 2024, max compression
```

## Comparing `python_coding_playground-1.1.tar` & `python_coding_playground-1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 17:03:02.477588 python_coding_playground-1.1/
--rw-rw-rw-   0        0        0      247 2024-04-30 17:03:02.475592 python_coding_playground-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-30 17:03:02.431510 python_coding_playground-1.1/python_coding_playground.egg-info/
--rw-rw-rw-   0        0        0      247 2024-04-30 17:03:02.000000 python_coding_playground-1.1/python_coding_playground.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-04-30 17:03:02.000000 python_coding_playground-1.1/python_coding_playground.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 17:03:02.000000 python_coding_playground-1.1/python_coding_playground.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 17:03:02.000000 python_coding_playground-1.1/python_coding_playground.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 17:03:02.478585 python_coding_playground-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1757 2024-04-30 17:02:43.000000 python_coding_playground-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 17:28:50.977092 python_coding_playground-1.2/
+-rw-rw-rw-   0        0        0      247 2024-04-30 17:28:50.976096 python_coding_playground-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 17:28:50.974100 python_coding_playground-1.2/python_coding_playground.egg-info/
+-rw-rw-rw-   0        0        0      247 2024-04-30 17:28:50.000000 python_coding_playground-1.2/python_coding_playground.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2024-04-30 17:28:50.000000 python_coding_playground-1.2/python_coding_playground.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 17:28:50.000000 python_coding_playground-1.2/python_coding_playground.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 17:28:50.000000 python_coding_playground-1.2/python_coding_playground.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 17:28:50.978089 python_coding_playground-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1757 2024-04-30 17:28:37.000000 python_coding_playground-1.2/setup.py
```

### Comparing `python_coding_playground-1.1/setup.py` & `python_coding_playground-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,11 +54,11 @@
 # Merge setup parameters for all packages
 merged_setup_params = {}
 for params in setup_params:
     name = params.pop("name")  # Remove 'name' to avoid conflicts
     merged_setup_params[name] = params
 
 # Call setup() function with combined author name, name, and version
-setup(name="python_coding_playground",version="1.1",author=combined_author, **merged_setup_params)
+setup(name="python_coding_playground",version="1.2",author=combined_author, **merged_setup_params)
```

