# Comparing `tmp/mashumaro-3.9.tar.gz` & `tmp/mashumaro-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mashumaro-3.9.tar", last modified: Wed Aug  2 20:00:20 2023, max compression
+gzip compressed data, was "mashumaro-3.9.1.tar", last modified: Tue Aug 22 21:37:55 2023, max compression
```

## Comparing `mashumaro-3.9.tar` & `mashumaro-3.9.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-02 20:00:20.399084 mashumaro-3.9/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    10763 2023-06-22 18:41:04.000000 mashumaro-3.9/LICENSE
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    95909 2023-08-02 20:00:20.398848 mashumaro-3.9/PKG-INFO
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    94990 2023-08-02 19:58:06.000000 mashumaro-3.9/README.md
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-02 20:00:20.382670 mashumaro-3.9/mashumaro/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      258 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1674 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/config.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-02 20:00:20.384059 mashumaro-3.9/mashumaro/core/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/core/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1013 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/core/const.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      825 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/core/helpers.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-02 20:00:20.384634 mashumaro-3.9/mashumaro/core/meta/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/core/meta/__init__.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-02 20:00:20.385145 mashumaro-3.9/mashumaro/core/meta/code/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/core/meta/code/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    43193 2023-08-02 19:56:28.000000 mashumaro-3.9/mashumaro/core/meta/code/builder.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      815 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/core/meta/code/lines.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    22345 2023-08-02 19:56:28.000000 mashumaro-3.9/mashumaro/core/meta/helpers.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1366 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/core/meta/mixin.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-02 20:00:20.385743 mashumaro-3.9/mashumaro/core/meta/types/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/core/meta/types/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     4882 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/core/meta/types/common.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    25046 2023-08-02 19:56:28.000000 mashumaro-3.9/mashumaro/core/meta/types/pack.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    42525 2023-08-02 19:56:28.000000 mashumaro-3.9/mashumaro/core/meta/types/unpack.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      469 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/dialect.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     5491 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/exceptions.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1472 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/helper.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-02 20:00:20.386654 mashumaro-3.9/mashumaro/jsonschema/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      214 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/jsonschema/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     2151 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/jsonschema/annotations.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     2837 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/jsonschema/builder.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      747 2023-08-02 19:56:28.000000 mashumaro-3.9/mashumaro/jsonschema/dialects.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     5946 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/jsonschema/models.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    26112 2023-08-02 19:56:28.000000 mashumaro-3.9/mashumaro/jsonschema/schema.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-02 20:00:20.397990 mashumaro-3.9/mashumaro/mixins/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/mixins/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1867 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/mixins/dict.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      790 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/mixins/json.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1558 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/mixins/msgpack.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1731 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/mixins/orjson.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1000 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/mixins/orjson.pyi
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1392 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/mixins/toml.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1108 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/mixins/yaml.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/py.typed
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     2715 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/types.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-02 20:00:20.383597 mashumaro-3.9/mashumaro.egg-info/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    95909 2023-08-02 20:00:20.000000 mashumaro-3.9/mashumaro.egg-info/PKG-INFO
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1210 2023-08-02 20:00:20.000000 mashumaro-3.9/mashumaro.egg-info/SOURCES.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-08-02 20:00:20.000000 mashumaro-3.9/mashumaro.egg-info/dependency_links.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-06-22 18:41:44.000000 mashumaro-3.9/mashumaro.egg-info/not-zip-safe
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      155 2023-08-02 20:00:20.000000 mashumaro-3.9/mashumaro.egg-info/requires.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)       10 2023-08-02 20:00:20.000000 mashumaro-3.9/mashumaro.egg-info/top_level.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      689 2023-06-22 18:41:04.000000 mashumaro-3.9/pyproject.toml
--rw-r--r--   0 tikhonov_a   (501) staff       (20)       38 2023-08-02 20:00:20.399135 mashumaro-3.9/setup.cfg
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1463 2023-08-02 20:00:13.000000 mashumaro-3.9/setup.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-22 21:37:55.258798 mashumaro-3.9.1/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    10763 2023-06-22 18:41:04.000000 mashumaro-3.9.1/LICENSE
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    95911 2023-08-22 21:37:55.258659 mashumaro-3.9.1/PKG-INFO
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    94990 2023-08-02 19:58:06.000000 mashumaro-3.9.1/README.md
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-22 21:37:55.253294 mashumaro-3.9.1/mashumaro/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      258 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1674 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/config.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-22 21:37:55.254530 mashumaro-3.9.1/mashumaro/core/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/core/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1013 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/core/const.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      825 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/core/helpers.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-22 21:37:55.255151 mashumaro-3.9.1/mashumaro/core/meta/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/core/meta/__init__.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-22 21:37:55.255576 mashumaro-3.9.1/mashumaro/core/meta/code/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/core/meta/code/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    43193 2023-08-02 19:56:28.000000 mashumaro-3.9.1/mashumaro/core/meta/code/builder.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      815 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/core/meta/code/lines.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    22345 2023-08-02 19:56:28.000000 mashumaro-3.9.1/mashumaro/core/meta/helpers.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1366 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/core/meta/mixin.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-22 21:37:55.256204 mashumaro-3.9.1/mashumaro/core/meta/types/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/core/meta/types/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     4924 2023-08-22 21:36:11.000000 mashumaro-3.9.1/mashumaro/core/meta/types/common.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    25046 2023-08-02 19:56:28.000000 mashumaro-3.9.1/mashumaro/core/meta/types/pack.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    42525 2023-08-02 19:56:28.000000 mashumaro-3.9.1/mashumaro/core/meta/types/unpack.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      469 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/dialect.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     5491 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/exceptions.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1472 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/helper.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-22 21:37:55.257038 mashumaro-3.9.1/mashumaro/jsonschema/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      214 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/jsonschema/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     2151 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/jsonschema/annotations.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     2837 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/jsonschema/builder.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      747 2023-08-02 19:56:28.000000 mashumaro-3.9.1/mashumaro/jsonschema/dialects.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     5946 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/jsonschema/models.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    27808 2023-08-22 21:36:11.000000 mashumaro-3.9.1/mashumaro/jsonschema/schema.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-22 21:37:55.258363 mashumaro-3.9.1/mashumaro/mixins/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/mixins/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1867 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/mixins/dict.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      790 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/mixins/json.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1558 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/mixins/msgpack.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1731 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/mixins/orjson.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1000 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/mixins/orjson.pyi
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1392 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/mixins/toml.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1108 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/mixins/yaml.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/py.typed
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     2715 2023-06-22 18:41:04.000000 mashumaro-3.9.1/mashumaro/types.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-22 21:37:55.254195 mashumaro-3.9.1/mashumaro.egg-info/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    95911 2023-08-22 21:37:55.000000 mashumaro-3.9.1/mashumaro.egg-info/PKG-INFO
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1210 2023-08-22 21:37:55.000000 mashumaro-3.9.1/mashumaro.egg-info/SOURCES.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-08-22 21:37:55.000000 mashumaro-3.9.1/mashumaro.egg-info/dependency_links.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-06-22 18:41:44.000000 mashumaro-3.9.1/mashumaro.egg-info/not-zip-safe
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      155 2023-08-22 21:37:55.000000 mashumaro-3.9.1/mashumaro.egg-info/requires.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       10 2023-08-22 21:37:55.000000 mashumaro-3.9.1/mashumaro.egg-info/top_level.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      689 2023-06-22 18:41:04.000000 mashumaro-3.9.1/pyproject.toml
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       38 2023-08-22 21:37:55.258842 mashumaro-3.9.1/setup.cfg
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1465 2023-08-22 21:37:39.000000 mashumaro-3.9.1/setup.py
```

### Comparing `mashumaro-3.9/LICENSE` & `mashumaro-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/PKG-INFO` & `mashumaro-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mashumaro
-Version: 3.9
+Version: 3.9.1
 Summary: Fast serialization library on top of dataclasses
 Home-page: https://github.com/Fatal1ty/mashumaro
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mashumaro-3.9/README.md` & `mashumaro-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/config.py` & `mashumaro-3.9.1/mashumaro/config.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/core/const.py` & `mashumaro-3.9.1/mashumaro/core/const.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/core/helpers.py` & `mashumaro-3.9.1/mashumaro/core/helpers.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/core/meta/code/builder.py` & `mashumaro-3.9.1/mashumaro/core/meta/code/builder.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/core/meta/code/lines.py` & `mashumaro-3.9.1/mashumaro/core/meta/code/lines.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/core/meta/helpers.py` & `mashumaro-3.9.1/mashumaro/core/meta/helpers.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/core/meta/mixin.py` & `mashumaro-3.9.1/mashumaro/core/meta/mixin.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/core/meta/types/common.py` & `mashumaro-3.9.1/mashumaro/core/meta/types/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     # for python 3.7
     cached_property = property  # type: ignore
 
 from typing_extensions import ParamSpec, TypeAlias
 
 from mashumaro.core.const import PEP_585_COMPATIBLE
 from mashumaro.core.meta.helpers import (
+    get_args,
     get_type_origin,
     is_annotated,
     is_generic,
     type_name,
 )
 from mashumaro.exceptions import UnserializableDataError, UnserializableField
 
