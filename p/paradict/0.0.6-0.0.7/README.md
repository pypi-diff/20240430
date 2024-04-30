# Comparing `tmp/paradict-0.0.6.tar.gz` & `tmp/paradict-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/paradict-0.0.6.tar", last modified: Wed Mar 13 23:05:37 2024, max compression
+gzip compressed data, was "dist/paradict-0.0.7.tar", last modified: Tue Apr 30 20:04:28 2024, max compression
```

## Comparing `paradict-0.0.6.tar` & `paradict-0.0.7.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:37.354543 paradict-0.0.6/
--rw-rw-r--   0 alex      (1002) alex      (1003)     1082 2024-01-11 12:42:56.000000 paradict-0.0.6/LICENSE
--rw-rw-r--   0 alex      (1002) alex      (1003)       70 2023-06-16 19:49:24.000000 paradict-0.0.6/MANIFEST.in
--rw-rw-r--   0 alex      (1002) alex      (1003)    25765 2024-03-13 23:05:37.354543 paradict-0.0.6/PKG-INFO
--rw-rw-r--   0 alex      (1002) alex      (1003)    25176 2024-03-13 20:01:20.000000 paradict-0.0.6/README.md
--rw-rw-r--   0 alex      (1002) alex      (1003)        5 2024-01-04 07:50:33.000000 paradict-0.0.6/VERSION
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:36.758528 paradict-0.0.6/paradict/
--rw-rw-r--   0 alex      (1002) alex      (1003)      827 2024-03-13 19:40:59.000000 paradict-0.0.6/paradict/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      134 2023-06-17 17:17:51.000000 paradict-0.0.6/paradict/__main__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:36.810529 paradict-0.0.6/paradict/box/
--rw-rw-r--   0 alex      (1002) alex      (1003)     2711 2024-01-03 15:20:06.000000 paradict-0.0.6/paradict/box/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:36.826530 paradict-0.0.6/paradict/const/
--rw-rw-r--   0 alex      (1002) alex      (1003)      184 2024-02-28 16:02:50.000000 paradict-0.0.6/paradict/const/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:36.878531 paradict-0.0.6/paradict/deserializer/
--rw-rw-r--   0 alex      (1002) alex      (1003)     2974 2023-10-24 15:52:06.000000 paradict-0.0.6/paradict/deserializer/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)    21785 2024-01-11 12:26:06.000000 paradict-0.0.6/paradict/deserializer/decoder.py
--rw-rw-r--   0 alex      (1002) alex      (1003)    23980 2024-01-11 12:26:06.000000 paradict-0.0.6/paradict/deserializer/unpacker.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:36.902531 paradict-0.0.6/paradict/errors/
--rw-rw-r--   0 alex      (1002) alex      (1003)      107 2023-09-23 07:46:13.000000 paradict-0.0.6/paradict/errors/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:36.918532 paradict-0.0.6/paradict/kv/
--rw-rw-r--   0 alex      (1002) alex      (1003)     2611 2023-12-28 21:03:34.000000 paradict-0.0.6/paradict/kv/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:36.934532 paradict-0.0.6/paradict/misc/
--rw-rw-r--   0 alex      (1002) alex      (1003)    13301 2023-12-26 16:07:04.000000 paradict-0.0.6/paradict/misc/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:36.974533 paradict-0.0.6/paradict/queue/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-08-24 14:03:53.000000 paradict-0.0.6/paradict/queue/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)    10813 2024-01-11 12:26:06.000000 paradict-0.0.6/paradict/queue/bin_queue.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     1259 2024-01-11 12:26:07.000000 paradict-0.0.6/paradict/queue/txt_queue.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:37.026535 paradict-0.0.6/paradict/serializer/
--rw-rw-r--   0 alex      (1002) alex      (1003)     2057 2023-10-24 15:52:06.000000 paradict-0.0.6/paradict/serializer/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)    15019 2024-02-01 12:16:02.000000 paradict-0.0.6/paradict/serializer/encoder.py
--rw-rw-r--   0 alex      (1002) alex      (1003)    16024 2024-01-06 10:21:01.000000 paradict-0.0.6/paradict/serializer/packer.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:37.058536 paradict-0.0.6/paradict/spec/
--rw-rw-r--   0 alex      (1002) alex      (1003)    27053 2024-01-04 07:43:51.000000 paradict-0.0.6/paradict/spec/bin_paradict_spec.md
--rw-rw-r--   0 alex      (1002) alex      (1003)    12568 2024-01-03 15:43:43.000000 paradict-0.0.6/paradict/spec/txt_paradict_spec.md
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:37.090536 paradict-0.0.6/paradict/tags/
--rw-rw-r--   0 alex      (1002) alex      (1003)     6594 2024-01-04 07:33:20.000000 paradict-0.0.6/paradict/tags/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     2928 2023-12-15 11:03:29.000000 paradict-0.0.6/paradict/tags/misc.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:37.106537 paradict-0.0.6/paradict/typeref/
--rw-rw-r--   0 alex      (1002) alex      (1003)    16285 2024-01-03 15:20:05.000000 paradict-0.0.6/paradict/typeref/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:37.122537 paradict-0.0.6/paradict/validator/
--rw-rw-r--   0 alex      (1002) alex      (1003)     7115 2024-01-03 15:20:06.000000 paradict-0.0.6/paradict/validator/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:36.810529 paradict-0.0.6/paradict.egg-info/
--rw-r--r--   0 alex      (1002) alex      (1003)    25765 2024-03-13 23:05:36.000000 paradict-0.0.6/paradict.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1002) alex      (1003)     1605 2024-03-13 23:05:36.000000 paradict-0.0.6/paradict.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2024-03-13 23:05:36.000000 paradict-0.0.6/paradict.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)       53 2024-03-13 23:05:36.000000 paradict-0.0.6/paradict.egg-info/entry_points.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2023-06-16 19:52:16.000000 paradict-0.0.6/paradict.egg-info/not-zip-safe
--rw-rw-r--   0 alex      (1002) alex      (1003)       15 2024-03-13 23:05:36.000000 paradict-0.0.6/paradict.egg-info/requires.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)       15 2024-03-13 23:05:36.000000 paradict-0.0.6/paradict.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)      100 2023-06-16 19:49:24.000000 paradict-0.0.6/pyproject.toml
--rw-rw-r--   0 alex      (1002) alex      (1003)      805 2024-03-13 23:05:37.354543 paradict-0.0.6/setup.cfg
--rw-rw-r--   0 alex      (1002) alex      (1003)      100 2023-06-16 19:49:24.000000 paradict-0.0.6/setup.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:37.142538 paradict-0.0.6/tests/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-06-16 19:49:24.000000 paradict-0.0.6/tests/__init__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:37.170539 paradict-0.0.6/tests/box/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-08-24 14:10:25.000000 paradict-0.0.6/tests/box/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     4283 2023-11-25 16:22:31.000000 paradict-0.0.6/tests/box/test_box.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:37.222540 paradict-0.0.6/tests/deserializer/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-07-30 16:21:57.000000 paradict-0.0.6/tests/deserializer/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)    27493 2024-01-03 15:28:32.000000 paradict-0.0.6/tests/deserializer/test_decoder.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      921 2023-10-21 10:15:59.000000 paradict-0.0.6/tests/deserializer/test_funcs.py
--rw-rw-r--   0 alex      (1002) alex      (1003)    26707 2024-01-03 15:28:33.000000 paradict-0.0.6/tests/deserializer/test_unpacker.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:37.222540 paradict-0.0.6/tests/kv/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-08-24 14:09:21.000000 paradict-0.0.6/tests/kv/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     2816 2023-08-16 11:48:13.000000 paradict-0.0.6/tests/kv/test_kv.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:37.238540 paradict-0.0.6/tests/misc/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-08-24 14:10:37.000000 paradict-0.0.6/tests/misc/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     2629 2023-10-21 09:18:12.000000 paradict-0.0.6/tests/misc/test_misc.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:37.270541 paradict-0.0.6/tests/queue/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-08-24 17:19:40.000000 paradict-0.0.6/tests/queue/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     8280 2024-01-11 12:26:06.000000 paradict-0.0.6/tests/queue/test_bin_queue.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      754 2024-01-11 12:26:06.000000 paradict-0.0.6/tests/queue/test_txt_queue.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:37.286542 paradict-0.0.6/tests/serializer/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-07-30 16:22:30.000000 paradict-0.0.6/tests/serializer/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)    28682 2024-01-03 15:28:33.000000 paradict-0.0.6/tests/serializer/test_encoder.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      967 2023-10-21 10:15:30.000000 paradict-0.0.6/tests/serializer/test_funcs.py
--rw-rw-r--   0 alex      (1002) alex      (1003)    71368 2024-01-06 10:21:02.000000 paradict-0.0.6/tests/serializer/test_packer.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:37.322543 paradict-0.0.6/tests/streaming/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-08-24 14:09:40.000000 paradict-0.0.6/tests/streaming/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     1442 2023-08-12 10:23:31.000000 paradict-0.0.6/tests/streaming/test_bin_streaming.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     1477 2023-11-19 17:06:46.000000 paradict-0.0.6/tests/streaming/test_txt_streaming.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     1042 2024-03-13 19:41:14.000000 paradict-0.0.6/tests/test_imports.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-03-13 23:05:37.342543 paradict-0.0.6/tests/validator/
--rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-10-16 19:15:05.000000 paradict-0.0.6/tests/validator/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)    15508 2023-12-28 22:12:49.000000 paradict-0.0.6/tests/validator/test_validator.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.421003 paradict-0.0.7/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1082 2024-01-11 12:42:56.000000 paradict-0.0.7/LICENSE
+-rw-rw-r--   0 alex      (1002) alex      (1003)       70 2023-06-16 19:49:24.000000 paradict-0.0.7/MANIFEST.in
+-rw-rw-r--   0 alex      (1002) alex      (1003)    26032 2024-04-30 20:04:28.421003 paradict-0.0.7/PKG-INFO
+-rw-rw-r--   0 alex      (1002) alex      (1003)    25443 2024-04-30 15:07:56.000000 paradict-0.0.7/README.md
+-rw-rw-r--   0 alex      (1002) alex      (1003)        5 2024-03-13 23:05:38.000000 paradict-0.0.7/VERSION
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.020987 paradict-0.0.7/paradict/
+-rw-rw-r--   0 alex      (1002) alex      (1003)      868 2024-04-29 20:10:26.000000 paradict-0.0.7/paradict/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)      308 2024-04-30 00:50:34.000000 paradict-0.0.7/paradict/__main__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.052988 paradict-0.0.7/paradict/box/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     2818 2024-04-30 00:50:34.000000 paradict-0.0.7/paradict/box/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.068989 paradict-0.0.7/paradict/const/
+-rw-rw-r--   0 alex      (1002) alex      (1003)      184 2024-02-28 16:02:50.000000 paradict-0.0.7/paradict/const/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.108990 paradict-0.0.7/paradict/deserializer/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     3989 2024-04-30 00:50:34.000000 paradict-0.0.7/paradict/deserializer/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)    21806 2024-04-30 00:50:34.000000 paradict-0.0.7/paradict/deserializer/decoder.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)    24000 2024-04-30 00:50:34.000000 paradict-0.0.7/paradict/deserializer/unpacker.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.128991 paradict-0.0.7/paradict/errors/
+-rw-rw-r--   0 alex      (1002) alex      (1003)      107 2023-09-23 07:46:13.000000 paradict-0.0.7/paradict/errors/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.136991 paradict-0.0.7/paradict/kv/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     2636 2024-04-30 00:50:34.000000 paradict-0.0.7/paradict/kv/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.136991 paradict-0.0.7/paradict/misc/
+-rw-rw-r--   0 alex      (1002) alex      (1003)    13326 2024-04-30 00:50:34.000000 paradict-0.0.7/paradict/misc/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.140992 paradict-0.0.7/paradict/queue/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-08-24 14:03:53.000000 paradict-0.0.7/paradict/queue/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)    10813 2024-04-30 00:50:34.000000 paradict-0.0.7/paradict/queue/bin_queue.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1284 2024-04-30 00:50:33.000000 paradict-0.0.7/paradict/queue/txt_queue.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.184993 paradict-0.0.7/paradict/serializer/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     2724 2024-04-30 00:50:34.000000 paradict-0.0.7/paradict/serializer/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)    15014 2024-04-29 20:47:47.000000 paradict-0.0.7/paradict/serializer/encoder.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)    16042 2024-04-30 00:50:34.000000 paradict-0.0.7/paradict/serializer/packer.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.200994 paradict-0.0.7/paradict/spec/
+-rw-rw-r--   0 alex      (1002) alex      (1003)    27053 2024-01-04 07:43:51.000000 paradict-0.0.7/paradict/spec/bin_paradict_spec.md
+-rw-rw-r--   0 alex      (1002) alex      (1003)    12568 2024-01-03 15:43:43.000000 paradict-0.0.7/paradict/spec/txt_paradict_spec.md
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.228995 paradict-0.0.7/paradict/tags/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     6600 2024-04-30 19:38:11.000000 paradict-0.0.7/paradict/tags/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     2943 2024-04-30 00:50:34.000000 paradict-0.0.7/paradict/tags/misc.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.232995 paradict-0.0.7/paradict/typeref/
+-rw-rw-r--   0 alex      (1002) alex      (1003)    16304 2024-04-30 00:50:34.000000 paradict-0.0.7/paradict/typeref/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.232995 paradict-0.0.7/paradict/validator/
+-rw-rw-r--   0 alex      (1002) alex      (1003)     7184 2024-04-30 00:50:34.000000 paradict-0.0.7/paradict/validator/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.052988 paradict-0.0.7/paradict.egg-info/
+-rw-r--r--   0 alex      (1002) alex      (1003)    26032 2024-04-30 20:04:27.000000 paradict-0.0.7/paradict.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1605 2024-04-30 20:04:27.000000 paradict-0.0.7/paradict.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2024-04-30 20:04:27.000000 paradict-0.0.7/paradict.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)       53 2024-04-30 20:04:27.000000 paradict-0.0.7/paradict.egg-info/entry_points.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2023-06-16 19:52:16.000000 paradict-0.0.7/paradict.egg-info/not-zip-safe
+-rw-rw-r--   0 alex      (1002) alex      (1003)       15 2024-04-30 20:04:27.000000 paradict-0.0.7/paradict.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)       15 2024-04-30 20:04:27.000000 paradict-0.0.7/paradict.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)      100 2023-06-16 19:49:24.000000 paradict-0.0.7/pyproject.toml
+-rw-rw-r--   0 alex      (1002) alex      (1003)      805 2024-04-30 20:04:28.421003 paradict-0.0.7/setup.cfg
+-rw-rw-r--   0 alex      (1002) alex      (1003)      100 2023-06-16 19:49:24.000000 paradict-0.0.7/setup.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.232995 paradict-0.0.7/tests/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-06-16 19:49:24.000000 paradict-0.0.7/tests/__init__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.236996 paradict-0.0.7/tests/box/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-08-24 14:10:25.000000 paradict-0.0.7/tests/box/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     4283 2023-11-25 16:22:31.000000 paradict-0.0.7/tests/box/test_box.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.276997 paradict-0.0.7/tests/deserializer/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-07-30 16:21:57.000000 paradict-0.0.7/tests/deserializer/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)    27493 2024-01-03 15:28:32.000000 paradict-0.0.7/tests/deserializer/test_decoder.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1365 2024-04-29 20:33:37.000000 paradict-0.0.7/tests/deserializer/test_funcs.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)    26707 2024-01-03 15:28:33.000000 paradict-0.0.7/tests/deserializer/test_unpacker.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.276997 paradict-0.0.7/tests/kv/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-08-24 14:09:21.000000 paradict-0.0.7/tests/kv/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     2816 2023-08-16 11:48:13.000000 paradict-0.0.7/tests/kv/test_kv.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.292998 paradict-0.0.7/tests/misc/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-08-24 14:10:37.000000 paradict-0.0.7/tests/misc/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     2629 2023-10-21 09:18:12.000000 paradict-0.0.7/tests/misc/test_misc.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.320999 paradict-0.0.7/tests/queue/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-08-24 17:19:40.000000 paradict-0.0.7/tests/queue/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     8280 2024-01-11 12:26:06.000000 paradict-0.0.7/tests/queue/test_bin_queue.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)      754 2024-01-11 12:26:06.000000 paradict-0.0.7/tests/queue/test_txt_queue.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.353000 paradict-0.0.7/tests/serializer/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-07-30 16:22:30.000000 paradict-0.0.7/tests/serializer/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)    28682 2024-01-03 15:28:33.000000 paradict-0.0.7/tests/serializer/test_encoder.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1481 2024-04-29 20:29:13.000000 paradict-0.0.7/tests/serializer/test_funcs.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)    71368 2024-01-06 10:21:02.000000 paradict-0.0.7/tests/serializer/test_packer.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.385002 paradict-0.0.7/tests/streaming/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-08-24 14:09:40.000000 paradict-0.0.7/tests/streaming/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1442 2023-08-12 10:23:31.000000 paradict-0.0.7/tests/streaming/test_bin_streaming.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1477 2023-11-19 17:06:46.000000 paradict-0.0.7/tests/streaming/test_txt_streaming.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     1119 2024-04-29 20:24:33.000000 paradict-0.0.7/tests/test_imports.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2024-04-30 20:04:28.405002 paradict-0.0.7/tests/validator/
+-rw-rw-r--   0 alex      (1002) alex      (1003)        0 2023-10-16 19:15:05.000000 paradict-0.0.7/tests/validator/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)    15508 2023-12-28 22:12:49.000000 paradict-0.0.7/tests/validator/test_validator.py
```

### Comparing `paradict-0.0.6/LICENSE` & `paradict-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `paradict-0.0.6/PKG-INFO` & `paradict-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradict
-Version: 0.0.6
+Version: 0.0.7
 Summary: Streamable multi-format serialization with schema
 Home-page: https://github.com/pyrustic/paradict
 Author: Pyrustic Evangelist
 Author-email: rusticalex@yahoo.com
 Maintainer: Pyrustic Evangelist
 Maintainer-email: rusticalex@yahoo.com
 License: MIT
@@ -263,22 +263,21 @@
 # Application programming interface
 The API exposes four foundational classes, Encoder, Decoder, Packer, and Unpacker, that serialize and deserialize data iteratively. 
 
 On top of these classes, four functions, encode, decode, pack, and unpack, do the same thing but in bulk. 
 
 Then there are additional classes and functions to do various stuff such as the TypeRef class for types customization, load and dump functions for reading and writing binary Paradict file, etc.
 
-Note that this section is just an overview of the API, thus it doesn't replace the module documentation.
+Note that this section is just an overview of the API, thus it doesn't replace the **API reference**.
 
-> Please explore the source code ! The documentation generator isn't yet ready !
+> Explore [API reference](https://github.com/pyrustic/paradict/tree/master/docs/api).
 
 ## Textual serialization
 Encoder and Decoder are the foundation classes for serializing and deserializing data. These classes process data iteratively. On top of these classes, two functions, encode and decode, do the same thing but in bulk.
 
-
 ### Using the Encoder class
 The Encoder constructor accepts `mode`, type_ref, skip_comments and skip_bin_data as arguments. 
 
 The `encode` method of this class takes as input a Python dictionary, then iteratively serialize it, yielding a line after another.
 
 ```python
 from paradict import Encoder
