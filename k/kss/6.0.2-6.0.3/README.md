# Comparing `tmp/kss-6.0.2.tar.gz` & `tmp/kss-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kss-6.0.2.tar", last modified: Sun Apr 28 14:10:23 2024, max compression
+gzip compressed data, was "kss-6.0.3.tar", last modified: Tue Apr 30 18:37:40 2024, max compression
```

## Comparing `kss-6.0.2.tar` & `kss-6.0.3.tar`

### file list

```diff
@@ -1,236 +1,238 @@
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.275951 kss-6.0.2/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1569 2024-04-01 04:29:21.000000 kss-6.0.2/LICENSE
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      379 2024-04-28 13:40:34.000000 kss-6.0.2/MANIFEST.in
--rw-r--r--   0 hyunwoongko   (501) staff       (20)   162021 2024-04-28 14:10:23.276173 kss-6.0.2/PKG-INFO
--rw-r--r--   0 hyunwoongko   (501) staff       (20)   161269 2024-04-28 14:10:14.000000 kss-6.0.2/README.md
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.250137 kss-6.0.2/bench/
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.255436 kss-6.0.2/bench/sentence_split/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.2/bench/sentence_split/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4379 2024-04-27 14:55:22.000000 kss-6.0.2/bench/sentence_split/sentence_split.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      615 2024-04-27 14:55:22.000000 kss-6.0.2/bench/sentence_split/test_baseline.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      600 2024-04-27 14:55:22.000000 kss-6.0.2/bench/sentence_split/test_kiwi.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1015 2024-04-27 14:55:22.000000 kss-6.0.2/bench/sentence_split/test_koalanlp.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      700 2024-04-27 14:55:22.000000 kss-6.0.2/bench/sentence_split/test_kss.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      587 2024-04-27 14:55:22.000000 kss-6.0.2/bench/sentence_split/test_word_split.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.255866 kss-6.0.2/csrc/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2024-03-31 20:12:01.000000 kss-6.0.2/csrc/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      563 2024-03-31 20:36:14.000000 kss-6.0.2/csrc/kss_cython.pyx
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5965 2024-03-31 20:12:01.000000 kss-6.0.2/csrc/sentence_splitter.cpp
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7830 2024-03-31 20:12:01.000000 kss-6.0.2/csrc/sentence_splitter.h
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.255993 kss-6.0.2/kss/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7569 2024-04-28 14:08:30.000000 kss-6.0.2/kss/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.257135 kss-6.0.2/kss/_elements/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.2/kss/_elements/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4888 2023-08-22 23:38:03.000000 kss-6.0.2/kss/_elements/element.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2702 2023-08-22 23:38:03.000000 kss-6.0.2/kss/_elements/empty.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      536 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_elements/subclasses.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.257239 kss-6.0.2/kss/_modules/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.2/kss/_modules/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.257751 kss-6.0.2/kss/_modules/augmentation/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/augmentation/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.257856 kss-6.0.2/kss/_modules/augmentation/assets/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)  4865459 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/augmentation/assets/wordnet.json
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3892 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/augmentation/augment.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3251 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/augmentation/distance.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3602 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/augmentation/replacement.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1411 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/augmentation/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.260839 kss-6.0.2/kss/_modules/collocation/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/collocation/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     9351 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/collocation/collocate.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.261554 kss-6.0.2/kss/_modules/g2p/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/g2p/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.261887 kss-6.0.2/kss/_modules/g2p/assets/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2634 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/g2p/assets/idioms.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    14802 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/g2p/assets/rules.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5390 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/g2p/assets/table.csv
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6586 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/g2p/english.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7191 2024-04-28 13:55:26.000000 kss-6.0.2/kss/_modules/g2p/g2p.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4459 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/g2p/numerals.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2722 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/g2p/regular.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4949 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/g2p/special.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     8131 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/g2p/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.262086 kss-6.0.2/kss/_modules/hangulization/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3616 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulization.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.262633 kss-6.0.2/kss/_modules/hangulization/hangulize/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2277 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    10423 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/hangul.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.262740 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1426 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.262851 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/aze/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5272 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/aze/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.262962 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/bel/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5425 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/bel/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.263071 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/bul/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4925 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/bul/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.263173 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/cat/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4328 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/cat/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.263284 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/ces/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4820 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/ces/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.263391 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/cym/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5791 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/cym/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.263502 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/deu/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7415 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/deu/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.263603 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/ell/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     9068 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/ell/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.263714 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/epo/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4103 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/epo/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.263833 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/est/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3931 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/est/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.263935 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/fin/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3410 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/fin/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.264039 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/grc/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     8626 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/grc/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.264152 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/hbs/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5606 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/hbs/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.264361 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/hun/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4990 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/hun/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.264532 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/isl/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5626 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/isl/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.264701 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/ita/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4371 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/ita/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.264828 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/jpn/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4446 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/jpn/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.265038 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/kat/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6118 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/kat/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6408 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/kat/narrow.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.265157 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/lat/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3314 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/lat/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.265269 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/lav/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4116 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/lav/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.265371 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/lit/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4080 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/lit/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.265491 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/mkd/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5354 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/mkd/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.265601 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/nld/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    22064 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/nld/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.265738 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/pol/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5785 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/pol/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.265948 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/por/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6048 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/por/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6056 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/por/br.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.266055 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/ron/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5120 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/ron/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.266161 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/rus/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4994 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/rus/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.266271 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/slk/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6693 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/slk/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.266372 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/slv/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3836 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/slv/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.266482 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/spa/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4002 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/spa/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.266588 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/sqi/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3177 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/sqi/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.266695 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/swe/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7896 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/swe/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.266802 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/tur/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3528 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/tur/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.266903 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/ukr/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5072 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/ukr/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.267018 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/vie/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4742 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/vie/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.267126 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/wlm/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5599 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/langs/wlm/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    16108 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/models.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1069 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/normalization.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2897 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hangulization/hangulize/processing.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.267431 kss-6.0.2/kss/_modules/hanja/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hanja/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4462 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hanja/_hanja.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2021 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/hanja/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.267728 kss-6.0.2/kss/_modules/jamo/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/jamo/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    12624 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/jamo/_jamo.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      912 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/jamo/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.268005 kss-6.0.2/kss/_modules/josa/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/josa/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2580 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/josa/josa.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7030 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/josa/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.268290 kss-6.0.2/kss/_modules/keywords/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/keywords/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6529 2024-04-28 13:58:52.000000 kss-6.0.2/kss/_modules/keywords/extract_keywords.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    17289 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/keywords/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.269018 kss-6.0.2/kss/_modules/morphemes/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.2/kss/_modules/morphemes/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2652 2024-03-31 13:42:10.000000 kss-6.0.2/kss/_modules/morphemes/analyzers.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1849 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/morphemes/split_morphemes.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3588 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/morphemes/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.269222 kss-6.0.2/kss/_modules/paradigm/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/paradigm/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    18316 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/paradigm/paradigm.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.270483 kss-6.0.2/kss/_modules/preprocessing/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/preprocessing/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    15538 2024-04-27 14:56:06.000000 kss-6.0.2/kss/_modules/preprocessing/anonymize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    29795 2024-04-27 14:58:49.000000 kss-6.0.2/kss/_modules/preprocessing/clean_news.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    81165 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/preprocessing/completed_form.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    24570 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/preprocessing/filter_out.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2088 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/preprocessing/half2full.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6056 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/preprocessing/normalize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    26257 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/preprocessing/preprocess.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7186 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/preprocessing/reduce_repeats.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     7661 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/preprocessing/remove_invisible_chars.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.270775 kss-6.0.2/kss/_modules/qwerty/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/qwerty/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6262 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/qwerty/qwerty.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5941 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/qwerty/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.271058 kss-6.0.2/kss/_modules/romanization/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/romanization/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5813 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/romanization/romanize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     8901 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/romanization/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.271343 kss-6.0.2/kss/_modules/safety/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/safety/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3531 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/safety/check_safety.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    35374 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/safety/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.272248 kss-6.0.2/kss/_modules/sentences/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.2/kss/_modules/sentences/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     9334 2023-08-22 23:38:03.000000 kss-6.0.2/kss/_modules/sentences/embracing_processor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    22898 2023-08-22 23:38:03.000000 kss-6.0.2/kss/_modules/sentences/sentence_postprocessor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6751 2024-03-31 07:55:02.000000 kss-6.0.2/kss/_modules/sentences/sentence_preprocessor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2298 2023-08-22 23:38:03.000000 kss-6.0.2/kss/_modules/sentences/sentence_processor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    30242 2023-08-22 23:38:03.000000 kss-6.0.2/kss/_modules/sentences/sentence_splitter.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    13304 2024-03-31 20:36:14.000000 kss-6.0.2/kss/_modules/sentences/sentence_splitter_fast.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     8322 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/sentences/split_sentences.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.272535 kss-6.0.2/kss/_modules/spacing/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/spacing/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5539 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/spacing/correct_spacing.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)   296979 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/spacing/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.273028 kss-6.0.2/kss/_modules/summarization/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.2/kss/_modules/summarization/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5603 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/summarization/summarize_sentences.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3396 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_modules/summarization/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.273774 kss-6.0.2/kss/_utils/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.2/kss/_utils/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       66 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_utils/api.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    10329 2024-03-31 07:46:03.000000 kss-6.0.2/kss/_utils/const.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1399 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_utils/emojis.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      910 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_utils/logger.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1001 2023-08-22 23:38:03.000000 kss-6.0.2/kss/_utils/multiprocessing.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    17275 2024-04-27 14:55:22.000000 kss-6.0.2/kss/_utils/sanity_checks.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.256732 kss-6.0.2/kss.egg-info/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)   162021 2024-04-28 14:10:23.000000 kss-6.0.2/kss.egg-info/PKG-INFO
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6374 2024-04-28 14:10:23.000000 kss-6.0.2/kss.egg-info/SOURCES.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-28 14:10:23.000000 kss-6.0.2/kss.egg-info/dependency_links.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-27 14:04:55.000000 kss-6.0.2/kss.egg-info/not-zip-safe
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      136 2024-04-28 14:10:23.000000 kss-6.0.2/kss.egg-info/requires.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       32 2024-04-28 14:10:23.000000 kss-6.0.2/kss.egg-info/top_level.txt
--rwxr-xr-x   0 hyunwoongko   (501) staff       (20)      160 2024-04-28 14:10:23.276440 kss-6.0.2/setup.cfg
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6191 2024-04-27 14:55:22.000000 kss-6.0.2/setup.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-28 14:10:23.275841 kss-6.0.2/tests/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.2/tests/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1033 2024-04-27 14:55:22.000000 kss-6.0.2/tests/test_augmentation.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     8258 2024-04-27 14:55:22.000000 kss-6.0.2/tests/test_collocation.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      250 2024-04-27 14:55:22.000000 kss-6.0.2/tests/test_g2p.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      238 2024-04-27 14:55:22.000000 kss-6.0.2/tests/test_hangulize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      747 2024-04-27 14:55:22.000000 kss-6.0.2/tests/test_hanja.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      978 2024-04-27 14:55:22.000000 kss-6.0.2/tests/test_jamo.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      442 2024-04-27 14:55:22.000000 kss-6.0.2/tests/test_josa.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3405 2024-04-27 14:55:22.000000 kss-6.0.2/tests/test_keywords.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      378 2024-04-27 14:55:22.000000 kss-6.0.2/tests/test_morphemes.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    19148 2024-04-27 14:55:22.000000 kss-6.0.2/tests/test_paradigm.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    97981 2024-04-27 14:55:22.000000 kss-6.0.2/tests/test_preprocessing.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      290 2024-04-27 14:55:22.000000 kss-6.0.2/tests/test_qwerty.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      257 2024-04-27 14:55:22.000000 kss-6.0.2/tests/test_romanize.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      313 2024-04-27 14:55:22.000000 kss-6.0.2/tests/test_safety.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      776 2024-04-27 14:55:22.000000 kss-6.0.2/tests/test_sentences.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      236 2024-04-27 14:55:22.000000 kss-6.0.2/tests/test_spacing.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1966 2024-04-27 14:55:22.000000 kss-6.0.2/tests/test_summarization.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.818108 kss-6.0.3/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1569 2024-04-01 04:29:21.000000 kss-6.0.3/LICENSE
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      423 2024-04-30 18:36:13.000000 kss-6.0.3/MANIFEST.in
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   162021 2024-04-30 18:37:40.818281 kss-6.0.3/PKG-INFO
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   161269 2024-04-28 14:10:14.000000 kss-6.0.3/README.md
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.780104 kss-6.0.3/bench/
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.785844 kss-6.0.3/bench/sentence_split/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.3/bench/sentence_split/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4379 2024-04-27 14:55:22.000000 kss-6.0.3/bench/sentence_split/sentence_split.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      615 2024-04-27 14:55:22.000000 kss-6.0.3/bench/sentence_split/test_baseline.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      600 2024-04-27 14:55:22.000000 kss-6.0.3/bench/sentence_split/test_kiwi.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1015 2024-04-27 14:55:22.000000 kss-6.0.3/bench/sentence_split/test_koalanlp.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      700 2024-04-27 14:55:22.000000 kss-6.0.3/bench/sentence_split/test_kss.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      587 2024-04-27 14:55:22.000000 kss-6.0.3/bench/sentence_split/test_word_split.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.786867 kss-6.0.3/csrc/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2024-03-31 20:12:01.000000 kss-6.0.3/csrc/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      563 2024-03-31 20:36:14.000000 kss-6.0.3/csrc/kss_cython.pyx
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5965 2024-03-31 20:12:01.000000 kss-6.0.3/csrc/sentence_splitter.cpp
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7830 2024-03-31 20:12:01.000000 kss-6.0.3/csrc/sentence_splitter.h
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.786973 kss-6.0.3/kss/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7568 2024-04-30 18:37:30.000000 kss-6.0.3/kss/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.788693 kss-6.0.3/kss/_elements/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.3/kss/_elements/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4888 2023-08-22 23:38:03.000000 kss-6.0.3/kss/_elements/element.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2702 2023-08-22 23:38:03.000000 kss-6.0.3/kss/_elements/empty.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      536 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_elements/subclasses.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.788913 kss-6.0.3/kss/_modules/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.3/kss/_modules/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.789771 kss-6.0.3/kss/_modules/augmentation/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/augmentation/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.789994 kss-6.0.3/kss/_modules/augmentation/assets/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)  4865459 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/augmentation/assets/wordnet.json
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3892 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/augmentation/augment.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3251 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/augmentation/distance.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3602 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/augmentation/replacement.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1411 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/augmentation/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.793341 kss-6.0.3/kss/_modules/collocation/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/collocation/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     9351 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/collocation/collocate.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.798180 kss-6.0.3/kss/_modules/g2p/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/g2p/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.798527 kss-6.0.3/kss/_modules/g2p/assets/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2634 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/g2p/assets/idioms.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    14802 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/g2p/assets/rules.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5390 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/g2p/assets/table.csv
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6586 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/g2p/english.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7191 2024-04-28 13:55:26.000000 kss-6.0.3/kss/_modules/g2p/g2p.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4459 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/g2p/numerals.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2722 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/g2p/regular.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4949 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/g2p/special.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8131 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/g2p/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.798727 kss-6.0.3/kss/_modules/hangulization/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3616 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulization.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.799426 kss-6.0.3/kss/_modules/hangulization/hangulize/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2277 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    10423 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/hangul.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.799538 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1426 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.799653 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/aze/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5272 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/aze/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.799789 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/bel/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5425 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/bel/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.799934 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/bul/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4925 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/bul/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.800089 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/cat/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4328 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/cat/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.800226 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/ces/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4820 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/ces/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.800353 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/cym/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5791 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/cym/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.800483 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/deu/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7415 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/deu/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.800619 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/ell/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     9068 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/ell/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.800828 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/epo/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4103 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/epo/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.801048 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/est/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3931 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/est/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.801174 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/fin/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3410 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/fin/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.801300 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/grc/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8626 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/grc/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.801437 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/hbs/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5606 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/hbs/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.801575 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/hun/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4990 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/hun/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.801708 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/isl/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5626 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/isl/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.801840 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/ita/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4371 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/ita/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.801945 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/jpn/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4446 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/jpn/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.802213 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/kat/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6118 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/kat/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6408 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/kat/narrow.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.802347 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/lat/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3314 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/lat/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.802471 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/lav/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4116 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/lav/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.802613 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/lit/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4080 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/lit/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.802771 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/mkd/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5354 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/mkd/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.802898 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/nld/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    22064 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/nld/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.803112 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/pol/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5785 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/pol/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.803475 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/por/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6048 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/por/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6056 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/por/br.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.803605 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/ron/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5120 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/ron/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.803733 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/rus/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4994 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/rus/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.803864 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/slk/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6693 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/slk/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.803993 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/slv/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3836 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/slv/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.804119 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/spa/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4002 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/spa/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.804245 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/sqi/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3177 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/sqi/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.804379 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/swe/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7896 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/swe/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.804515 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/tur/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3528 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/tur/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.804649 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/ukr/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5072 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/ukr/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.804781 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/vie/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4742 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/vie/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.804907 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/wlm/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5599 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/langs/wlm/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    16108 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/models.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1069 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/normalization.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2897 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hangulization/hangulize/processing.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.805231 kss-6.0.3/kss/_modules/hanja/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/hanja/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.805333 kss-6.0.3/kss/_modules/hanja/assets/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   522443 2024-04-24 16:39:29.000000 kss-6.0.3/kss/_modules/hanja/assets/table.yml
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5330 2024-04-30 18:33:50.000000 kss-6.0.3/kss/_modules/hanja/hanja.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5243 2024-04-30 18:34:28.000000 kss-6.0.3/kss/_modules/hanja/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.806244 kss-6.0.3/kss/_modules/jamo/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/jamo/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    12624 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/jamo/_jamo.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      912 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/jamo/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.806553 kss-6.0.3/kss/_modules/josa/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/josa/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2580 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/josa/josa.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7030 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/josa/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.807162 kss-6.0.3/kss/_modules/keywords/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/keywords/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6529 2024-04-28 13:58:52.000000 kss-6.0.3/kss/_modules/keywords/extract_keywords.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    17289 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/keywords/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.807949 kss-6.0.3/kss/_modules/morphemes/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.3/kss/_modules/morphemes/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2652 2024-03-31 13:42:10.000000 kss-6.0.3/kss/_modules/morphemes/analyzers.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1849 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/morphemes/split_morphemes.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3588 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/morphemes/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.808185 kss-6.0.3/kss/_modules/paradigm/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/paradigm/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    18316 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/paradigm/paradigm.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.810330 kss-6.0.3/kss/_modules/preprocessing/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/preprocessing/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    15538 2024-04-27 14:56:06.000000 kss-6.0.3/kss/_modules/preprocessing/anonymize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    29795 2024-04-27 14:58:49.000000 kss-6.0.3/kss/_modules/preprocessing/clean_news.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    81165 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/preprocessing/completed_form.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    24570 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/preprocessing/filter_out.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2088 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/preprocessing/half2full.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6056 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/preprocessing/normalize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    26257 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/preprocessing/preprocess.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7186 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/preprocessing/reduce_repeats.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     7661 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/preprocessing/remove_invisible_chars.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.810785 kss-6.0.3/kss/_modules/qwerty/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/qwerty/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6262 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/qwerty/qwerty.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5941 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/qwerty/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.811104 kss-6.0.3/kss/_modules/romanization/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/romanization/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5813 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/romanization/romanize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8901 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/romanization/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.811433 kss-6.0.3/kss/_modules/safety/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/safety/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3531 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/safety/check_safety.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    35374 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/safety/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.813659 kss-6.0.3/kss/_modules/sentences/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.3/kss/_modules/sentences/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     9334 2023-08-22 23:38:03.000000 kss-6.0.3/kss/_modules/sentences/embracing_processor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    22898 2023-08-22 23:38:03.000000 kss-6.0.3/kss/_modules/sentences/sentence_postprocessor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6751 2024-03-31 07:55:02.000000 kss-6.0.3/kss/_modules/sentences/sentence_preprocessor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2298 2023-08-22 23:38:03.000000 kss-6.0.3/kss/_modules/sentences/sentence_processor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    30242 2023-08-22 23:38:03.000000 kss-6.0.3/kss/_modules/sentences/sentence_splitter.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    13304 2024-03-31 20:36:14.000000 kss-6.0.3/kss/_modules/sentences/sentence_splitter_fast.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8322 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/sentences/split_sentences.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.814202 kss-6.0.3/kss/_modules/spacing/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/spacing/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5539 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/spacing/correct_spacing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   296979 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/spacing/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.814848 kss-6.0.3/kss/_modules/summarization/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.3/kss/_modules/summarization/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5603 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/summarization/summarize_sentences.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3396 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_modules/summarization/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.816026 kss-6.0.3/kss/_utils/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      129 2023-08-22 23:38:03.000000 kss-6.0.3/kss/_utils/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       66 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_utils/api.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    10329 2024-03-31 07:46:03.000000 kss-6.0.3/kss/_utils/const.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1399 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_utils/emojis.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      910 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_utils/logger.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1001 2023-08-22 23:38:03.000000 kss-6.0.3/kss/_utils/multiprocessing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    17275 2024-04-27 14:55:22.000000 kss-6.0.3/kss/_utils/sanity_checks.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.787886 kss-6.0.3/kss.egg-info/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)   162021 2024-04-30 18:37:40.000000 kss-6.0.3/kss.egg-info/PKG-INFO
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6409 2024-04-30 18:37:40.000000 kss-6.0.3/kss.egg-info/SOURCES.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-30 18:37:40.000000 kss-6.0.3/kss.egg-info/dependency_links.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2024-04-27 14:04:55.000000 kss-6.0.3/kss.egg-info/not-zip-safe
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      134 2024-04-30 18:37:40.000000 kss-6.0.3/kss.egg-info/requires.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       32 2024-04-30 18:37:40.000000 kss-6.0.3/kss.egg-info/top_level.txt
+-rwxr-xr-x   0 hyunwoongko   (501) staff       (20)      160 2024-04-30 18:37:40.818525 kss-6.0.3/setup.cfg
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6239 2024-04-30 18:37:30.000000 kss-6.0.3/setup.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2024-04-30 18:37:40.818012 kss-6.0.3/tests/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2024-04-27 14:55:22.000000 kss-6.0.3/tests/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1033 2024-04-27 14:55:22.000000 kss-6.0.3/tests/test_augmentation.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     8258 2024-04-27 14:55:22.000000 kss-6.0.3/tests/test_collocation.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      250 2024-04-27 14:55:22.000000 kss-6.0.3/tests/test_g2p.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      238 2024-04-27 14:55:22.000000 kss-6.0.3/tests/test_hangulize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      747 2024-04-27 14:55:22.000000 kss-6.0.3/tests/test_hanja.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      978 2024-04-27 14:55:22.000000 kss-6.0.3/tests/test_jamo.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      442 2024-04-27 14:55:22.000000 kss-6.0.3/tests/test_josa.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3405 2024-04-27 14:55:22.000000 kss-6.0.3/tests/test_keywords.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      378 2024-04-27 14:55:22.000000 kss-6.0.3/tests/test_morphemes.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    19148 2024-04-27 14:55:22.000000 kss-6.0.3/tests/test_paradigm.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    97981 2024-04-27 14:55:22.000000 kss-6.0.3/tests/test_preprocessing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      290 2024-04-27 14:55:22.000000 kss-6.0.3/tests/test_qwerty.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      257 2024-04-27 14:55:22.000000 kss-6.0.3/tests/test_romanize.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      313 2024-04-27 14:55:22.000000 kss-6.0.3/tests/test_safety.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      776 2024-04-27 14:55:22.000000 kss-6.0.3/tests/test_sentences.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      236 2024-04-27 14:55:22.000000 kss-6.0.3/tests/test_spacing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1966 2024-04-27 14:55:22.000000 kss-6.0.3/tests/test_summarization.py
```

### Comparing `kss-6.0.2/LICENSE` & `kss-6.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/PKG-INFO` & `kss-6.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kss
-Version: 6.0.2
+Version: 6.0.3
 Summary: A Toolkit for Korean sentence segmentation
 Home-page: https://github.com/hyunwoongko/kss
 Author: Hyunwoong Ko
 Author-email: kevin.brain@kakaobrain.com
 License: BSD 3-Clause "New" or "Revised" License
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kss Version: 6.0.2 Summary: A Toolkit for Korean
+Metadata-Version: 2.1 Name: kss Version: 6.0.3 Summary: A Toolkit for Korean
 sentence segmentation Home-page: https://github.com/hyunwoongko/kss Author:
 Hyunwoong Ko Author-email: kevin.brain@kakaobrain.com License: BSD 3-Clause
 "New" or "Revised" License Platform: any Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.2 Classifier:
 Programming Language :: Python :: 3.3 Classifier: Programming Language ::
 Python :: 3.4 Classifier: Programming Language :: Python :: 3.5 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