@@ -120,15 +121,15 @@
                 return expr
         raise UnserializableField(
             spec.field_ctx.name, spec.type, spec.builder.cls
         )
 
 
 def ensure_generic_collection(spec: ValueSpec) -> bool:
-    if not PEP_585_COMPATIBLE:
+    if not PEP_585_COMPATIBLE and not get_args(spec.type):
         proper_type = PROPER_COLLECTION_TYPES.get(spec.type)
         if proper_type:
             raise UnserializableField(
                 field_name=spec.field_ctx.name,
                 field_type=spec.type,
                 holder_class=spec.builder.cls,
                 msg=f"Use {proper_type} instead",
```

### Comparing `mashumaro-3.9/mashumaro/core/meta/types/pack.py` & `mashumaro-3.9.1/mashumaro/core/meta/types/pack.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/core/meta/types/unpack.py` & `mashumaro-3.9.1/mashumaro/core/meta/types/unpack.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/exceptions.py` & `mashumaro-3.9.1/mashumaro/exceptions.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/helper.py` & `mashumaro-3.9.1/mashumaro/helper.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/jsonschema/annotations.py` & `mashumaro-3.9.1/mashumaro/jsonschema/annotations.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/jsonschema/builder.py` & `mashumaro-3.9.1/mashumaro/jsonschema/builder.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/jsonschema/dialects.py` & `mashumaro-3.9.1/mashumaro/jsonschema/dialects.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/jsonschema/models.py` & `mashumaro-3.9.1/mashumaro/jsonschema/models.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/jsonschema/schema.py` & `mashumaro-3.9.1/mashumaro/jsonschema/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from fractions import Fraction
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     List,
-    Mapping,
     Optional,
     Tuple,
     Type,
     Union,
 )
 from uuid import UUID
 