@@ -371,14 +370,29 @@
 print(r)
 ```
 Output:
 ```text
 {'id': 42, 'name': 'alex'}
 ```
 
+### Load and dump
+
+```python
+from paradict import read, write
+
+path = "/home/alex/user_card.bin"
+data = {"id": 42, "name": "alex"}
+# Serialize and write data to user_card.text
+write(data, path)
+# Read and deserialize data
+r = read(path)
+# test
+assert data == r
+```
+
 
 ### Miscellaneous functions
 Under the hood, the `Deserializer` class uses a public function for splitting a key-value line into three parts:
 - the key,
 - the value,
 - and the separator character.
```

### Comparing `paradict-0.0.6/README.md` & `paradict-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -244,22 +244,21 @@
 # Application programming interface
 The API exposes four foundational classes, Encoder, Decoder, Packer, and Unpacker, that serialize and deserialize data iteratively. 
 
 On top of these classes, four functions, encode, decode, pack, and unpack, do the same thing but in bulk. 
 
 Then there are additional classes and functions to do various stuff such as the TypeRef class for types customization, load and dump functions for reading and writing binary Paradict file, etc.
 
-Note that this section is just an overview of the API, thus it doesn't replace the module documentation.
+Note that this section is just an overview of the API, thus it doesn't replace the **API reference**.
 
