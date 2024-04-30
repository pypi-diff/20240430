# Comparing `tmp/bioomics-0.2.5.tar.gz` & `tmp/bioomics-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioomics-0.2.5.tar", last modified: Mon Apr 29 14:05:14 2024, max compression
+gzip compressed data, was "bioomics-0.2.6.tar", last modified: Tue Apr 30 12:21:58 2024, max compression
```

## Comparing `bioomics-0.2.5.tar` & `bioomics-0.2.6.tar`

### file list

```diff
@@ -1,58 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.998437 bioomics-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 14:05:10.000000 bioomics-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-29 14:05:14.998437 bioomics-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-29 14:05:10.000000 bioomics-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:05:14.998437 bioomics-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-29 14:05:10.000000 bioomics-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.986437 bioomics-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.990437 bioomics-0.2.5/src/bioomics/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/bio_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.990437 bioomics-0.2.5/src/bioomics/connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/connector/conn_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/connector/conn_ftplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/connector/conn_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/connector/conn_redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.990437 bioomics-0.2.5/src/bioomics/constants/
--rw-r--r--   0 runner    (1001) docker     (127)    26628 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/constants/IEDB.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.994437 bioomics-0.2.5/src/bioomics/immune/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/immune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15672 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/immune/iedb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/immune/iedb_antigen.py
--rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/immune/iedb_epitope.py
--rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/integrate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/mirbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/ncbi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.994437 bioomics-0.2.5/src/bioomics/protein/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/protein/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/protein/expasy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/protein/uniprot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/protein/uniprot_sprot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/protein/uniprot_trembl.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/bioomics/rnacentral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.994437 bioomics-0.2.5/src/bioomics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-29 14:05:14.000000 bioomics-0.2.5/src/bioomics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-29 14:05:14.000000 bioomics-0.2.5/src/bioomics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:05:14.000000 bioomics-0.2.5/src/bioomics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-29 14:05:14.000000 bioomics-0.2.5/src/bioomics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 14:05:14.000000 bioomics-0.2.5/src/bioomics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.994437 bioomics-0.2.5/src/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/pipelines/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-29 14:05:10.000000 bioomics-0.2.5/src/pipelines/retrieve_epitopes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:05:14.994437 bioomics-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_conn_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_conn_ftplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_conn_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_conn_redis.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_expasy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_iedb.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_iedb_antigen.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_iedb_epitope.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_mirbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_ncbi.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_rnacentral.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_uniprot.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_uniprot_sprot.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-29 14:05:10.000000 bioomics-0.2.5/tests/test_uniprot_trembl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.724175 bioomics-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 12:21:49.000000 bioomics-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-30 12:21:58.724175 bioomics-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-30 12:21:49.000000 bioomics-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 12:21:58.724175 bioomics-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-30 12:21:49.000000 bioomics-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.716174 bioomics-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.716174 bioomics-0.2.6/src/bioomics/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/bio_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/bio_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.720174 bioomics-0.2.6/src/bioomics/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/connector/conn_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/connector/conn_ftplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/connector/conn_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/connector/conn_redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.720174 bioomics-0.2.6/src/bioomics/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)    26628 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/constants/IEDB.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.720174 bioomics-0.2.6/src/bioomics/immune/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/immune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15672 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/immune/iedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/immune/iedb_antigen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/immune/iedb_epitope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/integrate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/mirbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.720174 bioomics-0.2.6/src/bioomics/ncbi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/ncbi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/ncbi/ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/ncbi/refseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/ncbi/retrieve_ncbi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.720174 bioomics-0.2.6/src/bioomics/protein/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/protein/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/protein/expasy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/protein/uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/protein/uniprot_sprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/protein/uniprot_trembl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/rnacentral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.724175 bioomics-0.2.6/src/bioomics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-30 12:21:58.000000 bioomics-0.2.6/src/bioomics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-30 12:21:58.000000 bioomics-0.2.6/src/bioomics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 12:21:58.000000 bioomics-0.2.6/src/bioomics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-30 12:21:58.000000 bioomics-0.2.6/src/bioomics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-30 12:21:58.000000 bioomics-0.2.6/src/bioomics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.720174 bioomics-0.2.6/src/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/pipelines/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/pipelines/retrieve_epitopes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.724175 bioomics-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_conn_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_conn_ftplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_conn_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_conn_redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_expasy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_iedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_iedb_antigen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_iedb_epitope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_mirbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_refseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_rnacentral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_uniprot_sprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_uniprot_trembl.py
```

### Comparing `bioomics-0.2.5/LICENSE` & `bioomics-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/PKG-INFO` & `bioomics-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioomics
-Version: 0.2.5
+Version: 0.2.6
 Summary: Download, retrieve and process omics data for further bioinformatics
 Home-page: https://github.com/Tiezhengyuan/bio_omics
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `bioomics-0.2.5/README.md` & `bioomics-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/setup.py` & `bioomics-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="bioomics",
-    version='0.2.5',
+    version='0.2.6',
     author="Tiezheng Yuan",
     author_email="tiezhengyuan@hotmail.com",
     description="Download, retrieve and process omics data for further bioinformatics",
     url = "https://github.com/Tiezhengyuan/bio_omics",
     long_description_content_type="text/markdown",
     long_description=long_description,
     package_dir={"": "src"},
```