@@ -98,109 +97,134 @@
 UTC_OFFSET_PATTERN = r"^UTC([+-][0-2][0-9]:[0-5][0-9])?$"
 
 
 @dataclass
 class Instance:
     type: Type
     name: Optional[str] = None
+
+    __owner_builder: Optional[CodeBuilder] = None
+    __self_builder: Optional[CodeBuilder] = None
+
     origin_type: Type = field(init=False)
     annotations: List[Annotation] = field(init=False, default_factory=list)
-    __builder: Optional[CodeBuilder] = None
+
+    __metadata: Optional[Dict[str, Any]] = field(init=False, default=None)
 
     @property
-    def _builder(self) -> CodeBuilder:
-        assert self.__builder
-        return self.__builder
+    # TODO: switch to cached_property after dropping python 3.7 support
+    def metadata(self) -> Dict[str, Any]:
+        if self.__metadata is None:
+            if self.name and self.__owner_builder:
+                self.__metadata = dict(
+                    **self.__owner_builder.metadatas.get(self.name, {})
+                )
+            else:
+                self.__metadata = {}
+        return self.__metadata
 
     @property
-    def metadata(self) -> Mapping[str, Any]:
-        if not self.name:
-            return {}
-        return self._builder.metadatas.get(self.name, {})
+    def _self_builder(self) -> CodeBuilder:
+        assert self.__self_builder
+        return self.__self_builder
 
     @property
     def alias(self) -> Optional[str]:
         alias = self.metadata.get("alias")
         if alias is None:
