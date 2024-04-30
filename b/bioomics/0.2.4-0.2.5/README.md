# Comparing `tmp/bioomics-0.2.4.tar.gz` & `tmp/bioomics-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioomics-0.2.4.tar", last modified: Fri Apr 26 20:07:24 2024, max compression
+gzip compressed data, was "bioomics-0.2.5.tar", last modified: Mon Apr 29 14:05:14 2024, max compression
```

## Comparing `bioomics-0.2.4.tar` & `bioomics-0.2.5.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.984609 bioomics-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 20:07:18.000000 bioomics-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-26 20:07:24.984609 bioomics-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-26 20:07:18.000000 bioomics-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 20:07:24.984609 bioomics-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-26 20:07:18.000000 bioomics-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.976609 bioomics-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.980609 bioomics-0.2.4/src/bioomics/
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.980609 bioomics-0.2.4/src/bioomics/connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/connector/conn_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/connector/conn_ftplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/connector/conn_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/connector/conn_redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.980609 bioomics-0.2.4/src/bioomics/constants/
--rw-r--r--   0 runner    (1001) docker     (127)    26628 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/constants/IEDB.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.980609 bioomics-0.2.4/src/bioomics/immune/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/immune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15672 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/immune/iedb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/immune/iedb_antigen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/immune/iedb_epitope.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/integrate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/mirbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/ncbi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.980609 bioomics-0.2.4/src/bioomics/protein/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/protein/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/protein/expasy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/protein/uniprot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/protein/uniprot_sprot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/protein/uniprot_trembl.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/bioomics/rnacentral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.984609 bioomics-0.2.4/src/bioomics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-26 20:07:24.000000 bioomics-0.2.4/src/bioomics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-26 20:07:24.000000 bioomics-0.2.4/src/bioomics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:07:24.000000 bioomics-0.2.4/src/bioomics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-26 20:07:24.000000 bioomics-0.2.4/src/bioomics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-26 20:07:24.000000 bioomics-0.2.4/src/bioomics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.984609 bioomics-0.2.4/src/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/pipelines/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-26 20:07:18.000000 bioomics-0.2.4/src/pipelines/retrieve_epitopes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:07:24.984609 bioomics-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_conn_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_conn_ftplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_conn_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_conn_redis.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_expasy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_iedb.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_iedb_antigen.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_iedb_epitope.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_mirbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_ncbi.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_rnacentral.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_uniprot.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_uniprot_sprot.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-26 20:07:18.000000 bioomics-0.2.4/tests/test_uniprot_trembl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.998437 bioomics-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 14:05:10.000000 bioomics-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-29 14:05:14.998437 bioomics-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-29 14:05:10.000000 bioomics-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:05:14.998437 bioomics-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-29 14:05:10.000000 bioomics-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.986437 bioomics-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.990437 bioomics-0.2.5/src/bioomics/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/bio_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.990437 bioomics-0.2.5/src/bioomics/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/connector/conn_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/connector/conn_ftplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/connector/conn_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/connector/conn_redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.990437 bioomics-0.2.5/src/bioomics/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)    26628 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/constants/IEDB.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.994437 bioomics-0.2.5/src/bioomics/immune/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/immune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15672 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/immune/iedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/immune/iedb_antigen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/immune/iedb_epitope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/integrate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/mirbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/ncbi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.994437 bioomics-0.2.5/src/bioomics/protein/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/protein/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/protein/expasy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/protein/uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/protein/uniprot_sprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/protein/uniprot_trembl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/rnacentral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.994437 bioomics-0.2.5/src/bioomics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-29 14:05:14.000000 bioomics-0.2.5/src/bioomics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-29 14:05:14.000000 bioomics-0.2.5/src/bioomics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:05:14.000000 bioomics-0.2.5/src/bioomics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-29 14:05:14.000000 bioomics-0.2.5/src/bioomics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 14:05:14.000000 bioomics-0.2.5/src/bioomics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.994437 bioomics-0.2.5/src/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/pipelines/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/pipelines/retrieve_epitopes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.994437 bioomics-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_conn_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_conn_ftplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_conn_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_conn_redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_expasy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_iedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_iedb_antigen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_iedb_epitope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_mirbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_rnacentral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_uniprot_sprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_uniprot_trembl.py
```

### Comparing `bioomics-0.2.4/LICENSE` & `bioomics-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/PKG-INFO` & `bioomics-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioomics
-Version: 0.2.4
+Version: 0.2.5
 Summary: Download, retrieve and process omics data for further bioinformatics
 Home-page: https://github.com/Tiezhengyuan/bio_omics
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -46,18 +46,19 @@
 - The key-value is defined by this corresponding database source.
 - Used for Integration rather than enrichment. Therefore, data combination or aggregation is not recommended.
 - Data from various source could be different or invalid. Those would be validated in the afterwards step rather than this step.
 ```
 {
     "ID": "79541",
     "key": "H0YED9",
-    "Uni-Prot": {
+    "UniProt_SwissProt": {
         ....
     },
     "NCBI": {
         ....
     },
     "PDB": {
         ....
     },
+    ....    
 }
 ```
