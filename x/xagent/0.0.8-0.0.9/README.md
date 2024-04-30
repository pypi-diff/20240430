# Comparing `tmp/xagent-0.0.8.tar.gz` & `tmp/xagent-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xagent-0.0.8.tar", last modified: Mon Apr 29 03:01:01 2024, max compression
+gzip compressed data, was "xagent-0.0.9.tar", last modified: Tue Apr 30 06:46:17 2024, max compression
```

## Comparing `xagent-0.0.8.tar` & `xagent-0.0.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-29 03:01:01.605608 xagent-0.0.8/
--rw-r--r--   0 chenhao    (501) staff       (20)     1063 2024-03-14 09:35:14.000000 xagent-0.0.8/LICENSE
--rw-r--r--   0 chenhao    (501) staff       (20)      231 2024-04-29 03:01:01.605418 xagent-0.0.8/PKG-INFO
--rw-r--r--   0 chenhao    (501) staff       (20)     5714 2024-04-29 02:59:57.000000 xagent-0.0.8/README.md
--rw-r--r--   0 chenhao    (501) staff       (20)       38 2024-04-29 03:01:01.605661 xagent-0.0.8/setup.cfg
--rw-r--r--   0 chenhao    (501) staff       (20)     1207 2024-03-21 03:48:59.000000 xagent-0.0.8/setup.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-29 03:01:01.603088 xagent-0.0.8/tests/
--rw-r--r--   0 chenhao    (501) staff       (20)     2193 2024-04-19 07:38:46.000000 xagent-0.0.8/tests/test_job.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4058 2024-04-28 11:46:32.000000 xagent-0.0.8/tests/test_kb.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3422 2024-04-29 02:32:45.000000 xagent-0.0.8/tests/test_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2567 2024-04-29 02:35:16.000000 xagent-0.0.8/tests/test_local_model.py
--rw-r--r--   0 chenhao    (501) staff       (20)     8094 2024-04-25 05:55:07.000000 xagent-0.0.8/tests/test_xagent.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4747 2024-04-15 04:02:55.000000 xagent-0.0.8/tests/test_zhipu_api_model.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-29 03:01:01.605187 xagent-0.0.8/xagent.egg-info/
--rw-r--r--   0 chenhao    (501) staff       (20)      231 2024-04-29 03:01:01.000000 xagent-0.0.8/xagent.egg-info/PKG-INFO
--rw-r--r--   0 chenhao    (501) staff       (20)     1432 2024-04-29 03:01:01.000000 xagent-0.0.8/xagent.egg-info/SOURCES.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-04-29 03:01:01.000000 xagent-0.0.8/xagent.egg-info/dependency_links.txt
--rw-r--r--   0 chenhao    (501) staff       (20)      210 2024-04-29 03:01:01.000000 xagent-0.0.8/xagent.egg-info/requires.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        8 2024-04-29 03:01:01.000000 xagent-0.0.8/xagent.egg-info/top_level.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-04-29 03:01:01.000000 xagent-0.0.8/xagent.egg-info/zip-safe
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-29 03:01:01.584305 xagent-0.0.8/xagents/
--rw-r--r--   0 chenhao    (501) staff       (20)      667 2024-04-15 04:02:55.000000 xagent-0.0.8/xagents/__init__.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-29 03:01:01.586600 xagent-0.0.8/xagents/agent/
--rw-r--r--   0 chenhao    (501) staff       (20)      213 2024-04-15 04:02:55.000000 xagent-0.0.8/xagents/agent/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3554 2024-04-28 11:37:00.000000 xagent-0.0.8/xagents/agent/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2206 2024-04-19 08:20:14.000000 xagent-0.0.8/xagents/agent/common.py
--rw-r--r--   0 chenhao    (501) staff       (20)      811 2024-04-08 07:28:32.000000 xagent-0.0.8/xagents/agent/memory.py
--rw-r--r--   0 chenhao    (501) staff       (20)     8093 2024-04-28 11:37:00.000000 xagent-0.0.8/xagents/agent/xagent.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1940 2024-04-25 06:21:58.000000 xagent-0.0.8/xagents/config.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-29 03:01:01.588957 xagent-0.0.8/xagents/kb/
--rw-r--r--   0 chenhao    (501) staff       (20)      178 2024-03-19 07:40:40.000000 xagent-0.0.8/xagents/kb/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)    11768 2024-04-28 11:37:00.000000 xagent-0.0.8/xagents/kb/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     7948 2024-04-28 11:37:00.000000 xagent-0.0.8/xagents/kb/common.py
--rw-r--r--   0 chenhao    (501) staff       (20)    13120 2024-04-28 11:37:00.000000 xagent-0.0.8/xagents/kb/kb.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3248 2024-04-25 02:50:51.000000 xagent-0.0.8/xagents/kb/kb_file.py
--rw-r--r--   0 chenhao    (501) staff       (20)     5516 2024-04-25 02:50:51.000000 xagent-0.0.8/xagents/kb/vector_store.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-29 03:01:01.595004 xagent-0.0.8/xagents/loader/
--rw-r--r--   0 chenhao    (501) staff       (20)      152 2024-03-19 10:48:10.000000 xagent-0.0.8/xagents/loader/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     5379 2024-04-28 11:37:00.000000 xagent-0.0.8/xagents/loader/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4226 2024-04-25 06:23:17.000000 xagent-0.0.8/xagents/loader/common.py
--rw-r--r--   0 chenhao    (501) staff       (20)      945 2024-04-25 06:24:43.000000 xagent-0.0.8/xagents/loader/csv_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1388 2024-04-28 11:37:00.000000 xagent-0.0.8/xagents/loader/doc_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     6064 2024-04-29 02:27:35.000000 xagent-0.0.8/xagents/loader/docx_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1075 2024-04-25 06:24:55.000000 xagent-0.0.8/xagents/loader/excel_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1594 2024-04-25 02:50:51.000000 xagent-0.0.8/xagents/loader/json_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)      842 2024-04-25 02:50:51.000000 xagent-0.0.8/xagents/loader/jsonl_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)      961 2024-04-25 02:50:51.000000 xagent-0.0.8/xagents/loader/markdown_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3236 2024-04-29 02:27:35.000000 xagent-0.0.8/xagents/loader/pdf_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1328 2024-04-28 11:37:00.000000 xagent-0.0.8/xagents/loader/ppt_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2593 2024-04-29 02:27:35.000000 xagent-0.0.8/xagents/loader/pptx_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3374 2024-04-22 05:58:02.000000 xagent-0.0.8/xagents/loader/splitter.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1809 2024-04-08 07:28:32.000000 xagent-0.0.8/xagents/loader/structed.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1425 2024-04-29 02:27:35.000000 xagent-0.0.8/xagents/loader/utils.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-29 03:01:01.597709 xagent-0.0.8/xagents/model/
--rw-r--r--   0 chenhao    (501) staff       (20)      179 2024-03-20 06:50:45.000000 xagent-0.0.8/xagents/model/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2800 2024-04-15 04:02:55.000000 xagent-0.0.8/xagents/model/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2426 2024-04-26 05:26:11.000000 xagent-0.0.8/xagents/model/common.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2243 2024-04-26 06:06:20.000000 xagent-0.0.8/xagents/model/local.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1234 2024-03-21 07:20:01.000000 xagent-0.0.8/xagents/model/openai.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4048 2024-04-26 05:26:29.000000 xagent-0.0.8/xagents/model/zhipu.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-29 03:01:01.600522 xagent-0.0.8/xagents/tool/
--rw-r--r--   0 chenhao    (501) staff       (20)      226 2024-04-15 04:02:55.000000 xagent-0.0.8/xagents/tool/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1429 2024-04-19 08:20:14.000000 xagent-0.0.8/xagents/tool/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1641 2024-04-22 03:01:50.000000 xagent-0.0.8/xagents/tool/common_tool.py
--rw-r--r--   0 chenhao    (501) staff       (20)      463 2024-04-22 05:36:21.000000 xagent-0.0.8/xagents/tool/core.py
--rw-r--r--   0 chenhao    (501) staff       (20)     6639 2024-04-22 08:53:58.000000 xagent-0.0.8/xagents/tool/web_search.py
--rw-r--r--   0 chenhao    (501) staff       (20)      560 2024-04-19 07:38:46.000000 xagent-0.0.8/xagents/util.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-30 06:46:17.965921 xagent-0.0.9/
+-rw-r--r--   0 chenhao    (501) staff       (20)     1063 2024-03-14 09:35:14.000000 xagent-0.0.9/LICENSE
+-rw-r--r--   0 chenhao    (501) staff       (20)      231 2024-04-30 06:46:17.965714 xagent-0.0.9/PKG-INFO
+-rw-r--r--   0 chenhao    (501) staff       (20)     7350 2024-04-29 10:55:35.000000 xagent-0.0.9/README.md
+-rw-r--r--   0 chenhao    (501) staff       (20)       38 2024-04-30 06:46:17.965980 xagent-0.0.9/setup.cfg
+-rw-r--r--   0 chenhao    (501) staff       (20)     1207 2024-03-21 03:48:59.000000 xagent-0.0.9/setup.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-30 06:46:17.963467 xagent-0.0.9/tests/
+-rw-r--r--   0 chenhao    (501) staff       (20)     2193 2024-04-19 07:38:46.000000 xagent-0.0.9/tests/test_job.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4058 2024-04-29 10:55:36.000000 xagent-0.0.9/tests/test_kb.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3422 2024-04-29 10:55:36.000000 xagent-0.0.9/tests/test_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2567 2024-04-29 10:55:36.000000 xagent-0.0.9/tests/test_local_model.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     8094 2024-04-29 10:55:36.000000 xagent-0.0.9/tests/test_xagent.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4747 2024-04-15 04:02:55.000000 xagent-0.0.9/tests/test_zhipu_api_model.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-30 06:46:17.965452 xagent-0.0.9/xagent.egg-info/
+-rw-r--r--   0 chenhao    (501) staff       (20)      231 2024-04-30 06:46:17.000000 xagent-0.0.9/xagent.egg-info/PKG-INFO
+-rw-r--r--   0 chenhao    (501) staff       (20)     1432 2024-04-30 06:46:17.000000 xagent-0.0.9/xagent.egg-info/SOURCES.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-04-30 06:46:17.000000 xagent-0.0.9/xagent.egg-info/dependency_links.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)      210 2024-04-30 06:46:17.000000 xagent-0.0.9/xagent.egg-info/requires.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)        8 2024-04-30 06:46:17.000000 xagent-0.0.9/xagent.egg-info/top_level.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-04-30 06:46:17.000000 xagent-0.0.9/xagent.egg-info/zip-safe
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-30 06:46:17.942276 xagent-0.0.9/xagents/
+-rw-r--r--   0 chenhao    (501) staff       (20)      667 2024-04-15 04:02:55.000000 xagent-0.0.9/xagents/__init__.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-30 06:46:17.944952 xagent-0.0.9/xagents/agent/
+-rw-r--r--   0 chenhao    (501) staff       (20)      213 2024-04-15 04:02:55.000000 xagent-0.0.9/xagents/agent/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3554 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/agent/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2206 2024-04-19 08:20:14.000000 xagent-0.0.9/xagents/agent/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      811 2024-04-08 07:28:32.000000 xagent-0.0.9/xagents/agent/memory.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     8118 2024-04-30 06:16:53.000000 xagent-0.0.9/xagents/agent/xagent.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2041 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/config.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-30 06:46:17.948925 xagent-0.0.9/xagents/kb/
+-rw-r--r--   0 chenhao    (501) staff       (20)      178 2024-03-19 07:40:40.000000 xagent-0.0.9/xagents/kb/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)    12021 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/kb/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     8108 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/kb/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)    13371 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/kb/kb.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3961 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/kb/kb_file.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     5516 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/kb/vector_store.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-30 06:46:17.956458 xagent-0.0.9/xagents/loader/
+-rw-r--r--   0 chenhao    (501) staff       (20)      152 2024-03-19 10:48:10.000000 xagent-0.0.9/xagents/loader/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     5376 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4226 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      945 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/csv_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1388 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/doc_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     6064 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/docx_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1075 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/excel_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1594 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/json_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      842 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/jsonl_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      961 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/markdown_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3236 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/pdf_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1328 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/ppt_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2593 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/pptx_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3374 2024-04-22 05:58:02.000000 xagent-0.0.9/xagents/loader/splitter.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1809 2024-04-08 07:28:32.000000 xagent-0.0.9/xagents/loader/structed.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1429 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/utils.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-30 06:46:17.958825 xagent-0.0.9/xagents/model/
+-rw-r--r--   0 chenhao    (501) staff       (20)      179 2024-03-20 06:50:45.000000 xagent-0.0.9/xagents/model/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2800 2024-04-15 04:02:55.000000 xagent-0.0.9/xagents/model/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2426 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/model/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2243 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/model/local.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1234 2024-03-21 07:20:01.000000 xagent-0.0.9/xagents/model/openai.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4048 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/model/zhipu.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-30 06:46:17.960735 xagent-0.0.9/xagents/tool/
+-rw-r--r--   0 chenhao    (501) staff       (20)      226 2024-04-15 04:02:55.000000 xagent-0.0.9/xagents/tool/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1429 2024-04-19 08:20:14.000000 xagent-0.0.9/xagents/tool/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1641 2024-04-22 03:01:50.000000 xagent-0.0.9/xagents/tool/common_tool.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      463 2024-04-22 05:36:21.000000 xagent-0.0.9/xagents/tool/core.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     6639 2024-04-22 08:53:58.000000 xagent-0.0.9/xagents/tool/web_search.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      560 2024-04-19 07:38:46.000000 xagent-0.0.9/xagents/util.py
```

### Comparing `xagent-0.0.8/LICENSE` & `xagent-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/README.md` & `xagent-0.0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
 ## 20240422
 
 version: 0.0.8
 
 #### FEATURE
 