-> Please explore the source code ! The documentation generator isn't yet ready !
+> Explore [API reference](https://github.com/pyrustic/paradict/tree/master/docs/api).
 
 ## Textual serialization
 Encoder and Decoder are the foundation classes for serializing and deserializing data. These classes process data iteratively. On top of these classes, two functions, encode and decode, do the same thing but in bulk.
 
-
 ### Using the Encoder class
 The Encoder constructor accepts `mode`, type_ref, skip_comments and skip_bin_data as arguments. 
 
 The `encode` method of this class takes as input a Python dictionary, then iteratively serialize it, yielding a line after another.
 
 ```python
 from paradict import Encoder
@@ -352,14 +351,29 @@
 print(r)
 ```
 Output:
 ```text
 {'id': 42, 'name': 'alex'}
 ```
 
+### Load and dump
+
+```python
+from paradict import read, write
+
+path = "/home/alex/user_card.bin"
+data = {"id": 42, "name": "alex"}
+# Serialize and write data to user_card.text
+write(data, path)
+# Read and deserialize data
+r = read(path)
+# test
+assert data == r
+```
+
 
 ### Miscellaneous functions
 Under the hood, the `Deserializer` class uses a public function for splitting a key-value line into three parts:
 - the key,
 - the value,
 - and the separator character.
```

### Comparing `paradict-0.0.6/paradict/__init__.py` & `paradict-0.0.7/paradict/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from paradict.serializer import encode, pack, dump
+from paradict.serializer import encode, pack, dump, write
 from paradict.serializer.encoder import Encoder
 from paradict.serializer.packer import Packer
-from paradict.deserializer import decode, unpack, load
+from paradict.deserializer import decode, unpack, load, read
 from paradict.deserializer.decoder import Decoder
 from paradict.deserializer.unpacker import Unpacker
 from paradict.typeref import TypeRef
 from paradict.validator import validate, Validator
 from paradict.kv import split as split_kv
 from paradict.misc import forge_bin, stringify_bin
 from paradict.const import CONFIG_MODE, DATA_MODE
 
 
 __all__ = ["encode", "decode",
+           "write", "read",
            "pack", "unpack",
            "load", "dump",
            "validate", "split_kv",
            "forge_bin", "stringify_bin",
            "Encoder", "Decoder",
            "Packer", "Unpacker",
            "TypeRef", "Validator", "CONFIG_MODE", "DATA_MODE"]
```

### Comparing `paradict-0.0.6/paradict/box/__init__.py` & `paradict-0.0.7/paradict/box/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """Boxes to hold comments, grids, hexadecimal integers, et cetera"""
 from paradict import misc
 from ustrid import ustrid
 
+__all__ = ["Grid", "Obj", "HexInt", "OctInt", "BinInt",
+           "CommentID", "Comment"]
 
 class Grid(list):
     """
     Box to hold a grid. A grid is made of numbers and should
     be consistent (rows should be of same size)
 
     Example:
-        # a grid with 2 rows and 3 columns
-        my_grid = Grid([(0, 1, 0),
-                        (1, 0, 1)])
+    ```
+    # a grid with 2 rows and 3 columns
+    my_grid = Grid([(0, 1, 0),
+                    (1, 0, 1)])
+    ```
     """
     pass
 
 
 class Obj(dict):
     """
     Box to hold an Extension Object. Such objects behave like a dictionary.
@@ -83,15 +87,17 @@
 
 
 class CommentID(str):
     """
     Box to hold a unique comment id.
     Instantiating this class will generate a new unique string.
     Under the hood, the 'ustrid' library is used.
-        CommentID() != CommentID()
+    ```
+    CommentID() != CommentID()
+    ```
     """
     def __new__(cls, *args, **kwargs):
         return super().__new__(cls, ustrid())
 
 
 class Comment(str):
     """Box to hold a comment string"""
```

### Comparing `paradict-0.0.6/paradict/deserializer/__init__.py` & `paradict-0.0.7/paradict/deserializer/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """High-level functions to deserialize Paradict binary/text data into a Python dict"""
 import pathlib
 from paradict.deserializer.decoder import Decoder
 from paradict.deserializer.unpacker import Unpacker
 
 
+__all__ = ["decode", "read", "unpack", "load"]
+
+
 def decode(text, type_ref=None, receiver=None, obj_builder=None,
            skip_comments=False):
     """
     Convert some textual Paradict data into a Python dictionary
 
-    [parameters]
+    [param]
     - text: string to convert into a Python dict
     - type_ref: optional TypeRef object
     - receiver: callback function that will be called at the end of conversion.
     This callback function accepts the Decoder instance as argument
     - obj_builder: function that accepts a paradict.box.Obj container and
     returns a fresh new Python object
     - skip_comments: boolean to tell whether comments should be ignored or not
@@ -27,20 +30,44 @@
     decoder.feed(text)
     if decoder.queue.buffer:
         decoder.feed("\n")
     decoder.feed("===\n")
     return decoder.data
 
 
+def read(path, type_ref=None, receiver=None, obj_builder=None,
+         skip_comments=False):
+    """
+    Open a textual Paradict file then read its contents into Python dict
+
+    [param]
+    - path: a path string, or a pathlib.Path instance
+    - type_ref: optional TypeRef object
+    - receiver: callback function that will be called at the end of conversion.
+    This callback function accepts the Decoder instance as argument
+    - obj_builder: function that accepts a paradict.box.Obj container and
+    returns a fresh new Python object
+    - skip_comments: boolean to tell whether comments should be ignored or not
+
+    [return]
+    Return the newly built Python object
+    """
+    path = str(pathlib.Path(path).resolve())
+    with open(path, "r", encoding="utf-8") as file:
+        r = file.read()
+    return decode(r, obj_builder=obj_builder, type_ref=type_ref,
+                  receiver=receiver, skip_comments=skip_comments)
+
+
 def unpack(raw, type_ref=None, receiver=None, obj_builder=None,
            skip_comments=False):
     """
     Convert some binary Paradict data into a Python dictionary
 
-    [parameters]
+    [param]
     - raw: raw data previously packed with Paradict
     - type_ref: optional TypeRef object
     - receiver: callback function that will be called at the end of conversion.
     This callback function accepts the Decoder instance as argument
     - obj_builder: function that accepts a paradict.box.Obj container and
     returns a fresh new Python object
     - skip_comments: boolean to tell whether comments should be ignored or not
@@ -52,19 +79,20 @@
                         receiver=receiver,
                         obj_builder=obj_builder,
                         skip_comments=skip_comments)
     unpacker.feed(raw)
     return unpacker.data
 
 
-def load(path, type_ref=None, obj_builder=None, skip_comments=False):
+def load(path, type_ref=None, receiver=None,
+         obj_builder=None, skip_comments=False):
     """
     Open a binary Paradict file then unpack its contents into Python dict
 
-    [parameters]
+    [param]
     - path: a path string, or a pathlib.Path instance
     - type_ref: optional TypeRef object
     - receiver: callback function that will be called at the end of conversion.
     This callback function accepts the Decoder instance as argument
     - obj_builder: function that accepts a paradict.box.Obj container and
     returns a fresh new Python object
     - skip_comments: boolean to tell whether comments should be ignored or not
@@ -72,8 +100,8 @@
     [return]
     Return the newly built Python object
     """
     path = str(pathlib.Path(path).resolve())
     with open(path, "rb") as file:
         r = file.read()
     return unpack(r, obj_builder=obj_builder, type_ref=type_ref,
-                  skip_comments=skip_comments)
+                  receiver=receiver, skip_comments=skip_comments)
```

### Comparing `paradict-0.0.6/paradict/deserializer/decoder.py` & `paradict-0.0.7/paradict/deserializer/decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 import datetime
 import base64
 from paradict import errors, misc, const, kv, box
 from paradict.typeref import TypeRef
 from paradict.queue.txt_queue import TxtQueue
 
 
+__all__ = ["Decoder"]
+
+
 class Decoder:
     """Class to convert some textual Paradict data into a Python dict"""
     def __init__(self, *, type_ref=None, receiver=None, obj_builder=None,
                  skip_comments=False):
         """
         Init
 
-        [parameters]
+        [param]
         - type_ref: optional TypeRef object
         - receiver: callback function that will be called at the end of conversion.
         This callback function accepts the Decoder instance as argument
         - obj_builder: function that accepts a paradict.box.Obj container and
         returns a fresh new Python object
         - skip_comments: boolean to tell whether comments should be ignored or not
         """
@@ -101,15 +104,15 @@
         Feed the decoder engine with some string.
         The string might represent a line in the textual Paradict data,
         or an arbitrary length of characters.
 
         Note: it is very important to make sure that each line is ended
         by a "\n" newline character
 
-        Check the paradict.decode function to see an example of
+        Check the `paradict.decode` function to see an example of
         how to use this class
         """
         if not self._feedable:
             return False
         self._queue.enqueue(s)
         for line in self._queue.dequeue():
             line = line.rstrip("\n")
```

### Comparing `paradict-0.0.6/paradict/deserializer/unpacker.py` & `paradict-0.0.7/paradict/deserializer/unpacker.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,26 @@
 from paradict.tags.misc import ALPHABET
 from paradict.typeref import TypeRef
 from paradict import errors
 from paradict.queue.bin_queue import BinQueue
 from paradict import misc, box
 
 
+__all__ = ["Unpacker"]
+
+
 class Unpacker:
     """Class to convert some binary Paradict data into a Python dict"""
 
     def __init__(self, type_ref=None, receiver=None, obj_builder=None,
                  skip_comments=False):
         """
         Init
 
-        [parameters]
+        [param]
         - type_ref: optional TypeRef object
         - receiver: callback function that will be called at the end of conversion.
         This callback function accepts the Unpacker instance as argument
         - obj_builder: function that accepts a paradict.box.Obj container and
         returns a fresh new Python object
         - skip_comments: boolean to tell whether comments should be ignored or not
         """
```

### Comparing `paradict-0.0.6/paradict/kv/__init__.py` & `paradict-0.0.7/paradict/kv/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """This module exposes the split function that will parse a valid key-value string"""
 import re
 from paradict import errors, const
 from collections import namedtuple
 
 
+__all__ = ["Info", "split"]
+
+
 Info = namedtuple("Info", ["key", "val", "sep", "mode"])
 
 
 def split(val):
     """
     Split a non-empty string into key val.
     The string should follow one of these format:
     - data_mode format: key: value
     - config_mode format: key = value
 
-    [parameters]
+    [param]
     - val: non-empty string
 
     [return]
     Return an Info namedtuple made of: key, val, sep, and mode attributes.
     The key and val are strings. The sep is either ":" or "=".
     The mode is either paradict.const.DATA_MODE or paradict.const.CONFIG_MODE.
     Note that if the sep is a colon, it means that the mode is DATA_MODE.
```

### Comparing `paradict-0.0.6/paradict/misc/__init__.py` & `paradict-0.0.7/paradict/misc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-"""Private miscellaneous functions and classes. Do not use them !"""
+"""Private miscellaneous functions and classes."""
 import math
 import datetime
 from collections import namedtuple
 from paradict import errors, const
 
 
+__all__ = ["forge_bin", "stringify_bin"]
+
+
 # TODO: update this module (write/correct docstrings, etc), and write tests
 
 IntParts = namedtuple("IntParts", ["sign", "prefix", "leading_zeros", "val"])
 FloatParts = namedtuple("FloatParts", ["sign", "left_significand",
                                        "right_significand", "exponent"])
```

### Comparing `paradict-0.0.6/paradict/queue/bin_queue.py` & `paradict-0.0.7/paradict/queue/bin_queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """A FIFO queue for processing binary Paradict data"""
 from collections import namedtuple
 from paradict import tags, errors
 from paradict.tags.misc import SIZE_TO_STR
-from paradict import misc
+
+
+__all__ = ["BinQueue"]
+
 
 # a datum is made of a header and payload
 # The header is made of a tag and optional bytes to store the size of the payload
 # The width is the size of the datum: size of header + size of payload
 Datum = namedtuple("Datum", ["tag", "payload", "width"])
```

### Comparing `paradict-0.0.6/paradict/queue/txt_queue.py` & `paradict-0.0.7/paradict/queue/txt_queue.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """A FIFO queue for processing textual Paradict data"""
 from collections import namedtuple
 
 
+__all__ = ["TxtQueue"]
+
+
 class TxtQueue:
     """A FIFO queue for processing textual Paradict data"""
     def __init__(self):
         self._buffer = list()
 
     @property
     def buffer(self):
```

### Comparing `paradict-0.0.6/paradict/serializer/__init__.py` & `paradict-0.0.7/paradict/serializer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """High-level functions to serialize Python dict in Paradict binary/text format"""
 import written
 from paradict.serializer.encoder import Encoder
 from paradict.serializer.packer import Packer
 from paradict import const
 
 
+__all__ = ["encode", "write", "pack", "dump"]
+
+
 def encode(data, *, mode=const.DATA_MODE, type_ref=None,
            skip_comments=False, skip_bin_data=False):
     """
     Convert a Python dictionary object to Paradict binary format
 
-    [parameters]
+    [param]
     - data: Python dict
     - mode: either const.DATA_MODE or const.CONFIG_MODE. Defaults to DATA_MODE.
     - type_ref: optional TypeRef object
     - skip_comments: boolean to tell whether comments should be ignored or not
     - skip_bin_data: boolean to tell whether bin data should be ignored or not
 
     [return]
@@ -25,19 +28,36 @@
                       skip_bin_data=skip_bin_data)
     lines = list()
     for r in encoder.encode(data):
         lines.append(r)
     return "\n".join(lines)
 
 
