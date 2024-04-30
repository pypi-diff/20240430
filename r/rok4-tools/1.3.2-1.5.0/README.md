# Comparing `tmp/rok4-tools-1.3.2.tar.gz` & `tmp/rok4_tools-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rok4-tools-1.3.2.tar", last modified: Wed Jan 31 15:49:09 2024, max compression
+gzip compressed data, was "rok4_tools-1.5.0.tar", last modified: Tue Apr 30 07:30:03 2024, max compression
```

## Comparing `rok4-tools-1.3.2.tar` & `rok4_tools-1.5.0.tar`

### file list

```diff
@@ -1,42 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 15:49:09.649440 rok4-tools-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    21863 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    31230 2024-01-31 15:49:09.649440 rok4-tools-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/README.pypi.md
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-01-31 15:48:40.000000 rok4-tools-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 15:49:09.649440 rok4-tools-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 15:49:09.645440 rok4-tools-1.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 15:49:09.645440 rok4-tools-1.3.2/src/rok4_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-31 15:48:40.000000 rok4-tools-1.3.2/src/rok4_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 15:49:09.645440 rok4-tools-1.3.2/src/rok4_tools/global_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     6636 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/src/rok4_tools/global_utils/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/src/rok4_tools/joincache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 15:49:09.645440 rok4-tools-1.3.2/src/rok4_tools/joincache_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     9868 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/src/rok4_tools/joincache_utils/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/src/rok4_tools/joincache_utils/example.json
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/src/rok4_tools/joincache_utils/finisher.py
--rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/src/rok4_tools/joincache_utils/master.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/src/rok4_tools/joincache_utils/schema.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     3941 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/src/rok4_tools/make_layer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5728 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/src/rok4_tools/pyr2pyr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 15:49:09.649440 rok4-tools-1.3.2/src/rok4_tools/pyr2pyr_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/src/rok4_tools/pyr2pyr_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/src/rok4_tools/pyr2pyr_utils/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/src/rok4_tools/pyr2pyr_utils/example.json
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/src/rok4_tools/pyr2pyr_utils/finisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/src/rok4_tools/pyr2pyr_utils/master.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/src/rok4_tools/pyr2pyr_utils/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 15:49:09.649440 rok4-tools-1.3.2/src/rok4_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    31230 2024-01-31 15:49:09.000000 rok4-tools-1.3.2/src/rok4_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-01-31 15:49:09.000000 rok4-tools-1.3.2/src/rok4_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 15:49:09.000000 rok4-tools-1.3.2/src/rok4_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-31 15:49:09.000000 rok4-tools-1.3.2/src/rok4_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-01-31 15:49:09.000000 rok4-tools-1.3.2/src/rok4_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-31 15:49:09.000000 rok4-tools-1.3.2/src/rok4_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 15:49:09.649440 rok4-tools-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/tests/test_joincache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/tests/test_joincache_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/tests/test_joincache_finisher.py
--rw-r--r--   0 runner    (1001) docker     (127)    11798 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/tests/test_joincache_master.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-01-31 15:48:16.000000 rok4-tools-1.3.2/tests/test_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:30:03.830950 rok4_tools-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    21863 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    39278 2024-04-30 07:30:03.830950 rok4_tools-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15015 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/README.pypi.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-30 07:29:43.000000 rok4_tools-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 07:30:03.830950 rok4_tools-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:30:03.822950 rok4_tools-1.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:30:03.822950 rok4_tools-1.5.0/src/rok4_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 07:29:43.000000 rok4_tools-1.5.0/src/rok4_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:30:03.822950 rok4_tools-1.5.0/src/rok4_tools/global_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     6636 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/global_utils/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/joincache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:30:03.826950 rok4_tools-1.5.0/src/rok4_tools/joincache_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     9868 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/joincache_utils/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/joincache_utils/example.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/joincache_utils/finisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/joincache_utils/master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/joincache_utils/schema.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3941 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/make_layer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5830 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/pyr2pyr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:30:03.826950 rok4_tools-1.5.0/src/rok4_tools/pyr2pyr_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/pyr2pyr_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/pyr2pyr_utils/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/pyr2pyr_utils/example.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/pyr2pyr_utils/finisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/pyr2pyr_utils/master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/pyr2pyr_utils/schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/pyrolyse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/tmsizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:30:03.822950 rok4_tools-1.5.0/src/rok4_tools/tmsizer_utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:30:03.826950 rok4_tools-1.5.0/src/rok4_tools/tmsizer_utils/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/tmsizer_utils/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8429 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/tmsizer_utils/processors/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13862 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/tmsizer_utils/processors/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/tmsizer_utils/processors/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/src/rok4_tools/tmsizer_utils/processors/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:30:03.826950 rok4_tools-1.5.0/src/rok4_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    39278 2024-04-30 07:30:03.000000 rok4_tools-1.5.0/src/rok4_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-30 07:30:03.000000 rok4_tools-1.5.0/src/rok4_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 07:30:03.000000 rok4_tools-1.5.0/src/rok4_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-30 07:30:03.000000 rok4_tools-1.5.0/src/rok4_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-30 07:30:03.000000 rok4_tools-1.5.0/src/rok4_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 07:30:03.000000 rok4_tools-1.5.0/src/rok4_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:30:03.826950 rok4_tools-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/tests/test_joincache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/tests/test_joincache_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/tests/test_joincache_finisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/tests/test_joincache_master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/tests/test_processors_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/tests/test_processors_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/tests/test_processors_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-30 07:29:21.000000 rok4_tools-1.5.0/tests/test_source.py
```

### Comparing `rok4-tools-1.3.2/LICENSE.txt` & `rok4_tools-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rok4-tools-1.3.2/PKG-INFO` & `rok4_tools-1.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rok4-tools
-Version: 1.3.2
+Version: 1.5.0
 Summary: Python tools for ROK4 project
 Author-email: Géoportail Developer <tout_rdev@ign.fr>
 License: 
         CeCILL-C FREE SOFTWARE LICENSE AGREEMENT
         
         
             Notice
