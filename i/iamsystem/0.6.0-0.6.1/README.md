# Comparing `tmp/iamsystem-0.6.0.tar.gz` & `tmp/iamsystem-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamsystem-0.6.0.tar", last modified: Mon Jan  8 07:13:41 2024, max compression
+gzip compressed data, was "iamsystem-0.6.1.tar", last modified: Tue Apr 30 07:31:06 2024, max compression
```

## Comparing `iamsystem-0.6.0.tar` & `iamsystem-0.6.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-01-08 07:13:41.095050 iamsystem-0.6.0/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1074 2024-01-01 10:19:47.000000 iamsystem-0.6.0/LICENSE
--rw-r--r--   0 cossin    (1000) cossin    (1000)     4691 2024-01-08 07:13:41.095050 iamsystem-0.6.0/PKG-INFO
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     3400 2024-01-03 07:20:57.000000 iamsystem-0.6.0/README.md
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1808 2024-01-08 07:02:46.000000 iamsystem-0.6.0/pyproject.toml
--rw-rw-r--   0 cossin    (1000) cossin    (1000)       38 2024-01-08 07:13:41.095050 iamsystem-0.6.0/setup.cfg
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-01-08 07:13:41.043050 iamsystem-0.6.0/src/
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-01-08 07:13:41.047050 iamsystem-0.6.0/src/iamsystem/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     4070 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/__init__.py
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-01-08 07:13:41.047050 iamsystem-0.6.0/src/iamsystem/brat/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/brat/__init__.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     8882 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/brat/adapter.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     3479 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/brat/formatter.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)      508 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/brat/util.py
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-01-08 07:13:41.047050 iamsystem-0.6.0/src/iamsystem/fuzzy/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/fuzzy/__init__.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     3324 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/fuzzy/abbreviations.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     7075 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/fuzzy/api.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     2625 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/fuzzy/cache.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)      650 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/fuzzy/exact.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     2261 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/fuzzy/norm_fun.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     2764 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/fuzzy/regex.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     4182 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/fuzzy/simstring.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     4594 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/fuzzy/spellwise.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1286 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/fuzzy/util.py
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-01-08 07:13:41.047050 iamsystem-0.6.0/src/iamsystem/keywords/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/keywords/__init__.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)      705 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/keywords/api.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1803 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/keywords/collection.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1116 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/keywords/keywords.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)      877 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/keywords/util.py
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-01-08 07:13:41.047050 iamsystem-0.6.0/src/iamsystem/matcher/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/matcher/__init__.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)    11783 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/matcher/annotation.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     4214 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/matcher/api.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)    19387 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/matcher/matcher.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1648 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/matcher/printannot.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)    14119 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/matcher/strategy.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     2985 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/matcher/util.py
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-01-08 07:13:41.051050 iamsystem-0.6.0/src/iamsystem/spacy/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)      487 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/spacy/__init__.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     8151 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/spacy/component.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)      424 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/spacy/stopwords.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1051 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/spacy/token.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1437 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/spacy/tokenizer.py
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-01-08 07:13:41.051050 iamsystem-0.6.0/src/iamsystem/stopwords/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/stopwords/__init__.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1629 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/stopwords/api.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     3983 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/stopwords/negative.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1492 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/stopwords/simple.py
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-01-08 07:13:41.051050 iamsystem-0.6.0/src/iamsystem/tokenization/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/tokenization/__init__.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     2162 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/tokenization/api.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)      476 2024-01-03 07:20:57.000000 iamsystem-0.6.0/src/iamsystem/tokenization/normalize.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     3110 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/tokenization/span.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1873 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/tokenization/token.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     4254 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/tokenization/tokenize.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     5664 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/tokenization/util.py
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-01-08 07:13:41.051050 iamsystem-0.6.0/src/iamsystem/tree/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/tree/__init__.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)      275 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/tree/api.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     7732 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/tree/nodes.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     3502 2024-01-01 10:19:52.000000 iamsystem-0.6.0/src/iamsystem/tree/trie.py
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-01-08 07:13:41.095050 iamsystem-0.6.0/src/iamsystem.egg-info/
--rw-r--r--   0 cossin    (1000) cossin    (1000)     4691 2024-01-08 07:13:41.000000 iamsystem-0.6.0/src/iamsystem.egg-info/PKG-INFO
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     2022 2024-01-08 07:13:41.000000 iamsystem-0.6.0/src/iamsystem.egg-info/SOURCES.txt
--rw-rw-r--   0 cossin    (1000) cossin    (1000)        1 2024-01-08 07:13:41.000000 iamsystem-0.6.0/src/iamsystem.egg-info/dependency_links.txt
--rw-rw-r--   0 cossin    (1000) cossin    (1000)      207 2024-01-08 07:13:41.000000 iamsystem-0.6.0/src/iamsystem.egg-info/requires.txt
--rw-rw-r--   0 cossin    (1000) cossin    (1000)       10 2024-01-08 07:13:41.000000 iamsystem-0.6.0/src/iamsystem.egg-info/top_level.txt
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-01-08 07:13:41.095050 iamsystem-0.6.0/tests/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)    10966 2024-01-01 10:19:52.000000 iamsystem-0.6.0/tests/test_annotation.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)    12681 2024-01-01 10:19:52.000000 iamsystem-0.6.0/tests/test_brat.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)    11902 2024-01-01 10:19:52.000000 iamsystem-0.6.0/tests/test_detect.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)    38661 2024-01-01 10:19:52.000000 iamsystem-0.6.0/tests/test_doc.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)    13519 2024-01-01 10:19:52.000000 iamsystem-0.6.0/tests/test_fuzzy.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)    23629 2024-01-01 10:19:52.000000 iamsystem-0.6.0/tests/test_matcher.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     5524 2024-01-01 10:19:52.000000 iamsystem-0.6.0/tests/test_simstring.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     7437 2024-01-01 10:19:52.000000 iamsystem-0.6.0/tests/test_spacy.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     6818 2024-01-01 10:19:52.000000 iamsystem-0.6.0/tests/test_spellwise.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     3768 2024-01-01 10:19:52.000000 iamsystem-0.6.0/tests/test_stopwords.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     3092 2024-01-01 10:19:52.000000 iamsystem-0.6.0/tests/test_terminology.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     5704 2024-01-01 10:19:52.000000 iamsystem-0.6.0/tests/test_toknorm.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     9402 2024-01-01 10:19:52.000000 iamsystem-0.6.0/tests/test_tree.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-04-30 07:31:06.582615 iamsystem-0.6.1/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1074 2024-01-01 10:19:47.000000 iamsystem-0.6.1/LICENSE
+-rw-r--r--   0 cossin    (1000) cossin    (1000)     4743 2024-04-30 07:31:06.582615 iamsystem-0.6.1/PKG-INFO
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     3400 2024-01-08 07:25:20.000000 iamsystem-0.6.1/README.md
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1784 2024-04-30 07:30:39.000000 iamsystem-0.6.1/pyproject.toml
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)       38 2024-04-30 07:31:06.582615 iamsystem-0.6.1/setup.cfg
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-04-30 07:31:06.570615 iamsystem-0.6.1/src/
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-04-30 07:31:06.570615 iamsystem-0.6.1/src/iamsystem/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     4070 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/__init__.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-04-30 07:31:06.570615 iamsystem-0.6.1/src/iamsystem/brat/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/brat/__init__.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     8882 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/brat/adapter.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     3479 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/brat/formatter.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)      508 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/brat/util.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-04-30 07:31:06.574615 iamsystem-0.6.1/src/iamsystem/fuzzy/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/fuzzy/__init__.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     3324 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/fuzzy/abbreviations.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     7075 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/fuzzy/api.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     2625 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/fuzzy/cache.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)      650 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/fuzzy/exact.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     2261 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/fuzzy/norm_fun.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     2764 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/fuzzy/regex.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     4182 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/fuzzy/simstring.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     4594 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/fuzzy/spellwise.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1286 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/fuzzy/util.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-04-30 07:31:06.574615 iamsystem-0.6.1/src/iamsystem/keywords/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/keywords/__init__.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)      705 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/keywords/api.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1803 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/keywords/collection.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1116 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/keywords/keywords.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)      877 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/keywords/util.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-04-30 07:31:06.574615 iamsystem-0.6.1/src/iamsystem/matcher/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/matcher/__init__.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)    11783 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/matcher/annotation.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     4214 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/matcher/api.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)    19387 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/matcher/matcher.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1648 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/matcher/printannot.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)    14119 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/matcher/strategy.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     2985 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/matcher/util.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-04-30 07:31:06.574615 iamsystem-0.6.1/src/iamsystem/spacy/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)      487 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/spacy/__init__.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     8151 2024-01-08 07:25:20.000000 iamsystem-0.6.1/src/iamsystem/spacy/component.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)      424 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/spacy/stopwords.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1051 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/spacy/token.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1437 2024-01-08 07:25:20.000000 iamsystem-0.6.1/src/iamsystem/spacy/tokenizer.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-04-30 07:31:06.578615 iamsystem-0.6.1/src/iamsystem/stopwords/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/stopwords/__init__.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1629 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/stopwords/api.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     3983 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/stopwords/negative.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1492 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/stopwords/simple.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-04-30 07:31:06.578615 iamsystem-0.6.1/src/iamsystem/tokenization/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/tokenization/__init__.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     2162 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/tokenization/api.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)      476 2024-01-08 07:25:20.000000 iamsystem-0.6.1/src/iamsystem/tokenization/normalize.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     3110 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/tokenization/span.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1873 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/tokenization/token.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     4254 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/tokenization/tokenize.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     5664 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/tokenization/util.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-04-30 07:31:06.578615 iamsystem-0.6.1/src/iamsystem/tree/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/tree/__init__.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)      275 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/tree/api.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     7732 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/tree/nodes.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     3502 2024-01-01 10:19:52.000000 iamsystem-0.6.1/src/iamsystem/tree/trie.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-04-30 07:31:06.578615 iamsystem-0.6.1/src/iamsystem.egg-info/
+-rw-r--r--   0 cossin    (1000) cossin    (1000)     4743 2024-04-30 07:31:06.000000 iamsystem-0.6.1/src/iamsystem.egg-info/PKG-INFO
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     2022 2024-04-30 07:31:06.000000 iamsystem-0.6.1/src/iamsystem.egg-info/SOURCES.txt
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)        1 2024-04-30 07:31:06.000000 iamsystem-0.6.1/src/iamsystem.egg-info/dependency_links.txt
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)      131 2024-04-30 07:31:06.000000 iamsystem-0.6.1/src/iamsystem.egg-info/requires.txt
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)       10 2024-04-30 07:31:06.000000 iamsystem-0.6.1/src/iamsystem.egg-info/top_level.txt
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2024-04-30 07:31:06.578615 iamsystem-0.6.1/tests/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)    10966 2024-01-01 10:19:52.000000 iamsystem-0.6.1/tests/test_annotation.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)    12681 2024-01-01 10:19:52.000000 iamsystem-0.6.1/tests/test_brat.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)    11902 2024-01-01 10:19:52.000000 iamsystem-0.6.1/tests/test_detect.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)    38661 2024-01-01 10:19:52.000000 iamsystem-0.6.1/tests/test_doc.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)    13519 2024-01-01 10:19:52.000000 iamsystem-0.6.1/tests/test_fuzzy.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)    23629 2024-01-01 10:19:52.000000 iamsystem-0.6.1/tests/test_matcher.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     5524 2024-01-01 10:19:52.000000 iamsystem-0.6.1/tests/test_simstring.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     7437 2024-01-08 07:25:20.000000 iamsystem-0.6.1/tests/test_spacy.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     6818 2024-01-01 10:19:52.000000 iamsystem-0.6.1/tests/test_spellwise.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     3768 2024-01-01 10:19:52.000000 iamsystem-0.6.1/tests/test_stopwords.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     3092 2024-01-01 10:19:52.000000 iamsystem-0.6.1/tests/test_terminology.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     5704 2024-01-01 10:19:52.000000 iamsystem-0.6.1/tests/test_toknorm.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     9402 2024-01-01 10:19:52.000000 iamsystem-0.6.1/tests/test_tree.py
```

### Comparing `iamsystem-0.6.0/LICENSE` & `iamsystem-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/PKG-INFO` & `iamsystem-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamsystem
-Version: 0.6.0
+Version: 0.6.1
 Summary: A python implementation of IAMsystem algorithm
 Author-email: Sebastien Cossin <cossin.sebastien@gmail.com>
 Project-URL: Homepage, https://github.com/scossin/iamsystem_python
 Project-URL: Bug Tracker, https://github.com/scossin/iamsystem_python/issues
 Keywords: NLP,semantic annotation,entity linking
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
@@ -14,24 +14,28 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: anyascii>=0.3.2
-Requires-Dist: typing_extensions>=4.7.0; python_version >= "3.12"
-Requires-Dist: typing_extensions~=4.4.0; python_version < "3.12"
-Requires-Dist: spellwise>=0.8.0
-Requires-Dist: pysimstring~=1.2.1
-Provides-Extra: tests
-Requires-Dist: nltk>=3.8.0; extra == "tests"
-Requires-Dist: spacy>=3.2.0; extra == "tests"
+Requires-Dist: anyascii
+Requires-Dist: pysimstring
+Requires-Dist: spellwise
+Requires-Dist: typing_extensions
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx-rtd-theme; extra == "doc"
+Provides-Extra: tests
+Requires-Dist: nltk; extra == "tests"
+Requires-Dist: spacy; extra == "tests"
 
 # iamsystem
 ![test](https://github.com/scossin/iamsystem_python/actions/workflows/tests.yml/badge.svg)
 [![PyPI version fury.io](https://badge.fury.io/py/iamsystem.svg)](https://pypi.org/project/iamsystem/)
 [![PyPI license](https://img.shields.io/pypi/l/iamsystem.svg)](https://pypi.python.org/pypi/iamsystem/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/iamsystem.svg)](https://pypi.python.org/pypi/iamsystem/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
```

### Comparing `iamsystem-0.6.0/README.md` & `iamsystem-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/pyproject.toml` & `iamsystem-0.6.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "iamsystem"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
   { name="Sebastien Cossin", email="cossin.sebastien@gmail.com" },
 ]
 description = "A python implementation of IAMsystem algorithm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -16,24 +16,34 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["NLP", "semantic annotation", "entity linking"]
 dependencies = [
-    "anyascii>=0.3.2",
-    "typing_extensions>=4.7.0; python_version>='3.12'",
-    "typing_extensions~=4.4.0; python_version<'3.12'",
-    "spellwise>=0.8.0",
-    "pysimstring~=1.2.1",
+    "anyascii",
+    "pysimstring",
+    "spellwise",
+    "typing_extensions",
 ]
 
 [project.optional-dependencies]
-tests = ['nltk>=3.8.0', 'spacy>=3.2.0']
-doc = ["sphinx"]
+dev = [
+    "black",
+    "flake8",
+    "pre-commit",
+]
+doc = [
+    "sphinx",
+    "sphinx-rtd-theme",
+]
+tests = [
+    "nltk",
+    "spacy",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/scossin/iamsystem_python"
 "Bug Tracker" = "https://github.com/scossin/iamsystem_python/issues"
 
 
 [tool.black]
```

### Comparing `iamsystem-0.6.0/src/iamsystem/__init__.py` & `iamsystem-0.6.1/src/iamsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/brat/adapter.py` & `iamsystem-0.6.1/src/iamsystem/brat/adapter.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/brat/formatter.py` & `iamsystem-0.6.1/src/iamsystem/brat/formatter.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/fuzzy/abbreviations.py` & `iamsystem-0.6.1/src/iamsystem/fuzzy/abbreviations.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/fuzzy/api.py` & `iamsystem-0.6.1/src/iamsystem/fuzzy/api.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/fuzzy/cache.py` & `iamsystem-0.6.1/src/iamsystem/fuzzy/cache.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/fuzzy/exact.py` & `iamsystem-0.6.1/src/iamsystem/fuzzy/exact.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/fuzzy/norm_fun.py` & `iamsystem-0.6.1/src/iamsystem/fuzzy/norm_fun.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/fuzzy/regex.py` & `iamsystem-0.6.1/src/iamsystem/fuzzy/regex.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/fuzzy/simstring.py` & `iamsystem-0.6.1/src/iamsystem/fuzzy/simstring.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/fuzzy/spellwise.py` & `iamsystem-0.6.1/src/iamsystem/fuzzy/spellwise.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/fuzzy/util.py` & `iamsystem-0.6.1/src/iamsystem/fuzzy/util.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/keywords/api.py` & `iamsystem-0.6.1/src/iamsystem/keywords/api.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/keywords/collection.py` & `iamsystem-0.6.1/src/iamsystem/keywords/collection.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/keywords/keywords.py` & `iamsystem-0.6.1/src/iamsystem/keywords/keywords.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/keywords/util.py` & `iamsystem-0.6.1/src/iamsystem/keywords/util.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/matcher/annotation.py` & `iamsystem-0.6.1/src/iamsystem/matcher/annotation.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/matcher/api.py` & `iamsystem-0.6.1/src/iamsystem/matcher/api.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/matcher/matcher.py` & `iamsystem-0.6.1/src/iamsystem/matcher/matcher.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/matcher/printannot.py` & `iamsystem-0.6.1/src/iamsystem/matcher/printannot.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/matcher/strategy.py` & `iamsystem-0.6.1/src/iamsystem/matcher/strategy.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/matcher/util.py` & `iamsystem-0.6.1/src/iamsystem/matcher/util.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/spacy/component.py` & `iamsystem-0.6.1/src/iamsystem/spacy/component.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/spacy/token.py` & `iamsystem-0.6.1/src/iamsystem/spacy/token.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/spacy/tokenizer.py` & `iamsystem-0.6.1/src/iamsystem/spacy/tokenizer.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/stopwords/api.py` & `iamsystem-0.6.1/src/iamsystem/stopwords/api.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/stopwords/negative.py` & `iamsystem-0.6.1/src/iamsystem/stopwords/negative.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/stopwords/simple.py` & `iamsystem-0.6.1/src/iamsystem/stopwords/simple.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/tokenization/api.py` & `iamsystem-0.6.1/src/iamsystem/tokenization/api.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/tokenization/span.py` & `iamsystem-0.6.1/src/iamsystem/tokenization/span.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/tokenization/token.py` & `iamsystem-0.6.1/src/iamsystem/tokenization/token.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/tokenization/tokenize.py` & `iamsystem-0.6.1/src/iamsystem/tokenization/tokenize.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/tokenization/util.py` & `iamsystem-0.6.1/src/iamsystem/tokenization/util.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/tree/nodes.py` & `iamsystem-0.6.1/src/iamsystem/tree/nodes.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem/tree/trie.py` & `iamsystem-0.6.1/src/iamsystem/tree/trie.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/src/iamsystem.egg-info/PKG-INFO` & `iamsystem-0.6.1/src/iamsystem.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamsystem
-Version: 0.6.0
+Version: 0.6.1
 Summary: A python implementation of IAMsystem algorithm
 Author-email: Sebastien Cossin <cossin.sebastien@gmail.com>
 Project-URL: Homepage, https://github.com/scossin/iamsystem_python
 Project-URL: Bug Tracker, https://github.com/scossin/iamsystem_python/issues
 Keywords: NLP,semantic annotation,entity linking
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
@@ -14,24 +14,28 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: anyascii>=0.3.2
-Requires-Dist: typing_extensions>=4.7.0; python_version >= "3.12"
-Requires-Dist: typing_extensions~=4.4.0; python_version < "3.12"
-Requires-Dist: spellwise>=0.8.0
-Requires-Dist: pysimstring~=1.2.1
-Provides-Extra: tests
-Requires-Dist: nltk>=3.8.0; extra == "tests"
-Requires-Dist: spacy>=3.2.0; extra == "tests"
+Requires-Dist: anyascii
+Requires-Dist: pysimstring
+Requires-Dist: spellwise
+Requires-Dist: typing_extensions
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx-rtd-theme; extra == "doc"
+Provides-Extra: tests
+Requires-Dist: nltk; extra == "tests"
+Requires-Dist: spacy; extra == "tests"
 
 # iamsystem
 ![test](https://github.com/scossin/iamsystem_python/actions/workflows/tests.yml/badge.svg)
 [![PyPI version fury.io](https://badge.fury.io/py/iamsystem.svg)](https://pypi.org/project/iamsystem/)
 [![PyPI license](https://img.shields.io/pypi/l/iamsystem.svg)](https://pypi.python.org/pypi/iamsystem/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/iamsystem.svg)](https://pypi.python.org/pypi/iamsystem/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
```

### Comparing `iamsystem-0.6.0/src/iamsystem.egg-info/SOURCES.txt` & `iamsystem-0.6.1/src/iamsystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/tests/test_annotation.py` & `iamsystem-0.6.1/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/tests/test_brat.py` & `iamsystem-0.6.1/tests/test_brat.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/tests/test_detect.py` & `iamsystem-0.6.1/tests/test_detect.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/tests/test_doc.py` & `iamsystem-0.6.1/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/tests/test_fuzzy.py` & `iamsystem-0.6.1/tests/test_fuzzy.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/tests/test_matcher.py` & `iamsystem-0.6.1/tests/test_matcher.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/tests/test_simstring.py` & `iamsystem-0.6.1/tests/test_simstring.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/tests/test_spacy.py` & `iamsystem-0.6.1/tests/test_spacy.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/tests/test_spellwise.py` & `iamsystem-0.6.1/tests/test_spellwise.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/tests/test_stopwords.py` & `iamsystem-0.6.1/tests/test_stopwords.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/tests/test_terminology.py` & `iamsystem-0.6.1/tests/test_terminology.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/tests/test_toknorm.py` & `iamsystem-0.6.1/tests/test_toknorm.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.6.0/tests/test_tree.py` & `iamsystem-0.6.1/tests/test_tree.py`

 * *Files identical despite different names*