```

### Comparing `kss-6.0.2/README.md` & `kss-6.0.3/README.md`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/bench/sentence_split/sentence_split.py` & `kss-6.0.3/bench/sentence_split/sentence_split.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/bench/sentence_split/test_baseline.py` & `kss-6.0.3/bench/sentence_split/test_baseline.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/bench/sentence_split/test_kiwi.py` & `kss-6.0.3/bench/sentence_split/test_kiwi.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/bench/sentence_split/test_koalanlp.py` & `kss-6.0.3/bench/sentence_split/test_koalanlp.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/bench/sentence_split/test_kss.py` & `kss-6.0.3/bench/sentence_split/test_kss.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/bench/sentence_split/test_word_split.py` & `kss-6.0.3/bench/sentence_split/test_word_split.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/csrc/kss_cython.pyx` & `kss-6.0.3/csrc/kss_cython.pyx`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/csrc/sentence_splitter.cpp` & `kss-6.0.3/csrc/sentence_splitter.cpp`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/csrc/sentence_splitter.h` & `kss-6.0.3/csrc/sentence_splitter.h`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/__init__.py` & `kss-6.0.3/kss/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2021 Hyunwoong Ko <kevin.brain@kakaobrain.com> and Sang-Kil Park <skpark1224@hyundai.com>
 # All rights reserved.
 
 from kss._modules.augmentation.augment import augment
 from kss._modules.collocation.collocate import collocate
 from kss._modules.g2p.g2p import g2p
 from kss._modules.hangulization.hangulization import hangulize
