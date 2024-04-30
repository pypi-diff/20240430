# Comparing `tmp/nonebot_plugin_bilichat-5.7.1.tar.gz` & `tmp/nonebot_plugin_bilichat-5.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-5.7.1.tar", last modified: Mon Apr 29 14:03:53 2024, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-5.8.0.tar", last modified: Mon Apr 29 17:14:05 2024, max compression
```

## Comparing `nonebot_plugin_bilichat-5.7.1.tar` & `nonebot_plugin_bilichat-5.8.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0    34523 2024-04-29 14:03:46.593820 nonebot_plugin_bilichat-5.7.1/LICENSE
--rw-r--r--   0        0        0    17907 2024-04-29 14:03:46.593820 nonebot_plugin_bilichat-5.7.1/README.md
--rw-r--r--   0        0        0     2718 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     1120 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/__init__.py
--rw-r--r--   0        0        0      740 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/base.py
--rw-r--r--   0        0        0     2176 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/bilibili_auth.py
--rw-r--r--   0        0        0     1622 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/subs_config.py
--rw-r--r--   0        0        0     2655 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/webui.py
--rw-r--r--   0        0        0     7996 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/base_content_parsing.py
--rw-r--r--   0        0        0       60 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/__init__.py
--rw-r--r--   0        0        0     1280 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/auto_delete_subs.py
--rw-r--r--   0        0        0     1063 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/base.py
--rw-r--r--   0        0        0      942 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/functions.py
--rw-r--r--   0        0        0     3848 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/login.py
--rw-r--r--   0        0        0     5196 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/subs.py
--rw-r--r--   0        0        0     4996 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/subs_cfg.py
--rw-r--r--   0        0        0     9227 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0       81 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/content/__init__.py
--rw-r--r--   0        0        0     3130 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/content/column.py
--rw-r--r--   0        0        0     4227 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/content/dynamic.py
--rw-r--r--   0        0        0     3958 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/content/video.py
--rw-r--r--   0        0        0      494 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6142 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0      506 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
--rw-r--r--   0        0        0     2346 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
--rw-r--r--   0        0        0      966 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
--rw-r--r--   0        0        0     2653 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
--rw-r--r--   0        0        0     2657 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/browser.py
--rw-r--r--   0        0        0      456 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/cache/__init__.py
--rw-r--r--   0        0        0      366 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/cache/cache.py
--rw-r--r--   0        0        0      871 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/cache/json_cache.py
--rw-r--r--   0        0        0      531 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
--rw-r--r--   0        0        0      521 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/__init__.py
--rw-r--r--   0        0        0      217 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/column/__init__.py
--rw-r--r--   0        0        0     3379 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
--rw-r--r--   0        0        0      220 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
--rw-r--r--   0        0        0     5145 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
--rw-r--r--   0        0        0     1136 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
--rw-r--r--   0        0        0     7275 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/video/__init__.py
--rw-r--r--   0        0        0     6326 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
--rw-r--r--   0        0        0     3040 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
--rw-r--r--   0        0        0     3187 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/fetch_dynamic.py
--rw-r--r--   0        0        0     3376 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      525 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     3091 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     3329 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/text_to_image.py
--rw-r--r--   0        0        0     1701 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/tools.py
--rw-r--r--   0        0        0     1739 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/uid_extract.py
--rw-r--r--   0        0        0     3988 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      552 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/api/__init__.py
--rw-r--r--   0        0        0      184 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/api/bilibili_auth.py
--rw-r--r--   0        0        0      809 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/api/subs_config.py
--rw-r--r--   0        0        0      532 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     3030 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1326 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/bilibili/live.py
--rw-r--r--   0        0        0     1016 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/bilibili/summary.py
--rw-r--r--   0        0        0      596 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/const.py
--rw-r--r--   0        0        0     1163 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      291 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      270 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0     9390 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/browser/mobile_style.js
--rw-r--r--   0        0        0     1187 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2024-04-29 14:03:46.613820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    93905 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7545 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     5777 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/summary/bilibili.png
--rw-r--r--   0        0        0     2098 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/summary/index.html
--rw-r--r--   0        0        0    47433 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/summary/marked.min.js
--rw-r--r--   0        0        0    59199 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/summary/openai.png
--rw-r--r--   0        0        0     9556 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/upload-webui.html
--rw-r--r--   0        0        0   300664 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/webui.tar.gz
--rw-r--r--   0        0        0     3111 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/subscribe/__init__.py
--rw-r--r--   0        0        0     7187 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/subscribe/dynamic.py
--rw-r--r--   0        0        0     4023 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/subscribe/live.py
--rw-r--r--   0        0        0    15592 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/subscribe/manager.py
--rw-r--r--   0        0        0      478 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     4894 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2243 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1578 2024-04-29 14:03:46.617820 nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/wordcloud.py
--rw-r--r--   0        0        0     1755 2024-04-29 14:03:53.033960 nonebot_plugin_bilichat-5.7.1/pyproject.toml
--rw-r--r--   0        0        0    19603 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.7.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-29 17:13:59.639274 nonebot_plugin_bilichat-5.8.0/LICENSE
+-rw-r--r--   0        0        0    17907 2024-04-29 17:13:59.643273 nonebot_plugin_bilichat-5.8.0/README.md
+-rw-r--r--   0        0        0     2718 2024-04-29 17:13:59.659273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     1120 2024-04-29 17:13:59.659273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/api/__init__.py
+-rw-r--r--   0        0        0      740 2024-04-29 17:13:59.659273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/api/base.py
+-rw-r--r--   0        0        0     2176 2024-04-29 17:13:59.659273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/api/bilibili_auth.py
+-rw-r--r--   0        0        0     1622 2024-04-29 17:13:59.659273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/api/subs_config.py
+-rw-r--r--   0        0        0     2655 2024-04-29 17:13:59.659273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/api/webui.py
+-rw-r--r--   0        0        0     7996 2024-04-29 17:13:59.659273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/base_content_parsing.py
+-rw-r--r--   0        0        0       60 2024-04-29 17:13:59.659273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/commands/__init__.py
+-rw-r--r--   0        0        0     1280 2024-04-29 17:13:59.659273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/commands/auto_delete_subs.py
+-rw-r--r--   0        0        0     1063 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/commands/base.py
+-rw-r--r--   0        0        0      942 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/commands/functions.py
+-rw-r--r--   0        0        0     3848 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/commands/login.py
+-rw-r--r--   0        0        0     5196 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/commands/subs.py
+-rw-r--r--   0        0        0     4996 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/commands/subs_cfg.py
+-rw-r--r--   0        0        0     9227 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0       81 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/content/__init__.py
+-rw-r--r--   0        0        0     3130 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/content/column.py
+-rw-r--r--   0        0        0     4227 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/content/dynamic.py
+-rw-r--r--   0        0        0     3958 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/content/video.py
+-rw-r--r--   0        0        0      494 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6142 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0      506 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
+-rw-r--r--   0        0        0     2346 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
+-rw-r--r--   0        0        0      966 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
+-rw-r--r--   0        0        0     2653 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
+-rw-r--r--   0        0        0     2657 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/browser.py
+-rw-r--r--   0        0        0      456 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/cache/__init__.py
+-rw-r--r--   0        0        0      366 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/cache/cache.py
+-rw-r--r--   0        0        0      871 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/cache/json_cache.py
+-rw-r--r--   0        0        0      531 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
+-rw-r--r--   0        0        0      521 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/draw/__init__.py
+-rw-r--r--   0        0        0      217 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/draw/column/__init__.py
+-rw-r--r--   0        0        0     3379 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
+-rw-r--r--   0        0        0      220 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
+-rw-r--r--   0        0        0     5145 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
+-rw-r--r--   0        0        0     1136 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
+-rw-r--r--   0        0        0     7275 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py
+-rw-r--r--   0        0        0     6326 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
+-rw-r--r--   0        0        0     3040 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
+-rw-r--r--   0        0        0     3187 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py
+-rw-r--r--   0        0        0     3376 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      525 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     3091 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     3329 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/text_to_image.py
+-rw-r--r--   0        0        0     1701 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/tools.py
+-rw-r--r--   0        0        0     1739 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/uid_extract.py
+-rw-r--r--   0        0        0     3988 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      552 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/model/api/__init__.py
+-rw-r--r--   0        0        0      184 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/model/api/bilibili_auth.py
+-rw-r--r--   0        0        0      809 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/model/api/subs_config.py
+-rw-r--r--   0        0        0      532 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     3030 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1326 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/model/bilibili/live.py
+-rw-r--r--   0        0        0     1016 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/model/bilibili/summary.py
+-rw-r--r--   0        0        0      596 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/model/const.py
+-rw-r--r--   0        0        0     1163 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      291 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      270 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0     9390 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/browser/mobile_style.js
+-rw-r--r--   0        0        0     1187 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    93905 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7545 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     5777 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/summary/bilibili.png
+-rw-r--r--   0        0        0     2098 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/summary/index.html
+-rw-r--r--   0        0        0    47433 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/summary/marked.min.js
+-rw-r--r--   0        0        0    59199 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/summary/openai.png
+-rw-r--r--   0        0        0     9556 2024-04-29 17:13:59.663273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/upload-webui.html
+-rw-r--r--   0        0        0   300664 2024-04-29 17:13:59.667273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/webui.tar.gz
+-rw-r--r--   0        0        0     3111 2024-04-29 17:13:59.667273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/subscribe/__init__.py
+-rw-r--r--   0        0        0     7187 2024-04-29 17:13:59.667273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/subscribe/dynamic.py
+-rw-r--r--   0        0        0     4023 2024-04-29 17:13:59.667273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/subscribe/live.py
+-rw-r--r--   0        0        0    16423 2024-04-29 17:13:59.667273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/subscribe/manager.py
+-rw-r--r--   0        0        0      478 2024-04-29 17:13:59.667273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     4894 2024-04-29 17:13:59.667273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2243 2024-04-29 17:13:59.667273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1578 2024-04-29 17:13:59.667273 nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/wordcloud.py
+-rw-r--r--   0        0        0     1646 2024-04-29 17:14:05.083270 nonebot_plugin_bilichat-5.8.0/pyproject.toml
+-rw-r--r--   0        0        0    19603 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.8.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-5.7.1/LICENSE` & `nonebot_plugin_bilichat-5.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/README.md` & `nonebot_plugin_bilichat-5.8.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/__init__.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/base.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/api/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/bilibili_auth.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/api/bilibili_auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/subs_config.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/api/subs_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/api/webui.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/api/webui.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/base_content_parsing.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/base_content_parsing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/auto_delete_subs.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/commands/auto_delete_subs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/base.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/commands/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/functions.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/commands/functions.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/login.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/commands/login.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/subs.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/commands/subs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/commands/subs_cfg.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/commands/subs_cfg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/content/column.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/content/column.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/content/dynamic.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/content/dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/content/video.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/content/video.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/bilibili_request/auth.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/browser.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/cache/json_cache.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/cache/json_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/cache/mongo_cache.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/__init__.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/video/__init__.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/draw/video/style_blue.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/fetch_dynamic.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/text_to_image.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/tools.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/tools.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/uid_extract.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/uid_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/api/__init__.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/model/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/api/subs_config.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/model/api/subs_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/arguments.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/model/arguments.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/bilibili/live.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/model/bilibili/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/bilibili/summary.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/model/bilibili/summary.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/const.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/model/const.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/model/exception.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/model/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/browser/mobile_style.js` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/browser/mobile_style.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/summary/bilibili.png` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/summary/bilibili.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/summary/index.html` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/summary/index.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/summary/marked.min.js` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/summary/marked.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/summary/openai.png` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/summary/openai.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/upload-webui.html` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/upload-webui.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/static/webui.tar.gz` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/static/webui.tar.gz`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/subscribe/__init__.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/subscribe/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/subscribe/dynamic.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/subscribe/dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/subscribe/live.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/subscribe/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/subscribe/manager.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/subscribe/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import json
 import random
 import time
