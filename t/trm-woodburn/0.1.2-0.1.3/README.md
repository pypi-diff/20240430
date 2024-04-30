# Comparing `tmp/trm_woodburn-0.1.2.tar.gz` & `tmp/trm_woodburn-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trm_woodburn-0.1.2.tar", last modified: Wed Apr 24 12:26:34 2024, max compression
+gzip compressed data, was "trm_woodburn-0.1.3.tar", last modified: Tue Apr 30 21:53:56 2024, max compression
```

## Comparing `trm_woodburn-0.1.2.tar` & `trm_woodburn-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 12:26:34.661321 trm_woodburn-0.1.2/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.1.2/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     6871 2024-04-24 12:26:34.661267 trm_woodburn-0.1.2/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     6392 2024-04-24 12:26:17.000000 trm_woodburn-0.1.2/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.1.2/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-24 12:26:34.661546 trm_woodburn-0.1.2/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 12:26:34.659348 trm_woodburn-0.1.2/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 12:26:34.660255 trm_woodburn-0.1.2/src/trm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.1.2/src/trm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    25274 2024-04-24 12:24:26.000000 trm_woodburn-0.1.2/src/trm/trm.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-24 12:26:34.661085 trm_woodburn-0.1.2/src/trm_woodburn.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     6871 2024-04-24 12:26:34.000000 trm_woodburn-0.1.2/src/trm_woodburn.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-24 12:26:34.000000 trm_woodburn-0.1.2/src/trm_woodburn.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-24 12:26:34.000000 trm_woodburn-0.1.2/src/trm_woodburn.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-24 12:26:34.000000 trm_woodburn-0.1.2/src/trm_woodburn.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-24 12:26:34.000000 trm_woodburn-0.1.2/src/trm_woodburn.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-30 21:53:56.404857 trm_woodburn-0.1.3/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.1.3/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     7637 2024-04-30 21:53:56.404799 trm_woodburn-0.1.3/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     7158 2024-04-30 21:53:11.000000 trm_woodburn-0.1.3/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.1.3/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-30 21:53:56.405081 trm_woodburn-0.1.3/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-30 21:53:56.402725 trm_woodburn-0.1.3/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-30 21:53:56.403582 trm_woodburn-0.1.3/src/trm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.1.3/src/trm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    25274 2024-04-24 12:24:26.000000 trm_woodburn-0.1.3/src/trm/trm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-30 21:53:56.404614 trm_woodburn-0.1.3/src/trm_woodburn.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     7637 2024-04-30 21:53:56.000000 trm_woodburn-0.1.3/src/trm_woodburn.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-30 21:53:56.000000 trm_woodburn-0.1.3/src/trm_woodburn.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-30 21:53:56.000000 trm_woodburn-0.1.3/src/trm_woodburn.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-30 21:53:56.000000 trm_woodburn-0.1.3/src/trm_woodburn.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-30 21:53:56.000000 trm_woodburn-0.1.3/src/trm_woodburn.egg-info/top_level.txt
```

### Comparing `trm_woodburn-0.1.2/LICENSE.txt` & `trm_woodburn-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `trm_woodburn-0.1.2/PKG-INFO` & `trm_woodburn-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -85,14 +85,18 @@
 magenta. If you have more than 5 curves (This is just a terminal-based plot; why
 would you do that?), then the colors will recycle.
 
 If you want equal axis scaling, set `equal` to `1`. However, since terminal
 fonts are not always the same aspect ratio and because the line spacing in your
 terminal might be adjustable, you can adjust this value to tune.
 
+| Single curve    | Multiple curves |
+| --------------- | --------------- |
+| ![](https://gitlab.com/davidwoodburn/trm/-/raw/main/figures/fig_plot_1.png) | ![]()https://gitlab.com/davidwoodburn/trm/-/raw/main/figures/fig_plot_5.png) |
+
 ## Bars
 
 ```python
 trm.bars(x, labels=None, cols=1, fat=False)
 ```
 
 It can be convenient to plot a simple bar graph. The `x` input is the vector of
@@ -118,14 +122,18 @@
 
 The `heat` function will generate a heat map of the `matrix` input using 24
 shades of gray. Black is used for the lowest value and white for the highest
 value. If `trm.config.uni` is `True`, half-block characters from the Unicode
 table will be used. If it is `False`, two spaces per element of the matrix will
 be used.
 
+| With Unicode      | Without Unicode     |
+| ----------------- | ------------------- |
+| ![](https://gitlab.com/davidwoodburn/trm/-/raw/main/figures/fig_heat_uni.png) | ![](https://gitlab.com/davidwoodburn/trm/-/raw/main/figures/fig_heat_ascii.png) |
+
 ## Tables
 
 ```python
 trm.table(matrix, head=None, left=None, width=10, sep='  ')
 ```
 
 You can print a nicely spaced table of the `matrix` data. The `head` and `left`
@@ -147,14 +155,18 @@
 ```python
 trm.sparsity(matrix, label='')
 ```
 
 If all you want to see is the sparsity of a matrix, use this function. The
 `label` input will be placed in the bottom-right corner of the render.
 
+| With Unicode          | Without Unicode         |
+| --------------------- | ----------------------- |
+| ![](https://gitlab.com/davidwoodburn/trm/-/raw/main/figures/fig_sparsity_uni.png) | ![](https://gitlab.com/davidwoodburn/trm/-/raw/main/figures/fig_sparsity_ascii.png) |
+
 ## Progress bars
 
 ```python
 trm.progress(k, K, t_init=None, cols=1, fat=False)
 ```
 
 There are many progress bar libraries available for Python. But, many of them
```

