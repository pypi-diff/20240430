# Comparing `tmp/model_explorer-0.0.81.tar.gz` & `tmp/model_explorer-0.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_explorer-0.0.81.tar", last modified: Tue Apr 30 00:43:33 2024, max compression
+gzip compressed data, was "model_explorer-0.0.82.tar", last modified: Tue Apr 30 00:51:54 2024, max compression
```

## Comparing `model_explorer-0.0.81.tar` & `model_explorer-0.0.82.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 jingjin  (83079) primarygroup (89939)        0 2024-04-30 00:43:33.177454 model_explorer-0.0.81/
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      755 2024-04-30 00:43:33.173454 model_explorer-0.0.81/PKG-INFO
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      977 2024-04-30 00:43:20.000000 model_explorer-0.0.81/pyproject.toml
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)       38 2024-04-30 00:43:33.177454 model_explorer-0.0.81/setup.cfg
-drwxr-xr-x   0 jingjin  (83079) primarygroup (89939)        0 2024-04-30 00:43:33.157454 model_explorer-0.0.81/src/
-drwxr-xr-x   0 jingjin  (83079) primarygroup (89939)        0 2024-04-30 00:43:33.161454 model_explorer-0.0.81/src/model_explorer/
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      473 2024-04-27 16:25:43.000000 model_explorer-0.0.81/src/model_explorer/__init__.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)       96 2024-03-27 17:14:33.000000 model_explorer-0.0.81/src/model_explorer/__main__.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1023 2024-04-01 19:24:19.000000 model_explorer-0.0.81/src/model_explorer/adapter.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)      783 2024-04-01 19:24:02.000000 model_explorer-0.0.81/src/model_explorer/adapter_runner.py
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     2930 2024-04-28 02:33:55.000000 model_explorer-0.0.81/src/model_explorer/apis.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1115 2024-04-01 19:24:30.000000 model_explorer-0.0.81/src/model_explorer/builtin_graphdef_adapter.py
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      849 2024-04-01 19:24:46.000000 model_explorer-0.0.81/src/model_explorer/builtin_pytorch_exportedprogram_adapter.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1322 2024-04-01 23:17:42.000000 model_explorer-0.0.81/src/model_explorer/builtin_tf_direct_adapter.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1279 2024-04-01 23:17:42.000000 model_explorer-0.0.81/src/model_explorer/builtin_tf_mlir_adapter.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1184 2024-04-01 19:25:03.000000 model_explorer-0.0.81/src/model_explorer/builtin_tflite_flatbuffer_adapter.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1131 2024-04-01 19:25:08.000000 model_explorer-0.0.81/src/model_explorer/builtin_tflite_mlir_adapter.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     2230 2024-04-28 00:21:58.000000 model_explorer-0.0.81/src/model_explorer/cmdline.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     4202 2024-04-28 02:40:44.000000 model_explorer-0.0.81/src/model_explorer/config.py
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      106 2024-04-20 20:11:17.000000 model_explorer-0.0.81/src/model_explorer/consts.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)      338 2024-03-27 17:14:33.000000 model_explorer-0.0.81/src/model_explorer/extension_base.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1111 2024-03-28 23:18:49.000000 model_explorer-0.0.81/src/model_explorer/extension_class_processor.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     4294 2024-03-28 22:24:29.000000 model_explorer-0.0.81/src/model_explorer/extension_manager.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)      198 2024-03-27 17:14:33.000000 model_explorer-0.0.81/src/model_explorer/extension_matadata.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     4043 2024-04-25 21:03:05.000000 model_explorer-0.0.81/src/model_explorer/graph_builder.py
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4834 2024-04-28 02:42:33.000000 model_explorer-0.0.81/src/model_explorer/node_data_builder.py
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     6776 2024-04-25 21:04:47.000000 model_explorer-0.0.81/src/model_explorer/pytorch_exported_program_adater_impl.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)      353 2024-03-27 17:14:33.000000 model_explorer-0.0.81/src/model_explorer/registered_extension.py
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    11158 2024-04-28 16:09:25.000000 model_explorer-0.0.81/src/model_explorer/server.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)      349 2024-03-27 17:14:33.000000 model_explorer-0.0.81/src/model_explorer/singleton.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)      605 2024-04-25 21:04:04.000000 model_explorer-0.0.81/src/model_explorer/types.py
--rw-r-----   0 jingjin  (83079) primarygroup (89939)     1846 2024-04-25 23:26:34.000000 model_explorer-0.0.81/src/model_explorer/utils.py
-drwxr-xr-x   0 jingjin  (83079) primarygroup (89939)        0 2024-04-30 00:43:33.165454 model_explorer-0.0.81/src/model_explorer/web_app/
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      456 2024-03-27 17:14:33.000000 model_explorer-0.0.81/src/model_explorer/web_app/index.html
-drwxr-xr-x   0 jingjin  (83079) primarygroup (89939)        0 2024-04-30 00:43:33.173454 model_explorer-0.0.81/src/model_explorer/web_app/static_files/
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     9028 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gh09GixI.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4020 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Ghk9GixI.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15476 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GiU9G.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5340 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gik9GixI.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8332 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GjU9GixI.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8756 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmZjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     3800 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmdjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15208 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmhjtg.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5012 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmtjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     7976 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmxjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8700 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmZjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     3744 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmdjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    14796 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmhjtg.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4924 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmtjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     7764 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmxjtiu7.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8352 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTsDO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15468 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtDO_.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5424 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtzO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     9004 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTujO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4000 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTuzO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8528 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTsDO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15864 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtDO_.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5388 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtzO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     9100 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTujO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4084 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTuzO_PZ0.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     7860 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qE52i1dC.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8592 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qER2i1dC.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     3792 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEV2i1dC.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4992 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEl2i1dC.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    14796 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEp2iw.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32907 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/GoogleSansTextBold.json
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)   144302 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/GoogleSansTextBold.png
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32921 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/GoogleSansTextMedium.json
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)   138086 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/GoogleSansTextMedium.png
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32905 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/GoogleSansTextRegular.json
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)   132192 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/GoogleSansTextRegular.png
--rwxr-xr-x   0 jingjin  (83079) primarygroup (89939)  1193672 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/app_bundle.js
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     1234 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/favicon.svg
--rw-r-----   0 jingjin  (83079) primarygroup (89939)   169616 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/google_material_icon.woff2
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      828 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/icons_2024021202.json
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     2092 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/icons_2024021202.png
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      456 2024-04-28 05:02:59.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/index.html
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)   615601 2024-03-27 17:14:33.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/main_deps.js
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)   128352 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/material_icon.woff2
--r-xr-x---   0 jingjin  (83079) primarygroup (89939)   245609 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/styles.css
--rwxr-xr-x   0 jingjin  (83079) primarygroup (89939)  2572044 2024-04-30 00:43:04.000000 model_explorer-0.0.81/src/model_explorer/web_app/static_files/worker_bin.js
-drwxr-xr-x   0 jingjin  (83079) primarygroup (89939)        0 2024-04-30 00:43:33.173454 model_explorer-0.0.81/src/model_explorer.egg-info/
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      755 2024-04-30 00:43:33.000000 model_explorer-0.0.81/src/model_explorer.egg-info/PKG-INFO
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4876 2024-04-30 00:43:33.000000 model_explorer-0.0.81/src/model_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)        1 2024-04-30 00:43:33.000000 model_explorer-0.0.81/src/model_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      108 2024-04-30 00:43:33.000000 model_explorer-0.0.81/src/model_explorer.egg-info/entry_points.txt
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)      114 2024-04-30 00:43:33.000000 model_explorer-0.0.81/src/model_explorer.egg-info/requires.txt
--rw-r--r--   0 jingjin  (83079) primarygroup (89939)       15 2024-04-30 00:43:33.000000 model_explorer-0.0.81/src/model_explorer.egg-info/top_level.txt
+drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-30 00:51:54.313022 model_explorer-0.0.82/
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      755 2024-04-30 00:51:54.309022 model_explorer-0.0.82/PKG-INFO
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      977 2024-04-30 00:51:43.000000 model_explorer-0.0.82/pyproject.toml
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)       38 2024-04-30 00:51:54.313022 model_explorer-0.0.82/setup.cfg
+drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-30 00:51:54.297021 model_explorer-0.0.82/src/
+drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-30 00:51:54.301022 model_explorer-0.0.82/src/model_explorer/
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      473 2024-04-27 16:25:43.000000 model_explorer-0.0.82/src/model_explorer/__init__.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)       96 2024-03-27 17:14:33.000000 model_explorer-0.0.82/src/model_explorer/__main__.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1023 2024-04-01 19:24:19.000000 model_explorer-0.0.82/src/model_explorer/adapter.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)      783 2024-04-01 19:24:02.000000 model_explorer-0.0.82/src/model_explorer/adapter_runner.py
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     2930 2024-04-28 02:33:55.000000 model_explorer-0.0.82/src/model_explorer/apis.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1115 2024-04-01 19:24:30.000000 model_explorer-0.0.82/src/model_explorer/builtin_graphdef_adapter.py
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      849 2024-04-01 19:24:46.000000 model_explorer-0.0.82/src/model_explorer/builtin_pytorch_exportedprogram_adapter.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1322 2024-04-01 23:17:42.000000 model_explorer-0.0.82/src/model_explorer/builtin_tf_direct_adapter.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1279 2024-04-01 23:17:42.000000 model_explorer-0.0.82/src/model_explorer/builtin_tf_mlir_adapter.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1184 2024-04-01 19:25:03.000000 model_explorer-0.0.82/src/model_explorer/builtin_tflite_flatbuffer_adapter.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1131 2024-04-01 19:25:08.000000 model_explorer-0.0.82/src/model_explorer/builtin_tflite_mlir_adapter.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     2230 2024-04-28 00:21:58.000000 model_explorer-0.0.82/src/model_explorer/cmdline.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     4202 2024-04-28 02:40:44.000000 model_explorer-0.0.82/src/model_explorer/config.py
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      106 2024-04-20 20:11:17.000000 model_explorer-0.0.82/src/model_explorer/consts.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)      338 2024-03-27 17:14:33.000000 model_explorer-0.0.82/src/model_explorer/extension_base.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1111 2024-03-28 23:18:49.000000 model_explorer-0.0.82/src/model_explorer/extension_class_processor.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     4294 2024-03-28 22:24:29.000000 model_explorer-0.0.82/src/model_explorer/extension_manager.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)      198 2024-03-27 17:14:33.000000 model_explorer-0.0.82/src/model_explorer/extension_matadata.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     4043 2024-04-25 21:03:05.000000 model_explorer-0.0.82/src/model_explorer/graph_builder.py
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4834 2024-04-30 00:51:33.000000 model_explorer-0.0.82/src/model_explorer/node_data_builder.py
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     6776 2024-04-25 21:04:47.000000 model_explorer-0.0.82/src/model_explorer/pytorch_exported_program_adater_impl.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)      353 2024-03-27 17:14:33.000000 model_explorer-0.0.82/src/model_explorer/registered_extension.py
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    11156 2024-04-30 00:51:16.000000 model_explorer-0.0.82/src/model_explorer/server.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)      349 2024-03-27 17:14:33.000000 model_explorer-0.0.82/src/model_explorer/singleton.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)      605 2024-04-25 21:04:04.000000 model_explorer-0.0.82/src/model_explorer/types.py
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)     1846 2024-04-25 23:26:34.000000 model_explorer-0.0.82/src/model_explorer/utils.py
+drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-30 00:51:54.301022 model_explorer-0.0.82/src/model_explorer/web_app/
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      456 2024-03-27 17:14:33.000000 model_explorer-0.0.82/src/model_explorer/web_app/index.html
+drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-30 00:51:54.309022 model_explorer-0.0.82/src/model_explorer/web_app/static_files/
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     9028 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gh09GixI.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4020 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Ghk9GixI.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15476 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GiU9G.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5340 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gik9GixI.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8332 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GjU9GixI.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8756 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmZjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     3800 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmdjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15208 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmhjtg.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5012 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmtjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     7976 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmxjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8700 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmZjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     3744 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmdjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    14796 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmhjtg.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4924 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmtjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     7764 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmxjtiu7.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8352 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTsDO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15468 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtDO_.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5424 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtzO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     9004 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTujO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4000 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTuzO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8528 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTsDO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    15864 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtDO_.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     5388 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtzO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     9100 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTujO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4084 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTuzO_PZ0.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     7860 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qE52i1dC.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     8592 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qER2i1dC.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     3792 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEV2i1dC.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4992 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEl2i1dC.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    14796 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEp2iw.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32907 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/GoogleSansTextBold.json
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)   144302 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/GoogleSansTextBold.png
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32921 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/GoogleSansTextMedium.json
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)   138086 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/GoogleSansTextMedium.png
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)    32905 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/GoogleSansTextRegular.json
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)   132192 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/GoogleSansTextRegular.png
+-rwxr-xr-x   0 jingjin  (83079) primarygroup (89939)  1193672 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/app_bundle.js
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     1234 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/favicon.svg
+-rw-r-----   0 jingjin  (83079) primarygroup (89939)   169616 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/google_material_icon.woff2
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      828 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/icons_2024021202.json
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     2092 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/icons_2024021202.png
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      456 2024-04-28 05:02:59.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/index.html
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)   615601 2024-03-27 17:14:33.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/main_deps.js
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)   128352 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/material_icon.woff2
+-r-xr-x---   0 jingjin  (83079) primarygroup (89939)   245609 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/styles.css
+-rwxr-xr-x   0 jingjin  (83079) primarygroup (89939)  2572044 2024-04-30 00:43:04.000000 model_explorer-0.0.82/src/model_explorer/web_app/static_files/worker_bin.js
+drwxr-x---   0 jingjin  (83079) primarygroup (89939)        0 2024-04-30 00:51:54.309022 model_explorer-0.0.82/src/model_explorer.egg-info/
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      755 2024-04-30 00:51:54.000000 model_explorer-0.0.82/src/model_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)     4876 2024-04-30 00:51:54.000000 model_explorer-0.0.82/src/model_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)        1 2024-04-30 00:51:54.000000 model_explorer-0.0.82/src/model_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      108 2024-04-30 00:51:54.000000 model_explorer-0.0.82/src/model_explorer.egg-info/entry_points.txt
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)      114 2024-04-30 00:51:54.000000 model_explorer-0.0.82/src/model_explorer.egg-info/requires.txt
+-rw-r--r--   0 jingjin  (83079) primarygroup (89939)       15 2024-04-30 00:51:54.000000 model_explorer-0.0.82/src/model_explorer.egg-info/top_level.txt
```

### Comparing `model_explorer-0.0.81/PKG-INFO` & `model_explorer-0.0.82/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer
-Version: 0.0.81
+Version: 0.0.82
 Summary: A modern model graph visualizer and debugger
 Author-email: Google LLC <opensource@google.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `model_explorer-0.0.81/pyproject.toml` & `model_explorer-0.0.82/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "model-explorer"
-version = "0.0.81"
+version = "0.0.82"
 authors = [
   { name="Google LLC", email="opensource@google.com" },
 ]
 description = "A modern model graph visualizer and debugger"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `model_explorer-0.0.81/src/model_explorer/adapter.py` & `model_explorer-0.0.82/src/model_explorer/adapter.py`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/adapter_runner.py` & `model_explorer-0.0.82/src/model_explorer/adapter_runner.py`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/apis.py` & `model_explorer-0.0.82/src/model_explorer/apis.py`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/builtin_graphdef_adapter.py` & `model_explorer-0.0.82/src/model_explorer/builtin_graphdef_adapter.py`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/builtin_pytorch_exportedprogram_adapter.py` & `model_explorer-0.0.82/src/model_explorer/builtin_pytorch_exportedprogram_adapter.py`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/builtin_tf_direct_adapter.py` & `model_explorer-0.0.82/src/model_explorer/builtin_tf_direct_adapter.py`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/builtin_tf_mlir_adapter.py` & `model_explorer-0.0.82/src/model_explorer/builtin_tf_mlir_adapter.py`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/builtin_tflite_flatbuffer_adapter.py` & `model_explorer-0.0.82/src/model_explorer/builtin_tflite_flatbuffer_adapter.py`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/builtin_tflite_mlir_adapter.py` & `model_explorer-0.0.82/src/model_explorer/builtin_tflite_mlir_adapter.py`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/cmdline.py` & `model_explorer-0.0.82/src/model_explorer/cmdline.py`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/config.py` & `model_explorer-0.0.82/src/model_explorer/config.py`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/extension_class_processor.py` & `model_explorer-0.0.82/src/model_explorer/extension_class_processor.py`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/extension_manager.py` & `model_explorer-0.0.82/src/model_explorer/extension_manager.py`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/graph_builder.py` & `model_explorer-0.0.82/src/model_explorer/graph_builder.py`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/node_data_builder.py` & `model_explorer-0.0.82/src/model_explorer/node_data_builder.py`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/pytorch_exported_program_adater_impl.py` & `model_explorer-0.0.82/src/model_explorer/pytorch_exported_program_adater_impl.py`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/server.py` & `model_explorer-0.0.82/src/model_explorer/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,17 +54,17 @@
     # Get version from repo.
     repo_version = _get_latest_version_from_repo(
         f'https://pypi.python.org/pypi/{PACKAGE_NAME}/json')
 
     if repo_version != '0':
       # Compare with the local installed version.
       installed_version = metadata.version(PACKAGE_NAME)