+from datetime import datetime
 from typing import Any
 
 from apscheduler.job import Job
 from nonebot import get_driver
 from nonebot.adapters import Bot
 from nonebot.compat import PYDANTIC_V2
 from nonebot.log import logger
@@ -21,23 +22,25 @@
     TargetQQGroup,
     TargetQQGuildChannel,
     TargetQQPrivate,
 )
 from nonebot_plugin_auto_bot_selector.utils.alconna import create_target, extract_target
 from pydantic import BaseModel, Field, validator
 
-from ..lib.store import data_dir
+from ..lib.store import cache_dir, data_dir
 from ..lib.tools import calc_time_total
 from ..lib.uid_extract import uid_extract_sync
 from ..optional import capture_exception
 
 CONFIG_LOCK = asyncio.Lock()
 
-subscribe_file = data_dir.joinpath("subscribe.json")
-subscribe_file.touch(0o755, True)
+SUBSCRIBE_FILE = data_dir.joinpath("subscribe.json")
+SUBSCRIBE_FILE.touch(0o755, True)
+SUBSCRIBE_FILE_ARCHIVE_DIR = cache_dir.joinpath("subscribe_archive")
+SUBSCRIBE_FILE_ARCHIVE_DIR.mkdir(0o755, True, True)
 
 driver = get_driver()
 
 
 class Uploader(BaseModel):
     """Represents an Uploader"""
 
