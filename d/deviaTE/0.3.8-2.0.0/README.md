# Comparing `tmp/deviaTE-0.3.8.tar.gz` & `tmp/deviate-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deviaTE-0.3.8.tar", last modified: Thu May  7 19:04:24 2020, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `deviaTE-0.3.8.tar` & `deviate-2.0.0.tar`

### file list

```diff
@@ -1,39 +1,14 @@
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2020-05-07 19:04:24.796043 deviaTE-0.3.8/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    35148 2020-05-07 17:51:54.000000 deviaTE-0.3.8/LICENSE
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      112 2020-05-07 17:51:54.000000 deviaTE-0.3.8/MANIFEST.in
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     4036 2020-05-07 19:04:24.796043 deviaTE-0.3.8/PKG-INFO
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3048 2020-05-07 17:51:54.000000 deviaTE-0.3.8/README.md
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2020-05-07 19:04:24.792043 deviaTE-0.3.8/bin/
--rwxrwxr-x   0 lukas     (1000) lukas     (1000)     5055 2020-05-07 18:52:46.000000 deviaTE-0.3.8/bin/deviaTE
--rwxrwxr-x   0 lukas     (1000) lukas     (1000)     4566 2020-05-07 17:51:54.000000 deviaTE-0.3.8/bin/deviaTE_analyse
--rwxrwxr-x   0 lukas     (1000) lukas     (1000)     4222 2020-05-07 17:51:54.000000 deviaTE-0.3.8/bin/deviaTE_fuse
--rwxrwxr-x   0 lukas     (1000) lukas     (1000)    18152 2020-05-07 17:51:54.000000 deviaTE-0.3.8/bin/deviaTE_plot
--rwxrwxr-x   0 lukas     (1000) lukas     (1000)     2987 2020-05-07 17:51:54.000000 deviaTE-0.3.8/bin/deviaTE_prep
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    34522 2020-05-07 17:51:54.000000 deviaTE-0.3.8/bin/deviaTE_trim.pl
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     8602 2020-05-07 17:51:54.000000 deviaTE-0.3.8/bin/deviaTE_trim.pm
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2020-05-07 19:04:24.792043 deviaTE-0.3.8/deviaTE/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)        0 2020-05-07 17:51:54.000000 deviaTE-0.3.8/deviaTE/__init__.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3711 2020-05-07 17:51:54.000000 deviaTE-0.3.8/deviaTE/deviaTE_IO.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     9022 2020-05-07 17:51:54.000000 deviaTE-0.3.8/deviaTE/deviaTE_multiHSP.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    17629 2020-05-07 17:51:54.000000 deviaTE-0.3.8/deviaTE/deviaTE_pileup.py
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2020-05-07 19:04:24.796043 deviaTE-0.3.8/deviaTE/lib/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    15670 2020-05-07 17:51:54.000000 deviaTE-0.3.8/deviaTE/lib/te_features.gff
--rw-rw-r--   0 lukas     (1000) lukas     (1000)   811667 2020-05-07 17:51:54.000000 deviaTE-0.3.8/deviaTE/lib/te_library
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      542 2020-05-07 17:51:54.000000 deviaTE-0.3.8/deviaTE/lib/te_library.amb
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     5509 2020-05-07 17:51:54.000000 deviaTE-0.3.8/deviaTE/lib/te_library.ann
--rw-rw-r--   0 lukas     (1000) lukas     (1000)   810096 2020-05-07 17:51:54.000000 deviaTE-0.3.8/deviaTE/lib/te_library.bwt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)   202500 2020-05-07 17:51:54.000000 deviaTE-0.3.8/deviaTE/lib/te_library.pac
--rw-rw-r--   0 lukas     (1000) lukas     (1000)   405048 2020-05-07 17:51:54.000000 deviaTE-0.3.8/deviaTE/lib/te_library.sa
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     7649 2020-05-07 17:51:54.000000 deviaTE-0.3.8/deviaTE/lib/te_table
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2020-05-07 19:04:24.796043 deviaTE-0.3.8/deviaTE/tests/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)        0 2020-05-07 17:51:54.000000 deviaTE-0.3.8/deviaTE/tests/__init__.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     8888 2020-05-07 17:51:54.000000 deviaTE-0.3.8/deviaTE/tests/unittest_buildcigar.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     5559 2020-05-07 17:51:54.000000 deviaTE-0.3.8/deviaTE/tests/unittest_is_snp.py
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2020-05-07 19:04:24.792043 deviaTE-0.3.8/deviaTE.egg-info/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     4036 2020-05-07 19:04:24.000000 deviaTE-0.3.8/deviaTE.egg-info/PKG-INFO
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      713 2020-05-07 19:04:24.000000 deviaTE-0.3.8/deviaTE.egg-info/SOURCES.txt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)        1 2020-05-07 19:04:24.000000 deviaTE-0.3.8/deviaTE.egg-info/dependency_links.txt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)       13 2020-05-07 19:04:24.000000 deviaTE-0.3.8/deviaTE.egg-info/requires.txt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)        8 2020-05-07 19:04:24.000000 deviaTE-0.3.8/deviaTE.egg-info/top_level.txt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)       38 2020-05-07 19:04:24.796043 deviaTE-0.3.8/setup.cfg
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      745 2020-05-07 19:04:05.000000 deviaTE-0.3.8/setup.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 deviate-2.0.0/deviaTE/__init__.py
+-rw-r--r--   0        0        0     7067 2020-02-02 00:00:00.000000 deviate-2.0.0/deviaTE/analyse.py
+-rw-r--r--   0        0        0    31611 2020-02-02 00:00:00.000000 deviate-2.0.0/deviaTE/config.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 deviate-2.0.0/deviaTE/deviate.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 deviate-2.0.0/deviaTE/mapping.py
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 deviate-2.0.0/deviaTE/paf.py
+-rw-r--r--   0        0        0     7236 2020-02-02 00:00:00.000000 deviate-2.0.0/deviaTE/plot.py
+-rw-r--r--   0        0        0    11563 2020-02-02 00:00:00.000000 deviate-2.0.0/deviaTE/reference.py
+-rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 deviate-2.0.0/deviaTE/utils.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 deviate-2.0.0/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 deviate-2.0.0/LICENSE
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 deviate-2.0.0/README.md
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 deviate-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 deviate-2.0.0/PKG-INFO
```

### Comparing `deviaTE-0.3.8/LICENSE` & `deviate-2.0.0/LICENSE`

 * *Files identical despite different names*