+def write(data, path, *, mode=const.DATA_MODE, type_ref=None,
+          skip_comments=False, skip_bin_data=False):
+    """
+    Convert some Python dict in the Paradict textual format
+    then write it to a file
+
+    [param]
+    - path: path string or pathlib.Path instance
+    - mode: either const.DATA_MODE or const.CONFIG_MODE. Defaults to DATA_MODE.
+    - type_ref: optional TypeRef object
+    - skip_comments: boolean to tell whether comments should be ignored or not
+    """
+    r = encode(data, mode=mode, skip_comments=skip_comments,
+               type_ref=type_ref, skip_bin_data=skip_bin_data)
+    written.write(r, path)
+
+
 def pack(data, *, type_ref=None, skip_comments=False):
     """
     Convert a Python dictionary object to Paradict binary format
 
-    [parameters]
+    [param]
     - data: Python dict
     - type_ref: optional TypeRef object
     - skip_comments: boolean to tell whether comments should be ignored or not
 
     [return]
     Return a Python bytes object packed in the Paradict binary format
     """
@@ -48,14 +68,15 @@
     return bytes(buffer)
 
 
 def dump(data, path, *, type_ref=None, skip_comments=False):
     """
     Convert some Python dict in the Paradict binary format
     then dump it in a file
-    [parameters]
+
+    [param]
     - path: path string or pathlib.Path instance
     - type_ref: optional TypeRef object
     - skip_comments: boolean to tell whether comments should be ignored or not
     """
     r = pack(data, skip_comments=skip_comments, type_ref=type_ref)
     written.write(r, path)
