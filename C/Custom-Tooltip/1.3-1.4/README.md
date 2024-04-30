# Comparing `tmp/Custom-Tooltip-1.3.tar.gz` & `tmp/Custom-Tooltip-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Custom-Tooltip-1.3.tar", last modified: Tue Jul 19 15:24:40 2022, max compression
+gzip compressed data, was "Custom-Tooltip-1.4.tar", last modified: Tue Apr 30 20:26:25 2024, max compression
```

## Comparing `Custom-Tooltip-1.3.tar` & `Custom-Tooltip-1.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-07-19 15:24:40.030134 Custom-Tooltip-1.3/
-drwxrwxrwx   0        0        0        0 2022-07-19 15:24:40.028133 Custom-Tooltip-1.3/Custom_Tooltip.egg-info/
--rw-rw-rw-   0        0        0      830 2022-07-19 15:24:39.000000 Custom-Tooltip-1.3/Custom_Tooltip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2022-07-19 15:24:39.000000 Custom-Tooltip-1.3/Custom_Tooltip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-19 15:24:39.000000 Custom-Tooltip-1.3/Custom_Tooltip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2022-07-19 15:24:39.000000 Custom-Tooltip-1.3/Custom_Tooltip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      830 2022-07-19 15:24:40.030134 Custom-Tooltip-1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-07-19 15:24:40.029133 Custom-Tooltip-1.3/custom_hovertip/
--rw-rw-rw-   0        0        0       49 2022-07-19 15:24:12.000000 Custom-Tooltip-1.3/custom_hovertip/__init__.py
--rw-rw-rw-   0        0        0     6993 2022-07-19 15:09:07.000000 Custom-Tooltip-1.3/custom_hovertip/tkinter_tooltip.py
--rw-rw-rw-   0        0        0       42 2022-07-19 15:24:40.030134 Custom-Tooltip-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1156 2022-07-19 15:24:31.000000 Custom-Tooltip-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 20:26:25.370355 Custom-Tooltip-1.4/
+drwxrwxrwx   0        0        0        0 2024-04-30 20:26:25.368353 Custom-Tooltip-1.4/Custom_Tooltip.egg-info/
+-rw-rw-rw-   0        0        0      830 2024-04-30 20:26:25.000000 Custom-Tooltip-1.4/Custom_Tooltip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2024-04-30 20:26:25.000000 Custom-Tooltip-1.4/Custom_Tooltip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 20:26:25.000000 Custom-Tooltip-1.4/Custom_Tooltip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-30 20:26:25.000000 Custom-Tooltip-1.4/Custom_Tooltip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      830 2024-04-30 20:26:25.370355 Custom-Tooltip-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1841 2022-07-19 16:00:48.000000 Custom-Tooltip-1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 20:26:25.369355 Custom-Tooltip-1.4/custom_hovertip/
+-rw-rw-rw-   0        0        0       49 2022-07-19 15:24:12.000000 Custom-Tooltip-1.4/custom_hovertip/__init__.py
+-rw-rw-rw-   0        0        0     3275 2024-04-30 20:22:39.000000 Custom-Tooltip-1.4/custom_hovertip/tkinter_tooltip.py
+-rw-rw-rw-   0        0        0       42 2024-04-30 20:26:25.371354 Custom-Tooltip-1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1156 2024-04-30 20:23:28.000000 Custom-Tooltip-1.4/setup.py
```

### Comparing `Custom-Tooltip-1.3/Custom_Tooltip.egg-info/PKG-INFO` & `Custom-Tooltip-1.4/Custom_Tooltip.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: Custom-Tooltip
-Version: 1.3
+Version: 1.4
 Summary: Basic Hover Tooltip for Tkinter based off of Tkinter's built in tooltip
 Home-page: https://github.com/jlw4049/Custom-Tkinter-Tooltip
 Author: jlw4049 (Jessie Wilson)
 Author-email: <jessielw4049@gmail.com>
 License: UNKNOWN
 Description: This package enables a customizable tooltip when you hover the mouse over a defined widget. It's built off of the Tkinter's built in Hovertip class. However it has most of the functionality of the label widget. You can set font, colors, relief, border, wrap length, anchor, border, textvariable, and width.
 Keywords: python,tkinter,hovertip,tooltip,infotip,bubble
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Development Status :: 6 - Mature
 Description-Content-Type: text/markdown
```

### Comparing `Custom-Tooltip-1.3/PKG-INFO` & `Custom-Tooltip-1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: Custom-Tooltip
-Version: 1.3
+Version: 1.4
 Summary: Basic Hover Tooltip for Tkinter based off of Tkinter's built in tooltip
 Home-page: https://github.com/jlw4049/Custom-Tkinter-Tooltip
 Author: jlw4049 (Jessie Wilson)
 Author-email: <jessielw4049@gmail.com>
 License: UNKNOWN
 Description: This package enables a customizable tooltip when you hover the mouse over a defined widget. It's built off of the Tkinter's built in Hovertip class. However it has most of the functionality of the label widget. You can set font, colors, relief, border, wrap length, anchor, border, textvariable, and width.
 Keywords: python,tkinter,hovertip,tooltip,infotip,bubble
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Development Status :: 6 - Mature
 Description-Content-Type: text/markdown
```

### Comparing `Custom-Tooltip-1.3/setup.py` & `Custom-Tooltip-1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-tool_version = '1.3'
+tool_version = '1.4'
 short_description = "Basic Hover Tooltip for Tkinter based off of Tkinter's built in tooltip"
 long_description = "This package enables a customizable tooltip when you hover the mouse over a defined widget. " \
                    "It's built off of the Tkinter's built in Hovertip class. However it has most of the " \
                    "functionality of the label widget. You can set font, colors, relief, border, wrap length, " \
                    "anchor, border, textvariable, and width."
 
 # Setting up
@@ -16,8 +16,8 @@
     description=short_description,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/jlw4049/Custom-Tkinter-Tooltip',
     keywords=['python', 'tkinter', 'hovertip', 'tooltip', 'infotip', 'bubble'],
-    classifiers=["Programming Language :: Python :: 3.8", 'Development Status :: 6 - Mature'])
+    classifiers=["Programming Language :: Python :: 3.6", 'Development Status :: 6 - Mature'])
```

