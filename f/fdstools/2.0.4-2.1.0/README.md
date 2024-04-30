# Comparing `tmp/fdstools-2.0.4.tar.gz` & `tmp/fdstools-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdstools-2.0.4.tar", last modified: Thu Mar  2 13:16:39 2023, max compression
+gzip compressed data, was "fdstools-2.1.0.tar", last modified: Tue Apr 30 20:32:37 2024, max compression
```

## Comparing `fdstools-2.0.4.tar` & `fdstools-2.1.0.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-03-02 13:16:39.957238 fdstools-2.0.4/
--rw-rw-rw-   0        0        0    39789 2023-03-02 12:48:16.000000 fdstools-2.0.4/CHANGELOG.md
--rw-rw-rw-   0        0        0    35819 2023-03-02 12:48:16.000000 fdstools-2.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     4775 2023-03-02 12:48:16.000000 fdstools-2.0.4/LICENSES-3RD-PARTY.txt
--rw-rw-rw-   0        0        0       71 2023-03-02 12:48:16.000000 fdstools-2.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0    10202 2023-03-02 13:16:39.950255 fdstools-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     9031 2023-03-02 12:48:16.000000 fdstools-2.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-02 13:16:37.992298 fdstools-2.0.4/fdstools/
--rw-rw-rw-   0        0        0     1567 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/__init__.py
--rw-rw-rw-   0        0        0     1063 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/__main__.py
-drwxrwxrwx   0        0        0        0 2023-03-02 13:16:37.923503 fdstools-2.0.4/fdstools/data/
-drwxrwxrwx   0        0        0        0 2023-03-02 13:16:38.161527 fdstools-2.0.4/fdstools/data/libraries/
--rw-rw-rw-   0        0        0     6831 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/data/libraries/ForenSeqA-UAS.ini
--rw-rw-rw-   0        0        0     6429 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/data/libraries/ForenSeqA.ini
--rw-rw-rw-   0        0        0    10122 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/data/libraries/ForenSeqB-UAS.ini
--rw-rw-rw-   0        0        0     9720 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/data/libraries/ForenSeqB.ini
--rw-rw-rw-   0        0        0     1982 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/data/libraries/ID-OmniSTR.ini
--rw-rw-rw-   0        0        0     1902 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/data/libraries/PowerSeq46GY.ini
--rw-rw-rw-   0        0        0     6988 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/fdstools.py
-drwxrwxrwx   0        0        0        0 2023-03-02 13:16:38.450763 fdstools-2.0.4/fdstools/lib/
--rw-rw-rw-   0        0        0        0 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/lib/__init__.py
--rw-rw-rw-   0        0        0    13627 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/lib/cli.py
--rw-rw-rw-   0        0        0     7531 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/lib/io.py
--rw-rw-rw-   0        0        0    19339 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/lib/library.py
--rw-rw-rw-   0        0        0     2961 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/lib/noise.py
--rw-rw-rw-   0        0        0     7903 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/lib/seq.py
--rw-rw-rw-   0        0        0    20491 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/lib/sg_align.c
--rw-rw-rw-   0        0        0     3147 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/lib/util.py
-drwxrwxrwx   0        0        0        0 2023-03-02 13:16:39.065119 fdstools-2.0.4/fdstools/tools/
--rw-rw-rw-   0        0        0        0 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/tools/__init__.py
--rw-rw-rw-   0        0        0    11035 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/tools/allelefinder.py
--rw-rw-rw-   0        0        0    10006 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/tools/bganalyse.py
--rw-rw-rw-   0        0        0    14128 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/tools/bgcorrect.py
--rw-rw-rw-   0        0        0    26674 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/tools/bgestimate.py
--rw-rw-rw-   0        0        0     9895 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/tools/bghomraw.py
--rw-rw-rw-   0        0        0     8875 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/tools/bghomstats.py
--rw-rw-rw-   0        0        0     4918 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/tools/bgmerge.py
--rw-rw-rw-   0        0        0    13973 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/tools/bgpredict.py
--rw-rw-rw-   0        0        0     4817 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/tools/findnewalleles.py
--rw-rw-rw-   0        0        0     4479 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/tools/libconvert.py
--rw-rw-rw-   0        0        0    11566 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/tools/library.py
--rw-rw-rw-   0        0        0    40231 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/tools/pipeline.py
--rw-rw-rw-   0        0        0    30784 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/tools/samplestats.py
--rw-rw-rw-   0        0        0     7775 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/tools/seqconvert.py
--rw-rw-rw-   0        0        0    20283 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/tools/stuttermark.py
--rw-rw-rw-   0        0        0    23925 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/tools/stuttermodel.py
--rw-rw-rw-   0        0        0    30395 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/tools/tssv.py
--rw-rw-rw-   0        0        0    22056 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/tools/vis.py
-drwxrwxrwx   0        0        0        0 2023-03-02 13:16:39.451080 fdstools-2.0.4/fdstools/vis/
-drwxrwxrwx   0        0        0        0 2023-03-02 13:16:39.512421 fdstools-2.0.4/fdstools/vis/allelevis/
--rw-rw-rw-   0        0        0     6535 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/vis/allelevis/allelevis.json
--rw-rw-rw-   0        0        0    26137 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/vis/allelevis/index.html
-drwxrwxrwx   0        0        0        0 2023-03-02 13:16:39.597194 fdstools-2.0.4/fdstools/vis/bganalysevis/
--rw-rw-rw-   0        0        0    12729 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/vis/bganalysevis/bganalysevis.json
--rw-rw-rw-   0        0        0    27598 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/vis/bganalysevis/index.html
-drwxrwxrwx   0        0        0        0 2023-03-02 13:16:39.707898 fdstools-2.0.4/fdstools/vis/bgrawvis/
--rw-rw-rw-   0        0        0     8843 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/vis/bgrawvis/bgrawvis.json
--rw-rw-rw-   0        0        0    27634 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/vis/bgrawvis/index.html
--rw-rw-rw-   0        0        0   151725 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/vis/d3.min.js
-drwxrwxrwx   0        0        0        0 2023-03-02 13:16:39.773726 fdstools-2.0.4/fdstools/vis/profilevis/
--rw-rw-rw-   0        0        0    29851 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/vis/profilevis/index.html
--rw-rw-rw-   0        0        0    16726 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/vis/profilevis/profilevis.json
-drwxrwxrwx   0        0        0        0 2023-03-02 13:16:39.859497 fdstools-2.0.4/fdstools/vis/samplevis/
--rw-rw-rw-   0        0        0    73747 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/vis/samplevis/index.html
--rw-rw-rw-   0        0        0    27746 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/vis/samplevis/samplevis.json
--rw-rw-rw-   0        0        0      984 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/vis/samplevis/warning.svg
-drwxrwxrwx   0        0        0        0 2023-03-02 13:16:39.944266 fdstools-2.0.4/fdstools/vis/stuttermodelvis/
--rw-rw-rw-   0        0        0    33022 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/vis/stuttermodelvis/index.html
--rw-rw-rw-   0        0        0    11835 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/vis/stuttermodelvis/stuttermodelvis.json
--rw-rw-rw-   0        0        0   307279 2023-03-02 12:48:16.000000 fdstools-2.0.4/fdstools/vis/vega.min.js
-drwxrwxrwx   0        0        0        0 2023-03-02 13:16:38.030211 fdstools-2.0.4/fdstools.egg-info/
--rw-rw-rw-   0        0        0    10202 2023-03-02 13:16:37.000000 fdstools-2.0.4/fdstools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1849 2023-03-02 13:16:37.000000 fdstools-2.0.4/fdstools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-02 13:16:37.000000 fdstools-2.0.4/fdstools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-03-02 13:16:37.000000 fdstools-2.0.4/fdstools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-03-02 13:16:37.000000 fdstools-2.0.4/fdstools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-02 13:16:37.000000 fdstools-2.0.4/fdstools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-02 13:16:39.958228 fdstools-2.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2913 2023-03-02 12:48:16.000000 fdstools-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 20:32:37.381709 fdstools-2.1.0/
+-rw-rw-rw-   0        0        0    41745 2024-04-30 18:45:32.000000 fdstools-2.1.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35819 2024-04-30 18:45:32.000000 fdstools-2.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     4775 2024-04-30 18:45:32.000000 fdstools-2.1.0/LICENSES-3RD-PARTY.txt
+-rw-rw-rw-   0        0        0       71 2024-04-30 18:45:32.000000 fdstools-2.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    11452 2024-04-30 20:32:37.366087 fdstools-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10199 2024-04-30 18:45:32.000000 fdstools-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 20:32:36.147622 fdstools-2.1.0/fdstools/
+-rw-rw-rw-   0        0        0     1567 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/__init__.py
+-rw-rw-rw-   0        0        0     1063 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 20:32:36.022650 fdstools-2.1.0/fdstools/data/
+drwxrwxrwx   0        0        0        0 2024-04-30 20:32:36.303881 fdstools-2.1.0/fdstools/data/libraries/
+-rw-rw-rw-   0        0        0     6831 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/data/libraries/ForenSeqA-UAS.ini
+-rw-rw-rw-   0        0        0     6429 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/data/libraries/ForenSeqA.ini
+-rw-rw-rw-   0        0        0    10122 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/data/libraries/ForenSeqB-UAS.ini
+-rw-rw-rw-   0        0        0     9720 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/data/libraries/ForenSeqB.ini
+-rw-rw-rw-   0        0        0     1986 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/data/libraries/ID-OmniSTR.ini
+-rw-rw-rw-   0        0        0     1902 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/data/libraries/PowerSeq46GY.ini
+-rw-rw-rw-   0        0        0     6860 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/fdstools.py
+drwxrwxrwx   0        0        0        0 2024-04-30 20:32:36.413185 fdstools-2.1.0/fdstools/lib/
+-rw-rw-rw-   0        0        0        0 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/lib/__init__.py
+-rw-rw-rw-   0        0        0    13797 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/lib/cli.py
+-rw-rw-rw-   0        0        0     7784 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/lib/io.py
+-rw-rw-rw-   0        0        0    20295 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/lib/library.py
+-rw-rw-rw-   0        0        0     2961 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/lib/noise.py
+-rw-rw-rw-   0        0        0     7900 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/lib/seq.py
+-rw-rw-rw-   0        0        0    20491 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/lib/sg_align.c
+-rw-rw-rw-   0        0        0     3147 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/lib/util.py
+drwxrwxrwx   0        0        0        0 2024-04-30 20:32:36.741233 fdstools-2.1.0/fdstools/tools/
+-rw-rw-rw-   0        0        0        0 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/__init__.py
+-rw-rw-rw-   0        0        0    11035 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/allelefinder.py
+-rw-rw-rw-   0        0        0    10006 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/bganalyse.py
+-rw-rw-rw-   0        0        0    14128 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/bgcorrect.py
+-rw-rw-rw-   0        0        0    26674 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/bgestimate.py
+-rw-rw-rw-   0        0        0     9895 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/bghomraw.py
+-rw-rw-rw-   0        0        0     8875 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/bghomstats.py
+-rw-rw-rw-   0        0        0     4918 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/bgmerge.py
+-rw-rw-rw-   0        0        0    13973 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/bgpredict.py
+-rw-rw-rw-   0        0        0     4817 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/findnewalleles.py
+-rw-rw-rw-   0        0        0     4479 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/libconvert.py
+-rw-rw-rw-   0        0        0    12033 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/library.py
+-rw-rw-rw-   0        0        0     9106 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/mps2ce.py
+-rw-rw-rw-   0        0        0    40185 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/pipeline.py
+-rw-rw-rw-   0        0        0    30784 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/samplestats.py
+-rw-rw-rw-   0        0        0     7775 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/seqconvert.py
+-rw-rw-rw-   0        0        0    20283 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/stuttermark.py
+-rw-rw-rw-   0        0        0    23925 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/stuttermodel.py
+-rw-rw-rw-   0        0        0    31230 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/tssv.py
+-rw-rw-rw-   0        0        0    22060 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/tools/vis.py
+drwxrwxrwx   0        0        0        0 2024-04-30 20:32:36.959930 fdstools-2.1.0/fdstools/vis/
+drwxrwxrwx   0        0        0        0 2024-04-30 20:32:37.038040 fdstools-2.1.0/fdstools/vis/allelevis/
+-rw-rw-rw-   0        0        0     6535 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/vis/allelevis/allelevis.json
+-rw-rw-rw-   0        0        0    26137 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/vis/allelevis/index.html
+drwxrwxrwx   0        0        0        0 2024-04-30 20:32:37.100523 fdstools-2.1.0/fdstools/vis/bganalysevis/
+-rw-rw-rw-   0        0        0    12729 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/vis/bganalysevis/bganalysevis.json
+-rw-rw-rw-   0        0        0    27598 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/vis/bganalysevis/index.html
+drwxrwxrwx   0        0        0        0 2024-04-30 20:32:37.163010 fdstools-2.1.0/fdstools/vis/bgrawvis/
+-rw-rw-rw-   0        0        0     8843 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/vis/bgrawvis/bgrawvis.json
+-rw-rw-rw-   0        0        0    27634 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/vis/bgrawvis/index.html
+-rw-rw-rw-   0        0        0   151725 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/vis/d3.min.js
+drwxrwxrwx   0        0        0        0 2024-04-30 20:32:37.225497 fdstools-2.1.0/fdstools/vis/profilevis/
+-rw-rw-rw-   0        0        0    29851 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/vis/profilevis/index.html
+-rw-rw-rw-   0        0        0    16726 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/vis/profilevis/profilevis.json
+drwxrwxrwx   0        0        0        0 2024-04-30 20:32:37.303601 fdstools-2.1.0/fdstools/vis/samplevis/
+-rw-rw-rw-   0        0        0    73747 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/vis/samplevis/index.html
+-rw-rw-rw-   0        0        0    27746 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/vis/samplevis/samplevis.json
+-rw-rw-rw-   0        0        0      984 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/vis/samplevis/warning.svg
+drwxrwxrwx   0        0        0        0 2024-04-30 20:32:37.366087 fdstools-2.1.0/fdstools/vis/stuttermodelvis/
+-rw-rw-rw-   0        0        0    33022 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/vis/stuttermodelvis/index.html
+-rw-rw-rw-   0        0        0    11835 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/vis/stuttermodelvis/stuttermodelvis.json
+-rw-rw-rw-   0        0        0   307279 2024-04-30 18:45:32.000000 fdstools-2.1.0/fdstools/vis/vega.min.js
+drwxrwxrwx   0        0        0        0 2024-04-30 20:32:37.366087 fdstools-2.1.0/fdstools.egg-info/
+-rw-rw-rw-   0        0        0    11452 2024-04-30 20:32:35.000000 fdstools-2.1.0/fdstools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1874 2024-04-30 20:32:35.000000 fdstools-2.1.0/fdstools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 20:32:35.000000 fdstools-2.1.0/fdstools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-30 20:32:35.000000 fdstools-2.1.0/fdstools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2024-04-30 20:32:35.000000 fdstools-2.1.0/fdstools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-30 20:32:35.000000 fdstools-2.1.0/fdstools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 20:32:37.381709 fdstools-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2913 2024-04-30 18:45:32.000000 fdstools-2.1.0/setup.py
```

### Comparing `fdstools-2.0.4/CHANGELOG.md` & `fdstools-2.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,31 @@
 FDSTools Changelog
 ==================
