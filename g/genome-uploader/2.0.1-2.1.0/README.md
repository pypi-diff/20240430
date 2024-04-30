# Comparing `tmp/genome_uploader-2.0.1.tar.gz` & `tmp/genome_uploader-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genome_uploader-2.0.1.tar", last modified: Mon Apr 29 14:21:00 2024, max compression
+gzip compressed data, was "genome_uploader-2.1.0.tar", last modified: Tue Apr 30 15:35:44 2024, max compression
```

## Comparing `genome_uploader-2.0.1.tar` & `genome_uploader-2.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:21:00.408441 genome_uploader-2.0.1/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11342 2024-04-29 14:20:56.000000 genome_uploader-2.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-29 14:21:00.408441 genome_uploader-2.0.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     7538 2024-04-29 14:20:56.000000 genome_uploader-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:21:00.408441 genome_uploader-2.0.1/genome_uploader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-29 14:21:00.000000 genome_uploader-2.0.1/genome_uploader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-29 14:21:00.000000 genome_uploader-2.0.1/genome_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:21:00.000000 genome_uploader-2.0.1/genome_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-29 14:21:00.000000 genome_uploader-2.0.1/genome_uploader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-29 14:21:00.000000 genome_uploader-2.0.1/genome_uploader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 14:21:00.000000 genome_uploader-2.0.1/genome_uploader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:21:00.408441 genome_uploader-2.0.1/genomeuploader/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 14:20:56.000000 genome_uploader-2.0.1/genomeuploader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15283 2024-04-29 14:20:56.000000 genome_uploader-2.0.1/genomeuploader/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    10563 2024-04-29 14:20:56.000000 genome_uploader-2.0.1/genomeuploader/ena.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    39568 2024-04-29 14:20:56.000000 genome_uploader-2.0.1/genomeuploader/genome_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-29 14:20:56.000000 genome_uploader-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:21:00.408441 genome_uploader-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:21:00.408441 genome_uploader-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-29 14:20:56.000000 genome_uploader-2.0.1/tests/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:35:44.607146 genome_uploader-2.1.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11342 2024-04-30 15:35:40.000000 genome_uploader-2.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-04-30 15:35:44.607146 genome_uploader-2.1.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7538 2024-04-30 15:35:40.000000 genome_uploader-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:35:44.603146 genome_uploader-2.1.0/genome_uploader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-04-30 15:35:44.000000 genome_uploader-2.1.0/genome_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-30 15:35:44.000000 genome_uploader-2.1.0/genome_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:35:44.000000 genome_uploader-2.1.0/genome_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 15:35:44.000000 genome_uploader-2.1.0/genome_uploader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-30 15:35:44.000000 genome_uploader-2.1.0/genome_uploader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-30 15:35:44.000000 genome_uploader-2.1.0/genome_uploader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:35:44.603146 genome_uploader-2.1.0/genomeuploader/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 15:35:40.000000 genome_uploader-2.1.0/genomeuploader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15283 2024-04-30 15:35:40.000000 genome_uploader-2.1.0/genomeuploader/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10563 2024-04-30 15:35:40.000000 genome_uploader-2.1.0/genomeuploader/ena.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    39568 2024-04-30 15:35:40.000000 genome_uploader-2.1.0/genomeuploader/genome_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-30 15:35:40.000000 genome_uploader-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:35:44.607146 genome_uploader-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:35:44.603146 genome_uploader-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-30 15:35:40.000000 genome_uploader-2.1.0/tests/test_dummy.py
```

### Comparing `genome_uploader-2.0.1/LICENSE.md` & `genome_uploader-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `genome_uploader-2.0.1/PKG-INFO` & `genome_uploader-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genome_uploader
-Version: 2.0.1
+Version: 2.1.0
 Summary: Python script to upload bins and MAGs in fasta format to ENA (European Nucleotide Archive). This script generates xmls and manifests necessary for submission with webin-cli.
 Author-email: MGnify team <metagenomics-help@ebi.ac.uk>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://github.com/EBI-Metagenomics/genome_uploader
 Project-URL: Issues, https://github.com/EBI-Metagenomics/genome_uploader/issues
 Keywords: bioinformatics,tool,metagenomics
 Classifier: Programming Language :: Python :: 3.8
@@ -24,15 +24,17 @@
 Provides-Extra: dev
 Requires-Dist: pre-commit==3.3.3; extra == "dev"
 Requires-Dist: black==23.7.0; extra == "dev"
 Requires-Dist: ruff==v0.0.286; extra == "dev"
 Requires-Dist: isort==5.12.0; extra == "dev"
 Requires-Dist: bump-my-version==0.9.2; extra == "dev"
 Provides-Extra: test
-Requires-Dist: pytest==7.1.2; extra == "test"
+Requires-Dist: pytest==7.4.0; extra == "test"
+Requires-Dist: pytest-md==0.2.0; extra == "test"
+Requires-Dist: pytest-workflow==2.0.1; extra == "test"
 Requires-Dist: pytest-cov==3.0.0; extra == "test"
 
 # Public bins and MAGs uploader
 Python script to upload bins and MAGs in fasta format to ENA (European Nucleotide Archive). This script generates xmls and manifests necessary for submission with webin-cli. 
 
 It takes as input one tsv (tab-separated values) table in the following format:
```