### Comparing `bioomics-0.2.5/src/bioomics/__init__.py` & `bioomics-0.2.6/src/bioomics/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # 
 from .integrate_data import IntegrateData
 from .bio_dict import BioDict
+from .bio_handler import BioHandler
 
 # connector
 from .connector.conn_http import ConnHTTP
 from .connector.conn_ftp import ConnFTP
 from .connector.conn_ftplib import ConnFTPlib
 from .connector.conn_redis import ConnRedis
 
-# comprehensive database
-from .ncbi import NCBI, ANATOMY_GROUPS
+# NCBI
+from .ncbi.ncbi import NCBI, ANATOMY_GROUPS
+from .ncbi.retrieve_ncbi import RetrieveNCBI
+from .ncbi.refseq import Refseq
+
+# ExPAsy/UniProt
 from .protein.expasy import Expasy
 from .protein.uniprot import UniProt
 from .protein.uniprot_sprot import UniProtSprot
 from .protein.uniprot_trembl import UniProtTrembl
 
 # RNA, non-coding RNA
 from .rnacentral import RNACentral
```

### Comparing `bioomics-0.2.5/src/bioomics/connector/conn_ftp.py` & `bioomics-0.2.6/src/bioomics/connector/conn_ftp.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,20 +6,24 @@
 import os
 import re
 from sh import gunzip
 
 
 
 class ConnFTP:
+    overwrite = False
+    run_gunzip = False
+
     def __init__(self, url:str, overwrite:bool=None):
         self.url = url
-        self.overwrite = True if overwrite else False
+        if overwrite:
+            self.overwrite = True
 
     def connect(self, endpoint:str=None):
-        ftp = FTP(self.url)
+        ftp = FTP(self.url, timeout=100)
         ftp.login()
         try: 
             if endpoint:
                 ftp.cwd(endpoint)
             return ftp
         except Exception as e:
             pass
@@ -41,34 +45,28 @@
         for file_name in ftp.nlst():
             if not self._is_dir(ftp, file_name):
                 if match is None or re.search(match, file_name):
                     ftp_files.append((endpoint, file_name))
         return ftp_files
 
     def _is_dir(self, ftp, name=str):
-        origin_dir = ftp.pwd()
         try:
+            origin_dir = ftp.pwd()
             ftp.cwd(name)
             ftp.cwd(origin_dir)
             return True
         except Exception as e:
             pass
         return False
 
-    def download_file(self,
-            endpoint:str,
-            file_name:str,
-            local_path:str,
-            run_gunzip:bool=None,
-        ):
+    def download_file(self, endpoint:str, file_name:str, local_path:str):
         '''
         download one file from FTP
         one download one connection avoiding timeout
         '''
-        if run_gunzip is None: run_gunzip = True
         Dir(local_path).init_dir()
         local_file = os.path.join(local_path, file_name)
         unzip_file = local_file.replace('.gz', '')
         # doesn't download if file exists and overwrite is False
         if self.overwrite is False:
             if os.path.isfile(unzip_file):
                 return unzip_file