-from kss._modules.hanja._hanja import split_hanja, is_hanja, hanja2hangul
+from kss._modules.hanja.hanja import split_hanja, is_hanja, hanja2hangul
 from kss._modules.jamo._jamo import h2j, h2hcj, j2h, j2hcj, hcj2h, hcj2j, is_jamo, is_jamo_modern, is_hcj, \
     is_hcj_modern, is_hangul_char
 from kss._modules.josa.josa import select_josa, combine_josa
 from kss._modules.keywords.extract_keywords import extract_keywords
 from kss._modules.morphemes.split_morphemes import split_morphemes
 from kss._modules.paradigm.paradigm import paradigm
 from kss._modules.preprocessing.anonymize import anonymize
@@ -197,8 +197,8 @@
         if closest_module is None:
             return None
         else:
             return closest_module
 
 
 __ALL__ = list(supported_modules.keys()) + ["Kss"]
-__version__ = "6.0.2"
+__version__ = "6.0.3"
```

### Comparing `kss-6.0.2/kss/_elements/element.py` & `kss-6.0.3/kss/_elements/element.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_elements/empty.py` & `kss-6.0.3/kss/_elements/empty.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_elements/subclasses.py` & `kss-6.0.3/kss/_elements/subclasses.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/augmentation/assets/wordnet.json` & `kss-6.0.3/kss/_modules/augmentation/assets/wordnet.json`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/augmentation/augment.py` & `kss-6.0.3/kss/_modules/augmentation/augment.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/augmentation/distance.py` & `kss-6.0.3/kss/_modules/augmentation/distance.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/augmentation/replacement.py` & `kss-6.0.3/kss/_modules/augmentation/replacement.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/augmentation/utils.py` & `kss-6.0.3/kss/_modules/augmentation/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/collocation/collocate.py` & `kss-6.0.3/kss/_modules/collocation/collocate.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/g2p/assets/idioms.txt` & `kss-6.0.3/kss/_modules/g2p/assets/idioms.txt`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/g2p/assets/rules.txt` & `kss-6.0.3/kss/_modules/g2p/assets/rules.txt`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/g2p/assets/table.csv` & `kss-6.0.3/kss/_modules/g2p/assets/table.csv`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/g2p/english.py` & `kss-6.0.3/kss/_modules/g2p/english.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/g2p/g2p.py` & `kss-6.0.3/kss/_modules/g2p/g2p.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/g2p/numerals.py` & `kss-6.0.3/kss/_modules/g2p/numerals.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/g2p/regular.py` & `kss-6.0.3/kss/_modules/g2p/regular.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/g2p/special.py` & `kss-6.0.3/kss/_modules/g2p/special.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/g2p/utils.py` & `kss-6.0.3/kss/_modules/g2p/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulization.py` & `kss-6.0.3/kss/_modules/hangulization/hangulization.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/hangul.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/hangul.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/aze/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/aze/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/bel/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/bel/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/bul/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/bul/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/cat/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/cat/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/ces/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/ces/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/cym/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/cym/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/deu/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/deu/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/ell/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/ell/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/epo/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/epo/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/est/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/est/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/fin/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/fin/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/grc/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/grc/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/hbs/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/hbs/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/hun/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/hun/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/isl/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/isl/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/ita/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/ita/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/jpn/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/jpn/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/kat/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/kat/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/kat/narrow.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/kat/narrow.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/lat/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/lat/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/lav/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/lav/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/lit/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/lit/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/mkd/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/mkd/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/nld/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/nld/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/pol/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/pol/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/por/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/por/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/por/br.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/por/br.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/ron/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/ron/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/rus/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/rus/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/slk/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/slk/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/slv/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/slv/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/spa/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/spa/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/sqi/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/sqi/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/swe/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/swe/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/tur/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/tur/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/ukr/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/ukr/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/vie/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/vie/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/langs/wlm/__init__.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/langs/wlm/__init__.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/models.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/models.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/normalization.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/normalization.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hangulization/hangulize/processing.py` & `kss-6.0.3/kss/_modules/hangulization/hangulize/processing.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/hanja/_hanja.py` & `kss-6.0.3/kss/_modules/hanja/hanja.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from functools import partial
 from typing import List, Union, Tuple
 