@@ -535,15 +535,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: jsonschema
-Requires-Dist: rok4<3.0.0,>=2.1.0
+Requires-Dist: tqdm
+Requires-Dist: rasterio
+Requires-Dist: rok4<3.0.0,>=2.1.5
 Provides-Extra: doc
 Requires-Dist: pdoc3>=0.10.0; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort>=5.12.0; extra == "dev"
 Requires-Dist: pre-commit<4,>3; extra == "dev"
 Requires-Dist: ruff>=0.0.281; extra == "dev"
@@ -556,27 +558,29 @@
 ![ROK4 Logo](https://rok4.github.io/assets/images/rok4.png)
 
 The `rok4-tools` package help to use [ROK4 project](https://rok4.github.io/) concepts, like Tile Matrix Sets, data pyramids or layers.
 
 ## Installation
 
 Required system packages :
+
 * debian : `apt install python3-rados python3-gdal`
 
 The `rok4` package is available on :
+
 * [PyPI](https://pypi.org/project/rok4/) : `pip install rok4`
 * [GitHub](https://github.com/rok4/core-python/releases/) : `pip install https://github.com/rok4/core-python/releases/download/<version>/rok4-<version>-py3-none-any.whl`
 
 ## Tools
 
 ### PYR2PYR
 
 PYR2PYR allow to copy a pyramid from a storage to another one. It is possible to ignore slab under a provided size. Copy is parallelized. If MD5 hash are in the pyramid's list file, they are used to check integrity after copy.
 
-To obtain an example of JSON configuration, call `pyr2pyr --role example`. To check a JSON configuration, call `pyr2pyr --role check --conf conf.json`. JSON configuratio can be a file or a S3 object(use a path's prefix, for example : `s3://bucket/configuration.json`)
+To obtain an example of JSON configuration, call `pyr2pyr --role example`. To check a JSON configuration, call `pyr2pyr --role check --conf conf.json`. JSON configuration can be a file or a S3 object(use a path's prefix, for example : `s3://bucket/configuration.json`)
 
 #### Usage
 
 A full copy requires the tool call with the three modes (all need the JSON configuration), in this order :
 
 1. `master` role
     * Actions : write N TODO lists, in a file or s3 directory.
@@ -584,20 +588,18 @@
 2. `agent` role :
     * Actions : read the TODO list from the work directory and copy slabs
     * Call (one by TODO list) : `pyr2pyr --role agent --conf conf.json --split X`
 3. `finisher` role:
     * Actions : read all TODO lists and write the output pyramid's list file and its descriptor
     * Call : `pyr2pyr --role finisher --conf conf.json`
 
-![PYR2PYR workflow](https://rok4.github.io/pytools/versions/latest/docs/images/pyr2pyr.png)
+![PYR2PYR workflow](https://rok4.github.io/pytools/latest/images/pyr2pyr.png)
 
 #### Configuration
 
-JSON configuration content (generated from the JSON schema with `jsonschema2md bin/pyr2pyr.schema.json /dev/stdout`)
-
 - **`logger`** *(object)*: Logger configuration.
     - **`layout`** *(string)*: Log format, according to logging python library. Default: `%(asctime)s %(levelname)s: %(message)s`.
     - **`file`** *(string)*: Path to log file. Standard output is used if not provided.
     - **`level`** *(string)*: Log level. Must be one of: `['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL', 'NOTSET']`. Default: `WARNING`.
 - **`from`** *(object)*: Pyramid to copy.
     - **`descriptor`** *(string)*: Path to pyramid's descriptor to copy.
 - **`to`** *(object)*: Pyramid to write.
@@ -608,15 +610,118 @@
         - **`depth`** *(integer)*: Tree depth, only for FILE storage. Minimum: `1`. Default: `2`.
 - **`process`** *(object)*: Processing parameters.
     - **`directory`** *(string)*: Directory to write copies to process, FILE directory or S3/CEPH prefix.
     - **`parallelization`** *(integer)*: Parallelization level, number of todo lists and agents working at the same time. Minimum: `1`. Default: `1`.
     - **`follow_links`** *(boolean)*: Do we follow links (data slabs in others pyramids than the 'from' one). Default: `False`.
     - **`slab_limit`** *(integer)*: Minimum slab size (if under, we do not copy). Minimum: `0`. Default: `0`.
 
+### JOINCACHE
+
+JOINCACHE build a raster pyramid from consistent pyramids (same TMS, same slab size, same bands format). Source pyramids are provided per levels.
+
+To obtain an example of JSON configuration, call `joincache --role example`. To check a JSON configuration, call `joincache --role check --conf conf.json`. JSON configuration can be a file or a S3 object(use a path's prefix, for example : `s3://bucket/configuration.json`)
+
+#### Usage
+
+A full build requires the tool call with the three modes (all need the JSON configuration), in this order :
+
+1. `master` role
+    * Actions : write N TODO lists, in a file or s3 directory.
+    * Call : `joincache --role master --conf conf.json`
+2. `agent` role :
+    * Actions : read the TODO list from the work directory and build or link slabs
+    * Call (one by TODO list) : `joincache --role agent --conf conf.json --split X`
+3. `finisher` role:
+    * Actions : read all TODO lists and write the output pyramid's list file and its descriptor
+    * Call : `joincache --role finisher --conf conf.json`
+
+#### Configuration
+
+- **`logger`** *(object)*: Paramètres du logger. Cannot contain additional properties.
+  - **`layout`** *(string)*: Log format, according to logging python library. Default: `"%(asctime)s %(levelname)s: %(message)s"`.
+  - **`file`** *(string)*: Path to log file. Standard output is used if not provided.
+  - **`level`** *(string)*: Log level. Must be one of: `["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL", "NOTSET"]`. Default: `"WARNING"`.
+- **`datasources`** *(array)*: Source pyramids.
+  - **Items** *(object)*: Cannot contain additional properties.
+    - **`bottom`** *(string, required)*: Bottom level's usage for source pyramids.
+    - **`top`** *(string, required)*: Top level's usage for source pyramids.
+    - **`source`** *(object, required)*: Pyramids as data source. Cannot contain additional properties.
+      - **`type`** *(string, required)*: Source type. Must be one of: `["PYRAMIDS"]`.
+      - **`descriptors`** *(array, required)*: Paths to pyramids' descriptors (all with the same characteritics : TMS, formats...). Length must be at least 1.
+        - **Items** *(string)*
+- **`pyramid`** *(object)*: Output pyramid's storage informations. Cannot contain additional properties.
+  - **`name`** *(string, required)*: Output pyramid's name.
+  - **`root`** *(string, required)*: Storage root : a directory for FILE storage, pool name for CEPH storage, bucket name for S3 storage.
+  - **`mask`** *(boolean)*: Mask export ? If true, masks are used for processing. Default: `false`.
+- **`process`** *(object)*: Processing parameters. Cannot contain additional properties.
+  - **`directory`** *(string, required)*: Directory to write copies to process, FILE directory or S3/CEPH prefix.
+  - **`parallelization`** *(integer)*: Parallelization level, number of todo lists and agents working at the same time. Minimum: `1`. Default: `1`.
+  - **`mask`** *(boolean)*: Source masks used for processing ? Default: `false`.
+  - **`only_links`** *(boolean)*: Only links are made ? If true, only top slab will be considered and linked. Default: `false`.
 
 ### MAKE-LAYER
 
 MAKE-LAYER generate a layer's descriptor, [ROK4 server](https://github.com/rok4/server/) compliant, from pyramids' descriptors
 
 #### Usage
 
-`make-layer [-h] --pyramids storage://path/to/pyr.json[>BOTTOM>TOP] [storage://path/to/pyr.json[>BOTTOM>TOP] ...] --name my data [--styles normal [normal ...]] [--title my data]`
+`make-layer [-h] [--version] --pyramids storage://path/to/pyr.json[>BOTTOM>TOP] [storage://path/to/pyr.json[>BOTTOM>TOP] ...] --name my_data [--styles normal [normal ...]] [--title my data] [--abstract my data description] [--resampling {nn,linear,bicubic,lanczos_2,lanczos_3,lanczos_4}] [--directory s3://layers_bucket]`
+
+* `-h, --help` : show this help message and exit
+* `--version` : show program's version number and exit
+* `--pyramids storage://path/to/pyr.json[>BOTTOM>TOP] [storage://path/to/pyr.json[>BOTTOM>TOP] ...]` : Pyramids' descriptors, with extrem levels to use if not all levels have to be used
+* `--name my_data` : Layer's technical name
+* `--styles normal [normal ...]` : Styles ID available for the layer (no controls, ID are added as provided)
+* `--title my data` : Layer title
+* `--abstract "my data description"` : Layer description
+* `--resampling {nn,linear,bicubic,lanczos_2,lanczos_3,lanczos_4}` : Layer resampling
+* `--directory s3://layers_bucket` : Directory (file or object) where to write layer's descriptor. Print in standard output if not provided
+
+### PYROLYSE
+
+PYROLYSE analyse a pyramid, to get slab/tile size and count, for the entire pyramide and per level. Slab and tile sizes are not all processed : a ratio limits the number of measures. This ratio is assumed for a level (to avoid to have mainly data for the best level). If tile statistics is enabled, access time are compiled.
+
+For size and access time, it's possible to get deciles and not all values.
+
+#### Usage
+
+`pyrolyse [-h] [--version] --pyramid storage://path/to/pyr.json [--json storage://path/to/conf.json] [--tiles] [--progress] [--deciles] [--ratio N]`
+
+* `-h, --help` : show this help message and exit
+* `--version` : show program's version number and exit
+* `--pyramid storage://path/to/pyr.json` : pyramid's descriptor, to analyse
+* `--output storage://path/to/conf.json` : file/object to write results. Print in standard output if not provided
+* `--tiles` : get size analysis for tiles
+* `--progress` : Print a progress bar (only with --output option)
+* `--deciles` : get deciles for sizes and read times rather than values
+* `--ratio N` : ratio of measured slabs and tiles (<ratio> choose one). All slabs are counted
+
+### TMSIZER
+
+TMSIZER converts data according to a pivot Tile Matrix Set. Input data can be read from a file, an object or standard input. The output data can be write to a file, an object or standard output. Several input and output formats are allowed.
+
+#### Usage
+
+`tmsizer [-h] [--version] --tms <TMS identifier> [-i storage://path/to/data] -if <format> [-io <KEY>:<VALUE> [<KEY>:<VALUE> ...]] [-o storage://path/to/results] -of <format> [-oo <KEY>:<VALUE> [<KEY>:<VALUE> ...]] [--progress]`
+
+* `-h, --help` : show this help message and exit
+* `--version` : show program's version number and exit
+* `--tms <TMS identifier>` : tile matrix set identifier
+* `-if <format>, --input-format <format>` : input format
+* `-of <format>, --output-format <format>` : output format
+* `-i storage://path/to/data, --input storage://path/to/data` : file/object to read data. Read from standard input if not provided
+* `-o storage://path/to/results, --output storage://path/to/results` : file/object to write results. Print in standard output if not provided
+* `-oo <KEY>:<VALUE> [<KEY>:<VALUE> ...], --output-option <KEY>:<VALUE> [<KEY>:<VALUE> ...]` : options for output
+* `-io <KEY>:<VALUE> [<KEY>:<VALUE> ...], --input-option <KEY>:<VALUE> [<KEY>:<VALUE> ...]` : options for input
+* `--progress` : print a progress bar (only with --output option)
+
+Availables conversions (mandatory options in bold, optionnal options in italic) :
+
+| Input format   | Input options                                     | Output format  | Output options                                                            | Description                                                                                          |
+|----------------|---------------------------------------------------|----------------|---------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|
+| GETTILE_PARAMS | *`level=<id>`*                                    | COUNT          |                                                                           | Count the GetTiles requests using the pivot TMS and optionnally the provided level                   |
+| GETTILE_PARAMS | *`level=<id>`*                                    | HEATMAP        | **`bbox=<xmin>,<ymin>,<xmax>,<ymax>`**, **`dimensions=<width>x<height>`** | Create an heat map of requested tiles on the provided area, optionnaly filtering with provided level |
+| GEOMETRY       | **`format=<WKT\|GeoJSON\|WKB>`**,**`level=<id>`** | GETTILE_PARAMS |                                                                           | Generate GetTile query parameters for tiles intersecting input geometries for the provided level     |
+
+Example (GETTILE_PARAMS -> HEATMAP) : 
+
+`tmsizer -i logs.txt --tms PM -io level=15 -if GETTILE_PARAMS -of HEATMAP -oo bbox=65000,6100000,665000,6500000 -oo dimensions=600x400 -o heatmap.tif`
```

### Comparing `rok4-tools-1.3.2/pyproject.toml` & `rok4_tools-1.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "rok4-tools"
-version = "1.3.2"
+version = "1.5.0"
 
 description = "Python tools for ROK4 project"
 readme = "README.pypi.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 
 keywords = ["ROK4", "tools", "data pyramids"]
@@ -28,15 +28,17 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3 :: Only",
 ]
 
 dependencies = [
   "jsonschema",
-  "rok4 >= 2.1.0, < 3.0.0"
+  "tqdm",
+  "rasterio",
+  "rok4 >= 2.1.5, < 3.0.0"
 ]
 
 [project.optional-dependencies]
 doc = [
   "pdoc3 >= 0.10.0"
 ]
 
@@ -58,14 +60,16 @@
 "Changelog" = "https://rok4.github.io/pytools/latest/CHANGELOG/"
 "Source" = "https://github.com/rok4/pytools"
 
 [project.scripts]
 pyr2pyr = "rok4_tools.pyr2pyr:main"
 make-layer = "rok4_tools.make_layer:main"
 joincache = "rok4_tools.joincache:main"
+pyrolyse = "rok4_tools.pyrolyse:main"
+tmsizer = "rok4_tools.tmsizer:main"
 
 [tool.setuptools.package-data]
 "rok4_tools.joincache_utils" = ["*.json"]
 "rok4_tools.pyr2pyr_utils" = ["*.json"]
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
```

### Comparing `rok4-tools-1.3.2/src/rok4_tools/global_utils/source.py` & `rok4_tools-1.5.0/src/rok4_tools/global_utils/source.py`

 * *Files identical despite different names*

### Comparing `rok4-tools-1.3.2/src/rok4_tools/joincache.py` & `rok4_tools-1.5.0/src/rok4_tools/joincache.py`

 * *Files identical despite different names*

### Comparing `rok4-tools-1.3.2/src/rok4_tools/joincache_utils/agent.py` & `rok4_tools-1.5.0/src/rok4_tools/joincache_utils/agent.py`

 * *Files identical despite different names*

### Comparing `rok4-tools-1.3.2/src/rok4_tools/joincache_utils/example.json` & `rok4_tools-1.5.0/src/rok4_tools/joincache_utils/example.json`

 * *Files identical despite different names*

### Comparing `rok4-tools-1.3.2/src/rok4_tools/joincache_utils/finisher.py` & `rok4_tools-1.5.0/src/rok4_tools/joincache_utils/finisher.py`

 * *Files identical despite different names*

### Comparing `rok4-tools-1.3.2/src/rok4_tools/joincache_utils/master.py` & `rok4_tools-1.5.0/src/rok4_tools/joincache_utils/master.py`

 * *Files identical despite different names*

### Comparing `rok4-tools-1.3.2/src/rok4_tools/joincache_utils/schema.json` & `rok4_tools-1.5.0/src/rok4_tools/joincache_utils/schema.json`

 * *Files identical despite different names*

### Comparing `rok4-tools-1.3.2/src/rok4_tools/make_layer.py` & `rok4_tools-1.5.0/src/rok4_tools/make_layer.py`

 * *Files identical despite different names*

### Comparing `rok4-tools-1.3.2/src/rok4_tools/pyr2pyr.py` & `rok4_tools-1.5.0/src/rok4_tools/pyr2pyr.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 def configuration() -> None:
     """Load configuration file
 
     Raises:
         JSONDecodeError: Configuration is not a valid JSON file
         ValidationError: Configuration is not a valid PYR2PYR configuration file
         MissingEnvironmentError: Missing object storage informations
-        storageError: storage read issue
+        StorageError: storage read issue
         FileNotFoundError: File or object does not exist
     """
 
     global config
 
     # Chargement du schéma JSON
     f = open(os.path.join(os.path.dirname(__file__), "pyr2pyr_utils", "schema.json"))
@@ -162,14 +162,18 @@
         logging.error(f"{args.configuration} is not a valid JSON file: {e}")
         sys.exit(1)
 
     except ValidationError as e:
         logging.error(f"{args.configuration} is not a valid configuration file: {e}")
         sys.exit(1)
 
+    except FileNotFoundError as e:
+        logging.error(f"{e} does not exists")
+        sys.exit(1)
+
     except Exception as e:
         logging.error(e)
         sys.exit(1)
 
     if args.role == "check":
         # On voulait juste valider le fichier de configuration, c'est chose faite
         # Si on est là c'est que tout est bon
```

### Comparing `rok4-tools-1.3.2/src/rok4_tools/pyr2pyr_utils/agent.py` & `rok4_tools-1.5.0/src/rok4_tools/pyr2pyr_utils/agent.py`

 * *Files identical despite different names*

### Comparing `rok4-tools-1.3.2/src/rok4_tools/pyr2pyr_utils/finisher.py` & `rok4_tools-1.5.0/src/rok4_tools/pyr2pyr_utils/finisher.py`

 * *Files identical despite different names*

### Comparing `rok4-tools-1.3.2/src/rok4_tools/pyr2pyr_utils/master.py` & `rok4_tools-1.5.0/src/rok4_tools/pyr2pyr_utils/master.py`

 * *Files identical despite different names*

### Comparing `rok4-tools-1.3.2/src/rok4_tools/pyr2pyr_utils/schema.json` & `rok4_tools-1.5.0/src/rok4_tools/pyr2pyr_utils/schema.json`

 * *Files identical despite different names*

### Comparing `rok4-tools-1.3.2/src/rok4_tools.egg-info/PKG-INFO` & `rok4_tools-1.5.0/src/rok4_tools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rok4-tools
-Version: 1.3.2
+Version: 1.5.0
 Summary: Python tools for ROK4 project
 Author-email: Géoportail Developer <tout_rdev@ign.fr>
 License: 
         CeCILL-C FREE SOFTWARE LICENSE AGREEMENT
         
         
             Notice
@@ -535,15 +535,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: jsonschema
-Requires-Dist: rok4<3.0.0,>=2.1.0
+Requires-Dist: tqdm
+Requires-Dist: rasterio
+Requires-Dist: rok4<3.0.0,>=2.1.5
 Provides-Extra: doc
 Requires-Dist: pdoc3>=0.10.0; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort>=5.12.0; extra == "dev"
 Requires-Dist: pre-commit<4,>3; extra == "dev"
 Requires-Dist: ruff>=0.0.281; extra == "dev"
@@ -556,27 +558,29 @@
 ![ROK4 Logo](https://rok4.github.io/assets/images/rok4.png)
 
 The `rok4-tools` package help to use [ROK4 project](https://rok4.github.io/) concepts, like Tile Matrix Sets, data pyramids or layers.
 
 ## Installation
 
 Required system packages :
+
 * debian : `apt install python3-rados python3-gdal`
 
 The `rok4` package is available on :
+
 * [PyPI](https://pypi.org/project/rok4/) : `pip install rok4`
 * [GitHub](https://github.com/rok4/core-python/releases/) : `pip install https://github.com/rok4/core-python/releases/download/<version>/rok4-<version>-py3-none-any.whl`
 
 ## Tools
 
 ### PYR2PYR
 
 PYR2PYR allow to copy a pyramid from a storage to another one. It is possible to ignore slab under a provided size. Copy is parallelized. If MD5 hash are in the pyramid's list file, they are used to check integrity after copy.
 
-To obtain an example of JSON configuration, call `pyr2pyr --role example`. To check a JSON configuration, call `pyr2pyr --role check --conf conf.json`. JSON configuratio can be a file or a S3 object(use a path's prefix, for example : `s3://bucket/configuration.json`)
+To obtain an example of JSON configuration, call `pyr2pyr --role example`. To check a JSON configuration, call `pyr2pyr --role check --conf conf.json`. JSON configuration can be a file or a S3 object(use a path's prefix, for example : `s3://bucket/configuration.json`)
 
 #### Usage
 
 A full copy requires the tool call with the three modes (all need the JSON configuration), in this order :
 
 1. `master` role
     * Actions : write N TODO lists, in a file or s3 directory.
@@ -584,20 +588,18 @@
 2. `agent` role :
     * Actions : read the TODO list from the work directory and copy slabs
     * Call (one by TODO list) : `pyr2pyr --role agent --conf conf.json --split X`
 3. `finisher` role:
     * Actions : read all TODO lists and write the output pyramid's list file and its descriptor
     * Call : `pyr2pyr --role finisher --conf conf.json`
 
-![PYR2PYR workflow](https://rok4.github.io/pytools/versions/latest/docs/images/pyr2pyr.png)
+![PYR2PYR workflow](https://rok4.github.io/pytools/latest/images/pyr2pyr.png)
 
 #### Configuration
 
-JSON configuration content (generated from the JSON schema with `jsonschema2md bin/pyr2pyr.schema.json /dev/stdout`)
-
 - **`logger`** *(object)*: Logger configuration.
     - **`layout`** *(string)*: Log format, according to logging python library. Default: `%(asctime)s %(levelname)s: %(message)s`.
     - **`file`** *(string)*: Path to log file. Standard output is used if not provided.
     - **`level`** *(string)*: Log level. Must be one of: `['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL', 'NOTSET']`. Default: `WARNING`.
 - **`from`** *(object)*: Pyramid to copy.
     - **`descriptor`** *(string)*: Path to pyramid's descriptor to copy.
 - **`to`** *(object)*: Pyramid to write.
@@ -608,15 +610,118 @@
         - **`depth`** *(integer)*: Tree depth, only for FILE storage. Minimum: `1`. Default: `2`.
 - **`process`** *(object)*: Processing parameters.
     - **`directory`** *(string)*: Directory to write copies to process, FILE directory or S3/CEPH prefix.
     - **`parallelization`** *(integer)*: Parallelization level, number of todo lists and agents working at the same time. Minimum: `1`. Default: `1`.
     - **`follow_links`** *(boolean)*: Do we follow links (data slabs in others pyramids than the 'from' one). Default: `False`.
     - **`slab_limit`** *(integer)*: Minimum slab size (if under, we do not copy). Minimum: `0`. Default: `0`.
 
+### JOINCACHE
+
+JOINCACHE build a raster pyramid from consistent pyramids (same TMS, same slab size, same bands format). Source pyramids are provided per levels.
+
+To obtain an example of JSON configuration, call `joincache --role example`. To check a JSON configuration, call `joincache --role check --conf conf.json`. JSON configuration can be a file or a S3 object(use a path's prefix, for example : `s3://bucket/configuration.json`)
+
+#### Usage
+
+A full build requires the tool call with the three modes (all need the JSON configuration), in this order :
+
+1. `master` role
+    * Actions : write N TODO lists, in a file or s3 directory.
+    * Call : `joincache --role master --conf conf.json`
+2. `agent` role :
+    * Actions : read the TODO list from the work directory and build or link slabs
+    * Call (one by TODO list) : `joincache --role agent --conf conf.json --split X`
+3. `finisher` role:
+    * Actions : read all TODO lists and write the output pyramid's list file and its descriptor
+    * Call : `joincache --role finisher --conf conf.json`
+
+#### Configuration
+
+- **`logger`** *(object)*: Paramètres du logger. Cannot contain additional properties.
+  - **`layout`** *(string)*: Log format, according to logging python library. Default: `"%(asctime)s %(levelname)s: %(message)s"`.
+  - **`file`** *(string)*: Path to log file. Standard output is used if not provided.
+  - **`level`** *(string)*: Log level. Must be one of: `["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL", "NOTSET"]`. Default: `"WARNING"`.
+- **`datasources`** *(array)*: Source pyramids.
+  - **Items** *(object)*: Cannot contain additional properties.
+    - **`bottom`** *(string, required)*: Bottom level's usage for source pyramids.
+    - **`top`** *(string, required)*: Top level's usage for source pyramids.
+    - **`source`** *(object, required)*: Pyramids as data source. Cannot contain additional properties.
+      - **`type`** *(string, required)*: Source type. Must be one of: `["PYRAMIDS"]`.
+      - **`descriptors`** *(array, required)*: Paths to pyramids' descriptors (all with the same characteritics : TMS, formats...). Length must be at least 1.
+        - **Items** *(string)*
+- **`pyramid`** *(object)*: Output pyramid's storage informations. Cannot contain additional properties.
+  - **`name`** *(string, required)*: Output pyramid's name.
+  - **`root`** *(string, required)*: Storage root : a directory for FILE storage, pool name for CEPH storage, bucket name for S3 storage.
+  - **`mask`** *(boolean)*: Mask export ? If true, masks are used for processing. Default: `false`.
+- **`process`** *(object)*: Processing parameters. Cannot contain additional properties.
+  - **`directory`** *(string, required)*: Directory to write copies to process, FILE directory or S3/CEPH prefix.
+  - **`parallelization`** *(integer)*: Parallelization level, number of todo lists and agents working at the same time. Minimum: `1`. Default: `1`.
+  - **`mask`** *(boolean)*: Source masks used for processing ? Default: `false`.
+  - **`only_links`** *(boolean)*: Only links are made ? If true, only top slab will be considered and linked. Default: `false`.
 
 ### MAKE-LAYER
 
 MAKE-LAYER generate a layer's descriptor, [ROK4 server](https://github.com/rok4/server/) compliant, from pyramids' descriptors
 
 #### Usage
 
-`make-layer [-h] --pyramids storage://path/to/pyr.json[>BOTTOM>TOP] [storage://path/to/pyr.json[>BOTTOM>TOP] ...] --name my data [--styles normal [normal ...]] [--title my data]`
+`make-layer [-h] [--version] --pyramids storage://path/to/pyr.json[>BOTTOM>TOP] [storage://path/to/pyr.json[>BOTTOM>TOP] ...] --name my_data [--styles normal [normal ...]] [--title my data] [--abstract my data description] [--resampling {nn,linear,bicubic,lanczos_2,lanczos_3,lanczos_4}] [--directory s3://layers_bucket]`
+
+* `-h, --help` : show this help message and exit
+* `--version` : show program's version number and exit
+* `--pyramids storage://path/to/pyr.json[>BOTTOM>TOP] [storage://path/to/pyr.json[>BOTTOM>TOP] ...]` : Pyramids' descriptors, with extrem levels to use if not all levels have to be used
+* `--name my_data` : Layer's technical name
+* `--styles normal [normal ...]` : Styles ID available for the layer (no controls, ID are added as provided)
+* `--title my data` : Layer title
+* `--abstract "my data description"` : Layer description
+* `--resampling {nn,linear,bicubic,lanczos_2,lanczos_3,lanczos_4}` : Layer resampling
+* `--directory s3://layers_bucket` : Directory (file or object) where to write layer's descriptor. Print in standard output if not provided
+
+### PYROLYSE
+
+PYROLYSE analyse a pyramid, to get slab/tile size and count, for the entire pyramide and per level. Slab and tile sizes are not all processed : a ratio limits the number of measures. This ratio is assumed for a level (to avoid to have mainly data for the best level). If tile statistics is enabled, access time are compiled.
+
+For size and access time, it's possible to get deciles and not all values.
+
+#### Usage
+
+`pyrolyse [-h] [--version] --pyramid storage://path/to/pyr.json [--json storage://path/to/conf.json] [--tiles] [--progress] [--deciles] [--ratio N]`
+
+* `-h, --help` : show this help message and exit
+* `--version` : show program's version number and exit
+* `--pyramid storage://path/to/pyr.json` : pyramid's descriptor, to analyse
+* `--output storage://path/to/conf.json` : file/object to write results. Print in standard output if not provided
+* `--tiles` : get size analysis for tiles
+* `--progress` : Print a progress bar (only with --output option)
+* `--deciles` : get deciles for sizes and read times rather than values
+* `--ratio N` : ratio of measured slabs and tiles (<ratio> choose one). All slabs are counted
+
+### TMSIZER
+
+TMSIZER converts data according to a pivot Tile Matrix Set. Input data can be read from a file, an object or standard input. The output data can be write to a file, an object or standard output. Several input and output formats are allowed.
+
+#### Usage
+
+`tmsizer [-h] [--version] --tms <TMS identifier> [-i storage://path/to/data] -if <format> [-io <KEY>:<VALUE> [<KEY>:<VALUE> ...]] [-o storage://path/to/results] -of <format> [-oo <KEY>:<VALUE> [<KEY>:<VALUE> ...]] [--progress]`
+
+* `-h, --help` : show this help message and exit
+* `--version` : show program's version number and exit
+* `--tms <TMS identifier>` : tile matrix set identifier
+* `-if <format>, --input-format <format>` : input format
+* `-of <format>, --output-format <format>` : output format
+* `-i storage://path/to/data, --input storage://path/to/data` : file/object to read data. Read from standard input if not provided
+* `-o storage://path/to/results, --output storage://path/to/results` : file/object to write results. Print in standard output if not provided
+* `-oo <KEY>:<VALUE> [<KEY>:<VALUE> ...], --output-option <KEY>:<VALUE> [<KEY>:<VALUE> ...]` : options for output
+* `-io <KEY>:<VALUE> [<KEY>:<VALUE> ...], --input-option <KEY>:<VALUE> [<KEY>:<VALUE> ...]` : options for input
+* `--progress` : print a progress bar (only with --output option)
+
+Availables conversions (mandatory options in bold, optionnal options in italic) :
+
+| Input format   | Input options                                     | Output format  | Output options                                                            | Description                                                                                          |
+|----------------|---------------------------------------------------|----------------|---------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|
+| GETTILE_PARAMS | *`level=<id>`*                                    | COUNT          |                                                                           | Count the GetTiles requests using the pivot TMS and optionnally the provided level                   |
+| GETTILE_PARAMS | *`level=<id>`*                                    | HEATMAP        | **`bbox=<xmin>,<ymin>,<xmax>,<ymax>`**, **`dimensions=<width>x<height>`** | Create an heat map of requested tiles on the provided area, optionnaly filtering with provided level |
+| GEOMETRY       | **`format=<WKT\|GeoJSON\|WKB>`**,**`level=<id>`** | GETTILE_PARAMS |                                                                           | Generate GetTile query parameters for tiles intersecting input geometries for the provided level     |
+
+Example (GETTILE_PARAMS -> HEATMAP) : 
+
+`tmsizer -i logs.txt --tms PM -io level=15 -if GETTILE_PARAMS -of HEATMAP -oo bbox=65000,6100000,665000,6500000 -oo dimensions=600x400 -o heatmap.tif`
```

### Comparing `rok4-tools-1.3.2/src/rok4_tools.egg-info/SOURCES.txt` & `rok4_tools-1.5.0/src/rok4_tools.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 README.pypi.md
 pyproject.toml
 setup.py
 src/rok4_tools/__init__.py
 src/rok4_tools/joincache.py
 src/rok4_tools/make_layer.py
 src/rok4_tools/pyr2pyr.py
+src/rok4_tools/pyrolyse.py
+src/rok4_tools/tmsizer.py
 src/rok4_tools.egg-info/PKG-INFO
 src/rok4_tools.egg-info/SOURCES.txt
 src/rok4_tools.egg-info/dependency_links.txt
 src/rok4_tools.egg-info/entry_points.txt
 src/rok4_tools.egg-info/requires.txt
 src/rok4_tools.egg-info/top_level.txt
 src/rok4_tools/global_utils/source.py
@@ -21,12 +23,20 @@
 src/rok4_tools/joincache_utils/schema.json
 src/rok4_tools/pyr2pyr_utils/__init__.py
 src/rok4_tools/pyr2pyr_utils/agent.py
 src/rok4_tools/pyr2pyr_utils/example.json
 src/rok4_tools/pyr2pyr_utils/finisher.py
 src/rok4_tools/pyr2pyr_utils/master.py
 src/rok4_tools/pyr2pyr_utils/schema.json
+src/rok4_tools/tmsizer_utils/processors/__init__.py
+src/rok4_tools/tmsizer_utils/processors/io.py
+src/rok4_tools/tmsizer_utils/processors/map.py
+src/rok4_tools/tmsizer_utils/processors/processor.py
+src/rok4_tools/tmsizer_utils/processors/reduce.py
 tests/test_joincache.py
 tests/test_joincache_agent.py
 tests/test_joincache_finisher.py
 tests/test_joincache_master.py
+tests/test_processors_io.py
+tests/test_processors_map.py
+tests/test_processors_reduce.py
 tests/test_source.py
```

### Comparing `rok4-tools-1.3.2/tests/test_joincache.py` & `rok4_tools-1.5.0/tests/test_joincache.py`

 * *Files identical despite different names*

### Comparing `rok4-tools-1.3.2/tests/test_joincache_agent.py` & `rok4_tools-1.5.0/tests/test_joincache_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,12 +30,12 @@
             {"bottom": "11", "top": "16", "source": {"descriptors": ["path2"]}},
         ],
         "pyramid": {"name": "joincache.png", "root": "bucket", "mask": True},
         "process": {
             "parallelization": 3,
             "mask": True,
             "only_links": False,
-            "directory": "tests/list_agent",
+            "directory": "tests/fixtures/list_agent",
         },
     }
     resultat = work(config, 1)
     mocked_from_descriptor.assert_called_once_with("path")
```

### Comparing `rok4-tools-1.3.2/tests/test_joincache_finisher.py` & `rok4_tools-1.5.0/tests/test_joincache_finisher.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from rok4_tools.joincache_utils.finisher import *
 
 
 @mock.patch("rok4_tools.joincache_utils.finisher.SourcePyramids")
 @mock.patch("rok4_tools.joincache_utils.finisher.Pyramid.from_other")
 @mock.patch("rok4_tools.joincache_utils.finisher.storage.copy")
 def test_ok(mocked_copy, mocked_from_other, mocked_source):
-    files = [f for f in os.listdir("tests/list_agent")]
+    files = [f for f in os.listdir("tests/fixtures/list_agent")]
     for file in files:
         print(file)
         shutil.copy2(
-            os.path.join("tests/list_agent", file), os.path.join("tests/list_finisher", file)
+            os.path.join("tests/fixtures/list_agent", file), os.path.join("tests/fixtures/list_finisher", file)
         )
     level6 = MagicMock()
     level6.id = "6"
     pyramid1 = MagicMock()
     pyramid1.storage_type = StorageType.S3
     pyramid1.get_levels.return_value = [level6]
     pyramid1.list_generator.return_value = [
@@ -95,15 +95,15 @@
             {"bottom": "11", "top": "16", "source": {"descriptors": ["path2"]}},
         ],
         "pyramid": {"name": "joincache.png", "root": "bucket", "mask": True},
         "process": {
             "parallelization": 3,
             "mask": True,
             "only_links": False,
-            "directory": "tests/list_finisher",
+            "directory": "tests/fixtures/list_finisher",
         },
     }
     storage_pyramid = {"type": StorageType.S3, "root": "bucket"}
 
     work(config)
     mocked_source.assert_has_calls([call("6", "10", ["path"]), call("11", "16", ["path2"])])
     mocked_from_other.assert_called_once_with(
```

### Comparing `rok4-tools-1.3.2/tests/test_joincache_master.py` & `rok4_tools-1.5.0/tests/test_joincache_master.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,17 +220,17 @@
         source1.pyramids[0], "joincache.png", storage_pyramid, mask="true"
     )
 
 
 @mock.patch("rok4_tools.joincache_utils.master.SourcePyramids")
 @mock.patch("rok4_tools.joincache_utils.master.Pyramid.from_other")
 def test_ok(mocked_from_other, mocked_source):
-    files = [f for f in os.listdir("tests/list_master")]
+    files = [f for f in os.listdir("tests/fixtures/list_master")]
     for file in files:
-        os.remove(os.path.join("tests/list_master", file))
+        os.remove(os.path.join("tests/fixtures/list_master", file))
     level6 = MagicMock()
     level6.id = "6"
     pyramid1 = MagicMock()
     pyramid1.storage_type = StorageType.S3
     pyramid1.get_levels.return_value = [level6]
     pyramid1.list_generator.return_value = [
         (
@@ -318,20 +318,20 @@
             {"bottom": "11", "top": "16", "source": {"descriptors": ["path2"]}},
         ],
         "pyramid": {"name": "joincache.png", "root": "bucket", "mask": True},
         "process": {
             "parallelization": 3,
             "mask": True,
             "only_links": False,
-            "directory": "tests/list_master",
+            "directory": "tests/fixtures/list_master",
         },
     }
 
     resultat = work(config)
-    with open("tests/list_master/todo.1.list") as f:
+    with open("tests/fixtures/list_master/todo.1.list") as f:
         lignes = f.read()
 
     assert (
         lignes
         == "c2w s3://path/DATA_6_1_1\nc2w s3://path/MASK_6_1_1\nc2w s3://path3/DATA_6_1_1\nc2w s3://path3/MASK_6_1_1\noNt\nw2c s3://path_final/DATA_6_1_1\nw2c s3://path_final/MASK_6_1_1\nlink s3://path_final/DATA_11_1_1 s3://path2/DATA_11_1_1 2\n"
     )
```

### Comparing `rok4-tools-1.3.2/tests/test_source.py` & `rok4_tools-1.5.0/tests/test_source.py`

 * *Files identical despite different names*