-- [支持表格类型的chunk](https://dev.aminer.cn/solution-center-algorithm/XAgents/-/issues/25)
+- [支持OCR识别图片信息](https://dev.aminer.cn/solution-center-algorithm/XAgents/-/issues/32)
 示例chunk
 ```json
 {
   "content": "|fdasg|gasdga|agdag|\n|gsadg|gdsg|",
   "content_type": "TABLE",
   "page_idx": 1
 }
@@ -202,7 +202,41 @@
 
 ## 20240429
 
 version: 0.0.8
 
 #### FEATURE
 
+- [支持OCR识别图片信息](https://dev.aminer.cn/solution-center-algorithm/XAgents/-/issues/32)
+在loader/parse和kb_file/create两个接口添加了ocr的参数，设置为True即可
+
+- 支持图像上传图像服务器，并生成链接
+
+
+- [ppt格式文件支持](https://dev.aminer.cn/solution-center-algorithm/XAgents/-/issues/33)
+可以上传.ppt和.pptx格式的文件
+
+- [支持知识库在切片维度做增、删、改](https://dev.aminer.cn/solution-center-algorithm/XAgents/-/issues/17)
+具体查api文档中chunk/xxx 路径的接口， chunk会有id来定位
+
+- [支持关键词检索](https://dev.aminer.cn/solution-center-algorithm/XAgents/-/issues/13)
+  - 执行start_es_service.sh启动es服务
+  - 在创建知识库的时候，向量存储配置添加
+  ```json
+  {
+    "cls": "XES",
+    "es_url": "http://localhost:9200"
+  }
+  ```
+
+#### BUG FIX
+- [expand的时候，可以精确到字地扩展，可以截断chunk](https://dev.aminer.cn/solution-center-algorithm/XAgents/-/issues/30)
+
+#### OTHER
+- [完善发布SDK的代码，以及单元测试](https://dev.aminer.cn/solution-center-algorithm/XAgents/-/issues/6)
+补充了接口级别的测试，确保把整个知识库创建、管理、Agent问答流程覆盖
+- 每期发布会上传docker image
+  - 示例docker名称
+  - pull的时候需要登录公司docker镜像源，登录账户密码联系@陈昊
+  - 如果要拉最新的镜像，使用
+- 基于镜像的部署，单独做了一个服务（可以考虑作为生产环境）：http://hz-model.bigmodel.cn/xagent/docs
+- 完成[部署文档](https://zhipu-ai.feishu.cn/docx/JzkzdgFiZolcgCxG5tacennWn1k)
```

### Comparing `xagent-0.0.8/setup.py` & `xagent-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/tests/test_job.py` & `xagent-0.0.9/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/tests/test_kb.py` & `xagent-0.0.9/tests/test_kb.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/tests/test_loader.py` & `xagent-0.0.9/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/tests/test_local_model.py` & `xagent-0.0.9/tests/test_local_model.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/tests/test_xagent.py` & `xagent-0.0.9/tests/test_xagent.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/tests/test_zhipu_api_model.py` & `xagent-0.0.9/tests/test_zhipu_api_model.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagent.egg-info/SOURCES.txt` & `xagent-0.0.9/xagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/__init__.py` & `xagent-0.0.9/xagents/__init__.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/agent/api.py` & `xagent-0.0.9/xagents/agent/api.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/agent/common.py` & `xagent-0.0.9/xagents/agent/common.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/agent/memory.py` & `xagent-0.0.9/xagents/agent/memory.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/agent/xagent.py` & `xagent-0.0.9/xagents/agent/xagent.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,34 +41,34 @@
 
 
 class XAgent(AbstractAgent):
 
     def __init__(self, name: str,
                  llm_config: dict,
                  memory_config: dict,
-                 kb_config:KBConfig,
+                 kb_config: KBConfig,
                  # web_search_config: WebSearchConfig,
                  tools: List[BaseTool] = []) -> None:
         super().__init__(name=name)
-        self.info = XAgentInfo(name=name,llm_config=llm_config, memory_config=memory_config,kb_config=kb_config,
+        self.info = XAgentInfo(name=name, llm_config=llm_config, memory_config=memory_config, kb_config=kb_config,
                                tools=[ToolDesc(**e.model_dump(exclude={})) for e in tools])
         self.llm_model = get_llm_model(llm_config)
         self.memory = BaseMemory(**memory_config)
         self._load_kb(kb_config)
         # print(f"web_search_config_0:{web_search_config}")
         # self._load_web_search(web_search_config)
         self.tools = tools
 
     def _load_kb(self, kb_config: KBConfig):
         if not kb_config:
             self.kb = None
             self.kb_prompt_template = None
         else:
             self.kb = get_knowledge_base(kb_config.name)
-            self.kb_prompt_template = kb_config.prompt_template     
+            self.kb_prompt_template = kb_config.prompt_template
             logger.info("load kb finish")
 
     def get_info(self):
         return self.info
 
     def search_kb(self, query: str, **kwargs) -> List[RecalledChunk]:
         chunks = self.kb.search(query=query, **kwargs)
@@ -84,48 +84,46 @@
         return os.path.join(dir_path, agent_name+".json")
 
     def save(self, save_dir: str):
         save_path = self._get_agent_config_path(save_dir, self.name)
         logger.info(f"save agent:{self.name} to {save_path}")
         logger.debug(f"agent info:{self.get_info()}")
         dump(self.get_info().model_dump(), save_path)
-        
+
     def delete(self, save_dir: str):
         save_path = self._get_agent_config_path(save_dir, self.name)
         if os.path.exists(save_path):
             logger.info(f"deleting agent:{self.name} from save_path:{save_path}")
             shutil.rmtree(save_path)
 
-
     @classmethod
     def load(cls, save_dir: str, name: str) -> "XAgent":
         config_path = cls._get_agent_config_path(save_dir, name)
         if not os.path.exists(config_path):
             raise FileExistsError(f"config file {config_path} not found")
 
         kwargs = load(config_path)
         if kwargs.get("kb_config"):
             kwargs["kb_config"] = KBConfig.model_validate(kwargs["kb_config"])
         logger.debug(f"{kwargs=}")
 
-        return XAgent(**kwargs)     
-
+        return XAgent(**kwargs)
 
-    def chat(self, message: str, do_remember=True, details=False, stream = False,
-             use_kb=False, kb_search_config:KBSearchConfig=KBSearchConfig(),
-             fake_chat=False, llm_gen_config:LLMGenConfig=LLMGenConfig(), key_word=True, **kwargs) -> AgentResp:
+    def chat(self, message: str, do_remember=True, details=False, stream=False,
+             use_kb=False, kb_search_config: KBSearchConfig = KBSearchConfig(),
+             fake_chat=False, llm_gen_config: LLMGenConfig = LLMGenConfig(), key_word=True, **kwargs) -> AgentResp:
 
         chunks = []
         if use_kb:
             if not self.kb or not self.kb_prompt_template:
                 logger.warning(f"agent:{self.name} has no related knowledge base, will not chat with kb! ")
                 prompt = message
                 chunks = None
             else:
-                logger.info("agent searching kb")
+                logger.info("agent searching kb with kb_name")
                 chunks = self.search_kb(query=message, **kb_search_config.model_dump())
                 context = "\n".join(f"{idx+1}." + c.to_plain_text() for idx, c in enumerate(chunks))
                 prompt = self.kb_prompt_template.format(question=message, context=context)
         else:
             prompt = message
             chunks = None
 
@@ -172,15 +170,16 @@
         if stream:
             content = _add_remember_callback(llm_resp.content)
         else:
             content = llm_resp.content
             logger.info(f"generate response:{content}")
             _remember_callback(content)
 
-        resp = AgentResp(content=content, tool_calls=tool_calls, usage=llm_resp.usage, references=chunks, details=llm_resp.details, web_search_result=web_search_result)
+        resp = AgentResp(content=content, tool_calls=tool_calls, usage=llm_resp.usage, references=chunks,
+                         details=llm_resp.details, web_search_result=web_search_result)
         return resp
 
     def remember(self, role: str, message: str):
         logger.debug(f"remembering {role=}, {message=}")
         self.memory.remember(role, message)
 
     def clear_memory(self):
```

### Comparing `xagent-0.0.8/xagents/config.py` & `xagent-0.0.9/xagents/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -62,10 +62,10 @@
 ### xagent缓存数目
 XAGENT_CACHE_NUM=1000
 XAGENT_CACHE_EXPIRE_SECONDS=3600
 
 
 
 ### MinIO对象存储相关
-MINIO_URL = '10.50.130.151:9000'
-MINIO_ACCESS_KEY='l7RJ3QCGX6gt7M8zfN1v'
-MINIO_SECRET_KEY='smGpFhcz0hLOup8V2s6SMkzgzxzJFtSJiuAuKFqS'
+MINIO_URL = os.environ.get("MINIO_URL", "10.50.130.151:9000")
+MINIO_ACCESS_KEY=os.environ.get("MINIO_ACCESS_KEY", 'l7RJ3QCGX6gt7M8zfN1v')
+MINIO_SECRET_KEY=os.environ.get("MINIO_SECRET_KEY", 'smGpFhcz0hLOup8V2s6SMkzgzxzJFtSJiuAuKFqS')
```

### Comparing `xagent-0.0.8/xagents/kb/api.py` & `xagent-0.0.9/xagents/kb/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,23 +170,27 @@
 def get_kb_file_info(kb_name: str, file_name: str) -> KnowledgeBaseFileInfo:
     kb_file = get_kb_file(kb_name=kb_name, file_name=file_name)
     return kb_file.get_info()
 
 
 def create_kb_file(kb_name: str, file: UploadFile | str, do_cut=True, do_index=True,
                    batch_size:int=16,
+                   upload_image:bool=False,
+                   ocr:bool=False,
                    cut_config: dict = dict(separator='\n',
                                            max_len=200,
                                            min_len=10)) -> KnowledgeBaseFile:
     """创建知识库文件
     Args:
         kb_name (str): 知识库名称
         file (UploadFile | str): 知识库文件，UploadFile(fast_api)或者str(文件路径)
         do_cut (bool, optional): 是否切分文件. Defaults to True.
         do_index (bool, optional): 是否添加到索引. Defaults to True.
+        upload_image (bool, optional): 是否上传图片. Defaults to False.
+        ocr (bool, optional): 是否OCR. Defaults to False.
         cut_config (dict, optional): 切分文件的参数. Defaults to dict(separator='\n', max_len=200, min_len=10).
 
     Raises:
         ValueError: 知识库文件已经存在
 
     Returns:
         KnowledgeBaseFileInfo: 知识库文件描述
@@ -204,15 +208,15 @@
         with open(file, "rb") as f:
             content = f.read()
     else:
         content = file.file.read()
     with open(kb_file_path, "wb") as f:
         f.write(content)
     if do_cut:
-        kb_file.cut(**cut_config)
+        kb_file.cut(upload_image=upload_image, ocr=ocr, **cut_config)
     if do_index:
         kb = get_knowledge_base(name=kb_name)
         kb.add_kb_file2index(kb_file=kb_file, reindex=True, do_save=True, batch_size=batch_size)
     return kb_file
 
 
 def delete_kb_file(kb_name: str, file_name: str) -> str:
```

### Comparing `xagent-0.0.8/xagents/kb/common.py` & `xagent-0.0.9/xagents/kb/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,17 @@
     return os.path.join(get_kb_dir(kb_name), "inverted_index")
 def get_config_path(kb_name)->str:
     return os.path.join(get_kb_dir(kb_name), "config.json")
 
 def get_chunk_path(kb_name, file_name) -> str:
     return os.path.join(get_chunk_dir(kb_name), file_name+".jsonl")
 
+def get_status_path(kb_name) -> str:
+    return os.path.join(get_kb_dir(kb_name), "status.json")
+
 def get_origin_path(kb_name, file_name) -> str:
     return os.path.join(get_origin_dir(kb_name), file_name)
 
 def get_id_path(kb_name, file_name) -> str:
     return os.path.join(get_id_dir(kb_name), file_name+".jsonl")
 def get_inverted_id_path(kb_name, file_name) -> str:
     return os.path.join(get_inverted_id_dir(kb_name), file_name+".jsonl")
@@ -202,8 +205,9 @@
 
 
 # 知识库文件类
 class KnowledgeBaseFileInfo(BaseModel):
     kb_name: str = Field(description="知识库名称")
     file_name: str = Field(description="知识库文件名称")
     is_cut:bool = Field(description="是否已经切片")
+    is_indexed:bool = Field(description="是否已经索引")
```

### Comparing `xagent-0.0.8/xagents/kb/kb.py` & `xagent-0.0.9/xagents/kb/kb.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 import re
 from typing import List, Type
 from loguru import logger
 from xagents.kb.kb_file import KnowledgeBaseFile
 from xagents.kb.vector_store import XES, LocalVecStore, XVecStore, get_vecstore_cls
 from xagents.loader.common import Chunk, ContentType
 from xagents.model.api import get_embd_model, get_rerank_model
-from xagents.kb.common import KnowledgeBaseInfo, RecalledChunk, chunk2document, get_chunk_dir, get_chunk_path, get_config_path, get_index_dir, get_kb_dir, get_origin_dir
-from snippets import load, log_cost_time, dump, jload
+from xagents.kb.common import KnowledgeBaseInfo, RecalledChunk, chunk2document, get_chunk_dir, get_chunk_path, get_config_path, get_index_dir, get_kb_dir, get_origin_dir, get_status_path
+from snippets import load, log_cost_time, dump, jload, jdump
 
 
 class KnowledgeBase():
 
     def __init__(self, name: str, desc, embedding_config: dict, vecstore_config: dict|List[dict]):
         self.name = name
         self.desc = desc
@@ -52,17 +52,20 @@
 
     def _build_dirs(self):
         self.kb_dir = get_kb_dir(self.name)
         self.origin_dir = get_origin_dir(self.name)
 
         self.chunk_dir = get_chunk_dir(self.name)
         self.config_path = get_config_path(self.name)
-
+        self.status_path = get_status_path(self.name)
+        
         os.makedirs(self.origin_dir, exist_ok=True)
         os.makedirs(self.chunk_dir, exist_ok=True)
+        if not os.path.exists(self.config_path):
+            jdump(dict(), self.status_path)
 
     def _save_config(self):
         dump(self._get_config(), self.config_path)
 
     def get_indexes(self) -> List[XVecStore]:
         """
         初始化向量存储、ES存储
@@ -143,15 +146,17 @@
         
 
     def add_kb_file2index(self,  kb_file: KnowledgeBaseFile, reindex=False, do_save=False, batch_size=16):
         if not kb_file.is_cut:
             logger.warning(f"{kb_file.file_name} is not cut, please cut it first")
             return
         chunks = kb_file.list_chunks()
-        return self.add_chunks2index(chunks=chunks, meta_info=dict(file_name=kb_file.file_name), reindex=reindex, do_save=do_save, batch_size=batch_size)
+        kb_file.set_index_status(False)
+        self.add_chunks2index(chunks=chunks, meta_info=dict(file_name=kb_file.file_name), reindex=reindex, do_save=do_save, batch_size=batch_size)
+        kb_file.set_index_status(True)
 
     @log_cost_time(name="rebuild_index")
     def rebuild_index(self, reindex:bool, batch_size:int):
         """
         重新构建向量知识库
         """
         indexes = self.get_indexes()
```

### Comparing `xagent-0.0.8/xagents/kb/kb_file.py` & `xagent-0.0.9/xagents/kb/kb_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 '''
 
 
 # 知识库文件类
 import os
 from loguru import logger
 from typing import List
-from xagents.kb.common import KnowledgeBaseFileInfo, get_chunk_path, get_origin_path
+from xagents.kb.common import KnowledgeBaseFileInfo, get_chunk_path, get_origin_path, get_status_path
 from xagents.loader.api import parse_file
 from xagents.loader.common import Chunk
-from snippets import dump, load
+from snippets import dump, load, jload, jdump
 
 
 class KnowledgeBaseFile:
     def __init__(self, kb_name: str, file_name: str):
         self.kb_name = kb_name
         self.file_name = file_name
         self.chunk_path = get_chunk_path(self.kb_name, self.file_name)
@@ -32,17 +32,34 @@
 
     @property
     def chunk_num(self) -> int:
         if not self.is_cut:
             return 0
         chunks = load(self.chunk_path)
         return len(chunks)
+    
+    def set_index_status(self, is_indexed:bool):
+        logger.debug(f"setting {self.file_name}'s is_indexed value to {is_indexed}")
+        status_path = get_status_path(self.kb_name)
+        status = jload(status_path)
+        if self.file_name not in status:
+            status[self.file_name] = {}
+        status[self.file_name]["indexed"] = is_indexed      
+        logger.debug(f"{status=}")   
+        jdump(status, status_path)
+        
 
+    @property
+    def is_indexed(self)->bool:
+        status_path = get_status_path(self.kb_name)
+        rs = jload(status_path).get(self.file_name, {}).get("indexed", False)
+        return rs
+        
     def get_info(self):
-        return KnowledgeBaseFileInfo(kb_name=self.kb_name, file_name=self.file_name, is_cut=self.is_cut)
+        return KnowledgeBaseFileInfo(kb_name=self.kb_name, file_name=self.file_name, is_cut=self.is_cut, is_indexed=self.is_indexed)
 
     def cut(self, *args, **kwargs) -> List[Chunk]:
         logger.info(f"start cut file: {self.file_name}")
         chunks: List[Chunk] = parse_file(file_path=self.origin_path, *args, **kwargs)
         self._save_chunks(chunks=chunks)
     
     def _save_chunks(self, chunks: List[Chunk]):
```

### Comparing `xagent-0.0.8/xagents/kb/vector_store.py` & `xagent-0.0.9/xagents/kb/vector_store.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/loader/api.py` & `xagent-0.0.9/xagents/loader/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,18 +102,18 @@
     with open(dst_path, 'w', encoding='utf-8') as f:
         for chunk in chunks:
             f.write(chunk.content)
     return dst_path
 
 
 def parse_file(file_path: str,
-               start_page: int = 1, 
-               end_page: int = None, 
+               start_page: int = 1,
+               end_page: int = None,
                upload_image=True,
-                ocr=False,
+               ocr=False,
                do_cut: bool = True,
                separator: str = '\n',
                max_len: int = 200,
                min_len: int = 10) -> List[Chunk]:
     """加载并切分切片
 
     Args:
```

### Comparing `xagent-0.0.8/xagents/loader/common.py` & `xagent-0.0.9/xagents/loader/common.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/loader/csv_loader.py` & `xagent-0.0.9/xagents/loader/csv_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/loader/doc_loader.py` & `xagent-0.0.9/xagents/loader/doc_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/loader/docx_loader.py` & `xagent-0.0.9/xagents/loader/docx_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/loader/excel_loader.py` & `xagent-0.0.9/xagents/loader/excel_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/loader/json_loader.py` & `xagent-0.0.9/xagents/loader/json_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/loader/jsonl_loader.py` & `xagent-0.0.9/xagents/loader/jsonl_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/loader/markdown_loader.py` & `xagent-0.0.9/xagents/loader/markdown_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/loader/pdf_loader.py` & `xagent-0.0.9/xagents/loader/pdf_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/loader/ppt_loader.py` & `xagent-0.0.9/xagents/loader/ppt_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/loader/pptx_loader.py` & `xagent-0.0.9/xagents/loader/pptx_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/loader/splitter.py` & `xagent-0.0.9/xagents/loader/splitter.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/loader/structed.py` & `xagent-0.0.9/xagents/loader/structed.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/loader/utils.py` & `xagent-0.0.9/xagents/loader/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 @Author  :   ChenHao
 @Description  :   load过程中的工具类
 @Contact :   jerrychen1990@gmail.com
 '''
 
 from loguru import logger
 from minio import Minio
-from cnocr import CnOcr
 from xagents.config import *
 
 
 
 def create_minio_client():
     return Minio(MINIO_URL,
                  access_key=MINIO_ACCESS_KEY,
@@ -32,14 +31,15 @@
         return url
     except Exception as err:
         logger.exception(err)
         return None
     
 
 def image2text(image_path):
+    from cnocr import CnOcr
     ocr = CnOcr(det_model_name='ch_PP-OCRv3_det')  # model_name 参考 https://gitee.com/cyahua/cnocr
     text = ocr.ocr(image_path)
     content = ','.join(item['text'] for item in text)
     return content
 
 
 if __name__ == "__main__":
```

### Comparing `xagent-0.0.8/xagents/model/api.py` & `xagent-0.0.9/xagents/model/api.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/model/common.py` & `xagent-0.0.9/xagents/model/common.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/model/local.py` & `xagent-0.0.9/xagents/model/local.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/model/openai.py` & `xagent-0.0.9/xagents/model/openai.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/model/zhipu.py` & `xagent-0.0.9/xagents/model/zhipu.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/tool/api.py` & `xagent-0.0.9/xagents/tool/api.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/tool/common_tool.py` & `xagent-0.0.9/xagents/tool/common_tool.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/tool/web_search.py` & `xagent-0.0.9/xagents/tool/web_search.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.8/xagents/util.py` & `xagent-0.0.9/xagents/util.py`

 * *Files identical despite different names*