### Comparing `trm_woodburn-0.1.2/README.md` & `trm_woodburn-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -70,14 +70,18 @@
 magenta. If you have more than 5 curves (This is just a terminal-based plot; why
 would you do that?), then the colors will recycle.
 
 If you want equal axis scaling, set `equal` to `1`. However, since terminal
 fonts are not always the same aspect ratio and because the line spacing in your
 terminal might be adjustable, you can adjust this value to tune.
 
+| Single curve    | Multiple curves |
+| --------------- | --------------- |
+| ![](https://gitlab.com/davidwoodburn/trm/-/raw/main/figures/fig_plot_1.png) | ![]()https://gitlab.com/davidwoodburn/trm/-/raw/main/figures/fig_plot_5.png) |
+
 ## Bars
 
 ```python
 trm.bars(x, labels=None, cols=1, fat=False)
 ```
 
 It can be convenient to plot a simple bar graph. The `x` input is the vector of
@@ -103,14 +107,18 @@
 
 The `heat` function will generate a heat map of the `matrix` input using 24
 shades of gray. Black is used for the lowest value and white for the highest
 value. If `trm.config.uni` is `True`, half-block characters from the Unicode
 table will be used. If it is `False`, two spaces per element of the matrix will
 be used.
 
+| With Unicode      | Without Unicode     |
+| ----------------- | ------------------- |
+| ![](https://gitlab.com/davidwoodburn/trm/-/raw/main/figures/fig_heat_uni.png) | ![](https://gitlab.com/davidwoodburn/trm/-/raw/main/figures/fig_heat_ascii.png) |
+
 ## Tables
 
 ```python
 trm.table(matrix, head=None, left=None, width=10, sep='  ')
 ```
 
 You can print a nicely spaced table of the `matrix` data. The `head` and `left`
@@ -132,14 +140,18 @@
 ```python
 trm.sparsity(matrix, label='')
 ```
 
 If all you want to see is the sparsity of a matrix, use this function. The
 `label` input will be placed in the bottom-right corner of the render.
 
+| With Unicode          | Without Unicode         |
+| --------------------- | ----------------------- |
+| ![](https://gitlab.com/davidwoodburn/trm/-/raw/main/figures/fig_sparsity_uni.png) | ![](https://gitlab.com/davidwoodburn/trm/-/raw/main/figures/fig_sparsity_ascii.png) |
+
 ## Progress bars
 
 ```python
 trm.progress(k, K, t_init=None, cols=1, fat=False)
 ```
 
 There are many progress bar libraries available for Python. But, many of them
```

### Comparing `trm_woodburn-0.1.2/setup.cfg` & `trm_woodburn-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trm-woodburn
-version = 0.1.2
+version = 0.1.3
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = A library for pretty printing to the terminal
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/trm
 classifiers =
```

### Comparing `trm_woodburn-0.1.2/src/trm/trm.py` & `trm_woodburn-0.1.3/src/trm/trm.py`

 * *Files identical despite different names*

### Comparing `trm_woodburn-0.1.2/src/trm_woodburn.egg-info/PKG-INFO` & `trm_woodburn-0.1.3/src/trm_woodburn.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -85,14 +85,18 @@
 magenta. If you have more than 5 curves (This is just a terminal-based plot; why
 would you do that?), then the colors will recycle.
 
 If you want equal axis scaling, set `equal` to `1`. However, since terminal
 fonts are not always the same aspect ratio and because the line spacing in your
 terminal might be adjustable, you can adjust this value to tune.
 
+| Single curve    | Multiple curves |
+| --------------- | --------------- |
+| ![](https://gitlab.com/davidwoodburn/trm/-/raw/main/figures/fig_plot_1.png) | ![]()https://gitlab.com/davidwoodburn/trm/-/raw/main/figures/fig_plot_5.png) |
+
 ## Bars
 
 ```python
 trm.bars(x, labels=None, cols=1, fat=False)
 ```
 
 It can be convenient to plot a simple bar graph. The `x` input is the vector of
@@ -118,14 +122,18 @@
 
 The `heat` function will generate a heat map of the `matrix` input using 24
 shades of gray. Black is used for the lowest value and white for the highest
 value. If `trm.config.uni` is `True`, half-block characters from the Unicode
 table will be used. If it is `False`, two spaces per element of the matrix will
 be used.
 
+| With Unicode      | Without Unicode     |
+| ----------------- | ------------------- |
+| ![](https://gitlab.com/davidwoodburn/trm/-/raw/main/figures/fig_heat_uni.png) | ![](https://gitlab.com/davidwoodburn/trm/-/raw/main/figures/fig_heat_ascii.png) |
+
 ## Tables
 
 ```python
 trm.table(matrix, head=None, left=None, width=10, sep='  ')
 ```
 
 You can print a nicely spaced table of the `matrix` data. The `head` and `left`
@@ -147,14 +155,18 @@
 ```python
 trm.sparsity(matrix, label='')
 ```
 
 If all you want to see is the sparsity of a matrix, use this function. The
 `label` input will be placed in the bottom-right corner of the render.
 
+| With Unicode          | Without Unicode         |
+| --------------------- | ----------------------- |
+| ![](https://gitlab.com/davidwoodburn/trm/-/raw/main/figures/fig_sparsity_uni.png) | ![](https://gitlab.com/davidwoodburn/trm/-/raw/main/figures/fig_sparsity_ascii.png) |
+
 ## Progress bars
 
 ```python
 trm.progress(k, K, t_init=None, cols=1, fat=False)
 ```
 
 There are many progress bar libraries available for Python. But, many of them
```

