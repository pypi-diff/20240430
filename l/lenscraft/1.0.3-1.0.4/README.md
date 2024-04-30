# Comparing `tmp/lenscraft-1.0.3.tar.gz` & `tmp/lenscraft-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lenscraft-1.0.3.tar", last modified: Fri Apr 26 14:09:31 2024, max compression
+gzip compressed data, was "lenscraft-1.0.4.tar", last modified: Tue Apr 30 14:42:07 2024, max compression
```

## Comparing `lenscraft-1.0.3.tar` & `lenscraft-1.0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:09:31.311537 lenscraft-1.0.3/
--rw-rw-rw-   0 root         (0) root         (0)     3947 2024-04-23 18:41:25.000000 lenscraft-1.0.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      503 2024-04-23 19:08:22.000000 lenscraft-1.0.3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1672 2024-04-23 18:41:25.000000 lenscraft-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1300 2024-04-26 14:09:31.311537 lenscraft-1.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      584 2024-04-23 19:24:28.000000 lenscraft-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:09:31.299537 lenscraft-1.0.3/images/
--rw-rw-rw-   0 root         (0) root         (0)   776666 2024-04-23 18:41:25.000000 lenscraft-1.0.3/images/0.9858_1.1766.png
--rw-rw-rw-   0 root         (0) root         (0)   192094 2024-04-23 18:41:25.000000 lenscraft-1.0.3/images/334.png
--rw-rw-rw-   0 root         (0) root         (0)  4916278 2024-04-23 18:41:25.000000 lenscraft-1.0.3/images/Ring_9_9.png
--rw-rw-rw-   0 root         (0) root         (0)    15666 2024-04-23 18:41:25.000000 lenscraft-1.0.3/images/mask.png
--rw-rw-rw-   0 root         (0) root         (0)   755205 2024-04-23 18:41:25.000000 lenscraft-1.0.3/images/spacer_top__13.png
--rw-rw-rw-   0 root         (0) root         (0)   609893 2024-04-23 18:41:25.000000 lenscraft-1.0.3/images/spacer_top__14.png
--rw-rw-rw-   0 root         (0) root         (0)   750759 2024-04-23 18:41:25.000000 lenscraft-1.0.3/images/spacer_top__3.png
--rw-rw-rw-   0 root         (0) root         (0)   916168 2024-04-23 18:41:25.000000 lenscraft-1.0.3/images/spacer_top__9.png
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-04-23 19:08:22.000000 lenscraft-1.0.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-23 18:41:25.000000 lenscraft-1.0.3/requirments.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 14:09:31.311537 lenscraft-1.0.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:09:31.263534 lenscraft-1.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:09:31.307537 lenscraft-1.0.3/src/lenscraft/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-24 19:00:28.000000 lenscraft-1.0.3/src/lenscraft/__main__.py
--rw-r--r--   0 root         (0) root         (0)      411 2024-04-26 14:09:31.000000 lenscraft-1.0.3/src/lenscraft/_version.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:09:31.311537 lenscraft-1.0.3/src/lenscraft/assets/
--rw-rw-rw-   0 root         (0) root         (0)      923 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/assets/CornerTemplate.png
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:09:31.311537 lenscraft-1.0.3/src/lenscraft/editor/
--rw-rw-rw-   0 root         (0) root         (0)     5370 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/editor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7721 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/gabor.py
--rw-rw-rw-   0 root         (0) root         (0)     5774 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/image.py
--rw-rw-rw-   0 root         (0) root         (0)    17849 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/nodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:09:31.311537 lenscraft-1.0.3/src/lenscraft/texture/
--rw-rw-rw-   0 root         (0) root         (0)      637 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/texture/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2682 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/texture/classify.py
--rw-rw-rw-   0 root         (0) root         (0)    14340 2024-04-26 14:03:03.000000 lenscraft-1.0.3/src/lenscraft/texture/tool.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-23 18:41:25.000000 lenscraft-1.0.3/src/lenscraft/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:09:31.311537 lenscraft-1.0.3/src/lenscraft.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1300 2024-04-26 14:09:31.000000 lenscraft-1.0.3/src/lenscraft.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      877 2024-04-26 14:09:31.000000 lenscraft-1.0.3/src/lenscraft.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 14:09:31.000000 lenscraft-1.0.3/src/lenscraft.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-04-26 14:09:31.000000 lenscraft-1.0.3/src/lenscraft.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      126 2024-04-26 14:09:31.000000 lenscraft-1.0.3/src/lenscraft.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-26 14:09:31.000000 lenscraft-1.0.3/src/lenscraft.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 14:09:31.311537 lenscraft-1.0.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:41:25.000000 lenscraft-1.0.3/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:42:07.294971 lenscraft-1.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)     3947 2024-04-23 18:41:25.000000 lenscraft-1.0.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      503 2024-04-23 19:08:22.000000 lenscraft-1.0.4/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2024-04-23 18:41:25.000000 lenscraft-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1300 2024-04-30 14:42:07.294971 lenscraft-1.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      584 2024-04-23 19:24:28.000000 lenscraft-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:42:07.290971 lenscraft-1.0.4/images/
+-rw-rw-rw-   0 root         (0) root         (0)   776666 2024-04-23 18:41:25.000000 lenscraft-1.0.4/images/0.9858_1.1766.png
+-rw-rw-rw-   0 root         (0) root         (0)   192094 2024-04-23 18:41:25.000000 lenscraft-1.0.4/images/334.png
+-rw-rw-rw-   0 root         (0) root         (0)  4916278 2024-04-23 18:41:25.000000 lenscraft-1.0.4/images/Ring_9_9.png
+-rw-rw-rw-   0 root         (0) root         (0)    15666 2024-04-23 18:41:25.000000 lenscraft-1.0.4/images/mask.png
+-rw-rw-rw-   0 root         (0) root         (0)   755205 2024-04-23 18:41:25.000000 lenscraft-1.0.4/images/spacer_top__13.png
+-rw-rw-rw-   0 root         (0) root         (0)   609893 2024-04-23 18:41:25.000000 lenscraft-1.0.4/images/spacer_top__14.png
+-rw-rw-rw-   0 root         (0) root         (0)   750759 2024-04-23 18:41:25.000000 lenscraft-1.0.4/images/spacer_top__3.png
+-rw-rw-rw-   0 root         (0) root         (0)   916168 2024-04-23 18:41:25.000000 lenscraft-1.0.4/images/spacer_top__9.png
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-04-23 19:08:22.000000 lenscraft-1.0.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-23 18:41:25.000000 lenscraft-1.0.4/requirments.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 14:42:07.294971 lenscraft-1.0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:42:07.286971 lenscraft-1.0.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:42:07.294971 lenscraft-1.0.4/src/lenscraft/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-24 19:00:28.000000 lenscraft-1.0.4/src/lenscraft/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-04-30 14:42:07.000000 lenscraft-1.0.4/src/lenscraft/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:42:07.294971 lenscraft-1.0.4/src/lenscraft/assets/
+-rw-rw-rw-   0 root         (0) root         (0)      923 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/assets/CornerTemplate.png
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:42:07.294971 lenscraft-1.0.4/src/lenscraft/editor/
+-rw-rw-rw-   0 root         (0) root         (0)     5370 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/editor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7721 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/gabor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5774 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/image.py
+-rw-rw-rw-   0 root         (0) root         (0)    17849 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/nodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:42:07.294971 lenscraft-1.0.4/src/lenscraft/texture/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/texture/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2682 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/texture/classify.py
+-rw-rw-rw-   0 root         (0) root         (0)    14493 2024-04-30 14:38:40.000000 lenscraft-1.0.4/src/lenscraft/texture/tool.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-23 18:41:25.000000 lenscraft-1.0.4/src/lenscraft/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:42:07.294971 lenscraft-1.0.4/src/lenscraft.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1300 2024-04-30 14:42:07.000000 lenscraft-1.0.4/src/lenscraft.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      877 2024-04-30 14:42:07.000000 lenscraft-1.0.4/src/lenscraft.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 14:42:07.000000 lenscraft-1.0.4/src/lenscraft.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-30 14:42:07.000000 lenscraft-1.0.4/src/lenscraft.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2024-04-30 14:42:07.000000 lenscraft-1.0.4/src/lenscraft.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-30 14:42:07.000000 lenscraft-1.0.4/src/lenscraft.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 14:42:07.294971 lenscraft-1.0.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:41:25.000000 lenscraft-1.0.4/tests/__init__.py
```

### Comparing `lenscraft-1.0.3/.gitignore` & `lenscraft-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/LICENSE` & `lenscraft-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/PKG-INFO` & `lenscraft-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lenscraft
-Version: 1.0.3
+Version: 1.0.4
 Summary: Application to quickly build machine vision pipelines with little or no code
 Author-email: Gudjon Einar Magnusson <gmagnusson@fraunhofer.org>
 Project-URL: Homepage, https://cma.fraunhofer.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `lenscraft-1.0.3/README.md` & `lenscraft-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/images/0.9858_1.1766.png` & `lenscraft-1.0.4/images/0.9858_1.1766.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/images/334.png` & `lenscraft-1.0.4/images/334.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/images/Ring_9_9.png` & `lenscraft-1.0.4/images/Ring_9_9.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/images/mask.png` & `lenscraft-1.0.4/images/mask.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/images/spacer_top__13.png` & `lenscraft-1.0.4/images/spacer_top__13.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/images/spacer_top__14.png` & `lenscraft-1.0.4/images/spacer_top__14.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/images/spacer_top__3.png` & `lenscraft-1.0.4/images/spacer_top__3.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/images/spacer_top__9.png` & `lenscraft-1.0.4/images/spacer_top__9.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/pyproject.toml` & `lenscraft-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/src/lenscraft/assets/CornerTemplate.png` & `lenscraft-1.0.4/src/lenscraft/assets/CornerTemplate.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/src/lenscraft/editor/__init__.py` & `lenscraft-1.0.4/src/lenscraft/editor/__init__.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/src/lenscraft/gabor.py` & `lenscraft-1.0.4/src/lenscraft/gabor.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/src/lenscraft/image.py` & `lenscraft-1.0.4/src/lenscraft/image.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/src/lenscraft/nodes.py` & `lenscraft-1.0.4/src/lenscraft/nodes.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/src/lenscraft/texture/__init__.py` & `lenscraft-1.0.4/src/lenscraft/texture/__init__.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/src/lenscraft/texture/classify.py` & `lenscraft-1.0.4/src/lenscraft/texture/classify.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/src/lenscraft/texture/tool.py` & `lenscraft-1.0.4/src/lenscraft/texture/tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,14 +316,18 @@
 
     def draw(self):
         dt = time.time() - self._last_draw
         if dt < 0.05:
             # Prevent drawing too fast
             return
         
+        if np.array_equal(self.start, self.end):
+            # Dont draw unless there is some distance between start and end
+            return
+        
         self.draw_line()
         self.draw_rectangles()
         self._last_draw = time.time()
 
     def draw_line(self):
         if self.line_id and dpg.does_item_exist(self.line_id):
             dpg.delete_item(self.line_id)
```

### Comparing `lenscraft-1.0.3/src/lenscraft/utils.py` & `lenscraft-1.0.4/src/lenscraft/utils.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.3/src/lenscraft.egg-info/PKG-INFO` & `lenscraft-1.0.4/src/lenscraft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lenscraft
-Version: 1.0.3
+Version: 1.0.4
 Summary: Application to quickly build machine vision pipelines with little or no code
 Author-email: Gudjon Einar Magnusson <gmagnusson@fraunhofer.org>
 Project-URL: Homepage, https://cma.fraunhofer.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `lenscraft-1.0.3/src/lenscraft.egg-info/SOURCES.txt` & `lenscraft-1.0.4/src/lenscraft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