```

### Comparing `bioomics-0.2.4/README.md` & `bioomics-0.2.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,18 +24,19 @@
 - The key-value is defined by this corresponding database source.
 - Used for Integration rather than enrichment. Therefore, data combination or aggregation is not recommended.
 - Data from various source could be different or invalid. Those would be validated in the afterwards step rather than this step.
 ```
 {
     "ID": "79541",
     "key": "H0YED9",
-    "Uni-Prot": {
+    "UniProt_SwissProt": {
         ....
     },
     "NCBI": {
         ....
     },
     "PDB": {
         ....
     },
+    ....    
 }
 ```
```

### Comparing `bioomics-0.2.4/setup.py` & `bioomics-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="bioomics",
-    version='0.2.4',
+    version='0.2.5',
     author="Tiezheng Yuan",
     author_email="tiezhengyuan@hotmail.com",
     description="Download, retrieve and process omics data for further bioinformatics",
     url = "https://github.com/Tiezhengyuan/bio_omics",
     long_description_content_type="text/markdown",
     long_description=long_description,
     package_dir={"": "src"},
```

### Comparing `bioomics-0.2.4/src/bioomics/__init__.py` & `bioomics-0.2.5/src/bioomics/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # 
 from .integrate_data import IntegrateData
+from .bio_dict import BioDict
 
 # connector
 from .connector.conn_http import ConnHTTP
 from .connector.conn_ftp import ConnFTP
 from .connector.conn_ftplib import ConnFTPlib
 from .connector.conn_redis import ConnRedis
```

### Comparing `bioomics-0.2.4/src/bioomics/connector/conn_ftp.py` & `bioomics-0.2.5/src/bioomics/connector/conn_ftp.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/src/bioomics/connector/conn_ftplib.py` & `bioomics-0.2.5/src/bioomics/connector/conn_ftplib.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/src/bioomics/connector/conn_http.py` & `bioomics-0.2.5/src/bioomics/connector/conn_http.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/src/bioomics/connector/conn_redis.py` & `bioomics-0.2.5/src/bioomics/connector/conn_redis.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/src/bioomics/constants/IEDB.py` & `bioomics-0.2.5/src/bioomics/constants/IEDB.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/src/bioomics/immune/iedb.py` & `bioomics-0.2.5/src/bioomics/immune/iedb.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/src/bioomics/immune/iedb_antigen.py` & `bioomics-0.2.5/src/bioomics/immune/iedb_antigen.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/src/bioomics/immune/iedb_epitope.py` & `bioomics-0.2.5/src/bioomics/immune/iedb_epitope.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 '''
 build data mapping of epitopes from IEDB
 entity is proteins with epitopes
 '''
 from biosequtils import Dir
+import json
 import os
 
 from .iedb import IEDB
 from ..integrate_data import IntegrateData
 
 class IEDBEpitope(IEDB):
     key = 'accession'
+    entity = 'epitope'
 
     def __init__(self, local_path:str, entity_path:str=None):
         super().__init__(local_path, None, False)
-        self.meta['entity'] = 'epitope'
+        self.meta['entity'] = self.entity
         self.meta['entity_path'] = entity_path if entity_path \
-            else os.path.join(self.meta['local_path'], 'epitope')
+            else os.path.join(self.meta['local_path'], self.entity)
         Dir(self.meta['entity_path']).init_dir()
         self.integrate = None
     
     def process(self):
         self.integrate = IntegrateData(self.meta['entity_path'])
 
         print("Process epitopes")
@@ -55,48 +57,48 @@
         # aggregate epitopes by protein
         agg, m, n = {}, 0, 0
         for epitope_id, data in entity_data.items():
             m += 1
             if self.key in data:
                 acc = data[self.key]
                 if acc not in agg:
-                    agg[acc] = {}
+                    agg[acc] = []
                     n += 1