@@ -352,32 +355,45 @@
             cls.save_to_file()
             await cls.refresh_activate_uploaders()
 
     @classmethod
     async def load_from_file(cls):
         """Load data from the JSON file."""
         try:
-            text = subscribe_file.read_text(encoding="utf-8")
+            text = SUBSCRIBE_FILE.read_text(encoding="utf-8")
         except UnicodeDecodeError:
             logger.warning("subscribe.json 非 UTF-8 编码, 尝试使用系统默认编码")
-            text = subscribe_file.read_text()
+            text = SUBSCRIBE_FILE.read_text()
         await cls.load(json.loads(text or "{}"))
 
     @classmethod
     def save_to_file(cls):
         """Save data to the JSON file."""
-        subscribe_file.write_text(
-            json.dumps(
-                cls.dump_dict(),
-                ensure_ascii=False,
-                indent=2,
-                sort_keys=True,
-            ),
+        try:
+            old = SUBSCRIBE_FILE.read_text(encoding="utf-8")
+        except UnicodeDecodeError:
+            logger.warning("subscribe.json 非 UTF-8 编码, 尝试使用系统默认编码")
+            old = SUBSCRIBE_FILE.read_text()
+        data = json.dumps(
+            cls.dump_dict(),
+            ensure_ascii=False,
+            indent=2,
+            sort_keys=True,
+        )
+        if old == data:
+            logger.info("配置文件未更改，无需保存")
+            return
+        SUBSCRIBE_FILE.write_text(
+            data=data,
             encoding="utf-8",
         )
+        backup_file = SUBSCRIBE_FILE_ARCHIVE_DIR.joinpath(f"{datetime.now().strftime('%Y-%m-%dT%H_%M_%S')}.json")
+        backup_file.touch(0o755, True)
+        backup_file.write_text(data=data, encoding="utf-8")
+        logger.info(f"配置文件已更改，备份修改后的配置文件到 {backup_file}")
 
     @classmethod
     def get_activate_uploaders(cls):
         at_ups = "\n".join([str(up) for up in cls.activate_uploaders.values()])
         logger.debug("已激活的UP:\n" + (at_ups or "无已激活的UP"))
         return at_ups
```

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/nonebot_plugin_bilichat/wordcloud.py` & `nonebot_plugin_bilichat-5.8.0/nonebot_plugin_bilichat/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.7.1/pyproject.toml` & `nonebot_plugin_bilichat-5.8.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bilichat"
-version = "5.7.1"
+version = "5.8.0"
 description = "多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.8",
@@ -47,28 +47,20 @@
     "wordcloud>=1.8.2.2",
     "nonebot-plugin-htmlrender>=0.2.0.3",
     "nonebot-plugin-mongodb>=0.1.0",
     "nonebot-plugin-sentry>=0.4.1",
     "tiktoken>=0.6.0",
 ]
 
-[tool.black]
+[tool.ruff]
 line-length = 120
-target-version = [
-    "py38",
-    "py39",
-    "py310",
-    "py311",
-]
-include = "\\.pyi?$"
-extend-exclude = ""
+target-version = "py310"
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "black>=23.3.0",
     "nonebot-adapter-onebot>=2.2.4",
     "nonebot-adapter-mirai2>=0.0.22",
     "nonebot-adapter-qq>=1.0.1",
     "viztracer>=0.16.1",
     "nonebot-adapter-satori>=0.10.3",
 ]
```

### Comparing `nonebot_plugin_bilichat-5.7.1/PKG-INFO` & `nonebot_plugin_bilichat-5.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 5.7.1
+Version: 5.8.0
 Summary: 多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.10
 Requires-Dist: bilireq>=0.2.8
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.7.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.8.0 Summary:
 å¤ç§Bç«é¾æ¥è§£æï¼è§é¢è¯äºï¼AIæ»ç»ï¼ä½ æ³è¦çé½å¨ bilichat
 Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.10 Requires-Dist:
 bilireq>=0.2.8 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot2[fastapi,websockets]>=2.0.0 Requires-Dist: httpx>=0.24.1
```