+      check_new_version_resp['runningVersion'] = installed_version
       if parse(installed_version) < parse(repo_version):
         check_new_version_resp['version'] = repo_version
-        check_new_version_resp['runningVersion'] = installed_version
         if print_msg:
           def c_print(x): return cprint(x, 'yellow')
           c_print(
               f'\n{PACKAGE_NAME} version {repo_version} is available, and you are using version {installed_version}.')
           c_print(
               'Consider upgrading via the following command:')
           c_print(
```

### Comparing `model_explorer-0.0.81/src/model_explorer/types.py` & `model_explorer-0.0.82/src/model_explorer/types.py`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/utils.py` & `model_explorer-0.0.82/src/model_explorer/utils.py`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gh09GixI.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gh09GixI.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Ghk9GixI.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Ghk9GixI.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GiU9G.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GiU9G.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gik9GixI.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9Gik9GixI.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GjU9GixI.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUo9-KzpRiLCAt4Unrc-xIKmCU5qE9GjU9GixI.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmZjtiu7.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmZjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmdjtiu7.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmdjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmhjtg.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmhjtg.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmtjtiu7.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmtjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmxjtiu7.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oLlVnmxjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmZjtiu7.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmZjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmdjtiu7.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmdjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmhjtg.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmhjtg.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmtjtiu7.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmtjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmxjtiu7.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUp9-KzpRiLCAt4Unrc-xIKmCU5oPFTnmxjtiu7.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTsDO_PZ0.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTsDO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtDO_.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtDO_.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtzO_PZ0.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTtzO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTujO_PZ0.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTujO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTuzO_PZ0.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OMmpTuzO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTsDO_PZ0.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTsDO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtDO_.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtDO_.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtzO_PZ0.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTtzO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTujO_PZ0.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTujO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTuzO_PZ0.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUr9-KzpRiLCAt4Unrc-xIKmCU5qE9OemxTuzO_PZ0.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qE52i1dC.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qE52i1dC.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qER2i1dC.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qER2i1dC.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEV2i1dC.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEV2i1dC.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEl2i1dC.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEl2i1dC.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEp2iw.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/5aUu9-KzpRiLCAt4Unrc-xIKmCU5qEp2iw.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/GoogleSansTextBold.json` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/GoogleSansTextBold.json`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/GoogleSansTextBold.png` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/GoogleSansTextBold.png`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/GoogleSansTextMedium.json` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/GoogleSansTextMedium.json`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/GoogleSansTextMedium.png` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/GoogleSansTextMedium.png`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/GoogleSansTextRegular.json` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/GoogleSansTextRegular.json`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/GoogleSansTextRegular.png` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/GoogleSansTextRegular.png`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/app_bundle.js` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/app_bundle.js`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/favicon.svg` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/favicon.svg`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/google_material_icon.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/google_material_icon.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/icons_2024021202.json` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/icons_2024021202.json`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/icons_2024021202.png` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/icons_2024021202.png`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/main_deps.js` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/main_deps.js`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/material_icon.woff2` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/material_icon.woff2`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/styles.css` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/styles.css`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer/web_app/static_files/worker_bin.js` & `model_explorer-0.0.82/src/model_explorer/web_app/static_files/worker_bin.js`

 * *Files identical despite different names*

### Comparing `model_explorer-0.0.81/src/model_explorer.egg-info/PKG-INFO` & `model_explorer-0.0.82/src/model_explorer.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer
-Version: 0.0.81
+Version: 0.0.82
 Summary: A modern model graph visualizer and debugger
 Author-email: Google LLC <opensource@google.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `model_explorer-0.0.81/src/model_explorer.egg-info/SOURCES.txt` & `model_explorer-0.0.82/src/model_explorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