### Comparing `genome_uploader-2.0.1/README.md` & `genome_uploader-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `genome_uploader-2.0.1/genome_uploader.egg-info/PKG-INFO` & `genome_uploader-2.1.0/genome_uploader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genome_uploader
-Version: 2.0.1
+Version: 2.1.0
 Summary: Python script to upload bins and MAGs in fasta format to ENA (European Nucleotide Archive). This script generates xmls and manifests necessary for submission with webin-cli.
 Author-email: MGnify team <metagenomics-help@ebi.ac.uk>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://github.com/EBI-Metagenomics/genome_uploader
 Project-URL: Issues, https://github.com/EBI-Metagenomics/genome_uploader/issues
 Keywords: bioinformatics,tool,metagenomics
 Classifier: Programming Language :: Python :: 3.8
@@ -24,15 +24,17 @@
 Provides-Extra: dev
 Requires-Dist: pre-commit==3.3.3; extra == "dev"
 Requires-Dist: black==23.7.0; extra == "dev"
 Requires-Dist: ruff==v0.0.286; extra == "dev"
 Requires-Dist: isort==5.12.0; extra == "dev"
 Requires-Dist: bump-my-version==0.9.2; extra == "dev"
 Provides-Extra: test
-Requires-Dist: pytest==7.1.2; extra == "test"
+Requires-Dist: pytest==7.4.0; extra == "test"
+Requires-Dist: pytest-md==0.2.0; extra == "test"
+Requires-Dist: pytest-workflow==2.0.1; extra == "test"
 Requires-Dist: pytest-cov==3.0.0; extra == "test"
 
 # Public bins and MAGs uploader
 Python script to upload bins and MAGs in fasta format to ENA (European Nucleotide Archive). This script generates xmls and manifests necessary for submission with webin-cli. 
 
 It takes as input one tsv (tab-separated values) table in the following format:
```

### Comparing `genome_uploader-2.0.1/genomeuploader/constants.py` & `genome_uploader-2.1.0/genomeuploader/constants.py`

 * *Files identical despite different names*

### Comparing `genome_uploader-2.0.1/genomeuploader/ena.py` & `genome_uploader-2.1.0/genomeuploader/ena.py`

 * *Files identical despite different names*

### Comparing `genome_uploader-2.0.1/genomeuploader/genome_upload.py` & `genome_uploader-2.1.0/genomeuploader/genome_upload.py`

 * *Files identical despite different names*

### Comparing `genome_uploader-2.0.1/pyproject.toml` & `genome_uploader-2.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "genome_uploader"
-version = "2.0.1"
+version = "2.1.0"
 readme = "README.md"
 authors = [
   {name = "MGnify team", email = "metagenomics-help@ebi.ac.uk"},
 ]
 license = {text = "Apache Software License 2.0"}
 keywords = ["bioinformatics", "tool", "metagenomics"]
 description = "Python script to upload bins and MAGs in fasta format to ENA (European Nucleotide Archive). This script generates xmls and manifests necessary for submission with webin-cli."
@@ -43,15 +43,17 @@
     "pre-commit==3.3.3",
     "black==23.7.0",
     "ruff==v0.0.286",
     "isort==5.12.0",
     "bump-my-version==0.9.2",
 ]
 test = [
-    "pytest==7.1.2",
+    "pytest==7.4.0",
+    "pytest-md==0.2.0",
+    "pytest-workflow==2.0.1",
     "pytest-cov==3.0.0",
 ]
 
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
```