-                agg[acc][epitope_id] = data
+                agg[acc].append(data)
         self.meta['epitopes'] = m
         self.meta['proteins'] = n
         # check if data exists in json
         for json_data in self.integrate.scan():
             acc = json_data.get('key')
             if  acc in agg:
                 if 'epitopes' not in json_data:
                     json_data['epitopes'] = {}
                 json_data['epitopes'][self.source] = agg[acc]
-                self.integrate.save_data(json_data)
+                self.integrate.save_data(json_data, (self.source, self.entity))
                 del agg[acc]
         # export new data
         for acc, data in agg.items():
             input = {
                 'epitopes': {self.source: data},
             }
-            self.integrate.add_data(input, acc)
+            self.integrate.add_data(input, acc, (self.source, self.entity))
 
     def integrate_antigen(self):
         '''
         Add antigen into eiptope-proteins parsed by accession
         '''
         n = 0
         entity_data = self.antigen_json()
         for json_data in self.integrate.scan():
             acc = json_data.get('key', '')
             if  acc in entity_data:
                 if 'antigen' not in json_data:
                     json_data['antigen'] = {}
                 json_data['antigen'][self.source] = entity_data[acc]
-                self.integrate.save_data(json_data)
+                self.integrate.save_data(json_data, (self.source, 'antigen'))
                 del entity_data[acc]
                 n += 1
         self.meta['antigens'] = n
         self.meta['unparsed_antigens'] = len(entity_data)
 
     def integrate_epitope_related(self, entity_data:dict, inner_key:str):
         # aggregate related data by epitope_id
@@ -105,29 +107,28 @@
             n += 1
             if 'epitope_id' in data:
                 epitope_id = data['epitope_id']
                 if epitope_id not in agg:
                     agg[epitope_id] = {}
                 agg[epitope_id][assay_id] = data
             # print(json.dumps(data, indent=4))
-            # break
         self.meta[inner_key] = n
         self.meta[f"{inner_key}_epitopes"] = len(agg)
 
         # inject related data into inner_key within that epitope
         m, n = 0, 0
         for json_data in self.integrate.scan():
             tag = 0
             # the key "epitopes" is defined by integrate_epitope()
             if 'epitopes' in json_data and self.source in json_data['epitopes']:
                 json_epitopes = json_data['epitopes'][self.source]
-                for epitope_id, epitope_data in json_epitopes.items():
-                    if epitope_id in agg:
+                for epitope_data in json_epitopes:
+                    if epitope_data.get('epitope_id') in agg:
                         epitope_data[inner_key] = agg[epitope_id]
                         # print(json.dumps(agg[epitope_id], indent=4))
                         m += 1
                         n += len(agg[epitope_id])
                         tag = 1
             if tag == 1:
-                self.integrate.save_data(json_data)
+                self.integrate.save_data(json_data, (self.source, inner_key))
         self.meta[f"parsed_{inner_key}_epitopes"] = m
         self.meta[f"parsed_{inner_key}"] = n
```

### Comparing `bioomics-0.2.4/src/bioomics/integrate_data.py` & `bioomics-0.2.5/src/bioomics/integrate_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,18 +38,17 @@
         return False
 
     def get_meta(self, updated_meta:dict):
         '''
         meta varies by database
         '''
         meta = {}
-        source = meta.get('source', '')
-        meta_file = os.path.join(self.entity_path, f"{source}_meta.json")
+        file_name = f"{updated_meta.get('source', '')}_meta.json"
+        meta_file = os.path.join(self.entity_path, file_name)
         if os.path.isfile(meta_file):
-            print('get meta.')
             with open(meta_file, 'r') as f:
                 meta = json.load(f)
         else:
             meta = {
                 'entity_path': self.entity_path,
                 'index_meta_file': self.index_meta_file,
                 'meta_file': meta_file,
@@ -89,15 +88,15 @@
         id_prefix = str(math.floor(int(new_id)/1000))
         sub_dirs = [id_prefix[i:i+2] for i in range(0, len(id_prefix), 2)]
         path = os.path.join(self.entity_path, *sub_dirs)
         Dir(path).init_dir()
         json_file = os.path.join(path, f'{new_id}.json')
         return json_file
     
-    def add_data(self, data:dict, key_value:str=None):
+    def add_data(self, data:dict, key_value:str=None, source:str=None):
         '''
         'key' and 'ID' are added into new data
         key is unique id for identification of data
         key could be new_id or accession
         '''
         new_id = self.next_id()
         json_file = self.new_json_path(new_id)
@@ -109,22 +108,28 @@
         }
         new_data.update(data)
         # update index_meta
         self.index_meta[key_value] = {
             'ID': new_id,
             'key': key_value,
             'json_file': json_file,
+            'source': [source if source else "UNKNOWN",],
         }
         with open(json_file, 'w') as f:
             json.dump(new_data, f, indent=4)
             return json_file
     