@@ -88,50 +86,42 @@
                 ftp.retrbinary(f"RETR {file_name}", f.write)
                 print(f"Download {ftp_file}")
         except Exception as e:
             print('Failure: download data from FTP, error=', e)
             os.remove(local_file)
             local_file = None
         # unzip .gz file
-        if run_gunzip and local_file and local_file.endswith('gz'):
+        if self.run_gunzip and local_file and local_file.endswith('gz'):
             print(f"decompress {local_file} to {unzip_file}")
             gunzip(local_file, '-f')
             return unzip_file
         return local_file
     
-    def download_files(self,
-            endpoint:str=None,
-            match:str=None,
-            local_path:str=None,
-        ):
+    def download_files(self, endpoint:str=None, match:str=None, local_path:str=None):
         '''
         download files from FTP path
         That isnot recursive
         '''
         # list all files
         ftp_files = self.list_files(endpoint, match)
+        print(endpoint, ftp_files)
 
         # download files
         local_files = []
         for current_endpoint, file_name in ftp_files:
             local_file = self.download_file(
                 endpoint = current_endpoint,
                 file_name = file_name,
                 local_path = local_path,
             )
             if local_file and local_file not in local_files:
                 local_files.append(local_file)
         return local_files
 
-    # TODO: need more testing
-    def download_tree(self,
-            local_path:str,
-            endpoint:str=None,
-            match:str=None
-        ):
+    def download_tree(self, local_path:str, endpoint:str=None, match:str=None):
         '''
         arg: local_name is determined by os.path.join()
         Download FTP directory recursively
         '''
         # initialize endpoint
         ftp = FTP(self.url)
         ftp.login()
@@ -150,10 +140,10 @@
             for name in ftp.nlst():
                 if self._is_dir(ftp, name):
                     sub_endpoint = f"{_endpoint}/{name}"
                     sub_local_path = os.path.join(_local_path, name)
                     Dir(sub_local_path).init_dir()
                     pool.append((sub_endpoint, sub_local_path))
             #download files
-            local_files += self.download_files(None, match, _local_path)
+            local_files += self.download_files(_endpoint, match, _local_path)
         return local_files
```

### Comparing `bioomics-0.2.5/src/bioomics/connector/conn_ftplib.py` & `bioomics-0.2.6/src/bioomics/connector/conn_ftplib.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/src/bioomics/connector/conn_http.py` & `bioomics-0.2.6/src/bioomics/connector/conn_http.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/src/bioomics/connector/conn_redis.py` & `bioomics-0.2.6/src/bioomics/connector/conn_redis.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/src/bioomics/constants/IEDB.py` & `bioomics-0.2.6/src/bioomics/constants/IEDB.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/src/bioomics/immune/iedb.py` & `bioomics-0.2.6/src/bioomics/immune/iedb.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/src/bioomics/immune/iedb_antigen.py` & `bioomics-0.2.6/src/bioomics/immune/iedb_antigen.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/src/bioomics/immune/iedb_epitope.py` & `bioomics-0.2.6/src/bioomics/immune/iedb_epitope.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/src/bioomics/integrate_data.py` & `bioomics-0.2.6/src/bioomics/integrate_data.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/src/bioomics/mirbase.py` & `bioomics-0.2.6/src/bioomics/mirbase.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/src/bioomics/ncbi.py` & `bioomics-0.2.6/src/bioomics/ncbi/ncbi.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,114 @@
 """
 download data from NCIB FTP
 """
 import os
 
-from .connector.conn_ftp import ConnFTP
-from .connector.conn_ftplib import ConnFTPlib
+from ..connector.conn_ftp import ConnFTP
+from ..connector.conn_ftplib import ConnFTPlib
 
 # lock the scope of groups in local version
 ANATOMY_GROUPS = ['archaea', 'bacteria', 'fungi', 'invertebrate', 'plant',
     'protozoa', 'vertebrate_mammalian', 'vertebrate_other', 'viral', ]
 
 
 class NCBI(ConnFTP):
     url = 'ftp.ncbi.nlm.nih.gov'
 
-    def __init__(self, local_dir:str, overwrite:bool=None):
+    def __init__(self, local_path:str, overwrite:bool=None):
         super().__init__(url=self.url, overwrite=overwrite)
