# Comparing `tmp/nn_mouse-1.0.0.tar.gz` & `tmp/nn_mouse-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nn_mouse-1.0.0.tar", last modified: Mon Apr 29 04:34:38 2024, max compression
+gzip compressed data, was "nn_mouse-1.0.1.tar", last modified: Tue Apr 30 06:12:17 2024, max compression
```

## Comparing `nn_mouse-1.0.0.tar` & `nn_mouse-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:34:38.511725 nn_mouse-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-29 04:34:34.000000 nn_mouse-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 04:34:34.000000 nn_mouse-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-29 04:34:38.511725 nn_mouse-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-29 04:34:34.000000 nn_mouse-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:34:38.511725 nn_mouse-1.0.0/nn_mouse/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 04:34:34.000000 nn_mouse-1.0.0/nn_mouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   813475 2024-04-29 04:34:34.000000 nn_mouse-1.0.0/nn_mouse/path.onnx
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-29 04:34:34.000000 nn_mouse-1.0.0/nn_mouse/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 04:34:34.000000 nn_mouse-1.0.0/nn_mouse/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    90042 2024-04-29 04:34:34.000000 nn_mouse-1.0.0/nn_mouse/time.onnx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 04:34:38.511725 nn_mouse-1.0.0/nn_mouse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-29 04:34:38.000000 nn_mouse-1.0.0/nn_mouse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-29 04:34:38.000000 nn_mouse-1.0.0/nn_mouse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 04:34:38.000000 nn_mouse-1.0.0/nn_mouse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-29 04:34:38.000000 nn_mouse-1.0.0/nn_mouse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 04:34:38.000000 nn_mouse-1.0.0/nn_mouse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-29 04:34:34.000000 nn_mouse-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 04:34:38.511725 nn_mouse-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:12:17.092780 nn_mouse-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-30 06:12:12.000000 nn_mouse-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-30 06:12:12.000000 nn_mouse-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-30 06:12:17.092780 nn_mouse-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-30 06:12:12.000000 nn_mouse-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:12:17.088780 nn_mouse-1.0.1/nn_mouse/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 06:12:12.000000 nn_mouse-1.0.1/nn_mouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   813475 2024-04-30 06:12:12.000000 nn_mouse-1.0.1/nn_mouse/path.onnx
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-30 06:12:12.000000 nn_mouse-1.0.1/nn_mouse/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:12:12.000000 nn_mouse-1.0.1/nn_mouse/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    90042 2024-04-30 06:12:12.000000 nn_mouse-1.0.1/nn_mouse/time.onnx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:12:17.092780 nn_mouse-1.0.1/nn_mouse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-30 06:12:17.000000 nn_mouse-1.0.1/nn_mouse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-30 06:12:17.000000 nn_mouse-1.0.1/nn_mouse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:12:17.000000 nn_mouse-1.0.1/nn_mouse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 06:12:17.000000 nn_mouse-1.0.1/nn_mouse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 06:12:17.000000 nn_mouse-1.0.1/nn_mouse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-30 06:12:12.000000 nn_mouse-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 06:12:17.092780 nn_mouse-1.0.1/setup.cfg
```

### Comparing `nn_mouse-1.0.0/LICENSE` & `nn_mouse-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nn_mouse-1.0.0/PKG-INFO` & `nn_mouse-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nn-mouse
-Version: 1.0.0
+Version: 1.0.1
 Summary: Neural network based humanized mouse movements
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `nn_mouse-1.0.0/README.md` & `nn_mouse-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nn_mouse-1.0.0/nn_mouse/path.onnx` & `nn_mouse-1.0.1/nn_mouse/path.onnx`

 * *Files identical despite different names*

### Comparing `nn_mouse-1.0.0/nn_mouse/predict.py` & `nn_mouse-1.0.1/nn_mouse/predict.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,26 +14,39 @@
 def predict(model: Net, x: float, y: float):
     value = np.array([[x, y]])
     model.setInput(value)
     outputs = model.forward()
     return outputs
 
 
-def get_path(x: int, y: int, x1: int, y1: int, w: int, h: int):
+def get_path(
+    x: int, y: int, x1: int, y1: int, w: int, h: int
+) -> List[Tuple[float, float, float]]:
     """
     Returns a list of tuple (x, y, t) where x, y is
     the location and t is the time to stay on each location
 
     :param x: x coordinate of current mouse position
     :param y: y coordinate of current mouse position
     :param x1: x coordinate of target mouse position
     :param y1: y coordinate of target mouse position
     :param w: width of the monitor
     :param h: height of the monitor
     """
     dx, dy = (x1 - x) / w, (y1 - y) / h
+    if dx == 0 and dy == 0:
+        return []
+
+    # the model does not work properly for
+    # small distances, so scale dx, dy if
+    # distance is too small
+    dist = (dx**2 + dy**2) ** 0.5
+    f = 1 / dist if dist < 0.2 else 1
+
+    dx, dy = f * dx, f * dy
     path = predict(path_model, dx, dy)
     time = predict(time_model, dx, dy)
     output: List[Tuple[float, float, float]] = []
     for (x2, y2), [t] in zip(path[0], time[0]):
-        output.append((x + x2 * w, y + y2 * h, t / 100_000))
+        output.append((x + x2 / f * w, y + y2 / f * h, t / 100_000 / f))
+    output.append((x1, y1, 0))
     return output
```

### Comparing `nn_mouse-1.0.0/nn_mouse/time.onnx` & `nn_mouse-1.0.1/nn_mouse/time.onnx`

 * *Files identical despite different names*

### Comparing `nn_mouse-1.0.0/nn_mouse.egg-info/PKG-INFO` & `nn_mouse-1.0.1/nn_mouse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nn-mouse
-Version: 1.0.0
+Version: 1.0.1
 Summary: Neural network based humanized mouse movements
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `nn_mouse-1.0.0/pyproject.toml` & `nn_mouse-1.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nn-mouse"
-version = "1.0.0"
+version = "1.0.1"
 dependencies = ["opencv-python"]
 requires-python = ">=3"
 authors = [{ name = "Pradish Bijukchhe", email = "pradish@sandbox.com.np" }]
 description = "Neural network based humanized mouse movements"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = []
```