-from kss._modules.hanja.utils import _split_hanja, _is_hanja, _hanja2hangul
+from kss._modules.hanja.utils import translate
+from kss._modules.hanja.utils import split_hanja as _split_hanja
+from kss._modules.hanja.utils import is_hanja as _is_hanja
 from kss._utils.multiprocessing import _run_job
 from kss._utils.sanity_checks import _check_text, _check_num_workers, _check_char, _check_type
 
 
 def split_hanja(
     text: Union[str, List[str], Tuple[str]],
     num_workers: Union[int, str] = "auto",
@@ -142,7 +144,23 @@
             combination=combination,
             reverse=reverse,
             html=html,
         ),
         inputs=text,
         num_workers=num_workers,
     )
+
+
+def _hanja2hangul(text, combination=False, reverse=False, html=False):
+    # translate hangul to hanja
+    if combination is False:
+        return translate(text, 'substitution')
+    elif combination is True and reverse is False and html is False:
+        return translate(text, 'combination-text')
+    elif combination is True and reverse is True and html is False:
+        return translate(text, 'combination-text-reversed')
+    elif combination is True and reverse is False and html is True:
+        return translate(text, 'combination-html')
+    elif combination is True and reverse is True and html is True:
+        return translate(text, 'combination-html-reversed')
+    else:
+        raise ValueError("Invalid combination of `combination`, `reverse`, and `html`")
```

### Comparing `kss-6.0.2/kss/_modules/jamo/_jamo.py` & `kss-6.0.3/kss/_modules/jamo/_jamo.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/jamo/utils.py` & `kss-6.0.3/kss/_modules/jamo/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/josa/josa.py` & `kss-6.0.3/kss/_modules/josa/josa.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/josa/utils.py` & `kss-6.0.3/kss/_modules/josa/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/keywords/extract_keywords.py` & `kss-6.0.3/kss/_modules/keywords/extract_keywords.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/keywords/utils.py` & `kss-6.0.3/kss/_modules/keywords/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/morphemes/analyzers.py` & `kss-6.0.3/kss/_modules/morphemes/analyzers.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/morphemes/split_morphemes.py` & `kss-6.0.3/kss/_modules/morphemes/split_morphemes.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/morphemes/utils.py` & `kss-6.0.3/kss/_modules/morphemes/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/paradigm/paradigm.py` & `kss-6.0.3/kss/_modules/paradigm/paradigm.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/preprocessing/anonymize.py` & `kss-6.0.3/kss/_modules/preprocessing/anonymize.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/preprocessing/clean_news.py` & `kss-6.0.3/kss/_modules/preprocessing/clean_news.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/preprocessing/completed_form.py` & `kss-6.0.3/kss/_modules/preprocessing/completed_form.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/preprocessing/filter_out.py` & `kss-6.0.3/kss/_modules/preprocessing/filter_out.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/preprocessing/half2full.py` & `kss-6.0.3/kss/_modules/preprocessing/half2full.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/preprocessing/normalize.py` & `kss-6.0.3/kss/_modules/preprocessing/normalize.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/preprocessing/preprocess.py` & `kss-6.0.3/kss/_modules/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/preprocessing/reduce_repeats.py` & `kss-6.0.3/kss/_modules/preprocessing/reduce_repeats.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/preprocessing/remove_invisible_chars.py` & `kss-6.0.3/kss/_modules/preprocessing/remove_invisible_chars.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/qwerty/qwerty.py` & `kss-6.0.3/kss/_modules/qwerty/qwerty.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/qwerty/utils.py` & `kss-6.0.3/kss/_modules/qwerty/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/romanization/romanize.py` & `kss-6.0.3/kss/_modules/romanization/romanize.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/romanization/utils.py` & `kss-6.0.3/kss/_modules/romanization/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/safety/check_safety.py` & `kss-6.0.3/kss/_modules/safety/check_safety.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/safety/utils.py` & `kss-6.0.3/kss/_modules/safety/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/sentences/embracing_processor.py` & `kss-6.0.3/kss/_modules/sentences/embracing_processor.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/sentences/sentence_postprocessor.py` & `kss-6.0.3/kss/_modules/sentences/sentence_postprocessor.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/sentences/sentence_preprocessor.py` & `kss-6.0.3/kss/_modules/sentences/sentence_preprocessor.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/sentences/sentence_processor.py` & `kss-6.0.3/kss/_modules/sentences/sentence_processor.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/sentences/sentence_splitter.py` & `kss-6.0.3/kss/_modules/sentences/sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/sentences/sentence_splitter_fast.py` & `kss-6.0.3/kss/_modules/sentences/sentence_splitter_fast.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/sentences/split_sentences.py` & `kss-6.0.3/kss/_modules/sentences/split_sentences.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/spacing/correct_spacing.py` & `kss-6.0.3/kss/_modules/spacing/correct_spacing.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/spacing/utils.py` & `kss-6.0.3/kss/_modules/spacing/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/summarization/summarize_sentences.py` & `kss-6.0.3/kss/_modules/summarization/summarize_sentences.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_modules/summarization/utils.py` & `kss-6.0.3/kss/_modules/summarization/utils.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_utils/const.py` & `kss-6.0.3/kss/_utils/const.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_utils/emojis.py` & `kss-6.0.3/kss/_utils/emojis.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_utils/logger.py` & `kss-6.0.3/kss/_utils/logger.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_utils/multiprocessing.py` & `kss-6.0.3/kss/_utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss/_utils/sanity_checks.py` & `kss-6.0.3/kss/_utils/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/kss.egg-info/PKG-INFO` & `kss-6.0.3/kss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kss
-Version: 6.0.2
+Version: 6.0.3
 Summary: A Toolkit for Korean sentence segmentation
 Home-page: https://github.com/hyunwoongko/kss
 Author: Hyunwoong Ko
 Author-email: kevin.brain@kakaobrain.com
 License: BSD 3-Clause "New" or "Revised" License
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kss Version: 6.0.2 Summary: A Toolkit for Korean
+Metadata-Version: 2.1 Name: kss Version: 6.0.3 Summary: A Toolkit for Korean
 sentence segmentation Home-page: https://github.com/hyunwoongko/kss Author:
 Hyunwoong Ko Author-email: kevin.brain@kakaobrain.com License: BSD 3-Clause
 "New" or "Revised" License Platform: any Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.2 Classifier:
 Programming Language :: Python :: 3.3 Classifier: Programming Language ::
 Python :: 3.4 Classifier: Programming Language :: Python :: 3.5 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
