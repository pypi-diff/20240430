# Comparing `tmp/easykube-0.3.0.tar.gz` & `tmp/easykube-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easykube-0.3.0.tar", last modified: Tue Apr  2 14:01:50 2024, max compression
+gzip compressed data, was "easykube-0.3.1.tar", last modified: Tue Apr 30 15:13:14 2024, max compression
```

## Comparing `easykube-0.3.0.tar` & `easykube-0.3.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:50.182457 easykube-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:50.174457 easykube-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:50.178457 easykube-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-02 14:01:46.000000 easykube-0.3.0/.github/workflows/pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 14:01:46.000000 easykube-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 14:01:46.000000 easykube-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-02 14:01:50.182457 easykube-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 14:01:46.000000 easykube-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:50.178457 easykube-0.3.0/easykube/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/flow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:50.178457 easykube-0.3.0/easykube/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:50.178457 easykube-0.3.0/easykube/kubernetes/client/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/client/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/client/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/client/iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/client/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/client/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/kubernetes/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:50.182457 easykube-0.3.0/easykube/rest/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/rest/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/rest/iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/rest/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-02 14:01:46.000000 easykube-0.3.0/easykube/rest/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:50.182457 easykube-0.3.0/easykube.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-02 14:01:50.000000 easykube-0.3.0/easykube.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-02 14:01:50.000000 easykube-0.3.0/easykube.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:01:50.000000 easykube-0.3.0/easykube.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:01:49.000000 easykube-0.3.0/easykube.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 14:01:50.000000 easykube-0.3.0/easykube.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 14:01:50.000000 easykube-0.3.0/easykube.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-02 14:01:46.000000 easykube-0.3.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-04-02 14:01:50.182457 easykube-0.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-04-02 14:01:46.000000 easykube-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:13:14.774824 easykube-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:13:14.766824 easykube-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:13:14.770824 easykube-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-30 15:13:10.000000 easykube-0.3.1/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-30 15:13:10.000000 easykube-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 15:13:10.000000 easykube-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-30 15:13:14.774824 easykube-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 15:13:10.000000 easykube-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:13:14.770824 easykube-0.3.1/easykube/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/flow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:13:14.770824 easykube-0.3.1/easykube/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:13:14.770824 easykube-0.3.1/easykube/kubernetes/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/client/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/client/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/client/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/kubernetes/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:13:14.770824 easykube-0.3.1/easykube/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/rest/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/rest/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/rest/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-30 15:13:10.000000 easykube-0.3.1/easykube/rest/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:13:14.770824 easykube-0.3.1/easykube.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-30 15:13:14.000000 easykube-0.3.1/easykube.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-30 15:13:14.000000 easykube-0.3.1/easykube.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:13:14.000000 easykube-0.3.1/easykube.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:13:14.000000 easykube-0.3.1/easykube.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 15:13:14.000000 easykube-0.3.1/easykube.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 15:13:14.000000 easykube-0.3.1/easykube.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-30 15:13:10.000000 easykube-0.3.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-04-30 15:13:14.774824 easykube-0.3.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-04-30 15:13:10.000000 easykube-0.3.1/setup.py
```

### Comparing `easykube-0.3.0/.github/workflows/pypi-publish.yaml` & `easykube-0.3.1/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `easykube-0.3.0/LICENSE` & `easykube-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easykube-0.3.0/easykube/flow.py` & `easykube-0.3.1/easykube/flow.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.0/easykube/kubernetes/client/api.py` & `easykube-0.3.1/easykube/kubernetes/client/api.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.0/easykube/kubernetes/client/client.py` & `easykube-0.3.1/easykube/kubernetes/client/client.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.0/easykube/kubernetes/client/errors.py` & `easykube-0.3.1/easykube/kubernetes/client/errors.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.0/easykube/kubernetes/client/iterators.py` & `easykube-0.3.1/easykube/kubernetes/client/iterators.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.0/easykube/kubernetes/client/resource.py` & `easykube-0.3.1/easykube/kubernetes/client/resource.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.0/easykube/kubernetes/client/spec.py` & `easykube-0.3.1/easykube/kubernetes/client/spec.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.0/easykube/kubernetes/config.py` & `easykube-0.3.1/easykube/kubernetes/config.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.0/easykube/kubernetes/resources.py` & `easykube-0.3.1/easykube/kubernetes/resources.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.0/easykube/rest/client.py` & `easykube-0.3.1/easykube/rest/client.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.0/easykube/rest/iterators.py` & `easykube-0.3.1/easykube/rest/iterators.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.0/easykube/rest/resource.py` & `easykube-0.3.1/easykube/rest/resource.py`

 * *Files identical despite different names*

### Comparing `easykube-0.3.0/easykube/rest/util.py` & `easykube-0.3.1/easykube/rest/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from collections.abc import MutableMapping
+from yaml.representer import SafeRepresenter
 
 
 class PropertyDict(dict):
     """
     Dictionary that also supports property access.
     """
     def __init__(self, *args, **kwargs):
@@ -39,7 +39,11 @@
         try:
             return self[name]
         except KeyError:
             raise AttributeError(f"'{self.__class__.__name__}' has no attribute '{name}'")
 
     def __repr__(self):
         return f"{self.__class__.__name__}({super().__repr__()})"
+    
+
+# Make sure that YAML represents a PropertyDict like a regular dict
+SafeRepresenter.add_representer(PropertyDict, SafeRepresenter.represent_dict)
```

### Comparing `easykube-0.3.0/easykube.egg-info/SOURCES.txt` & `easykube-0.3.1/easykube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