-        self.local_dir = os.path.join(local_dir, "NCBI")
+        self.local_path = os.path.join(local_path, "NCBI")
 
     def download_assembly_summary(self, groups:list=None):
         '''
         download assembly_summary.txt. That is genome metadata
         '''
         if not groups:
             groups = ANATOMY_GROUPS
         groups = [i for i in groups if i in ANATOMY_GROUPS]
         
         res = {}
         for antonomy in groups:
-            outdir = os.path.join(self.local_dir, 'assembly_summary', antonomy)
+            outdir = os.path.join(self.local_path, 'assembly_summary', antonomy)
             local_file = self.download_file(
                 endpoint = f'genomes/refseq/{antonomy}/',
                 file_name = 'assembly_summary.txt',
                 local_path = outdir
             )
             res[antonomy] = local_file
-        return self.local_dir, res
+        return self.local_path, res
 
     def download_genome(self, ftp_path:str, specie:str, version:str=None):
         '''
         download genome including subdirectories and files
         '''
-        local_path = os.path.join(self.local_dir, 'genome', specie)
+        local_path = os.path.join(self.local_path, 'genome', specie)
         if version:
             local_path = os.path.join(local_path, version)
 
         # download sequences and annotations
         local_files = self.download_files(
             endpoint = ftp_path.replace('https://ftp.ncbi.nlm.nih.gov/', ''),
             match = '.gz',
             local_path = local_path,
         )
         return local_path, local_files
     
+    def download_refseq_uniprotkb(self):
+        '''
+        download gene_refseq_uniprotkb_collab.gz from 
+        https://ftp.ncbi.nlm.nih.gov/refseq/uniprotkb/
+        map refeseq ~ uniprotkb
+        '''
+        local_file = self.download_file(
+            endpoint='refseq/uniprotkb/',
+            file_name='gene_refseq_uniprotkb_collab.gz',
+            local_path=os.path.join(self.local_path, 'refseq'),
+        )
+        return local_file
+    
+    def download_refseq_gpff(self):
+        local_files = []
+        species = ['H_sapiens', 'D_rerio', 'B_taurus', 'M_musculus',\
+            'R_norvegicus', 'S_scrofa', 'X_tropicalis']
+        for sub in species:
+            local_files += self.download_files(
+                local_path = os.path.join(self.local_path, 'refseq', 'mRNA_Prot'),
+                endpoint = f'refseq/{sub}/mRNA_Prot',
+                match = '.gpff.gz$'
+            )
+        return local_files
+
+    def download_refseq_complete_gpff(self):
+        local_files = []
+        species = ['vertebrate_mammalian',]
+        for sub in species:
+            local_files += self.download_files(
+            local_path = os.path.join(self.local_path, 'refseq', 'release', 'gpff'),
+            endpoint = f'refseq/release/{sub}/',
+            match = '.gpff.gz$'
+        )
+        return local_files
+
+
     def download_gene_data(self):
         '''
         download /gene/DATA including subdirectories and files
         '''
         local_files = self.download_tree(
-            local_path = os.path.join(self.local_dir, 'gene', 'DATA'),
+            local_path = os.path.join(self.local_path, 'gene', 'DATA'),
             endpoint = 'gene/DATA',
             match = '.gz$'
         )
         return local_files
 
     def download_pubmed(self):
         '''
         download /PubMed including subdirectories and files
         '''
         res = ConnFTPlib.download_tree(
             ftp_endpoint = self.url,
             ftp_path = '/pubmed',
             match = '.gz',
-            local_path = self.local_dir
+            local_path = self.local_path
         )
         return res
```

### Comparing `bioomics-0.2.5/src/bioomics/protein/expasy.py` & `bioomics-0.2.6/src/bioomics/protein/expasy.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/src/bioomics/protein/uniprot.py` & `bioomics-0.2.6/src/bioomics/protein/uniprot.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                             'accession': record.id,
                             'source': BioDict.swiss_source(record),
                             'epitopes': [],
                         }
                         m += 1
                     n += 1
                     # update epitope to data
