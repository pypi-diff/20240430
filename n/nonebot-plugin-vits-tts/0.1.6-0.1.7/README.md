# Comparing `tmp/nonebot_plugin_vits_tts-0.1.6.tar.gz` & `tmp/nonebot_plugin_vits_tts-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_vits_tts-0.1.6.tar", last modified: Thu Mar  7 05:12:38 2024, max compression
+gzip compressed data, was "nonebot_plugin_vits_tts-0.1.7.tar", last modified: Tue Apr 30 10:14:39 2024, max compression
```

## Comparing `nonebot_plugin_vits_tts-0.1.6.tar` & `nonebot_plugin_vits_tts-0.1.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:12:38.799844 nonebot_plugin_vits_tts-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-03-07 05:12:38.795844 nonebot_plugin_vits_tts-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:12:38.791844 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:12:38.791844 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/utils/lang_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/utils/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:12:38.795844 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/attentions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/commons.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/language.py
--rw-r--r--   0 runner    (1001) docker     (127)    21551 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:12:38.795844 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/monotonic_align/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/monotonic_align/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/monotonic_align/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:12:38.795844 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/cantonese.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/cleaners.py
--rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/english.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/japanese.py
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/korean.py
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/mandarin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/ngu_dialect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/sanskrit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/shanghainese.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/thai.py
--rw-r--r--   0 runner    (1001) docker     (127)     8450 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    14225 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/voice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 05:12:38.795844 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-03-07 05:12:38.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-07 05:12:38.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 05:12:38.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-07 05:12:38.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-07 05:12:38.000000 nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 05:12:38.799844 nonebot_plugin_vits_tts-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-07 05:12:32.000000 nonebot_plugin_vits_tts-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:39.235400 nonebot_plugin_vits_tts-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-30 10:14:39.235400 nonebot_plugin_vits_tts-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:39.227400 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:39.231400 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/utils/lang_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/utils/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:39.231400 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/attentions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21551 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:39.231400 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/monotonic_align/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/monotonic_align/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/monotonic_align/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:39.235400 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/cantonese.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/cleaners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/english.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/japanese.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/korean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/mandarin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/ngu_dialect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/sanskrit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/shanghainese.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/thai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8450 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14225 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/voice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:39.235400 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-30 10:14:39.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-30 10:14:39.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 10:14:39.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-30 10:14:39.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 10:14:39.000000 nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 10:14:39.235400 nonebot_plugin_vits_tts-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-30 10:14:32.000000 nonebot_plugin_vits_tts-0.1.7/setup.py
```

### Comparing `nonebot_plugin_vits_tts-0.1.6/LICENSE` & `nonebot_plugin_vits_tts-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/PKG-INFO` & `nonebot_plugin_vits_tts-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_vits_tts
-Version: 0.1.6
+Version: 0.1.7
 Summary: nonebot-plugin-vits-tts
 Home-page: https://github.com/Redmomn/nonebot-plugin-vits-tts
 Author: Redmomn
 Author-email: 109732988+Redmomn@users.noreply.github.com
 License: Apache-2.0
 Keywords: nonebot2,vits,tts
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_vits_tts Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_vits_tts Version: 0.1.7 Summary:
 nonebot-plugin-vits-tts Home-page: https://github.com/Redmomn/nonebot-plugin-
 vits-tts Author: Redmomn Author-email:
 109732988+Redmomn@users.noreply.github.com License: Apache-2.0 Keywords:
 nonebot2,vits,tts Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: torch Requires-Dist: torchvision Requires-Dist: torchaudio
 Requires-Dist: numpy>=1.22.0 Requires-Dist: scipy Requires-Dist: regex
 Requires-Dist: cn2an Requires-Dist: opencc Requires-Dist: inflect Requires-
```

### Comparing `nonebot_plugin_vits_tts-0.1.6/README.md` & `nonebot_plugin_vits_tts-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/config.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/matcher.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/matcher.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/rule.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/rule.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/utils/audio.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/utils/audio.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/utils/lang_id.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/utils/lang_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 logging.basicConfig(level=logging.INFO)
 use_tencent_tmt = False
 if config.tencent_secret_key and config.tencent_secret_id:
     try:
         cred = credential.Credential(config.tencent_secret_id, config.tencent_secret_key)
         httpProfile = HttpProfile()
         httpProfile.endpoint = "tmt.tencentcloudapi.com"
-        httpProfile.req
         clientProfile = ClientProfile()
         clientProfile.httpProfile = httpProfile
         client = tmt_client.TmtClient(cred, "ap-beijing", clientProfile)
         use_tencent_tmt = True
     except:
         pass
```

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/utils/model.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/utils/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/attentions.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/attentions.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/commons.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/commons.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/models.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/modules.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/modules.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/monotonic_align/__init__.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/monotonic_align/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/monotonic_align/core.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/monotonic_align/core.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/__init__.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/cantonese.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/cantonese.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/cleaners.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/cleaners.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/english.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/english.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/japanese.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/japanese.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/korean.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/korean.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/mandarin.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/mandarin.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/ngu_dialect.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/ngu_dialect.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/sanskrit.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/sanskrit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/shanghainese.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/shanghainese.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/symbols.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/symbols.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/text/thai.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/text/thai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/transforms.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/transforms.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/utils.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts/vits/voice.py` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts/vits/voice.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts.egg-info/PKG-INFO` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_vits_tts
-Version: 0.1.6
+Version: 0.1.7
 Summary: nonebot-plugin-vits-tts
 Home-page: https://github.com/Redmomn/nonebot-plugin-vits-tts
 Author: Redmomn
 Author-email: 109732988+Redmomn@users.noreply.github.com
 License: Apache-2.0
 Keywords: nonebot2,vits,tts
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_vits_tts Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_vits_tts Version: 0.1.7 Summary:
 nonebot-plugin-vits-tts Home-page: https://github.com/Redmomn/nonebot-plugin-
 vits-tts Author: Redmomn Author-email:
 109732988+Redmomn@users.noreply.github.com License: Apache-2.0 Keywords:
 nonebot2,vits,tts Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: torch Requires-Dist: torchvision Requires-Dist: torchaudio
 Requires-Dist: numpy>=1.22.0 Requires-Dist: scipy Requires-Dist: regex
 Requires-Dist: cn2an Requires-Dist: opencc Requires-Dist: inflect Requires-
```

### Comparing `nonebot_plugin_vits_tts-0.1.6/nonebot_plugin_vits_tts.egg-info/SOURCES.txt` & `nonebot_plugin_vits_tts-0.1.7/nonebot_plugin_vits_tts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_vits_tts-0.1.6/setup.py` & `nonebot_plugin_vits_tts-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nonebot_plugin_vits_tts',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(),
     install_requires=[
         'torch',
         'torchvision',
         'torchaudio',
         'numpy>=1.22.0',
         'scipy',
```