-            alias = self.get_config().aliases.get(self.name)  # type: ignore
+            aliases_config = self.get_owner_config().aliases
+            alias = aliases_config.get(self.name)  # type: ignore
         if alias is None:
             alias = self.name
         return alias
 
     @property
-    def holder_class(self) -> Optional[Type]:
-        if self.__builder:
-            return self.__builder.cls
+    def owner_class(self) -> Optional[Type]:
+        if self.__owner_builder:
+            return self.__owner_builder.cls
         return None
 
-    def copy(self, **changes: Any) -> "Instance":
-        return replace(self, **changes)
+    def derive(self, **changes: Any) -> "Instance":
+        new_instance = replace(self, **changes)
+        if is_dataclass(self.origin_type):
+            new_instance.__owner_builder = self.__self_builder
+        return new_instance
 
     def __post_init__(self) -> None:
         self.update_type(self.type)
         if is_annotated(self.type):
             self.annotations = getattr(self.type, "__metadata__", [])
             self.type = get_args(self.type)[0]
             self.origin_type = get_type_origin(self.type)
 
     def update_type(self, new_type: Type) -> None:
-        if self.__builder:
-            self.type = self.__builder._get_real_type(
+        if self.__owner_builder:
+            self.type = self.__owner_builder._get_real_type(
                 field_name=self.name,  # type: ignore
                 field_type=new_type,
             )
         self.origin_type = get_type_origin(self.type)
         if is_dataclass(self.origin_type):
             type_args = get_args(self.type)
-            self.__builder = CodeBuilder(self.origin_type, type_args)
-            self.__builder.reset()
+            self.__self_builder = CodeBuilder(self.origin_type, type_args)
+            self.__self_builder.reset()
+        else:
+            self.__self_builder = None
 
     def fields(self) -> Iterable[Tuple[str, Type, bool, Any]]:
-        for f_name, f_type in self._builder.get_field_types(
+        for f_name, f_type in self._self_builder.get_field_types(
             include_extras=True
         ).items():
-            f = self._builder.dataclass_fields.get(f_name)  # type: ignore
+            f = self._self_builder.dataclass_fields.get(f_name)  # type: ignore
             if f and not f.init:
                 continue
             f_default = f.default
             if f_default is MISSING:
-                f_default = self._builder.namespace.get(f_name, MISSING)
+                f_default = self._self_builder.namespace.get(f_name, MISSING)
             if f_default is not MISSING:
-                f_default = _default(f_type, f_default)
+                f_default = _default(f_type, f_default, self.get_self_config())
 
             has_default = (
                 f.default is not MISSING or f.default_factory is not MISSING
             )
 
             yield f_name, f_type, has_default, f_default
 
     def get_overridden_serialization_method(
         self,
     ) -> Optional[Union[Callable, str]]:
-        if not self.__builder:
+        if not self.__owner_builder:
             return None
         serialize_option = self.metadata.get("serialize")
         if serialize_option is not None:
+            if callable(serialize_option):
+                self.metadata.pop("serialize", None)  # prevent recursion
             return serialize_option
-        for strategy in self.__builder.iter_serialization_strategies(
+        for strategy in self.__owner_builder.iter_serialization_strategies(
             self.metadata, self.type
         ):
             if strategy is pass_through:
                 return pass_through
             elif isinstance(strategy, dict):
                 serialize_option = strategy.get("serialize")
             elif isinstance(strategy, SerializationStrategy):
                 serialize_option = strategy.serialize
             if serialize_option is not None:
                 return serialize_option
         return None
 
-    def get_config(self) -> Type[BaseConfig]:
-        if self.__builder:
-            return self.__builder.get_config()
+    def get_owner_config(self) -> Type[BaseConfig]:
+        if self.__owner_builder:
+            return self.__owner_builder.get_config()
+        else:
+            return BaseConfig
+
+    def get_self_config(self) -> Type[BaseConfig]:
+        if self.__self_builder:
+            return self.__self_builder.get_config()
         else:
             return BaseConfig
 
 
 InstanceSchemaCreator: TypeAlias = Callable[
     [Instance, Context], Optional[JSONSchema]
 ]
@@ -231,81 +255,94 @@
         if schema is not None:
             if with_dialect_uri:
                 schema.schema = ctx.dialect.uri
             return schema
     raise NotImplementedError(
         (
             f'Type {type_name(instance.type)} of field "{instance.name}" '
-            f"in {type_name(instance.holder_class)} isn't supported"
+            f"in {type_name(instance.owner_class)} isn't supported"
         )
     )
 
 
 def _get_schema_or_none(
     instance: Instance, ctx: Context
 ) -> Optional[JSONSchema]:
     schema = get_schema(instance, ctx)
     if isinstance(schema, EmptyJSONSchema):
         return None
     return schema
 
 
-def _default(f_type: Type, f_value: Any) -> Any:
+def _default(f_type: Type, f_value: Any, config_cls: Type[BaseConfig]) -> Any:
     @dataclass
     class CC(DataClassJSONMixin):
         x: f_type = f_value  # type: ignore
 
+        class Config(config_cls):  # type: ignore
+            pass
+
     return CC(f_value).to_dict()["x"]
 
 
 Registry = InstanceSchemaCreatorRegistry()
 register = Registry.register
 
 
-def override_field_instance_type_if_needed(
-    root_instance: Instance, field_instance: Instance
-) -> None:
-    overridden_method = field_instance.get_overridden_serialization_method()
+@register
+def on_type_with_overridden_serialization(
+    instance: Instance, ctx: Context
+) -> Optional[JSONSchema]:
+    def override_with_any(reason: Any) -> None:
+        if instance.owner_class is not None:
+            name = f"{type_name(instance.owner_class)}.{instance.name}"
+        else:  # pragma: no cover
+            # we will have an owner class, but leave this here just in case
+            name = type_name(instance.type)
+        warnings.warn(
+            f"Type Any will be used for {name} with "
+            f"overridden serialization method: {reason}"
+        )
+        instance.update_type(Any)  # type: ignore[arg-type]
+
+    overridden_method = instance.get_overridden_serialization_method()
     if overridden_method is pass_through:
-        return
+        return None
     elif callable(overridden_method):
         try:
-            field_instance.update_type(
-                get_function_return_annotation(overridden_method)
-            )
+            new_type = get_function_return_annotation(overridden_method)
+            if new_type is instance.type:
+                return None
+            else:
+                instance.update_type(new_type)
         except Exception as e:
-            warnings.warn(
-                f"Type Any will be used for "
-                f"{type_name(root_instance.type)}.{field_instance.name} with "
-                f"overridden serialization method: {e}"
-            )
-            field_instance.update_type(Any)  # type: ignore[arg-type]
+            override_with_any(e)
+        return get_schema(instance, ctx)
 
 
 @register
 def on_dataclass(instance: Instance, ctx: Context) -> Optional[JSONSchema]:
     # TODO: Self references might not work
     if is_dataclass(instance.origin_type):
-        jsonschema_config = instance.get_config().json_schema
+        jsonschema_config = instance.get_self_config().json_schema
         schema = JSONObjectSchema(
             title=instance.origin_type.__name__,
             additionalProperties=jsonschema_config.get(
                 "additionalProperties", False
             ),
         )
         properties: Dict[str, JSONSchema] = {}
         required = []
         field_schema_overrides = jsonschema_config.get("properties", {})
         for f_name, f_type, has_default, f_default in instance.fields():
             override = field_schema_overrides.get(f_name)
-            f_instance = instance.copy(type=f_type, name=f_name)
+            f_instance = instance.derive(type=f_type, name=f_name)
             if override:
                 f_schema = JSONSchema.from_dict(override)
             else:
-                override_field_instance_type_if_needed(instance, f_instance)
                 f_schema = get_schema(f_instance, ctx)
             if f_instance.alias:
                 f_name = f_instance.alias
             if f_default is not MISSING:
                 f_schema.default = f_default
             description = f_instance.metadata.get("description")
             if description:
@@ -357,42 +394,46 @@
     if not is_special_typing_primitive(instance.origin_type):
         return None
 
     args = get_args(instance.type)
 
     if is_union(instance.type):
         return JSONSchema(
-            anyOf=[get_schema(instance.copy(type=arg), ctx) for arg in args]
+            anyOf=[get_schema(instance.derive(type=arg), ctx) for arg in args]
         )
     elif is_type_var_any(instance.type):
         return EmptyJSONSchema()
     elif is_type_var(instance.type):
         constraints = getattr(instance.type, "__constraints__")
         if constraints:
             return JSONSchema(
                 anyOf=[
-                    get_schema(instance.copy(type=arg), ctx)
+                    get_schema(instance.derive(type=arg), ctx)
                     for arg in constraints
                 ]
             )
         else:
             bound = getattr(instance.type, "__bound__")
-            return get_schema(instance.copy(type=bound), ctx)
+            return get_schema(instance.derive(type=bound), ctx)
     elif is_new_type(instance.type):
-        return get_schema(instance.copy(type=instance.type.__supertype__), ctx)
+        return get_schema(
+            instance.derive(type=instance.type.__supertype__), ctx
+        )
     elif is_literal(instance.type):
         return on_literal(instance, ctx)
     # elif is_self(instance.type):
     #     raise NotImplementedError
     elif is_required(instance.type) or is_not_required(instance.type):
-        return get_schema(instance.copy(type=args[0]), ctx)
+        return get_schema(instance.derive(type=args[0]), ctx)
     elif is_unpack(instance.type):
-        return get_schema(instance.copy(type=get_args(instance.type)[0]), ctx)
+        return get_schema(
+            instance.derive(type=get_args(instance.type)[0]), ctx
+        )
     elif is_type_var_tuple(instance.type):
-        return get_schema(instance.copy(type=Tuple[Any, ...]), ctx)
+        return get_schema(instance.derive(type=Tuple[Any, ...]), ctx)
 
 
 @register
 def on_number(instance: Instance, ctx: Context) -> Optional[JSONSchema]:
     if instance.origin_type is int:
         schema = JSONSchema(type=JSONSchemaInstanceType.INTEGER)
     elif instance.origin_type is float:
@@ -514,32 +555,32 @@
             args = [typing.Any, ...]  # type: ignore
         else:
             return JSONArraySchema(maxItems=0)
     elif len(args) == 1 and args[0] == ():
         if not PY_311_MIN:
             return JSONArraySchema(maxItems=0)
     if len(args) == 2 and args[1] is Ellipsis:
-        items_schema = _get_schema_or_none(instance.copy(type=args[0]), ctx)
+        items_schema = _get_schema_or_none(instance.derive(type=args[0]), ctx)
         return JSONArraySchema(items=items_schema)
     else:
         min_items: Optional[int] = 0
         max_items: Optional[int] = 0
         prefix_items = []
         items: Optional[JSONSchema] = None
         unpack_schema: Optional[JSONSchema] = None
         unpack_idx = 0
         for arg_idx, arg in enumerate(args, start=1):
             if not is_unpack(arg):
                 min_items += 1  # type: ignore
                 if not unpack_schema:
                     prefix_items.append(
-                        get_schema(instance.copy(type=arg), ctx)
+                        get_schema(instance.derive(type=arg), ctx)
                     )
             else:
-                unpack_schema = get_schema(instance.copy(type=arg), ctx)
+                unpack_schema = get_schema(instance.derive(type=arg), ctx)
                 unpack_idx = arg_idx
         if unpack_schema:
             prefix_items.extend(unpack_schema.prefixItems or [])
             min_items += unpack_schema.minItems or 0  # type: ignore
             max_items += unpack_schema.maxItems or 0  # type: ignore
             if unpack_idx == len(args):
                 items = unpack_schema.items
@@ -562,29 +603,33 @@
         k: resolved.get(v, v)
         for k, v in getattr(
             instance.origin_type, "__annotations__", {}
         ).items()
     }
     fields = getattr(instance.type, "_fields", ())
     defaults = getattr(instance.type, "_field_defaults", {})
-    as_dict = instance.get_config().namedtuple_as_dict
+    as_dict = instance.get_owner_config().namedtuple_as_dict
     serialize_option = instance.get_overridden_serialization_method()
     if serialize_option == "as_dict":
         as_dict = True
     elif serialize_option == "as_list":
         as_dict = False
     properties = {}
     for f_name in fields:
         f_type = annotations.get(f_name, typing.Any)
-        f_schema = get_schema(instance.copy(type=f_type), ctx)
+        f_schema = get_schema(instance.derive(type=f_type), ctx)
         f_default = defaults.get(f_name, MISSING)
         if f_default is not MISSING:
             if isinstance(f_schema, EmptyJSONSchema):
                 f_schema = JSONSchema()
-            f_schema.default = _default(f_type, f_default)  # type: ignore
+            f_schema.default = _default(
+                f_type,  # type: ignore[arg-type]
+                f_default,
+                instance.get_self_config(),
+            )
         properties[f_name] = f_schema
     if as_dict:
         return JSONObjectSchema(
             properties=properties or None,
             required=list(fields),
             additionalProperties=False,
         )
@@ -604,15 +649,15 @@
         k: resolved.get(v, v)
         for k, v in instance.origin_type.__annotations__.items()
     }
     all_keys = list(annotations.keys())
     required_keys = getattr(instance.type, "__required_keys__", all_keys)
     return JSONObjectSchema(
         properties={
-            key: get_schema(instance.copy(type=annotations[key]), ctx)
+            key: get_schema(instance.derive(type=annotations[key]), ctx)
             for key in all_keys
         }
         or None,
         required=sorted(required_keys) or None,
         additionalProperties=False,
     )
 
@@ -685,15 +730,15 @@
         return schema
     elif is_generic(instance.type) and issubclass(
         instance.origin_type, (List, typing.Deque)
     ):
         return apply_array_constraints(
             instance,
             JSONArraySchema(
-                items=_get_schema_or_none(instance.copy(type=args[0]), ctx)
+                items=_get_schema_or_none(instance.derive(type=args[0]), ctx)
                 if args
                 else None
             ),
         )
     elif issubclass(instance.origin_type, Tuple):  # type: ignore
         if is_named_tuple(instance.origin_type):
             return apply_array_constraints(
@@ -703,72 +748,74 @@
             return apply_array_constraints(instance, on_tuple(instance, ctx))
     elif is_generic(instance.type) and issubclass(
         instance.origin_type, (typing.FrozenSet, typing.AbstractSet)
     ):
         return apply_array_constraints(
             instance,
             JSONArraySchema(
-                items=_get_schema_or_none(instance.copy(type=args[0]), ctx)
+                items=_get_schema_or_none(instance.derive(type=args[0]), ctx)
                 if args
                 else None,
                 uniqueItems=True,
             ),
         )
     elif is_generic(instance.type) and issubclass(
         instance.origin_type, typing.ChainMap
     ):
         return apply_array_constraints(
             instance,
             JSONArraySchema(
                 items=get_schema(
-                    instance=instance.copy(
+                    instance=instance.derive(
                         type=(
                             Dict[args[0], args[1]]  # type: ignore
                             if args
                             else Dict
                         )
                     ),
                     ctx=ctx,
                 )
             ),
         )
     elif is_generic(instance.type) and issubclass(
         instance.origin_type, typing.Counter
     ):
         schema = JSONObjectSchema(
-            additionalProperties=get_schema(instance.copy(type=int), ctx),
+            additionalProperties=get_schema(instance.derive(type=int), ctx),
         )
         if args:
             schema.propertyNames = _get_schema_or_none(
-                instance.copy(type=args[0]), ctx
+                instance.derive(type=args[0]), ctx
             )
         return apply_object_constraints(instance, schema)
     elif is_typed_dict(instance.origin_type):
         return on_typed_dict(instance, ctx)
     elif is_generic(instance.type) and issubclass(
         instance.origin_type, typing.Mapping
     ):
         schema = JSONObjectSchema(
             additionalProperties=_get_schema_or_none(
-                instance.copy(type=args[1]), ctx
+                instance.derive(type=args[1]), ctx
             )
             if args
             else None,
-            propertyNames=_get_schema_or_none(instance.copy(type=args[0]), ctx)
+            propertyNames=_get_schema_or_none(
+                instance.derive(type=args[0]), ctx
+            )
             if args
             else None,
         )
         return apply_object_constraints(instance, schema)
     elif is_generic(instance.type) and issubclass(
         instance.origin_type, typing.Sequence
     ):
         return apply_array_constraints(
             instance,
             JSONArraySchema(
-                items=_get_schema_or_none(instance.copy(type=args[0]), ctx)
+                items=_get_schema_or_none(instance.derive(type=args[0]), ctx)
                 if args
                 else None
             ),
         )
 
 
 @register
```

### Comparing `mashumaro-3.9/mashumaro/mixins/dict.py` & `mashumaro-3.9.1/mashumaro/mixins/dict.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/mixins/json.py` & `mashumaro-3.9.1/mashumaro/mixins/json.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/mixins/msgpack.py` & `mashumaro-3.9.1/mashumaro/mixins/msgpack.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/mixins/orjson.py` & `mashumaro-3.9.1/mashumaro/mixins/orjson.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/mixins/orjson.pyi` & `mashumaro-3.9.1/mashumaro/mixins/orjson.pyi`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/mixins/toml.py` & `mashumaro-3.9.1/mashumaro/mixins/toml.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/mixins/yaml.py` & `mashumaro-3.9.1/mashumaro/mixins/yaml.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro/types.py` & `mashumaro-3.9.1/mashumaro/types.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/mashumaro.egg-info/PKG-INFO` & `mashumaro-3.9.1/mashumaro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mashumaro
-Version: 3.9
+Version: 3.9.1
 Summary: Fast serialization library on top of dataclasses
 Home-page: https://github.com/Fatal1ty/mashumaro
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mashumaro-3.9/mashumaro.egg-info/SOURCES.txt` & `mashumaro-3.9.1/mashumaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/pyproject.toml` & `mashumaro-3.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mashumaro-3.9/setup.py` & `mashumaro-3.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="mashumaro",
-    version="3.9",
+    version="3.9.1",
     description="Fast serialization library on top of dataclasses",
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     platforms="all",
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Intended Audience :: Developers",
```

