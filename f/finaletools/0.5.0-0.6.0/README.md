# Comparing `tmp/finaletools-0.5.0.tar.gz` & `tmp/finaletools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finaletools-0.5.0.tar", last modified: Wed Apr 24 06:37:57 2024, max compression
+gzip compressed data, was "finaletools-0.6.0.tar", last modified: Tue Apr 30 17:58:25 2024, max compression
```

## Comparing `finaletools-0.5.0.tar` & `finaletools-0.6.0.tar`

### file list

```diff
@@ -1,46 +1,11 @@
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:57.000000 finaletools-0.5.0/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1067 2024-03-29 01:22:35.000000 finaletools-0.5.0/LICENSE
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5911 2024-04-24 06:37:56.000000 finaletools-0.5.0/PKG-INFO
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3739 2024-04-22 12:55:15.000000 finaletools-0.5.0/README.md
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1058 2024-04-24 06:35:59.000000 finaletools-0.5.0/pyproject.toml
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-04-24 06:37:57.000000 finaletools-0.5.0/setup.cfg
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:54.000000 finaletools-0.5.0/src/
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:54.000000 finaletools-0.5.0/src/FinaleTools.egg-info/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5911 2024-04-24 06:37:32.000000 finaletools-0.5.0/src/FinaleTools.egg-info/PKG-INFO
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1083 2024-04-24 06:37:54.000000 finaletools-0.5.0/src/FinaleTools.egg-info/SOURCES.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        1 2024-04-24 06:37:53.000000 finaletools-0.5.0/src/FinaleTools.egg-info/dependency_links.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       57 2024-04-24 06:37:53.000000 finaletools-0.5.0/src/FinaleTools.egg-info/entry_points.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)      145 2024-04-24 06:37:53.000000 finaletools-0.5.0/src/FinaleTools.egg-info/requires.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       12 2024-04-24 06:37:53.000000 finaletools-0.5.0/src/FinaleTools.egg-info/top_level.txt
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:54.000000 finaletools-0.5.0/src/finaletools/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2023-06-21 12:51:49.000000 finaletools-0.5.0/src/finaletools/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:54.000000 finaletools-0.5.0/src/finaletools/cli/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-03-29 01:22:38.000000 finaletools-0.5.0/src/finaletools/cli/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    27956 2024-04-24 05:56:53.000000 finaletools-0.5.0/src/finaletools/cli/main_cli.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:55.000000 finaletools-0.5.0/src/finaletools/frag/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)      572 2024-04-24 06:06:01.000000 finaletools-0.5.0/src/finaletools/frag/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9664 2024-03-29 01:22:38.000000 finaletools-0.5.0/src/finaletools/frag/adjust_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     4402 2024-03-29 01:22:38.000000 finaletools-0.5.0/src/finaletools/frag/agg_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9329 2024-03-29 01:49:46.000000 finaletools-0.5.0/src/finaletools/frag/cleavage_profile.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     7553 2024-04-24 05:59:32.000000 finaletools-0.5.0/src/finaletools/frag/coverage.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14527 2024-04-24 04:05:00.000000 finaletools-0.5.0/src/finaletools/frag/delfi.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3973 2024-03-29 01:22:38.000000 finaletools-0.5.0/src/finaletools/frag/delfi_gc_correct.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     2585 2024-04-24 04:05:00.000000 finaletools-0.5.0/src/finaletools/frag/delfi_merge_bins.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    29182 2024-04-24 05:56:53.000000 finaletools-0.5.0/src/finaletools/frag/end_motifs.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14865 2024-04-22 12:55:17.000000 finaletools-0.5.0/src/finaletools/frag/frag_length.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     8466 2024-04-22 12:55:17.000000 finaletools-0.5.0/src/finaletools/frag/multi_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     6797 2024-03-29 01:49:46.000000 finaletools-0.5.0/src/finaletools/frag/wps.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:55.000000 finaletools-0.5.0/src/finaletools/genome/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       37 2024-03-29 01:22:39.000000 finaletools-0.5.0/src/finaletools/genome/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14339 2024-03-29 01:22:39.000000 finaletools-0.5.0/src/finaletools/genome/gaps.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:55.000000 finaletools-0.5.0/src/finaletools/methylation/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 finaletools-0.5.0/src/finaletools/methylation/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:56.000000 finaletools-0.5.0/src/finaletools/qc/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 finaletools-0.5.0/src/finaletools/qc/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:56.000000 finaletools-0.5.0/src/finaletools/too/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 finaletools-0.5.0/src/finaletools/too/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-24 06:37:56.000000 finaletools-0.5.0/src/finaletools/utils/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       90 2024-03-29 01:22:39.000000 finaletools-0.5.0/src/finaletools/utils/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1649 2024-03-29 01:22:39.000000 finaletools-0.5.0/src/finaletools/utils/cli_hist.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3917 2024-03-29 01:22:39.000000 finaletools-0.5.0/src/finaletools/utils/filter_bam.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    18436 2024-04-24 03:28:21.000000 finaletools-0.5.0/src/finaletools/utils/utils.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 17:58:25.000000 finaletools-0.6.0/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)      376 2024-04-30 17:58:25.000000 finaletools-0.6.0/PKG-INFO
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)      162 2024-04-30 17:56:08.000000 finaletools-0.6.0/README.md
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-30 17:58:25.000000 finaletools-0.6.0/finaletools.egg-info/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)      376 2024-04-30 17:58:25.000000 finaletools-0.6.0/finaletools.egg-info/PKG-INFO
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)      192 2024-04-30 17:58:25.000000 finaletools-0.6.0/finaletools.egg-info/SOURCES.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        1 2024-04-30 17:58:25.000000 finaletools-0.6.0/finaletools.egg-info/dependency_links.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       14 2024-04-30 17:58:25.000000 finaletools-0.6.0/finaletools.egg-info/requires.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        1 2024-04-30 17:58:25.000000 finaletools-0.6.0/finaletools.egg-info/top_level.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-04-30 17:58:25.000000 finaletools-0.6.0/setup.cfg
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)      545 2024-04-30 17:56:08.000000 finaletools-0.6.0/setup.py
```