-    def save_data(self, data:dict) -> str:
+    def save_data(self, data:dict, source:str=None) -> str:
+        '''
+        new data is added or data is updated
+        '''
         if 'key' in data:
             key_value = data['key']
+            if source and source not in self.index_meta[key_value]['source']:
+                    self.index_meta[key_value]['source'].append(source)
             json_file = self.index_meta[key_value]['json_file']
             if os.path.isfile(json_file):
                 with open(json_file, 'w') as f:
                     json.dump(data, f, indent=4)
                 return json_file
         # add data
         return self.add_data(data)
```

### Comparing `bioomics-0.2.4/src/bioomics/mirbase.py` & `bioomics-0.2.5/src/bioomics/mirbase.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/src/bioomics/ncbi.py` & `bioomics-0.2.5/src/bioomics/ncbi.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/src/bioomics/protein/expasy.py` & `bioomics-0.2.5/src/bioomics/protein/expasy.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/src/bioomics/rnacentral.py` & `bioomics-0.2.5/src/bioomics/rnacentral.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/src/bioomics.egg-info/PKG-INFO` & `bioomics-0.2.5/src/bioomics.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioomics
-Version: 0.2.4
+Version: 0.2.5
 Summary: Download, retrieve and process omics data for further bioinformatics
 Home-page: https://github.com/Tiezhengyuan/bio_omics
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -46,18 +46,19 @@
 - The key-value is defined by this corresponding database source.
 - Used for Integration rather than enrichment. Therefore, data combination or aggregation is not recommended.
 - Data from various source could be different or invalid. Those would be validated in the afterwards step rather than this step.
 ```
 {
     "ID": "79541",
     "key": "H0YED9",
-    "Uni-Prot": {
+    "UniProt_SwissProt": {
         ....
     },
     "NCBI": {
         ....
     },
     "PDB": {
         ....
     },
+    ....    
 }
 ```
```

### Comparing `bioomics-0.2.4/src/bioomics.egg-info/SOURCES.txt` & `bioomics-0.2.5/src/bioomics.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 src/bioomics/__init__.py
+src/bioomics/bio_dict.py
 src/bioomics/integrate_data.py
 src/bioomics/mirbase.py
 src/bioomics/ncbi.py
 src/bioomics/rnacentral.py
 src/bioomics.egg-info/PKG-INFO
 src/bioomics.egg-info/SOURCES.txt
 src/bioomics.egg-info/dependency_links.txt
```

### Comparing `bioomics-0.2.4/src/pipelines/retrieve_epitopes.py` & `bioomics-0.2.5/src/pipelines/retrieve_epitopes.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/tests/test_conn_ftp.py` & `bioomics-0.2.5/tests/test_conn_ftp.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/tests/test_conn_ftplib.py` & `bioomics-0.2.5/tests/test_conn_ftplib.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/tests/test_conn_http.py` & `bioomics-0.2.5/tests/test_conn_http.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/tests/test_conn_redis.py` & `bioomics-0.2.5/tests/test_conn_redis.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/tests/test_iedb.py` & `bioomics-0.2.5/tests/test_iedb.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/tests/test_mirbase.py` & `bioomics-0.2.5/tests/test_mirbase.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/tests/test_ncbi.py` & `bioomics-0.2.5/tests/test_ncbi.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/tests/test_rnacentral.py` & `bioomics-0.2.5/tests/test_rnacentral.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/tests/test_uniprot.py` & `bioomics-0.2.5/tests/test_uniprot.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.4/tests/test_uniprot_trembl.py` & `bioomics-0.2.5/tests/test_uniprot_trembl.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,18 +7,23 @@
 
 @ddt
 class TestUniProtTrembl(TestCase):
 
     def setUp(self):
         self.c = UniProtTrembl(DIR_DATA, False)
 
+    @skip
     def test_parse_epitope(self):
         dat_gz = self.c.download_dat()
         assert dat_gz == os.path.join(DIR_DATA, 'UniProt', 'uniprot_trembl.dat.gz')
 
         parser = self.c.parse_dat(dat_gz)
         assert parser
 
         entity_data = self.c.parse_epitope(parser)
         assert len(entity_data) > 0
         
+    def test_process_epitopes(self):
+        entity_path = os.path.join(DIR_DATA, 'epitope')
+        self.c.process_epitopes(entity_path)
+
```