-                    epitope = BioDict.feature(record, ft)
+                    epitope = BioDict.swiss_feature(record, ft)
                     data[record.id]['epitopes'].append(epitope)
                     print(json.dumps(data[record.id], indent=4))
         print(f"proteins={m},epitopes={n}")
         return data
 
     def integrate_epitope(self, integrate_obj:IntegrateData, entity_data:dict):
         '''
```

### Comparing `bioomics-0.2.5/src/bioomics/protein/uniprot_sprot.py` & `bioomics-0.2.6/src/bioomics/protein/uniprot_sprot.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/src/bioomics/protein/uniprot_trembl.py` & `bioomics-0.2.6/src/bioomics/protein/uniprot_trembl.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/src/bioomics/rnacentral.py` & `bioomics-0.2.6/src/bioomics/rnacentral.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/src/bioomics.egg-info/PKG-INFO` & `bioomics-0.2.6/src/bioomics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioomics
-Version: 0.2.5
+Version: 0.2.6
 Summary: Download, retrieve and process omics data for further bioinformatics
 Home-page: https://github.com/Tiezhengyuan/bio_omics
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `bioomics-0.2.5/src/bioomics.egg-info/SOURCES.txt` & `bioomics-0.2.6/src/bioomics.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENSE
 README.md
 setup.py
 src/bioomics/__init__.py
 src/bioomics/bio_dict.py
+src/bioomics/bio_handler.py
 src/bioomics/integrate_data.py
 src/bioomics/mirbase.py
-src/bioomics/ncbi.py
 src/bioomics/rnacentral.py
 src/bioomics.egg-info/PKG-INFO
 src/bioomics.egg-info/SOURCES.txt
 src/bioomics.egg-info/dependency_links.txt
 src/bioomics.egg-info/requires.txt
 src/bioomics.egg-info/top_level.txt
 src/bioomics/connector/__init__.py
@@ -18,14 +18,18 @@
 src/bioomics/connector/conn_http.py
 src/bioomics/connector/conn_redis.py
 src/bioomics/constants/IEDB.py
 src/bioomics/immune/__init__.py
 src/bioomics/immune/iedb.py
 src/bioomics/immune/iedb_antigen.py
 src/bioomics/immune/iedb_epitope.py
+src/bioomics/ncbi/__init__.py
+src/bioomics/ncbi/ncbi.py
+src/bioomics/ncbi/refseq.py
+src/bioomics/ncbi/retrieve_ncbi.py
 src/bioomics/protein/__init__.py
 src/bioomics/protein/expasy.py
 src/bioomics/protein/uniprot.py
 src/bioomics/protein/uniprot_sprot.py
 src/bioomics/protein/uniprot_trembl.py
 src/pipelines/__init__.py
 src/pipelines/app.py
@@ -36,11 +40,12 @@
 tests/test_conn_redis.py
 tests/test_expasy.py
 tests/test_iedb.py
 tests/test_iedb_antigen.py
 tests/test_iedb_epitope.py
 tests/test_mirbase.py
 tests/test_ncbi.py
+tests/test_refseq.py
 tests/test_rnacentral.py
 tests/test_uniprot.py
 tests/test_uniprot_sprot.py
 tests/test_uniprot_trembl.py
```

### Comparing `bioomics-0.2.5/src/pipelines/retrieve_epitopes.py` & `bioomics-0.2.6/src/pipelines/retrieve_epitopes.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/tests/test_conn_ftp.py` & `bioomics-0.2.6/tests/test_conn_ftp.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/tests/test_conn_ftplib.py` & `bioomics-0.2.6/tests/test_conn_ftplib.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/tests/test_conn_http.py` & `bioomics-0.2.6/tests/test_conn_http.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/tests/test_conn_redis.py` & `bioomics-0.2.6/tests/test_conn_redis.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/tests/test_iedb.py` & `bioomics-0.2.6/tests/test_iedb.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/tests/test_mirbase.py` & `bioomics-0.2.6/tests/test_mirbase.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/tests/test_rnacentral.py` & `bioomics-0.2.6/tests/test_rnacentral.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/tests/test_uniprot.py` & `bioomics-0.2.6/tests/test_uniprot.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/tests/test_uniprot_sprot.py` & `bioomics-0.2.6/tests/test_uniprot_sprot.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.5/tests/test_uniprot_trembl.py` & `bioomics-0.2.6/tests/test_uniprot_trembl.py`

 * *Files identical despite different names*