+### Version 2.1.0
+- Fixed compatibility issues with Python 3.12 and resolved various warnings.
+- Fixed an issue that made a single-base [genome_position] impossible.
+- Microhaplotype markers that include a repetitive sequence are now supported.
+- Microhaplotype markers can now consist of multiple [genome_position] ranges.
+- The [flanks] section of the library file can now contain 'REF' to indicate
+  that GRCh38 reference sequence should be used (the default). Specifying a
+  number in the [flanks] section is no longer supported.
+- Library files can now include a [flank_length] section to specify a marker-
+  specific minimum and maximum (or exact) flanking sequence length.
+- When reading sample data files, empty lines and lines that start with 'info_'
+  are now ignored.
+- Introduced the first suite of component tests, covering Allelefinder,
+  Seqconvert, Stuttermark and TSSV.
+- Includes [Library v1.1.2](#Library-112)
+- Includes [MPS2CE v1.0.0](#MPS2CE-100)
+- Includes [Pipeline v1.1.2](#Pipeline-112)
+- Includes [TSSV v2.2.0](#TSSV-220)
+- Includes [Vis v1.1.1](#Vis-111)
+- Updated dependency requirement (strnaming~=1.2.0).
+
+
 ### Version 2.0.4
 - Microhaplotype alleles with SNPs adjacent to any of the microhaplotype
   positions are now recognised.
 - Greatly improved loading speed for large library files.
 - Updated dependency requirement (strnaming~=1.1.4).
 
 
@@ -518,14 +540,20 @@
 ### Libconvert 1.0.0
 - Initial version.
 
 
 
 Library
 -------
+### Library 1.1.2
+- Updated explanatory text in [flanks] section to include 'REF' as a possible value.
+- Added the new [flank_length] section to configure marker-specific flanking sequence
+  length limitations.
+
+
 ### Library 1.1.1
 - Added the -m/--microhaplotypes option, to include the new [microhaplotype_positions]
   section in the library file.
 
 
 ### Library 1.1.0
 - Introduce the new 'smart' library file and make it the default. All explanatory comments
@@ -549,16 +577,27 @@
 
 
 ### Library 1.0.0
 - Initial version.
 
 
 
+MPS2CE
+--------
+### MPS2CE 1.0.0
+- Initial version.
+
+
+
 Pipeline
 --------
+### Pipeline 1.1.2
+- Updated tool import mechanism.
+
+
 ### Pipeline 1.1.1
 - Fixed issues with handling of TSSV's aggregate-filtered option.
 - Fixed issues with handling of the max-alleles option of Samplestats.
 - Removed access to the uncall-alleles option of Samplestats.
 
 
 ### Pipeline 1.1.0
@@ -764,14 +803,22 @@
 ### Stuttermodel 1.0.0
 - Initial version.
 
 
 
 TSSV
 ----
+### TSSV 2.2.0
+- The -L/--flank-length option is now applied to all markers, including those that
+  have an entry in the [flanks] section of the library file. If applicable, the value
+  is now clamped into the marker-specific range specified in the new [flank_length] section.
+- Fixed incorrect handling of overlapping ranges in TSSV. For example, TSSV would
+  sometimes use only the DYS389I part of reads that span the full DYS389II range.
+
+
 ### TSSV 2.1.1
 - Fixed "error: too many values to unpack (expected 2)" when using the -D/--dir option.
   Thanks to @agynna for reporting!
 
 
 ### TSSV 2.1.0
 - Changed the default value for -a/--minimum from 1 to 2.
@@ -835,14 +882,18 @@
 ### TSSV 1.0.0
 - Initial version.
 
 
 
 Vis
 ---
+### Vis 1.1.1
+- Minor code change to fix warnings.
+
+
 ### Vis 1.1.0
 - Changed the default value of the -B/--bias-threshold option from 25 to 0.
 - Changed the default value of the -Z/--allele-min-per-strand option from 1 to 0.
 - Removed the -O/--online option.
 
 
 ### Vis 1.0.4
```

### Comparing `fdstools-2.0.4/LICENSE.txt` & `fdstools-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/LICENSES-3RD-PARTY.txt` & `fdstools-2.1.0/LICENSES-3RD-PARTY.txt`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/PKG-INFO` & `fdstools-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdstools
-Version: 2.0.4
+Version: 2.1.0
 Summary: Forensic DNA Sequencing Tools
 Home-page: https://fdstools.nl
 Author: Jerry Hoogenboom
 Author-email: jerryhoogenboom@outlook.com
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/Jerrythafast/FDSTools/issues
 Project-URL: Source Code, https://github.com/Jerrythafast/FDSTools
@@ -16,14 +16,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Legal Industry
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: LICENSES-3RD-PARTY.txt
+Requires-Dist: numpy>=1.17
+Requires-Dist: strnaming~=1.2.0
 
 Forensic DNA Sequencing Tools
 =============================
 Tools for filtering and interpretation of Massively Parallel Sequencing data of
 forensic DNA samples. To obtain a list of included tools with a brief
 description of each tool, run:
 
@@ -48,14 +50,35 @@
 Alternatively, FDSTools can be installed by running:
 
     python setup.py install
 
 
 Release Notes
 -------------
+### Version 2.1.0 (2024-04-30)
+Updated STRNaming nomenclature to version 1.2. Please note that this is a
+backwards incompatible update: this version of FDSTools is unable to correctly
+interpret allele names that were produced with a prior version!
+Please see https://fdstools.nl/strnaming/updates for more information.
+
+Changed interpretation of the [flanks] section in the library file: it can no
+longer contain numbers, but the value 'REF' can be specified to indicate that
+GRCh38 reference sequence should be used (which was already the default).
+A new [flank_length] section is introduced to allow specifying marker-specific
+minimum and maximum (or exact) flanking sequence length; the value specified
+for TSSV's -L/--flank-length option is then clamped between these values.
+If a [flanks] section is present and contains a short sequence (possibly with
+IUPAC codes), it is implicitly extended with GRCh38 reference sequence to the
+requested length by TSSV.
+
+Greatly improved handling of microhaplotype markers, and we finally introduced
+the first suite of component tests, covering Allelefinder, Seqconvert,
+Stuttermark and TSSV. Welcome to the team, Brechtje!
+
+
 ### Version 2.0.4 (2023-03-02)
 Microhaplotype alleles with SNPs adjacent to any of the microhaplotype
 positions are now recognised. For example, an allele previously named
 "MH_N_123NC>GA" will now be named "MH_G_124C>A" instead.
 
 Greatly improved loading speed for large library files.
```

### Comparing `fdstools-2.0.4/README.md` & `fdstools-2.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,35 @@
 Alternatively, FDSTools can be installed by running:
 
     python setup.py install
 
 
 Release Notes
 -------------
+### Version 2.1.0 (2024-04-30)
+Updated STRNaming nomenclature to version 1.2. Please note that this is a
+backwards incompatible update: this version of FDSTools is unable to correctly
+interpret allele names that were produced with a prior version!
+Please see https://fdstools.nl/strnaming/updates for more information.
+
+Changed interpretation of the [flanks] section in the library file: it can no
+longer contain numbers, but the value 'REF' can be specified to indicate that
+GRCh38 reference sequence should be used (which was already the default).
+A new [flank_length] section is introduced to allow specifying marker-specific
+minimum and maximum (or exact) flanking sequence length; the value specified
+for TSSV's -L/--flank-length option is then clamped between these values.
+If a [flanks] section is present and contains a short sequence (possibly with
+IUPAC codes), it is implicitly extended with GRCh38 reference sequence to the
+requested length by TSSV.
+
+Greatly improved handling of microhaplotype markers, and we finally introduced
+the first suite of component tests, covering Allelefinder, Seqconvert,
+Stuttermark and TSSV. Welcome to the team, Brechtje!
+
+
 ### Version 2.0.4 (2023-03-02)
 Microhaplotype alleles with SNPs adjacent to any of the microhaplotype
 positions are now recognised. For example, an allele previously named
 "MH_N_123NC>GA" will now be named "MH_G_124C>A" instead.
 
 Greatly improved loading speed for large library files.
```

### Comparing `fdstools-2.0.4/fdstools/__init__.py` & `fdstools-2.1.0/fdstools/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2023 Jerry Hoogenboom
+# Copyright (C) 2024 Jerry Hoogenboom
 #
 # This file is part of FDSTools, data analysis tools for Massively
 # Parallel Sequencing of forensic DNA markers.
 #
 # FDSTools is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the
 # Free Software Foundation, either version 3 of the License, or (at
@@ -20,15 +20,15 @@
 
 """
 Data analysis tools for Massively Parallel Sequencing of forensic DNA markers,
 including tools for characterisation and filtering of PCR stutter artefacts and
 other systemic noise, and for automatic detection of the alleles in a sample.
 """
 
-__version__ = "2.0.4"
+__version__ = "2.1.0"
 usage = __doc__.split("\n\n\n")
 
 
 def version(name, toolname=None, toolversion=None):
     """Return a version string for the package or a given tool."""
     verformat = "%s %s"
     toolverformat = "%s (part of %s)"
```

### Comparing `fdstools-2.0.4/fdstools/__main__.py` & `fdstools-2.1.0/fdstools/__main__.py`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/data/libraries/ForenSeqA-UAS.ini` & `fdstools-2.1.0/fdstools/data/libraries/ForenSeqA-UAS.ini`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/data/libraries/ForenSeqA.ini` & `fdstools-2.1.0/fdstools/data/libraries/ForenSeqA.ini`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/data/libraries/ForenSeqB-UAS.ini` & `fdstools-2.1.0/fdstools/data/libraries/ForenSeqB-UAS.ini`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/data/libraries/ForenSeqB.ini` & `fdstools-2.1.0/fdstools/data/libraries/ForenSeqB.ini`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/data/libraries/ID-OmniSTR.ini` & `fdstools-2.1.0/fdstools/data/libraries/ID-OmniSTR.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-; IDseek OmniSTR library file for FDSTools v2.0.3.
+; IDseek OmniSTR library file for FDSTools v2.1.0.
 
 [genome_position]
 D1S1656     =  1, 230769584, 230769689
 TPOX        =  2,   1489646,   1489689
 D2S441      =  2,  68011912,  68011996
 D2S1338     =  2, 218014800, 218014953
 D3S1358     =  3,  45540738,  45540815
@@ -30,18 +30,18 @@
 PentaD      = 21,  43636196,  43636322
 D22S1045    = 22,  37140269,  37140342
 AmelogeninX =  X,  11296898,  11296955
 AmelogeninY =  Y,   6869871,   6869934
 DYS391      =  Y,  11982049,  11982159
 
 [flanks]
-SE33        = 16, TCACTCTTGTCRCCCA
-D20S482     = ACACYGAACCAATAAG, 16
-AmelogeninX = 16, CAGYTTCCCAGTTTAA
-AmelogeninY = TTAAACTGGGAARCTG, 16
+SE33        = REF, TCACTCTTGTCRCCCA
+D20S482     = ACACYGAACCAATAAG, REF
+AmelogeninX = REF, CAGYTTCCCAGTTTAA
+AmelogeninY = TTAAACTGGGAARCTG, REF
 
 [expected_allele_length]
 D1S1656     = 20
 TPOX        = 20
 D2S441      = 20
 D2S1338     = 20
 D3S1358     = 20
```

### Comparing `fdstools-2.0.4/fdstools/data/libraries/PowerSeq46GY.ini` & `fdstools-2.1.0/fdstools/data/libraries/PowerSeq46GY.ini`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/fdstools.py` & `fdstools-2.1.0/fdstools/fdstools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 #
-# Copyright (C) 2021 Jerry Hoogenboom
+# Copyright (C) 2023 Jerry Hoogenboom
 #
 # This file is part of FDSTools, data analysis tools for Massively
 # Parallel Sequencing of forensic DNA markers.
 #
 # FDSTools is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the
 # Free Software Foundation, either version 3 of the License, or (at
@@ -17,21 +17,23 @@
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with FDSTools.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 import argparse
-import os.path
+import importlib
 import pkgutil
 import re
 import sys
 import textwrap
 #import cProfile  # Imported only if the -d/--debug option is specified
 
+from pathlib import Path
+
 from . import tools, usage, version
 
 
 # Map tool names to argument parsers.
 tool_subparsers = {}
 
 
@@ -97,15 +99,15 @@
 #make_error_interceptor
 
 
 def main():
     """
     Main entry point.
     """
-    prog = os.path.splitext(os.path.basename(__file__))[0]
+    prog = Path(__file__).stem
     parser = argparse.ArgumentParser(formatter_class=_HelpFormatter, prog=prog,
                                      add_help=False, description=usage[0])
     parser.version = version(prog)
     make_error_interceptor(parser)
     parser.add_argument("-h", "--help", action=_HelpAction,
         default=argparse.SUPPRESS, nargs=argparse.REMAINDER,
         help="show this help message, or help for the specified TOOL, and exit")
@@ -115,20 +117,17 @@
     parser.add_argument("-d", "--debug", action="store_true",
         help="if specified, additional debug output is given")
     subparsers = parser.add_subparsers(title="available tools", dest="tool", metavar="TOOL",
         help="specify which tool to run")
     subparsers.required = True
 
     prefix = tools.__name__ + "."
-    for importer, name, ispkg in pkgutil.iter_modules(
-            path=[os.path.join(
-                os.path.dirname(os.path.abspath(__file__)),
-                "tools")]):
+    for importer, name, ispkg in pkgutil.iter_modules(tools.__path__):
         try:
-            module = importer.find_module(prefix + name).load_module(prefix + name)
+            module = importlib.import_module(prefix + name)
         except Exception as error:
             sys.stderr.write("FDSTools failed to load '%s': %s\n" % (name, error))
             continue
         subparser = subparsers.add_parser(
             name,
             formatter_class=_HelpFormatter,
             help=module.__doc__.split("\n\n", 1)[0],
```

### Comparing `fdstools-2.0.4/fdstools/lib/cli.py` & `fdstools-2.1.0/fdstools/lib/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,22 +83,27 @@
             return list_type(map(element_type, value.split(",")))
         except Exception as err:
             raise argparse.ArgumentTypeError(err)
     return parse_comma_separated_arg
 #comma_separated_arg
 
 
-def add_sequence_format_args(parser, *, default_format=None, force=False, require_library=False):
+def add_sequence_format_args(parser, *, default_format=None, force=False,
+                             require_library=False, ce_format=False):
     """Add arguments for sequence formatting to the given parser."""
     group = parser.add_argument_group("sequence format options")
     if force:
         group.set_defaults(sequence_format=default_format)
     else:
+        if ce_format:
+            choices = ("raw", "tssv", "allelename", "ce")
+        else:
+            choices = ("raw", "tssv", "allelename")
         group.add_argument("-F", "--sequence-format", metavar="FORMAT",
-            choices=("raw", "tssv", "allelename"), default=default_format,
+            choices=choices, default=default_format,
             help="convert sequences to the specified format: one of %(choices)s (default: " + (
                  "no conversion" if default_format is None else default_format)
                  + ")")
     if require_library:
         parser.add_argument("library", metavar="LIBRARY", type=library_arg,
             help="library file with marker definitions; custom file or built-in: '%s'" %
                 "', '".join(BUILTIN_NAMES))
```

### Comparing `fdstools-2.0.4/fdstools/lib/io.py` & `fdstools-2.1.0/fdstools/lib/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,17 +70,24 @@
     return alleles
 #parse_allelelist
 
 
 def read_sample_data_file(infile, data, annotation_column=None, seqformat=None, library=None,
                           default_marker=None, drop_special_seq=False, after_correction=False,
                           combine_strands=False, extra_columns=None):
-    """Add data from infile to data dict as [marker, sequence]=reads."""
+    """
+    Add data from infile to data dict as [marker, sequence]=reads.
+
+    extra_columns = {column_name_string: optional_boolean}
+    return {(marker, sequence): (reads, {column_name_string1: value1,
+    column_name_string2: value2})}
+    """
     # TODO: require keywords
     # Get column numbers.
+
     column_names = infile.readline().rstrip("\r\n").split("\t")
     if column_names == [""]:
         return []  # Empty file.
     colid_sequence = get_column_ids(column_names, "sequence")
     if combine_strands:
         colid_total = None
         numtype = int
@@ -121,14 +128,17 @@
         try:
             colid_annotation = get_column_ids(column_names, annotation_column)
         except:
             annotation_column = None
 
     found_alleles = []
     for line in infile:
+        if line.startswith("info_") or line.isspace():
+            continue
+
         line = line.rstrip("\r\n").split("\t")
         if drop_special_seq and line[colid_sequence] in SEQ_SPECIAL_VALUES:
             continue
         marker = line[colid_marker] if colid_marker is not None else default_marker
         sequence = line[colid_sequence] if seqformat is None else ensure_sequence_format(
             line[colid_sequence], seqformat, library=library, marker=marker)
         if annotation_column is not None and line[colid_annotation].startswith("ALLELE"):
```

### Comparing `fdstools-2.0.4/fdstools/lib/library.py` & `fdstools-2.1.0/fdstools/lib/library.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 #
-# Copyright (C) 2023 Jerry Hoogenboom
+# Copyright (C) 2024 Jerry Hoogenboom
 #
 # This file is part of FDSTools, data analysis tools for Massively
 # Parallel Sequencing of forensic DNA markers.
 #
 # FDSTools is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the
 # Free Software Foundation, either version 3 of the License, or (at
@@ -27,22 +27,22 @@
 from configparser import RawConfigParser, MissingSectionHeaderError
 from pathlib import Path
 from strnaming import classes, libstrnaming, libsequence
 
 from .seq import PAT_SEQ_RAW, PAT_SEQ_IUPAC
 
 # Patterns that match (parts of) an STR definition.
-PAT_STR_DEF = re.compile("^(?:(?:(?<=^)|(?<!^)\s+)[ACGT]+\s+\d+\s+\d+)*$")
-PAT_STR_DEF_BLOCK = re.compile("([ACGT]+)\s+(\d+)\s+(\d+)")
+PAT_STR_DEF = re.compile(r"^(?:(?:(?<=^)|(?<!^)\s+)[ACGT]+\s+\d+\s+\d+)*$")
+PAT_STR_DEF_BLOCK = re.compile(r"([ACGT]+)\s+(\d+)\s+(\d+)")
 
 # Pattern that matches a chromosome name/number.
-PAT_CHROMOSOME = re.compile("^(?:[Cc][Hh][Rr](?:[Oo][Mm])?)?([1-9XYM]|1\d|2[0-2])$")
+PAT_CHROMOSOME = re.compile(r"^(?:[Cc][Hh][Rr](?:[Oo][Mm])?)?([1-9XYM]|1\d|2[0-2])$")
 
 # Pattern to split a comma-, tab- or space-separated list.
-PAT_SPLIT = re.compile("\s*[, \t]\s*")
+PAT_SPLIT = re.compile(r"\s*[, \t]\s*")
 
 # TextWrapper object for formatting help texts in generated INI files.
 INI_COMMENT = textwrap.TextWrapper(width=79, initial_indent="; ",
     subsequent_indent="; ", break_on_hyphens=False)
 
 # Dict of built-in library files.
 BUILTIN_LIBS = {_.stem: _
@@ -82,15 +82,15 @@
             "Gapped or combined genomic range is not supported for STR marker %s" % marker)
 
     # Find units and overlong_gap.
     overlong_gap = ""
     units = {}
     for unit, min_repeats, max_repeats in blocks:
         if max_repeats == 1:
-            if len(unit) > max(libstrnaming.NAMING_OPTIONS["max_gap"], len(overlong_gap)):
+            if len(unit) > max(libstrnaming.MAX_GAP_LENGTH, len(overlong_gap)):
                 overlong_gap = unit
         else:
             units[unit] = units.get(unit, 0) + max_repeats
 
     # Start building refseq and stretches.
     flanks = options["flanks"]
     refseq = [flanks[0], prefix]
@@ -127,15 +127,15 @@
         else:
             # Move the positions of the last stretch.
             stretches[-1][0] += overlong_length
             stretches[-1][1] += overlong_length
 
     if stretches:
         # Make sure the structure is long enough to be accepted by STRNaming.
-        while end - stretches[0][0] < libstrnaming.NAMING_OPTIONS["min_structure_length"]:
+        while end - stretches[0][0] < libstrnaming.MIN_STRUCTURE_LENGTH:
             stretches[-1][1] += len(stretches[-1][2])
             end += len(stretches[-1][2])
             refseq[-1] += stretches[-1][2]
 
     # Add suffix.
     end += len(suffix)
     refseq.append(suffix)
@@ -153,45 +153,66 @@
             location -= len(flanks[0])
             length += len(flanks[0])
         refseq_store.add_refseq(genome_position[0], location, refseq[pos:pos+length])
         pos += length
     if stretches:
         struct_store.add_structure(genome_position[0],
             [[start, end, len(unit)] for start, end, unit in stretches])
+    options["autoload_reference"] = False
     if len(genome_position) > 3:
         return reported_range_store.add_complex_range(marker, genome_position, options=options)
     return reported_range_store.add_range(marker, genome_position[0], start, end, options=options)
 #add_legacy_range
 
 
 def parse_library(handle):
     """Parse an FDSTools library file as made with the library tool."""
     markers = {}
     ini = RawConfigParser()
     ini.optionxform = str
-    ini.readfp(handle)
+    ini.read_file(handle)
     for section in ini.sections():
         for marker in ini.options(section):
             value = ini.get(section, marker).split(";", 1)[0].strip()
             section_low = section.lower()
             if section_low == "flanks":
                 value = PAT_SPLIT.split(value)
                 if len(value) != 2:
                     raise ValueError(
-                        "For marker %s, %i flanking sequences were given, "
-                        "need exactly 2" % (marker, len(value)))
+                        "For marker %s, %i flanking sequences were given, need exactly two "
+                        "(note: specify 'REF' to automatically load genome reference)"
+                        % (marker, len(value)))
                 for i, val in enumerate(value):
-                    if PAT_SEQ_IUPAC.match(val) is None:
-                        try:
-                            value[i] = int(val)
-                            if value[i] < 1:
-                                raise ValueError
-                        except:
-                            raise ValueError(
-                                "Flanking sequence '%s' of marker %s is invalid" % (val, marker))
+                    if val == "REF":
+                        value[i] = ""
+                    elif val.isdigit():
+                        raise ValueError(
+                            "Specifying a flank length (%s for marker %s) in the [flanks] "
+                            "section of the library file is no longer supported. "
+                            "Use the [flank_length] section to specify marker-specific flank "
+                            "length limitations in the library file; specify 'REF' in the "
+                            "[flanks] section to automatically load genome reference"
+                            % (val, marker))
+                    elif PAT_SEQ_IUPAC.match(val) is None:
+                        raise ValueError(
+                            "Flanking sequence '%s' of marker %s is not a valid sequence "
+                            "(note: specify 'REF' to automatically load genome reference)"
+                            % (val, marker))
+            elif section_low == "flank_length":
+                value = PAT_SPLIT.split(value)
+                if len(value) != 4:
+                    raise ValueError(
+                        "Flank length should be four numbers, but %i values were "
+                        "given for marker %s" % (len(value), marker))
+                for i, val in enumerate(value):
+                    if not val.isdigit() or not int(val):
+                        raise ValueError(
+                            "Flank length '%s' of marker %s is not a valid positive "
+                            "integer" % (val, marker))
+                    value[i] = int(val)
             elif section_low in ("prefix", "suffix"):
                 if not PAT_SEQ_RAW.match(value):
                     raise ValueError(
                         "The %s sequence '%s' of marker %s is invalid (note: only one sequence "
                         "needs to be specified for reference)" % (section_low, value, marker))
             elif section_low == "genome_position":
                 value = PAT_SPLIT.split(value)
@@ -202,15 +223,15 @@
                 for i in range(1, len(value)):
                     try:
                         pos.append(int(value[i]))
                     except:
                         raise ValueError(
                             "Position '%s' of marker %s is not a valid integer"
                             % (value[i], marker))
-                    if not i % 2 and pos[-2] >= pos[-1]:
+                    if not i % 2 and pos[-2] > pos[-1]:
                         raise ValueError(
                             "End position %i of marker %s must be higher than "
                             "corresponding start position %i" % (pos[-1], marker, pos[-2]))
                 if len(value) == 1:
                     pos.append(1)
                 value = tuple(pos)
             elif section_low == "length_adjust":
@@ -302,15 +323,15 @@
             except KeyError:
                 raise ValueError("No genome_position or explicit repeat or no_repeat "
                                  "configuration provided for marker %s" % marker)
             if not len(genome_position) % 2:
                 raise ValueError(
                     "Invalid genomic position given for marker %s: need an odd number of values "
                     "(chromosome, start position, end position[, start2, end2, ...])" % marker)
-            if len(genome_position) == 3:
+            if len(genome_position) == 3 and "microhaplotype_positions" not in settings:
                 chromosome, start, end = genome_position
                 if chromosome not in ranges:
                     ranges[chromosome] = [(start, end + 1)]
                 else:
                     ranges[chromosome].append((start, end + 1))
 
     # Load the STR structures on the given ranges.
@@ -325,18 +346,14 @@
         options = {option: settings[option] for option in {"flanks", "max_expected_copies",
                 "expected_allele_length", "microhaplotype_positions"} & settings.keys()}
         if "explicit STR" in groups:
             # Legacy FDSTools-style definition of an STR marker.
             # TODO: Alias of STR markers was defined as excluding the prefix/suffix!
             if "flanks" not in options:
                 options["flanks"] = ("", "")
-            elif any(isinstance(flank, int) for flank in options["flanks"]):
-                raise ValueError(
-                    "Please specify an explit flanking sequence, not just a length, for marker %s"
-                        % marker)
             reported_range = add_legacy_range(reported_range_store, marker,
                 settings.get("prefix", ""),
                 settings.get("suffix", ""),
                 [(unit, int(min_repeats), int(max_repeats)) for unit, min_repeats, max_repeats in
                     PAT_STR_DEF_BLOCK.findall(settings.get("repeat", ""))],
                 options,
                 settings.get("genome_position", None))
@@ -344,18 +361,14 @@
                 reported_range.length_adjust -= settings["length_adjust"]
             if "block_length" in settings:
                 reported_range.block_length = settings["block_length"]
         elif "explicit non-STR" in groups:
             # Legacy FDSTools-style definition of a non-STR marker.
             if "flanks" not in options:
                 options["flanks"] = ("", "")
-            elif any(isinstance(flank, int) for flank in options["flanks"]):
-                raise ValueError(
-                    "Please specify an explit flanking sequence, not just a length, for marker %s"
-                        % marker)
             refseq = settings["no_repeat"]
             pos = None
             if "genome_position" in settings:
                 pos = settings["genome_position"]
 
                 # Sanity check: end position should reflect ref length.
                 length = sum(pos[i] - pos[i - 1] + 1 for i in range(2, len(pos), 2))
@@ -364,25 +377,25 @@
                         "Length of reference sequence of marker %s is %i bases, but "
                         "genome positions add up to %i bases" % (marker, len(refseq), length))
             add_legacy_range(reported_range_store, marker, refseq, "", [], options, pos)
         else:
             # Use STRNaming for this marker.
             # TODO: Alias of STR markers was defined as excluding the prefix/suffix!
             genome_position = settings["genome_position"]
-            if len(genome_position) == 3:
+            if len(genome_position) == 3 and "microhaplotype_positions" not in settings:
                 chromosome, start, end = genome_position
                 reported_range_store.add_range(
                     marker, chromosome, start, end + 1, options=options)
             else:
                 reported_range_store.add_complex_range(marker, genome_position, options=options)
 
         if "microhaplotype_positions" in settings:
             # Put Ns in reporting range refseq for microhaplotype markers.
             reported_range = reported_range_store.get_range(marker)
-            if reported_range.library:
+            if getattr(reported_range, "library", False):
                 raise ValueError(
                     "Cannot define microhaplotype positions for STR marker %s" % marker)
             refseq = list(reported_range.refseq)
             location = reported_range.location
             for position in settings["microhaplotype_positions"]:
                 refseq[libsequence.get_genome_pos(location, position, invert=True)] = "N"
             reported_range.refseq = "".join(refseq)
```

### Comparing `fdstools-2.0.4/fdstools/lib/noise.py` & `fdstools-2.1.0/fdstools/lib/noise.py`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/lib/seq.py` & `fdstools-2.1.0/fdstools/lib/seq.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,32 +23,32 @@
 import re
 
 from strnaming import libsequence
 
 # Patterns that match entire sequences.
 PAT_SEQ_RAW = re.compile("^[ACGT]*$")
 PAT_SEQ_IUPAC = re.compile("^[ACGTUWSMKRYBDHVN]*$")
-PAT_SEQ_TSSV = re.compile("^(?:[ACGT]+\(\d+\))*$")
+PAT_SEQ_TSSV = re.compile(r"^(?:[ACGT]+\(\d+\))*$")
 PAT_SEQ_ALLELENAME_STR = re.compile(
-    "^(?:CE)?-?\d+(?:\.\d+)?_"  # Second line: ACG[n][qA>C]GT[m]
-    "(?:[ACGT]+\[\d+\]|\[(?: ?\d+(?:\.1)?[ACGT-]+>[ACGT-]+)*\])*"
-    "(?:_[-+]\d+(?:\.1)?(?P<a>(?:(?<=\.1)-)|(?<!\.1)[ACGT]+)>"  # _+3A>
-        "(?!(?P=a))(?:[ACGT]+|-))*$")  # Portion of variants after '>'.
+    r"^(?:CE)?-?\d+(?:\.\d+)?_"  # Second line: ACG[n][qA>C]GT[m]
+    r"(?:[ACGT]+\[\d+\]|\[(?: ?\d+(?:\.1)?[ACGT-]+>[ACGT-]+)*\])*"
+    r"(?:_[-+]\d+(?:\.1)?(?P<a>(?:(?<=\.1)-)|(?<!\.1)[ACGT]+)>"  # _+3A>
+    "(?!(?P=a))(?:[ACGT]+|-))*$")  # Portion of variants after '>'.
 PAT_SEQ_ALLELENAME_SNP = re.compile(
-    "^REF$|^(?:(?:(?<=^)|(?<!^) )"  # 'REF' or space-separated variants.
-    "\d+(?:\.1)?(?P<a>(?:(?<=\.1)-)|(?<!\.1)[ACGT]+)>"
-        "(?!(?P=a))(?:[ACGT]+|-))+$")  # Portion of variants after '>'.
+    r"^REF$|^(?:(?:(?<=^)|(?<!^) )"  # 'REF' or space-separated variants.
+    r"\d+(?:\.1)?(?P<a>(?:(?<=\.1)-)|(?<!\.1)[ACGT]+)>"
+    "(?!(?P=a))(?:[ACGT]+|-))+$")  # Portion of variants after '>'.
 PAT_SEQ_ALLELENAME_MH = re.compile(
     "^MH_[ACGTN]*"  # Next line: variants preceded by '_', ref may have N.
-    "(?:_\d+(?:\.1)?(?P<a>(?:(?<=\.1)-)|(?<!\.1)[ACGTN]+)>"
-        "(?!(?P=a))(?:[ACGT]+|-))*$")  # Portion of variants after '>'.
+    r"(?:_\d+(?:\.1)?(?P<a>(?:(?<=\.1)-)|(?<!\.1)[ACGTN]+)>"
+    "(?!(?P=a))(?:[ACGT]+|-))*$")  # Portion of variants after '>'.
 PAT_SEQ_ALLELENAME_MT = re.compile(
     "^REF$|^(?:(?:(?<=^)|(?<!^) )"  # 'REF' or space-separated variants.
-    "(?:-?\d+\.\d+[ACGT]|(?P<a>[ACGT])?\d+(?(a)(?!(?P=a)))(?:[ACGT-]|DEL)))+$")
-PAT_VARIANT_MH = re.compile("^(\d+)([ACGTN]*N[ACGTN]*)>([ACGT-]+)$")
+    r"(?:-?\d+\.\d+[ACGT]|(?P<a>[ACGT])?\d+(?(a)(?!(?P=a)))(?:[ACGT-]|DEL)))+$")
+PAT_VARIANT_MH = re.compile(r"^(\d+)([ACGTN]*N[ACGTN]*)>([ACGT-]+)$")
 PAT_SEQ_OR_N = re.compile("[ACGT]+|N")
 
 # Special values that may appear in the place of a sequence.
 SEQ_SPECIAL_VALUES = ("No data", "Other sequences")
 
 
 # The following functions are moved to STRNaming.
```

### Comparing `fdstools-2.0.4/fdstools/lib/sg_align.c` & `fdstools-2.1.0/fdstools/lib/sg_align.c`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/lib/util.py` & `fdstools-2.1.0/fdstools/lib/util.py`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/tools/allelefinder.py` & `fdstools-2.1.0/fdstools/tools/allelefinder.py`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/tools/bganalyse.py` & `fdstools-2.1.0/fdstools/tools/bganalyse.py`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/tools/bgcorrect.py` & `fdstools-2.1.0/fdstools/tools/bgcorrect.py`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/tools/bgestimate.py` & `fdstools-2.1.0/fdstools/tools/bgestimate.py`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/tools/bghomraw.py` & `fdstools-2.1.0/fdstools/tools/bghomraw.py`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/tools/bghomstats.py` & `fdstools-2.1.0/fdstools/tools/bghomstats.py`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/tools/bgmerge.py` & `fdstools-2.1.0/fdstools/tools/bgmerge.py`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/tools/bgpredict.py` & `fdstools-2.1.0/fdstools/tools/bgpredict.py`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/tools/findnewalleles.py` & `fdstools-2.1.0/fdstools/tools/findnewalleles.py`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/tools/libconvert.py` & `fdstools-2.1.0/fdstools/tools/libconvert.py`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/tools/library.py` & `fdstools-2.1.0/fdstools/tools/library.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 from configparser import RawConfigParser
 from errno import EPIPE
 from types import MethodType
 
 from ..lib.library import BUILTIN_LIBS, BUILTIN_NAMES, INI_COMMENT
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 
 def ini_add_comment(ini, section, comment):
     for line in INI_COMMENT.wrap(comment):
         ini.set(section, line)
 #ini_add_comment
 
@@ -82,15 +82,15 @@
             "mtDNA fragments starts near the end of the reference sequence "
             "and continues at the beginning, you can obtain correct base "
             "numbering by specifying the fragment's genome position as \"M, "
             "(starting position), 16569, 1, (ending position)\". This tells "
             "FDSTools that the marker is a concatenation of two fragments, "
             "where the first fragment ends at position 16569 and the second "
             "fragment starts at position 1. Similarly, for a fragment that "
-            "spans position 3107 in the rCRS (which is nonexistent), you may "
+            "spans position 3107 in the rCRS (which is nonexistent), you must "
             "specify \"M, (starting position), 3106, 3108, (ending "
             "position)\".")
     if microhaplotypes or type == "full":
         ini.add_section("microhaplotype_positions")
         ini.add_comment("microhaplotype_positions",
             "For each microhaplotype marker, specify one or more positions of SNPs that should "
             "be reported as part of the microhaplotype.%s" % (
@@ -105,21 +105,27 @@
         "of each marker (e.g., primer sequences) to identify which input reads correspond to "
         "which marker. %s The sequence may contain IUPAC codes for ambiguous positions to account "
         "for degenerate bases in the primers or for bisulfite-converted targets in methylation-"
         "based studies (e.g., Y matches either C or T)." % (
             "Specify two comma-separated values: left flank and right flank sequence, in the same "
             "sequence orientation (strand)."
                 if type in ("str", "non-str") else
-            ("The default length of the anchor sequences used can be specified as an argument to "
-            "the TSSV tool. Individual alternative lengths can be specified here for each marker. "
-            "Specify two comma-separated values: one for the left and one for the right flank. "
-            "The value can be a number (the length of sequence to use) or an explicit anchor "
-            "sequence to use.%s" % (
+            ("By default, flanking sequence is loaded from the genome reference sequence, but an "
+            "alternative sequence can be specified here. To do so, provide two comma-separated "
+            "values: one for the left and one for the right flank. Each value can be 'REF' or an "
+            "explicit anchor sequence to use.%s" % (
                 " For markers configured explicitly in this library file, the anchor sequences "
-                "must be specified explicitly as well." if type == "full" else ""))))
+                "MUST be specified explicitly as well." if type == "full" else ""))))
+    ini.add_section("flank_length")
+    ini.add_comment("flank_length",
+        "The number of flanking bases used by TSSV can be controlled with the -L/--flank-length "
+        "option of that tool. If the flank length of a specific marker needs to be limited to a "
+        "specific value or range of values, this can be specified here. Provide four numbers "
+        "for each such marker: the minimum and maximum possible length for the left flank, "
+        "followed by the minimum and maximum possible length for the right flank.")
     ini.add_section("max_expected_copies")
     ini.add_comment("max_expected_copies",
         "By default, the Allelefinder tool will report up to 2 alleles per marker, but only a "
         "single allele for markers %son the Y chromosome. If this is incorrect, specify the "
         "maximum expected number of copies (i.e., alleles) for each marker in a "
         "single-contributor reference sample here." % (
             "on mitochondrial DNA or " if type != "str" else ""))
```

### Comparing `fdstools-2.0.4/fdstools/tools/pipeline.py` & `fdstools-2.1.0/fdstools/tools/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 #
-# Copyright (C) 2021 Jerry Hoogenboom
+# Copyright (C) 2023 Jerry Hoogenboom
 #
 # This file is part of FDSTools, data analysis tools for Massively
 # Parallel Sequencing of forensic DNA markers.
 #
 # FDSTools is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the
 # Free Software Foundation, either version 3 of the License, or (at
@@ -43,14 +43,15 @@
 analysis).
 
 All settings in the configuration file correspond to options of various
 tools in FDSTools.  Please refer to the tool-specific help for a full
 description of each tool.  Type 'fdstools -h TOOL' to get help with the
 given TOOL.
 """
+import importlib
 import os
 import pkgutil
 import re
 import subprocess
 import sys
 import tempfile
 import threading
@@ -61,15 +62,15 @@
 from functools import reduce
 
 from ..lib.cli import DEF_TAG_EXPR, DEF_TAG_FORMAT, get_tag, regex_arg, glob_path
 from ..lib.io import print_db
 from ..lib.library import INI_COMMENT
 
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 
 # Pattern to split a quoted string.
 PAT_SPLIT_QUOTED = re.compile(r""""((?:\\"|[^"])*)"|'((?:\\'|[^'])*)'|(\S+)""")
 
 # Pattern that matches a long argparse argument name.
 PAT_ARGNAME = re.compile("^(?:--)?([a-z0-9]+(?:-[a-z0-9]+)*)$")
@@ -209,21 +210,19 @@
             "-o/--output", "'outfiles'") % format_args)
     return INI_COMMENT.fill(text[:1].upper() + text[1:])
 #format_help
 
 
 def get_tools(hide_pipeline):
     tools = {}
-    for importer, name, ispkg in pkgutil.iter_modules(
-            path=fdstools.tools.__path__):
+    for importer, name, ispkg in pkgutil.iter_modules(fdstools.tools.__path__):
         if hide_pipeline and name == NAME:
             continue
         try:
-            tools[name] = importer.find_module(PACKAGE_PREFIX + name).load_module(
-                PACKAGE_PREFIX + name)
+            tools[name] = importlib.import_module(PACKAGE_PREFIX + name)
         except Exception as error:
             sys.stderr.write("FDSTools failed to load '%s': %s\n" % (name, error))
             continue
     return tools
 #get_tools
 
 
@@ -234,15 +233,15 @@
     return collector.get_argument_lists()
 #get_arguments
 
 
 def read_ini(infile):
     config = RawConfigParser()
     config.optionxform = str
-    config.readfp(infile)
+    config.read_file(infile)
     return config
 #read_ini
 
 
 def parse_bool_arg(section, option, value):
     if value.lower() in ("false", "no", "off", "0", ""):
         return False
@@ -966,8 +965,8 @@
         write_ini(args)
         args.config.close()
     else:
         raise ValueError(
             "Configuration file '%s' does not exist; if you wish to create a "
             "default configuration file, please specify the type of analysis "
             "pipeline using the -a/--analysis option" % args.config)
-#run
+#run
```

### Comparing `fdstools-2.0.4/fdstools/tools/samplestats.py` & `fdstools-2.1.0/fdstools/tools/samplestats.py`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/tools/seqconvert.py` & `fdstools-2.1.0/fdstools/tools/seqconvert.py`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/tools/stuttermark.py` & `fdstools-2.1.0/fdstools/tools/stuttermark.py`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/tools/stuttermodel.py` & `fdstools-2.1.0/fdstools/tools/stuttermodel.py`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/tools/tssv.py` & `fdstools-2.1.0/fdstools/tools/tssv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 #
-# Copyright (C) 2022 Jerry Hoogenboom
+# Copyright (C) 2024 Jerry Hoogenboom
 #
 # This file is part of FDSTools, data analysis tools for Massively
 # Parallel Sequencing of forensic DNA markers.
 #
 # FDSTools is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the
 # Free Software Foundation, either version 3 of the License, or (at
@@ -72,15 +72,15 @@
 
 from ..lib.cli import add_sequence_format_args, add_input_output_args, pos_int_arg,\
                       get_input_output_files
 from ..lib.io import try_write_pipe
 from ..lib.seq import PAT_SEQ_RAW, reverse_complement, ensure_sequence_format
 from ..lib.sg_align import align
 
-__version__ = "2.1.1"
+__version__ = "2.2.0"
 
 
 # Default values for parameters are specified below.
 
 # Default flanking sequence length.
 # This value can be overridden by the -L command line option.
 _DEF_FLANK_LENGTH = 16
@@ -114,22 +114,37 @@
         self.lock = Lock()
 
         # Convert library.
         refseq_store = library.get_structure_store().get_refseq_store()
         self.has_iupac = False
         self.tssv_library = {}
         for marker, reported_range in library.get_ranges().items():
-            flanks = list(reported_range.get_option("flanks", (flank_length, flank_length)))
-            if not all(flanks):
-                raise ValueError("Missing flanking sequence for marker %s" % marker)
+            flanks = list(reported_range.get_option("flanks", ["", ""]))
+            left_min, left_max, right_min, right_max = reported_range.get_option(
+                "flank_length", [flank_length] * 4)
+            left_length = sorted((left_min, flank_length, left_max))[1]
+            right_length = sorted((right_min, flank_length, right_max))[1]
+            autoload_reference = reported_range.get_option("autoload_reference")
             chromosome, start, *_, end = reported_range.location
-            if isinstance(flanks[0], int):
-                flanks[0] = refseq_store.get_refseq(chromosome, start - flanks[0], start)
-            if isinstance(flanks[1], int):
-                flanks[1] = refseq_store.get_refseq(chromosome, end + 1, end + 1 + flanks[1])
+            if left_length > len(flanks[0]):
+                # Extend left flank (to the left) with reference bases.
+                flanks[0] = refseq_store.get_refseq(
+                    chromosome, start - left_length, start - len(flanks[0]),
+                    autoload=autoload_reference) + flanks[0]
+            elif left_length < len(flanks[0]):
+                # Cut bases from the left end of the left flank.
+                flanks[0] = flanks[0][-left_length:]
+            if right_length > len(flanks[1]):
+                # Extend right flank (to the right) with reference bases.
+                flanks[1] += refseq_store.get_refseq(
+                    chromosome, end + len(flanks[1]) + 1, end + right_length + 1,
+                    autoload=autoload_reference)
+            elif right_length < len(flanks[1]):
+                # Cut bases from the right end of the right flank.
+                flanks[1] = flanks[1][:right_length]
             flanks[1] = reverse_complement(flanks[1])
             translate_flank = [0 if PAT_SEQ_RAW.match(flank) else 1 for flank in flanks]
             if any(translate_flank):
                 self.has_iupac = True
             pair = tuple((flank.translate(IUPAC_BITS) if trans else flank, trans)
                 for flank, trans in zip(flanks, translate_flank))
             self.tssv_library[marker] = (
@@ -410,19 +425,19 @@
     right_dist, right_pos = align(
         reference_rc[pair[1][1]], pair[1][0], indel_score, bitwise=pair[1][1])
     return (left_dist, left_pos), (right_dist, len(reference[0]) - right_pos)
 #align_pair
 
 
 def relative_distance(reference, sequence):
-    """Return (pct_changed, -len(reference))."""
+    """Return 2 * hamming_distance(ref, seq) - len(reference)."""
     len_reference = len(reference)
     if len_reference > len(sequence):
-        return (align(reference, sequence, 1, global_align=1)[0] / len_reference, -len_reference)
-    return (align(sequence, reference, 1, global_align=1)[0] / len_reference, -len_reference)
+        return 2 * align(reference, sequence, 1, global_align=1)[0] - len_reference
+    return 2 * align(sequence, reference, 1, global_align=1)[0] - len_reference
 #relative_distance
 
 
 def prune_matched_ranges(tssv_library, matched_ranges):
     """Removes overlapping ranges from the provided list."""
     if len(matched_ranges) < 2:
         return
@@ -439,16 +454,16 @@
                     y[1] - (y[1]-y[0])//2 <= matched_ranges[i][0])
                     for y in matched_ranges[group_start:i]):
             # End of group with at least 50% pairwise overlap.
             if i - group_start > 1:
                 # Overlapping group; eliminate the worst fit iteratively.
                 if not group_scores:
                     group_scores = [relative_distance(tssv_library[marker][2], seq)
-                        for start, end, seq, strand, marker in matched_ranges]
-                worst_range_index = group_scores.index(max(group_scores[:i - group_start]))
+                        for start, end, seq, strand, marker in matched_ranges[group_start : i]]
+                worst_range_index = group_scores.index(max(group_scores))
                 del matched_ranges[group_start + worst_range_index]
                 del group_scores[worst_range_index]
                 i = group_start + 1
                 continue
             # Group consisted of a single range; new group starts here.
             group_scores = group_scores[1:]
             group_start = i
@@ -645,16 +660,15 @@
 
 
 def add_arguments(parser):
     add_sequence_format_args(parser, default_format="raw", force=False, require_library=True)
     add_input_output_args(parser, single_in=True, batch_support=False, report_out=True)
     parser.add_argument("-L", "--flank-length", metavar="N", type=pos_int_arg,
         default=_DEF_FLANK_LENGTH,
-        help="length of anchor (flanking) sequences to use, if not specified in the library file "
-             "(default: %(default)s)")
+        help="length of anchor (flanking) sequences to use (default: %(default)s)")
     parser.add_argument("-D", "--dir",
         help="output directory for verbose output; when given, a subdirectory "
              "will be created for each marker, each with a separate "
              "sequences.csv file and a number of FASTA/FASTQ files containing "
              "unrecognised reads (unknown.fa), recognised reads "
              "(Marker/paired.fa), and reads that lack one of the flanks of a "
              "marker (Marker/noend.fa and Marker/nostart.fa)")
```

### Comparing `fdstools-2.0.4/fdstools/tools/vis.py` & `fdstools-2.1.0/fdstools/tools/vis.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 import re
 import sys
 
 from errno import EPIPE
 
 from ..lib.cli import pos_int_arg
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 
 # Default values for parameters are specified below.
 
 # Default minimum number of reads to require.
 # This value can be overridden by the -n command line option.
 _DEF_THRESHOLD_ABS = 5
@@ -143,18 +143,18 @@
 
 # Default data file that Vega will read when -V/--vega is specified
 # without providing data to embed in the file.
 # It is currently impossible to override this value.
 _DEF_DATA_FILENAME = "data.csv"
 
 
-_PAT_LIBRARIES = re.compile("<!--\s*BEGIN_LIBRARIES\s*-->\s*(.*?)\s*"
-                            "<!--\s*END_LIBRARIES\s*-->", flags=re.DOTALL)
-_PAT_LOAD_SCRIPT = re.compile("<!--\s*BEGIN_LOAD_SCRIPT\s*-->\s*(.*?)\s*"
-                              "<!--\s*END_LOAD_SCRIPT\s*-->", flags=re.DOTALL)
+_PAT_LIBRARIES = re.compile(r"<!--\s*BEGIN_LIBRARIES\s*-->\s*(.*?)\s*"
+                            r"<!--\s*END_LIBRARIES\s*-->", flags=re.DOTALL)
+_PAT_LOAD_SCRIPT = re.compile(r"<!--\s*BEGIN_LOAD_SCRIPT\s*-->\s*(.*?)\s*"
+                              r"<!--\s*END_LOAD_SCRIPT\s*-->", flags=re.DOTALL)
 
 _SCRIPT_BEGIN = '<script type="text/javascript">'
 _SCRIPT_END = "</script>"
 
 _EXTERNAL_LIBRARIES = ("vis/d3.min.js", "vis/vega.min.js")
```

### Comparing `fdstools-2.0.4/fdstools/vis/allelevis/allelevis.json` & `fdstools-2.1.0/fdstools/vis/allelevis/allelevis.json`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/vis/allelevis/index.html` & `fdstools-2.1.0/fdstools/vis/allelevis/index.html`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/vis/bganalysevis/bganalysevis.json` & `fdstools-2.1.0/fdstools/vis/bganalysevis/bganalysevis.json`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/vis/bganalysevis/index.html` & `fdstools-2.1.0/fdstools/vis/bganalysevis/index.html`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/vis/bgrawvis/bgrawvis.json` & `fdstools-2.1.0/fdstools/vis/bgrawvis/bgrawvis.json`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/vis/bgrawvis/index.html` & `fdstools-2.1.0/fdstools/vis/bgrawvis/index.html`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/vis/d3.min.js` & `fdstools-2.1.0/fdstools/vis/d3.min.js`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/vis/profilevis/index.html` & `fdstools-2.1.0/fdstools/vis/profilevis/index.html`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/vis/profilevis/profilevis.json` & `fdstools-2.1.0/fdstools/vis/profilevis/profilevis.json`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/vis/samplevis/index.html` & `fdstools-2.1.0/fdstools/vis/samplevis/index.html`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/vis/samplevis/samplevis.json` & `fdstools-2.1.0/fdstools/vis/samplevis/samplevis.json`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/vis/samplevis/warning.svg` & `fdstools-2.1.0/fdstools/vis/samplevis/warning.svg`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/vis/stuttermodelvis/index.html` & `fdstools-2.1.0/fdstools/vis/stuttermodelvis/index.html`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/vis/stuttermodelvis/stuttermodelvis.json` & `fdstools-2.1.0/fdstools/vis/stuttermodelvis/stuttermodelvis.json`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools/vis/vega.min.js` & `fdstools-2.1.0/fdstools/vis/vega.min.js`

 * *Files identical despite different names*

### Comparing `fdstools-2.0.4/fdstools.egg-info/PKG-INFO` & `fdstools-2.1.0/fdstools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdstools
-Version: 2.0.4
+Version: 2.1.0
 Summary: Forensic DNA Sequencing Tools
 Home-page: https://fdstools.nl
 Author: Jerry Hoogenboom
 Author-email: jerryhoogenboom@outlook.com
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/Jerrythafast/FDSTools/issues
 Project-URL: Source Code, https://github.com/Jerrythafast/FDSTools
@@ -16,14 +16,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Legal Industry
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: LICENSES-3RD-PARTY.txt
+Requires-Dist: numpy>=1.17
+Requires-Dist: strnaming~=1.2.0
 
 Forensic DNA Sequencing Tools
 =============================
 Tools for filtering and interpretation of Massively Parallel Sequencing data of
 forensic DNA samples. To obtain a list of included tools with a brief
 description of each tool, run:
 
@@ -48,14 +50,35 @@
 Alternatively, FDSTools can be installed by running:
 
     python setup.py install
 
 
 Release Notes
 -------------
+### Version 2.1.0 (2024-04-30)
+Updated STRNaming nomenclature to version 1.2. Please note that this is a
+backwards incompatible update: this version of FDSTools is unable to correctly
+interpret allele names that were produced with a prior version!
+Please see https://fdstools.nl/strnaming/updates for more information.
+
+Changed interpretation of the [flanks] section in the library file: it can no
+longer contain numbers, but the value 'REF' can be specified to indicate that
+GRCh38 reference sequence should be used (which was already the default).
+A new [flank_length] section is introduced to allow specifying marker-specific
+minimum and maximum (or exact) flanking sequence length; the value specified
+for TSSV's -L/--flank-length option is then clamped between these values.
+If a [flanks] section is present and contains a short sequence (possibly with
+IUPAC codes), it is implicitly extended with GRCh38 reference sequence to the
+requested length by TSSV.
+
+Greatly improved handling of microhaplotype markers, and we finally introduced
+the first suite of component tests, covering Allelefinder, Seqconvert,
+Stuttermark and TSSV. Welcome to the team, Brechtje!
+
+
 ### Version 2.0.4 (2023-03-02)
 Microhaplotype alleles with SNPs adjacent to any of the microhaplotype
 positions are now recognised. For example, an allele previously named
 "MH_N_123NC>GA" will now be named "MH_G_124C>A" instead.
 
 Greatly improved loading speed for large library files.
```

### Comparing `fdstools-2.0.4/fdstools.egg-info/SOURCES.txt` & `fdstools-2.1.0/fdstools.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 fdstools/tools/bghomraw.py
 fdstools/tools/bghomstats.py
 fdstools/tools/bgmerge.py
 fdstools/tools/bgpredict.py
 fdstools/tools/findnewalleles.py
 fdstools/tools/libconvert.py
 fdstools/tools/library.py
+fdstools/tools/mps2ce.py
 fdstools/tools/pipeline.py
 fdstools/tools/samplestats.py
 fdstools/tools/seqconvert.py
 fdstools/tools/stuttermark.py
 fdstools/tools/stuttermodel.py
 fdstools/tools/tssv.py
 fdstools/tools/vis.py
```

### Comparing `fdstools-2.0.4/setup.py` & `fdstools-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 #
-# Copyright (C) 2023 Jerry Hoogenboom
+# Copyright (C) 2024 Jerry Hoogenboom
 #
 # This file is part of FDSTools, data analysis tools for Massively
 # Parallel Sequencing of forensic DNA markers.
 #
 # FDSTools is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Public License as published by the
 # Free Software Foundation, either version 3 of the License, or (at
@@ -64,15 +64,15 @@
     ext_modules=[
         setuptools.extension.Extension("fdstools.lib.sg_align",
             sources=["fdstools/lib/sg_align.c"],
             extra_compile_args=["-O3"])],
     package_data={
         "fdstools": ["vis/*.*", "vis/*/*", "data/libraries/*.ini"]
     },
-    install_requires=["numpy>=1.17", "strnaming~=1.1.4"],
+    install_requires=["numpy>=1.17", "strnaming~=1.2.0"],
     python_requires=">=3.5",
     entry_points={
         "console_scripts": [
             "fdstools=fdstools.fdstools:main"
         ]
     }
 )
```