```

### Comparing `kss-6.0.2/kss.egg-info/SOURCES.txt` & `kss-6.0.3/kss.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -87,16 +87,17 @@
 kss/_modules/hangulization/hangulize/langs/sqi/__init__.py
 kss/_modules/hangulization/hangulize/langs/swe/__init__.py
 kss/_modules/hangulization/hangulize/langs/tur/__init__.py
 kss/_modules/hangulization/hangulize/langs/ukr/__init__.py
 kss/_modules/hangulization/hangulize/langs/vie/__init__.py
 kss/_modules/hangulization/hangulize/langs/wlm/__init__.py
 kss/_modules/hanja/__init__.py
-kss/_modules/hanja/_hanja.py
+kss/_modules/hanja/hanja.py
 kss/_modules/hanja/utils.py
+kss/_modules/hanja/assets/table.yml
 kss/_modules/jamo/__init__.py
 kss/_modules/jamo/_jamo.py
 kss/_modules/jamo/utils.py
 kss/_modules/josa/__init__.py
 kss/_modules/josa/josa.py
 kss/_modules/josa/utils.py
 kss/_modules/keywords/__init__.py
```

### Comparing `kss-6.0.2/setup.py` & `kss-6.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,17 +148,17 @@
             version = line.split("=")[1].strip().replace("'", "").replace('"', "")
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 install_requires = [
     "emoji==1.2.0", "pecab", "networkx", "jamo",
-    "hangul-jamo", "hanja==0.13.3", "tossi", "distance",
+    "hangul-jamo", "tossi", "distance", "pyyaml==6.0",
     "unidecode", "cmudict", "koparadigm", "kollocate",
-    "bs4", "numpy", "pytest", "scipy"
+    "bs4", "numpy", "pytest", "scipy",
 ]
 
 setup(
     name="kss",
     version=version,
     author="Hyunwoong Ko",
     author_email="kevin.brain@kakaobrain.com",
@@ -172,14 +172,15 @@
     packages=find_packages(exclude=["bench", "assets", ".java", ".pytest_cache"]),
     python_requires=">=3",
     zip_safe=False,
     package_data={
         "cython": ["csrc/*"],
         "g2p": ["kss/_modules/g2p/assets/*"],
         "augmentation": ["kss/_modules/augmentation/assets/*"],
+        "hanja": ["kss/_modules/hanja/assets/*"]
     },
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.2",
         "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
```

### Comparing `kss-6.0.2/tests/test_augmentation.py` & `kss-6.0.3/tests/test_augmentation.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/tests/test_collocation.py` & `kss-6.0.3/tests/test_collocation.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/tests/test_hanja.py` & `kss-6.0.3/tests/test_hanja.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/tests/test_jamo.py` & `kss-6.0.3/tests/test_jamo.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/tests/test_keywords.py` & `kss-6.0.3/tests/test_keywords.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/tests/test_paradigm.py` & `kss-6.0.3/tests/test_paradigm.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/tests/test_preprocessing.py` & `kss-6.0.3/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/tests/test_sentences.py` & `kss-6.0.3/tests/test_sentences.py`

 * *Files identical despite different names*

### Comparing `kss-6.0.2/tests/test_summarization.py` & `kss-6.0.3/tests/test_summarization.py`

 * *Files identical despite different names*