```

### Comparing `paradict-0.0.6/paradict/serializer/encoder.py` & `paradict-0.0.7/paradict/serializer/encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class Encoder:
     """Convert a Python dictionary object to Paradict text format"""
     def __init__(self, mode=const.DATA_MODE, type_ref=None,
                  skip_comments=False, skip_bin_data=False):
         """
         Init
 
-        [parameters]
+        [param]
         - mode: either const.DATA_MODE or const.CONFIG_MODE. Defaults to DATA_MODE.
         - type_ref: optional TypeRef object
         - skip_comments: boolean to tell whether comments should be ignored or not
         - skip_bin_data: boolean to tell whether bin data should be ignored or not
         """
         self._mode = mode
         self._type_ref = type_ref if type_ref else TypeRef()
```

### Comparing `paradict-0.0.6/paradict/serializer/packer.py` & `paradict-0.0.7/paradict/serializer/packer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 from paradict.typeref import TypeRef
 from paradict import tags
 from paradict.tags.misc import SIZE_TO_PINT, \
     SIZE_TO_NINT, ALPHABET, SIZE_TO_STR
 from paradict import errors, misc
 
 
+__all__ = ["Packer"]
+
+
 class Packer:
     """
     Class to convert some binary Python dict into Paradict binary format
     """
     def __init__(self, type_ref=None, skip_comments=False):
         """
         Init
 
-        [parameters]
+        [param]
         - type_ref: optional TypeRef object
         - skip_comments: boolean to tell whether comments should be ignored or not
         """
         self._type_ref = type_ref if type_ref else TypeRef()
         self._skip_comments = skip_comments
         self._converters = {"dict": self._pack_dict,
                             "list": self._pack_list,
```

### Comparing `paradict-0.0.6/paradict/spec/bin_paradict_spec.md` & `paradict-0.0.7/paradict/spec/bin_paradict_spec.md`

 * *Files identical despite different names*

### Comparing `paradict-0.0.6/paradict/spec/txt_paradict_spec.md` & `paradict-0.0.7/paradict/spec/txt_paradict_spec.md`

 * *Files identical despite different names*

### Comparing `paradict-0.0.6/paradict/tags/__init__.py` & `paradict-0.0.7/paradict/tags/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""binary Paradict: 256 tags from NOP (\x00) to END (\xff)"""
+"""binary Paradict: 256 tags from NOP (`\\x00`) to END (`\\xff`)"""
 
 
 # Nop
 NOP = b'\x00'
 
 # ----------- CONTAINERS -------------
```

### Comparing `paradict-0.0.6/paradict/tags/misc.py` & `paradict-0.0.7/paradict/tags/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """Private miscellaneous module for the Paradict binary format"""
 from paradict import tags
 
 
+__all__ = []
+
+
 # Mapping bytes number to INT tags. Eg: 1 byte int belongs to tags.INT_8
 SIZE_TO_PINT = {1: tags.PINT_8, 2: tags.PINT_16,
                 3: tags.PINT_24, 4: tags.PINT_32,
                 5: tags.PINT_40, 6: tags.PINT_48,
                 7: tags.PINT_56, 8: tags.PINT_64}
```

### Comparing `paradict-0.0.6/paradict/typeref/__init__.py` & `paradict-0.0.7/paradict/typeref/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """TypeRef for type specs and customization"""
 import datetime
 from decimal import Decimal
 from collections import OrderedDict
 from paradict import box, errors
 
 
+__all__ = ["TypeRef"]
+
+
 class TypeRef:
     """This class represents a mechanism for customizing
     Python types allowed for (de)serializing data with Paradict classes and functions.
     For example, one might want to only use Python OrderedDict instead of the regular
     dict. In this case, just create a TypeRef instance, and make sure that you
     set the dict_type attribute via the construction or a property.
 
@@ -436,15 +439,15 @@
         self._time_types = val
 
     def adapt(self, data):
         """Checks the 'adapters' attribute to find out if there is
         an adapter function registered for the type of the data argument.
         Then, calls the adapter on the data.
 
-        [parameters]
+        [param]
         - data: the data to adapt is an arbitrary Python object
 
         [return]
         Returns the adapted data or the same data if no adapter is registered for its type"""
         if not self._adapters:
             return data
         t = type(data)
```

### Comparing `paradict-0.0.6/paradict/validator/__init__.py` & `paradict-0.0.7/paradict/validator/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Data validation module"""
 from paradict.typeref import TypeRef
 from paradict.errors import Error
 
 
+__all__ = ["VALID_DATATYPES", "validate", "Spec", "Validator"]
+
+
 VALID_DATATYPES = ("dict", "list", "set", "obj", "bin",
                    "bool", "complex", "date", "datetime",
                    "float", "grid", "int", "str", "time")
 
 
 def validate(data, schema, type_ref=None):
     """This function returns True if the given data
     successfully validates against the given schema
 
-    [parameters]
+    [param]
     - data: some Python object (like a dict, a list, ...) that is
     part or include datatypes defined in VALID_DATATYPES.
     - schema: a valid schema. It might be a collection containing
     Spec instances and/or type-strings. The benefit of using Spec is
     that you can add a checker function that will serve as an extra
     programmatic validation.
     - type_ref: optional TypeRef object
@@ -58,15 +61,17 @@
         return self._checker
 
 
 class Validator:
     """Class to validate data against a schema"""
     def __init__(self, schema, type_ref=None):
         """
-        [parameters]
+        Init
+
+        [param]
         - schema: the schema
         - type_ref: optional TypeRef instance
         """
         self._schema = schema
         self._type_ref = type_ref if type_ref else TypeRef()
 
     @property
```

### Comparing `paradict-0.0.6/paradict.egg-info/PKG-INFO` & `paradict-0.0.7/paradict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradict
-Version: 0.0.6
+Version: 0.0.7
 Summary: Streamable multi-format serialization with schema
 Home-page: https://github.com/pyrustic/paradict
 Author: Pyrustic Evangelist
 Author-email: rusticalex@yahoo.com
 Maintainer: Pyrustic Evangelist
 Maintainer-email: rusticalex@yahoo.com
 License: MIT
@@ -263,22 +263,21 @@
 # Application programming interface
 The API exposes four foundational classes, Encoder, Decoder, Packer, and Unpacker, that serialize and deserialize data iteratively. 
 
 On top of these classes, four functions, encode, decode, pack, and unpack, do the same thing but in bulk. 
 
 Then there are additional classes and functions to do various stuff such as the TypeRef class for types customization, load and dump functions for reading and writing binary Paradict file, etc.
 
-Note that this section is just an overview of the API, thus it doesn't replace the module documentation.
+Note that this section is just an overview of the API, thus it doesn't replace the **API reference**.
 
-> Please explore the source code ! The documentation generator isn't yet ready !
+> Explore [API reference](https://github.com/pyrustic/paradict/tree/master/docs/api).
 
 ## Textual serialization
 Encoder and Decoder are the foundation classes for serializing and deserializing data. These classes process data iteratively. On top of these classes, two functions, encode and decode, do the same thing but in bulk.
 
-
 ### Using the Encoder class
 The Encoder constructor accepts `mode`, type_ref, skip_comments and skip_bin_data as arguments. 
 
 The `encode` method of this class takes as input a Python dictionary, then iteratively serialize it, yielding a line after another.
 
 ```python
 from paradict import Encoder
@@ -371,14 +370,29 @@
 print(r)
 ```
 Output:
 ```text
 {'id': 42, 'name': 'alex'}
 ```
 
+### Load and dump
+
+```python
+from paradict import read, write
+
+path = "/home/alex/user_card.bin"
+data = {"id": 42, "name": "alex"}
+# Serialize and write data to user_card.text
+write(data, path)
+# Read and deserialize data
+r = read(path)
+# test
+assert data == r
+```
+
 
 ### Miscellaneous functions
 Under the hood, the `Deserializer` class uses a public function for splitting a key-value line into three parts:
 - the key,
 - the value,
 - and the separator character.
```

### Comparing `paradict-0.0.6/paradict.egg-info/SOURCES.txt` & `paradict-0.0.7/paradict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paradict-0.0.6/setup.cfg` & `paradict-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `paradict-0.0.6/tests/box/test_box.py` & `paradict-0.0.7/tests/box/test_box.py`

 * *Files identical despite different names*

### Comparing `paradict-0.0.6/tests/deserializer/test_decoder.py` & `paradict-0.0.7/tests/deserializer/test_decoder.py`

 * *Files identical despite different names*

### Comparing `paradict-0.0.6/tests/deserializer/test_funcs.py` & `paradict-0.0.7/tests/deserializer/test_funcs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 import pathlib
 import tempfile
-from paradict import load, dump
+from paradict import load, dump, read, write
 
 
 class TestLoadFunc(unittest.TestCase):
 
     def setUp(self):
         file = tempfile.NamedTemporaryFile(delete=False)
         file.close()
@@ -25,16 +25,34 @@
 class TestDecodeFunc(unittest.TestCase):
     """The 'decode' function is already heavily
      used in the 'decoder' test module"""
     def test(self):
         self.assertTrue(True)
 
 
-class TestPackFunc(unittest.TestCase):
+class TestUnpackFunc(unittest.TestCase):
     """The 'unpack' function is already heavily
      used in the 'unpacker' test module"""
     def test(self):
         self.assertTrue(True)
 
 
+class TestReadFunc(unittest.TestCase):
+
+    def setUp(self):
+        file = tempfile.NamedTemporaryFile(delete=False)
+        file.close()
+        self._path = file.name
+
+    def tearDown(self):
+        pathlib.Path(self._path).unlink()
+
+    def test(self):
+        data = {0: "hello world", "pi": 3.14}
+        write(data, self._path)
+        r = read(self._path)
+        expected = data
+        self.assertEqual(expected, r)
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `paradict-0.0.6/tests/deserializer/test_unpacker.py` & `paradict-0.0.7/tests/deserializer/test_unpacker.py`

 * *Files identical despite different names*

### Comparing `paradict-0.0.6/tests/kv/test_kv.py` & `paradict-0.0.7/tests/kv/test_kv.py`

 * *Files identical despite different names*

### Comparing `paradict-0.0.6/tests/misc/test_misc.py` & `paradict-0.0.7/tests/misc/test_misc.py`

 * *Files identical despite different names*

### Comparing `paradict-0.0.6/tests/queue/test_bin_queue.py` & `paradict-0.0.7/tests/queue/test_bin_queue.py`

 * *Files identical despite different names*

### Comparing `paradict-0.0.6/tests/queue/test_txt_queue.py` & `paradict-0.0.7/tests/queue/test_txt_queue.py`

 * *Files identical despite different names*

### Comparing `paradict-0.0.6/tests/serializer/test_encoder.py` & `paradict-0.0.7/tests/serializer/test_encoder.py`

 * *Files identical despite different names*

### Comparing `paradict-0.0.6/tests/serializer/test_funcs.py` & `paradict-0.0.7/tests/serializer/test_funcs.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 import unittest
 import pathlib
 import tempfile
-from paradict import dump, pack
+from paradict import dump, pack, write, encode
+
+
+class TestPackFunc(unittest.TestCase):
+    """The 'pack' function is already heavily
+     used in the 'packer' test module"""
+    def test(self):
+        self.assertTrue(True)
 
 
 class TestDumpFunc(unittest.TestCase):
 
     def setUp(self):
         file = tempfile.NamedTemporaryFile(delete=False)
         file.close()
@@ -26,16 +33,28 @@
 class TestEncodeFunc(unittest.TestCase):
     """The 'encode' function is already heavily
      used in the 'encoder' test module"""
     def test(self):
         self.assertTrue(True)
 
 
-class TestPackFunc(unittest.TestCase):
-    """The 'pack' function is already heavily
-     used in the 'packer' test module"""
+class TestWriteFunc(unittest.TestCase):
+
+    def setUp(self):
+        file = tempfile.NamedTemporaryFile(delete=False)
+        file.close()
+        self._path = file.name
+
+    def tearDown(self):
+        pathlib.Path(self._path).unlink()
+
     def test(self):
-        self.assertTrue(True)
+        data = {0: "hello world", "pi": 3.14}
+        write(data, self._path)
+        with open(self._path, "r", encoding="utf-8") as file:
+            r = file.read()
+        expected = encode(data)
+        self.assertEqual(expected, r)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `paradict-0.0.6/tests/serializer/test_packer.py` & `paradict-0.0.7/tests/serializer/test_packer.py`

 * *Files identical despite different names*

### Comparing `paradict-0.0.6/tests/streaming/test_bin_streaming.py` & `paradict-0.0.7/tests/streaming/test_bin_streaming.py`

 * *Files identical despite different names*

### Comparing `paradict-0.0.6/tests/streaming/test_txt_streaming.py` & `paradict-0.0.7/tests/streaming/test_txt_streaming.py`

 * *Files identical despite different names*

### Comparing `paradict-0.0.6/tests/test_imports.py` & `paradict-0.0.7/tests/test_imports.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
     def test_import_funcs(self):
         try:
             # import functions
             from paradict import encode
             from paradict import decode
             from paradict import pack
+            from paradict import read
+            from paradict import write
             from paradict import unpack
             from paradict import load
             from paradict import dump
             from paradict import forge_bin
             from paradict import stringify_bin
             from paradict import validate
             from paradict import split_kv
```

### Comparing `paradict-0.0.6/tests/validator/test_validator.py` & `paradict-0.0.7/tests/validator/test_validator.py`

 * *Files identical despite different names*

