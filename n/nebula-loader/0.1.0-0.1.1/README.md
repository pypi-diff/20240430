# Comparing `tmp/nebula_loader-0.1.0.tar.gz` & `tmp/nebula_loader-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nebula_loader-0.1.0.tar", last modified: Tue Apr 30 08:02:35 2024, max compression
+gzip compressed data, was "nebula_loader-0.1.1.tar", last modified: Tue Apr 30 08:41:03 2024, max compression
```

## Comparing `nebula_loader-0.1.0.tar` & `nebula_loader-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3449 2024-04-25 03:26:11.537636 nebula_loader-0.1.0/README.md
--rw-r--r--   0        0        0      416 2024-04-30 08:02:35.562175 nebula_loader-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       91 2024-04-30 08:01:27.991659 nebula_loader-0.1.0/src/nebula_loader/__init__.py
--rw-r--r--   0        0        0    15941 2024-04-30 08:01:27.991659 nebula_loader-0.1.0/src/nebula_loader/ng_load.py
--rw-r--r--   0        0        0     3777 1970-01-01 00:00:00.000000 nebula_loader-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3449 2024-04-30 08:40:59.562426 nebula_loader-0.1.1/README.md
+-rw-r--r--   0        0        0      416 2024-04-30 08:41:03.022393 nebula_loader-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       91 2024-04-30 08:40:59.662425 nebula_loader-0.1.1/src/nebula_loader/__init__.py
+-rw-r--r--   0        0        0    15941 2024-04-30 08:40:59.662425 nebula_loader-0.1.1/src/nebula_loader/ng_load.py
+-rw-r--r--   0        0        0     3777 1970-01-01 00:00:00.000000 nebula_loader-0.1.1/PKG-INFO
```

### Comparing `nebula_loader-0.1.0/README.md` & `nebula_loader-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nebula_loader-0.1.0/src/nebula_loader/ng_load.py` & `nebula_loader-0.1.1/src/nebula_loader/ng_load.py`

 * *Files identical despite different names*

### Comparing `nebula_loader-0.1.0/PKG-INFO` & `nebula_loader-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nebula_loader
-Version: 0.1.0
+Version: 0.1.1
 Summary: Load from awesome-dataset into NebulaGraph
 Requires-Python: >=3.8
 Requires-Dist: requests>=2.31.0
 Requires-Dist: pandas>=2.0.3
 Requires-Dist: pydantic>=2.7.1
 Requires-Dist: tqdm>=4.66.2
 Requires-Dist: nebula3-python>=3.8
```

