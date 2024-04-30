# Comparing `tmp/chatllm-2024.4.3.18.28.17.tar.gz` & `tmp/chatllm-2024.4.30.15.10.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatllm-2024.4.3.18.28.17.tar", last modified: Wed Apr  3 10:28:18 2024, max compression
+gzip compressed data, was "chatllm-2024.4.30.15.10.38.tar", last modified: Tue Apr 30 07:10:39 2024, max compression
```

## Comparing `chatllm-2024.4.3.18.28.17.tar` & `chatllm-2024.4.30.15.10.38.tar`

### file list

```diff
@@ -1,317 +1,288 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.843667 chatllm-2024.4.3.18.28.17/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 chatllm-2024.4.3.18.28.17/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-10-16 03:44:58.000000 chatllm-2024.4.3.18.28.17/ITEMS.md
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)     2466 2023-10-13 02:46:31.000000 chatllm-2024.4.3.18.28.17/LLMS.md
--rw-r--r--   0 betterme   (501) staff       (20)      367 2023-08-28 09:11:46.000000 chatllm-2024.4.3.18.28.17/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     8983 2024-04-03 10:28:18.843305 chatllm-2024.4.3.18.28.17/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     6904 2023-11-09 00:43:20.000000 chatllm-2024.4.3.18.28.17/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     5851 2023-05-29 06:46:23.000000 chatllm-2024.4.3.18.28.17/README.md.bak
--rw-r--r--   0 betterme   (501) staff       (20)     1653 2023-07-31 01:36:20.000000 chatllm-2024.4.3.18.28.17/TODO.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.758033 chatllm-2024.4.3.18.28.17/apps/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2024-01-18 04:12:46.000000 chatllm-2024.4.3.18.28.17/apps/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      563 2024-01-18 04:18:13.000000 chatllm-2024.4.3.18.28.17/apps/allchat.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.758819 chatllm-2024.4.3.18.28.17/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.760486 chatllm-2024.4.3.18.28.17/chatllm/agent/
--rw-r--r--   0 betterme   (501) staff       (20)      769 2023-10-25 07:22:10.000000 chatllm-2024.4.3.18.28.17/chatllm/agent/MultiPrompt.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-10-25 06:26:02.000000 chatllm-2024.4.3.18.28.17/chatllm/agent/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.761171 chatllm-2024.4.3.18.28.17/chatllm/aigc/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-05-29 05:16:39.000000 chatllm-2024.4.3.18.28.17/chatllm/aigc/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      834 2023-05-29 05:17:00.000000 chatllm-2024.4.3.18.28.17/chatllm/aigc/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.763621 chatllm-2024.4.3.18.28.17/chatllm/api/
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-05-29 01:42:28.000000 chatllm-2024.4.3.18.28.17/chatllm/api/TODO.md
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 chatllm-2024.4.3.18.28.17/chatllm/api/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      569 2023-07-21 09:14:37.000000 chatllm-2024.4.3.18.28.17/chatllm/api/app.py
--rw-r--r--   0 betterme   (501) staff       (20)     2192 2023-06-26 05:53:59.000000 chatllm-2024.4.3.18.28.17/chatllm/api/config.py
--rw-r--r--   0 betterme   (501) staff       (20)     1010 2023-07-03 09:56:01.000000 chatllm-2024.4.3.18.28.17/chatllm/api/datamodels.py
--rw-r--r--   0 betterme   (501) staff       (20)     1748 2023-07-04 06:45:09.000000 chatllm-2024.4.3.18.28.17/chatllm/api/openai_client.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.771394 chatllm-2024.4.3.18.28.17/chatllm/api/routers/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-12-22 04:28:15.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2125 2024-03-08 11:26:53.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/all_chat_completions.py
--rw-r--r--   0 betterme   (501) staff       (20)     4363 2024-03-15 10:26:22.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/all_chat_completions_.py
--rw-r--r--   0 betterme   (501) staff       (20)     1020 2023-12-12 04:20:15.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/api.py
--rw-r--r--   0 betterme   (501) staff       (20)     1591 2024-03-27 05:39:55.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/audio_speech.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.771668 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2024-03-13 06:12:38.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2134 2024-03-22 05:53:28.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_copilot.py
--rw-r--r--   0 betterme   (501) staff       (20)     3062 2024-03-18 12:03:44.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_extra.py
--rw-r--r--   0 betterme   (501) staff       (20)     2149 2024-03-12 11:53:24.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_glm.py
--rw-r--r--   0 betterme   (501) staff       (20)     1961 2024-03-13 07:08:37.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_gptall.py
--rw-r--r--   0 betterme   (501) staff       (20)     2905 2024-03-07 09:38:32.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_kimi.py
--rw-r--r--   0 betterme   (501) staff       (20)     3151 2024-02-08 10:20:34.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_rag.py
--rw-r--r--   0 betterme   (501) staff       (20)     2286 2024-02-27 02:48:06.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_redirect.py
--rw-r--r--   0 betterme   (501) staff       (20)     2133 2024-03-25 04:10:14.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_smooth.py
--rw-r--r--   0 betterme   (501) staff       (20)     2011 2024-04-03 10:28:14.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_suno.py
--rw-r--r--   0 betterme   (501) staff       (20)     2273 2024-03-11 09:18:17.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/cocopilot.py
--rw-r--r--   0 betterme   (501) staff       (20)      407 2024-01-09 04:17:19.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     1997 2024-03-15 02:15:46.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/embeddings.py
--rw-r--r--   0 betterme   (501) staff       (20)     6180 2024-03-26 03:21:15.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/files.py
--rw-r--r--   0 betterme   (501) staff       (20)     4939 2024-03-04 06:31:29.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/files_moonshot.py
--rw-r--r--   0 betterme   (501) staff       (20)     4596 2024-03-13 06:15:25.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/files_moonshot_api.py
--rw-r--r--   0 betterme   (501) staff       (20)     1605 2023-12-20 02:41:07.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/local_embeddings.py
--rw-r--r--   0 betterme   (501) staff       (20)      779 2023-08-24 00:45:22.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/models.py
--rw-r--r--   0 betterme   (501) staff       (20)     2163 2023-12-22 04:08:42.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/smooth_completions.py
--rw-r--r--   0 betterme   (501) staff       (20)     4653 2023-11-22 03:55:32.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routers/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.773363 chatllm-2024.4.3.18.28.17/chatllm/api/routes/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routes/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      558 2023-07-24 09:51:52.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routes/api.py
--rw-r--r--   0 betterme   (501) staff       (20)     2200 2023-06-02 01:06:14.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routes/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     5023 2023-07-24 10:21:57.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routes/completions.py
--rw-r--r--   0 betterme   (501) staff       (20)     1904 2023-06-04 06:52:41.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routes/embeddings.py
--rw-r--r--   0 betterme   (501) staff       (20)     3336 2023-08-02 01:55:55.000000 chatllm-2024.4.3.18.28.17/chatllm/api/routes/responses.py
--rw-r--r--   0 betterme   (501) staff       (20)    11497 2023-05-25 09:59:48.000000 chatllm-2024.4.3.18.28.17/chatllm/api/sse_api.py
--rw-r--r--   0 betterme   (501) staff       (20)      845 2023-05-26 07:01:26.000000 chatllm-2024.4.3.18.28.17/chatllm/api/test.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.776984 chatllm-2024.4.3.18.28.17/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)     3937 2023-05-29 07:27:53.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/__chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2405 2023-06-27 08:56:59.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/chataudio.py
--rw-r--r--   0 betterme   (501) staff       (20)     2420 2023-06-29 01:53:20.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)      944 2023-05-29 04:11:25.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1693 2023-06-29 07:30:13.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/chatmind.py
--rw-r--r--   0 betterme   (501) staff       (20)     1350 2023-05-29 07:27:53.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     1875 2023-05-25 06:54:08.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 chatllm-2024.4.3.18.28.17/chatllm/applications/pipeline.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.778111 chatllm-2024.4.3.18.28.17/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-09-19 08:35:37.000000 chatllm-2024.4.3.18.28.17/chatllm/clis/TODO.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1077 2023-08-04 07:09:27.000000 chatllm-2024.4.3.18.28.17/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)     1029 2023-11-10 08:40:49.000000 chatllm-2024.4.3.18.28.17/chatllm/closeai.py
--rw-r--r--   0 betterme   (501) staff       (20)      995 2023-12-08 08:11:25.000000 chatllm-2024.4.3.18.28.17/chatllm/llm_test.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.778915 chatllm-2024.4.3.18.28.17/chatllm/llmchain/
--rw-r--r--   0 betterme   (501) staff       (20)      376 2023-12-14 00:46:13.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/TODO.md
--rw-r--r--   0 betterme   (501) staff       (20)     2244 2024-02-08 09:53:36.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.783756 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/
--rw-r--r--   0 betterme   (501) staff       (20)      548 2024-01-04 02:22:28.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2636 2024-02-08 02:05:28.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/_chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     1603 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/_chatocr.py
--rw-r--r--   0 betterme   (501) staff       (20)     4126 2024-02-07 08:58:52.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chat4all.py
--rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chataudio.py
--rw-r--r--   0 betterme   (501) staff       (20)     2365 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)      394 2023-11-01 04:09:02.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatbook.py
--rw-r--r--   0 betterme   (501) staff       (20)     5509 2024-02-07 08:58:52.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatfile.py
--rw-r--r--   0 betterme   (501) staff       (20)     5930 2024-03-18 12:05:06.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatfiles.py
--rw-r--r--   0 betterme   (501) staff       (20)     1923 2023-09-25 06:22:11.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatocr.py
--rw-r--r--   0 betterme   (501) staff       (20)     1026 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatpicture.py
--rw-r--r--   0 betterme   (501) staff       (20)     5362 2024-02-07 08:58:52.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatqa.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)     3974 2024-01-19 03:11:49.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chaturl.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-10-16 04:07:00.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatwx.py
--rw-r--r--   0 betterme   (501) staff       (20)     2728 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/summarizer.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.784308 chatllm-2024.4.3.18.28.17/chatllm/llmchain/audio/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-12-26 05:06:11.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/audio/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1660 2023-12-26 06:25:37.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/audio/speech.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.784764 chatllm-2024.4.3.18.28.17/chatllm/llmchain/callbacks/
--rw-r--r--   0 betterme   (501) staff       (20)      353 2023-07-31 03:48:34.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/callbacks/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1554 2023-08-11 07:26:25.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/callbacks/streaming.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.785229 chatllm-2024.4.3.18.28.17/chatllm/llmchain/chat_models/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-07-12 09:45:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/chat_models/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1933 2024-02-08 02:04:31.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/chat_models/openai.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.795262 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/
--rw-r--r--   0 betterme   (501) staff       (20)      509 2023-10-09 06:21:53.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3893 2023-09-11 02:31:54.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/_erniebot.py
--rw-r--r--   0 betterme   (501) staff       (20)     4777 2023-10-09 05:56:00.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/_hunyuan.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2024-01-19 03:12:52.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     3660 2024-01-24 07:46:48.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/chat_image.py
--rw-r--r--   0 betterme   (501) staff       (20)     3585 2024-01-24 07:32:54.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/chat_tts.py
--rw-r--r--   0 betterme   (501) staff       (20)     2860 2023-09-26 10:14:03.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/chatglm.py
--rw-r--r--   0 betterme   (501) staff       (20)    13871 2024-04-03 10:03:04.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/chatglm_web.py
--rw-r--r--   0 betterme   (501) staff       (20)     9862 2024-03-27 05:39:55.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/copilot.py
--rw-r--r--   0 betterme   (501) staff       (20)     6741 2024-01-05 08:26:54.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/deepseek.py
--rw-r--r--   0 betterme   (501) staff       (20)     3502 2024-04-03 08:20:19.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2521 2023-09-11 03:38:46.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/dify.py
--rw-r--r--   0 betterme   (501) staff       (20)     4875 2023-09-07 02:40:43.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/ernie.py
--rw-r--r--   0 betterme   (501) staff       (20)     9701 2024-03-15 05:39:17.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/github_copilot.py
--rw-r--r--   0 betterme   (501) staff       (20)    11369 2024-02-19 05:45:13.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/github_copilot_.py
--rw-r--r--   0 betterme   (501) staff       (20)     5515 2023-12-20 01:55:07.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/google_enerativeai.py
--rw-r--r--   0 betterme   (501) staff       (20)     2440 2023-12-14 05:38:47.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/google_enerativeai_.py
--rw-r--r--   0 betterme   (501) staff       (20)     6009 2024-03-18 07:59:15.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/gptall.py
--rw-r--r--   0 betterme   (501) staff       (20)     2024 2024-02-20 08:41:59.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/groq.py
--rw-r--r--   0 betterme   (501) staff       (20)     5146 2023-11-29 11:08:32.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/hunyuan.py
--rw-r--r--   0 betterme   (501) staff       (20)    16320 2024-03-21 10:49:51.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/kimi.py
--rw-r--r--   0 betterme   (501) staff       (20)    11454 2024-02-29 11:53:22.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/moonshot_kimi.py
--rw-r--r--   0 betterme   (501) staff       (20)    12421 2024-03-22 06:06:21.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/openai_completions.py
--rw-r--r--   0 betterme   (501) staff       (20)    12583 2024-02-28 08:56:13.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/openai_completions_bk.py
--rw-r--r--   0 betterme   (501) staff       (20)     2365 2024-03-25 04:28:28.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/smooth.py
--rw-r--r--   0 betterme   (501) staff       (20)     4275 2024-01-09 08:28:12.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/smooth_.py
--rw-r--r--   0 betterme   (501) staff       (20)     7397 2023-09-14 07:59:51.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/spark.py
--rw-r--r--   0 betterme   (501) staff       (20)     4496 2024-03-26 05:48:00.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/stepchat.py
--rw-r--r--   0 betterme   (501) staff       (20)     8300 2024-04-03 05:48:58.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/suno.py
--rw-r--r--   0 betterme   (501) staff       (20)    10613 2024-03-27 13:05:43.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/suno_.py
--rw-r--r--   0 betterme   (501) staff       (20)     6454 2024-03-28 05:02:51.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/suno__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5720 2024-04-03 10:28:14.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/suno_api.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.795684 chatllm-2024.4.3.18.28.17/chatllm/llmchain/decorators/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-07-31 03:48:34.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/decorators/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1982 2024-02-08 02:05:28.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/decorators/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.797894 chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/
--rw-r--r--   0 betterme   (501) staff       (20)     2448 2024-02-07 06:21:54.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/FilesLoader.py
--rw-r--r--   0 betterme   (501) staff       (20)      673 2024-03-18 03:22:30.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1713 2024-02-07 06:21:40.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/docx.py
--rw-r--r--   0 betterme   (501) staff       (20)     4836 2024-03-18 12:05:06.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/file.py
--rw-r--r--   0 betterme   (501) staff       (20)     3219 2024-03-18 07:47:50.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/file_loader.py
--rw-r--r--   0 betterme   (501) staff       (20)     2220 2024-02-07 06:21:54.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/image.py
--rw-r--r--   0 betterme   (501) staff       (20)     1842 2024-02-07 06:21:54.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/pdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     1787 2024-02-07 05:46:15.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/text.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.799740 chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/
--rw-r--r--   0 betterme   (501) staff       (20)      935 2024-02-07 08:58:55.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/ApiEmbeddings.py
--rw-r--r--   0 betterme   (501) staff       (20)     3534 2024-02-07 08:57:18.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/DashScopeEmbeddings.py
--rw-r--r--   0 betterme   (501) staff       (20)     1332 2024-02-07 08:57:18.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/HuggingFaceEmbeddings.py
--rw-r--r--   0 betterme   (501) staff       (20)     2327 2024-02-07 08:57:18.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/OpenAIEmbeddings.py
--rw-r--r--   0 betterme   (501) staff       (20)     2722 2023-12-20 01:40:26.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/XunfeiEmbedding.py
--rw-r--r--   0 betterme   (501) staff       (20)      507 2023-08-10 08:01:04.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7482 2024-03-15 05:39:32.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/openai_embeddings.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.801921 chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/
--rw-r--r--   0 betterme   (501) staff       (20)      546 2023-12-05 07:56:51.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1667 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/basellm.py
--rw-r--r--   0 betterme   (501) staff       (20)     3362 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/chatglm.py
--rw-r--r--   0 betterme   (501) staff       (20)     3901 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/ernie.py
--rw-r--r--   0 betterme   (501) staff       (20)     3395 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/hunyuan.py
--rw-r--r--   0 betterme   (501) staff       (20)     2437 2023-12-05 07:50:17.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/kimi.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-07-24 05:47:03.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/minimax.py
--rw-r--r--   0 betterme   (501) staff       (20)     2286 2024-02-08 01:57:34.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/spark.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.803723 chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/
--rw-r--r--   0 betterme   (501) staff       (20)      243 2023-11-09 05:49:28.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      639 2023-09-25 09:52:28.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/kb.py
--rw-r--r--   0 betterme   (501) staff       (20)     2963 2023-09-20 01:09:40.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/ocr.py
--rw-r--r--   0 betterme   (501) staff       (20)     4625 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/prompt_templates.py
--rw-r--r--   0 betterme   (501) staff       (20)      722 2023-07-13 02:06:43.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/prompt_watch.py
--rw-r--r--   0 betterme   (501) staff       (20)     2488 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/rag.py
--rw-r--r--   0 betterme   (501) staff       (20)     1973 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/格式化.py
--rw-r--r--   0 betterme   (501) staff       (20)     1650 2024-03-27 16:11:48.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/suno.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.804844 chatllm-2024.4.3.18.28.17/chatllm/llmchain/textsplitter/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-08-16 06:10:25.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/textsplitter/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1389 2023-05-15 07:48:48.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/textsplitter/ali_text_splitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     3356 2023-07-15 06:05:38.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/textsplitter/chinese_text_splitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     3179 2023-06-30 13:02:46.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/textsplitter/zh_title_enhance.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.805300 chatllm-2024.4.3.18.28.17/chatllm/llmchain/utils/
--rw-r--r--   0 betterme   (501) staff       (20)      280 2023-07-31 03:48:34.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2653 2024-02-08 02:05:02.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/utils/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.807444 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/
--rw-r--r--   0 betterme   (501) staff       (20)      910 2024-02-07 08:59:38.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/DocArrayInMemorySearch.py
--rw-r--r--   0 betterme   (501) staff       (20)     3891 2024-02-23 03:20:33.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/ElasticsearchStore.py
--rw-r--r--   0 betterme   (501) staff       (20)     4126 2024-02-07 08:59:38.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/FAISS.py
--rw-r--r--   0 betterme   (501) staff       (20)     1334 2024-02-07 08:59:38.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/Milvus.py
--rw-r--r--   0 betterme   (501) staff       (20)     4515 2024-02-07 08:59:38.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/Usearch.py
--rw-r--r--   0 betterme   (501) staff       (20)     4593 2024-02-07 08:59:38.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/VectorRecordManager.py
--rw-r--r--   0 betterme   (501) staff       (20)      661 2023-09-19 01:20:05.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1567 2023-07-14 01:13:07.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     1332 2024-02-07 08:59:38.000000 chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/index_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.808760 chatllm-2024.4.3.18.28.17/chatllm/llms/
--rw-r--r--   0 betterme   (501) staff       (20)     1526 2023-06-02 12:11:10.000000 chatllm-2024.4.3.18.28.17/chatllm/llms/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2307 2023-06-30 12:28:42.000000 chatllm-2024.4.3.18.28.17/chatllm/llms/chatglm.py
--rw-r--r--   0 betterme   (501) staff       (20)     1143 2023-07-03 09:18:07.000000 chatllm-2024.4.3.18.28.17/chatllm/llms/chatgpt.py
--rw-r--r--   0 betterme   (501) staff       (20)     1559 2023-05-22 08:19:27.000000 chatllm-2024.4.3.18.28.17/chatllm/llms/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2083 2023-05-22 08:39:00.000000 chatllm-2024.4.3.18.28.17/chatllm/llms/llama.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.809218 chatllm-2024.4.3.18.28.17/chatllm/prompts/
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-06-12 03:51:17.000000 chatllm-2024.4.3.18.28.17/chatllm/prompts/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1556 2023-11-20 08:02:57.000000 chatllm-2024.4.3.18.28.17/chatllm/prompts/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.812096 chatllm-2024.4.3.18.28.17/chatllm/schemas/
--rw-r--r--   0 betterme   (501) staff       (20)     1790 2023-12-11 10:49:08.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/4v.py
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-07-31 02:38:12.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5022 2024-03-21 06:09:38.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/chatglm_types.py
--rw-r--r--   0 betterme   (501) staff       (20)      867 2024-01-11 01:35:59.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.812654 chatllm-2024.4.3.18.28.17/chatllm/schemas/json_schema_extra/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2024-01-19 07:34:54.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/json_schema_extra/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.813598 chatllm-2024.4.3.18.28.17/chatllm/schemas/kimi/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-11-29 08:43:08.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/kimi/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2689 2023-12-28 01:16:22.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/kimi/protocol.py
--rw-r--r--   0 betterme   (501) staff       (20)     3193 2024-02-29 08:15:07.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/kimi/state.json
--rw-r--r--   0 betterme   (501) staff       (20)     3607 2024-03-21 11:03:35.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/kimi_types.py
--rw-r--r--   0 betterme   (501) staff       (20)      340 2023-11-03 10:59:44.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/metadata.py
--rw-r--r--   0 betterme   (501) staff       (20)    12079 2024-03-27 13:44:00.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/openai_api_protocol.py
--rw-r--r--   0 betterme   (501) staff       (20)     4451 2024-03-27 04:49:24.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/openai_types.py
--rw-r--r--   0 betterme   (501) staff       (20)     4065 2024-03-28 12:59:41.000000 chatllm-2024.4.3.18.28.17/chatllm/schemas/suno_types.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.815169 chatllm-2024.4.3.18.28.17/chatllm/serve/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-07-31 02:40:14.000000 chatllm-2024.4.3.18.28.17/chatllm/serve/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    29234 2023-07-31 02:44:27.000000 chatllm-2024.4.3.18.28.17/chatllm/serve/_openai_api_server.py
--rw-r--r--   0 betterme   (501) staff       (20)     1178 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/serve/app.py
--rw-r--r--   0 betterme   (501) staff       (20)     1870 2023-07-19 10:34:49.000000 chatllm-2024.4.3.18.28.17/chatllm/serve/constants.py
--rw-r--r--   0 betterme   (501) staff       (20)    25416 2023-08-24 00:45:22.000000 chatllm-2024.4.3.18.28.17/chatllm/serve/openai_api_server.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.817363 chatllm-2024.4.3.18.28.17/chatllm/utils/
--rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 chatllm-2024.4.3.18.28.17/chatllm/utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 chatllm-2024.4.3.18.28.17/chatllm/utils/_textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2270 2024-02-06 13:51:45.000000 chatllm-2024.4.3.18.28.17/chatllm/utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     2430 2023-05-19 09:28:43.000000 chatllm-2024.4.3.18.28.17/chatllm/utils/gpu_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     6342 2023-05-30 08:31:55.000000 chatllm-2024.4.3.18.28.17/chatllm/utils/nbce.py
--rw-r--r--   0 betterme   (501) staff       (20)     5208 2023-05-30 08:22:36.000000 chatllm-2024.4.3.18.28.17/chatllm/utils/nbce_test.py
--rw-r--r--   0 betterme   (501) staff       (20)     3360 2024-03-22 08:36:40.000000 chatllm-2024.4.3.18.28.17/chatllm/utils/openai_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.833471 chatllm-2024.4.3.18.28.17/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)     7568 2023-11-09 06:40:18.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/!.png
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)   225373 2023-09-28 00:58:21.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/bot.png
--rw-r--r--   0 betterme   (501) staff       (20)     2747 2023-08-11 06:45:35.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chat.py
--rw-r--r--   0 betterme   (501) staff       (20)     1826 2023-12-14 02:59:58.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chat_copilot.py
--rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-05-29 07:27:53.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)   123851 2023-10-26 08:17:41.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatbook.png
--rw-r--r--   0 betterme   (501) staff       (20)     5660 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatbook.py
--rw-r--r--   0 betterme   (501) staff       (20)    14406 2023-09-05 09:04:59.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatbot.png
--rw-r--r--   0 betterme   (501) staff       (20)     3389 2023-09-25 01:29:31.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatbot.py
--rw-r--r--   0 betterme   (501) staff       (20)     4044 2023-08-28 06:36:36.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile.py
--rw-r--r--   0 betterme   (501) staff       (20)     5642 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_nesc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1968 2024-03-25 06:05:55.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_nesc_glm_v0.1.py
--rw-r--r--   0 betterme   (501) staff       (20)     2417 2024-03-20 09:52:09.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_nesc_last.py
--rw-r--r--   0 betterme   (501) staff       (20)     5741 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_nesc_v1.py
--rw-r--r--   0 betterme   (501) staff       (20)     3103 2024-01-12 05:56:43.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_nesc_v2.py
--rw-r--r--   0 betterme   (501) staff       (20)     2781 2024-02-01 14:00:42.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_v0.1.py
--rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-06-29 07:59:43.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatmind.py
--rw-r--r--   0 betterme   (501) staff       (20)     3103 2023-08-23 04:01:26.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      134 2023-06-26 02:13:58.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/conf.yaml
--rw-r--r--   0 betterme   (501) staff       (20)     1093 2023-11-06 09:12:04.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/dalle.py
--rw-r--r--   0 betterme   (501) staff       (20)      554 2023-11-15 06:57:01.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     4235 2024-01-25 05:24:50.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/fire.png
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)   856440 2023-09-25 01:29:08.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/logo.png
--rw-r--r--   0 betterme   (501) staff       (20)   102641 2023-08-11 06:34:47.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/nesc.jpeg
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      557 2024-02-07 08:56:45.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/prompt_maker.py
--rw-r--r--   0 betterme   (501) staff       (20)     4445 2024-02-07 08:59:38.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/qa.py
--rw-r--r--   0 betterme   (501) staff       (20)      468 2024-03-26 09:28:22.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/run.sh
--rw-r--r--   0 betterme   (501) staff       (20)     4312 2023-08-08 10:37:46.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/user.jpg
--rw-r--r--   0 betterme   (501) staff       (20)     3506 2023-05-26 07:39:23.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/visualglm_st.py
--rw-r--r--   0 betterme   (501) staff       (20)   437368 2024-01-12 05:38:09.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/副本人工智能咨询服务协议 汉洁 南京当月糯 20240105(1)(1).docx
--rw-r--r--   0 betterme   (501) staff       (20)    10521 2024-02-01 13:14:34.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/同程报价.xlsx
--rw-r--r--   0 betterme   (501) staff       (20)   303359 2023-09-20 06:32:26.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/规丞相.png
--rw-r--r--   0 betterme   (501) staff       (20)   414314 2024-02-01 13:16:20.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/酒店百问百答.pdf
--rw-r--r--   0 betterme   (501) staff       (20)   741995 2024-01-12 05:38:20.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/附件1：东北证券股份有限公司员工合规手册（2023年12月）.doc
--rw-r--r--   0 betterme   (501) staff       (20)   416458 2023-12-27 07:56:52.000000 chatllm-2024.4.3.18.28.17/chatllm/webui/附件1：东北证券股份有限公司员工合规手册（2023年12月）.docx
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.841617 chatllm-2024.4.3.18.28.17/chatllm.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     8983 2024-04-03 10:28:18.000000 chatllm-2024.4.3.18.28.17/chatllm.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     9242 2024-04-03 10:28:18.000000 chatllm-2024.4.3.18.28.17/chatllm.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2024-04-03 10:28:18.000000 chatllm-2024.4.3.18.28.17/chatllm.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2024-04-03 10:28:18.000000 chatllm-2024.4.3.18.28.17/chatllm.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2024-04-03 10:28:18.000000 chatllm-2024.4.3.18.28.17/chatllm.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)      425 2024-04-03 10:28:18.000000 chatllm-2024.4.3.18.28.17/chatllm.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2024-04-03 10:28:18.000000 chatllm-2024.4.3.18.28.17/chatllm.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)      684 2023-03-20 02:44:39.000000 chatllm-2024.4.3.18.28.17/clear_git_history.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.840081 chatllm-2024.4.3.18.28.17/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/docs/readme.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      350 2023-10-16 06:38:24.000000 chatllm-2024.4.3.18.28.17/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)      137 2023-09-14 06:48:16.000000 chatllm-2024.4.3.18.28.17/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       14 2023-05-19 09:53:16.000000 chatllm-2024.4.3.18.28.17/requirements_ann.txt
--rw-r--r--   0 betterme   (501) staff       (20)       30 2023-05-31 02:41:18.000000 chatllm-2024.4.3.18.28.17/requirements_api.txt
--rw-r--r--   0 betterme   (501) staff       (20)       29 2023-05-26 08:03:09.000000 chatllm-2024.4.3.18.28.17/requirements_openai.txt
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-05-29 04:24:55.000000 chatllm-2024.4.3.18.28.17/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       22 2024-01-09 05:49:39.000000 chatllm-2024.4.3.18.28.17/requirements_rag.txt
--rw-r--r--   0 betterme   (501) staff       (20)       25 2023-05-29 04:24:55.000000 chatllm-2024.4.3.18.28.17/requirements_streamlit.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2024-04-03 10:28:18.843721 chatllm-2024.4.3.18.28.17/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1706 2023-07-19 10:53:05.000000 chatllm-2024.4.3.18.28.17/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-03 10:28:18.841030 chatllm-2024.4.3.18.28.17/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 chatllm-2024.4.3.18.28.17/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1224 2023-12-11 01:53:35.000000 chatllm-2024.4.3.18.28.17/tests/oneapi_test.py
--rw-r--r--   0 betterme   (501) staff       (20)      224 2023-10-25 08:02:40.000000 chatllm-2024.4.3.18.28.17/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 chatllm-2024.4.3.18.28.17/tests/内存型.ipynb
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.105306 chatllm-2024.4.30.15.10.38/
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 chatllm-2024.4.30.15.10.38/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      367 2023-08-28 09:11:46.000000 chatllm-2024.4.30.15.10.38/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     8984 2024-04-30 07:10:39.104968 chatllm-2024.4.30.15.10.38/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     6904 2023-11-09 00:43:20.000000 chatllm-2024.4.30.15.10.38/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     5851 2023-05-29 06:46:23.000000 chatllm-2024.4.30.15.10.38/README.md.bak
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.013394 chatllm-2024.4.30.15.10.38/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 chatllm-2024.4.30.15.10.38/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.015257 chatllm-2024.4.30.15.10.38/chatllm/agents/
+-rw-r--r--   0 betterme   (501) staff       (20)      769 2023-10-25 07:22:10.000000 chatllm-2024.4.30.15.10.38/chatllm/agents/MultiPrompt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-10-25 06:26:02.000000 chatllm-2024.4.30.15.10.38/chatllm/agents/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      265 2024-04-22 06:43:04.000000 chatllm-2024.4.30.15.10.38/chatllm/agents/glm_agent.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.015648 chatllm-2024.4.30.15.10.38/chatllm/aigc/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-05-29 05:16:39.000000 chatllm-2024.4.30.15.10.38/chatllm/aigc/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      834 2023-05-29 05:17:00.000000 chatllm-2024.4.30.15.10.38/chatllm/aigc/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.018394 chatllm-2024.4.30.15.10.38/chatllm/api/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 chatllm-2024.4.30.15.10.38/chatllm/api/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      569 2023-07-21 09:14:37.000000 chatllm-2024.4.30.15.10.38/chatllm/api/app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2192 2023-06-26 05:53:59.000000 chatllm-2024.4.30.15.10.38/chatllm/api/config.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1010 2023-07-03 09:56:01.000000 chatllm-2024.4.30.15.10.38/chatllm/api/datamodels.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1748 2023-07-04 06:45:09.000000 chatllm-2024.4.30.15.10.38/chatllm/api/openai_client.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.026738 chatllm-2024.4.30.15.10.38/chatllm/api/routers/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-12-22 04:28:15.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2125 2024-03-08 11:26:53.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/all_chat_completions.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4363 2024-03-15 10:26:22.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/all_chat_completions_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1020 2023-12-12 04:20:15.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/api.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1591 2024-03-27 05:39:55.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/audio_speech.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2118 2024-04-23 00:55:53.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_all.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1997 2024-04-30 06:55:18.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_cf.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.027006 chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2024-03-13 06:12:38.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2134 2024-03-22 05:53:28.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions_copilot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3062 2024-03-18 12:03:44.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions_extra.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2149 2024-03-12 11:53:24.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions_glm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1961 2024-03-13 07:08:37.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions_gptall.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2905 2024-03-07 09:38:32.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions_kimi.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3151 2024-02-08 10:20:34.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions_rag.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2286 2024-02-27 02:48:06.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions_redirect.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2133 2024-03-25 04:10:14.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions_smooth.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2027 2024-04-26 10:33:15.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions_suno.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1751 2024-04-30 01:46:09.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_deeplx.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2273 2024-03-11 09:18:17.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/cocopilot.py
+-rw-r--r--   0 betterme   (501) staff       (20)      407 2024-01-09 04:17:19.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1997 2024-03-15 02:15:46.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/embeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6180 2024-03-26 03:21:15.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/files.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4939 2024-03-04 06:31:29.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/files_moonshot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4596 2024-03-13 06:15:25.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/files_moonshot_api.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1605 2023-12-20 02:41:07.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/local_embeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)      779 2023-08-24 00:45:22.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/models.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2163 2023-12-22 04:08:42.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/smooth_completions.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4653 2023-11-22 03:55:32.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routers/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.028591 chatllm-2024.4.30.15.10.38/chatllm/api/routes/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routes/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      558 2023-07-24 09:51:52.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routes/api.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2200 2023-06-02 01:06:14.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routes/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5023 2023-07-24 10:21:57.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routes/completions.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1904 2023-06-04 06:52:41.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routes/embeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3336 2023-08-02 01:55:55.000000 chatllm-2024.4.30.15.10.38/chatllm/api/routes/responses.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11497 2023-05-25 09:59:48.000000 chatllm-2024.4.30.15.10.38/chatllm/api/sse_api.py
+-rw-r--r--   0 betterme   (501) staff       (20)      845 2023-05-26 07:01:26.000000 chatllm-2024.4.30.15.10.38/chatllm/api/test.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.032441 chatllm-2024.4.30.15.10.38/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 chatllm-2024.4.30.15.10.38/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3937 2023-05-29 07:27:53.000000 chatllm-2024.4.30.15.10.38/chatllm/applications/__chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 chatllm-2024.4.30.15.10.38/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2405 2023-06-27 08:56:59.000000 chatllm-2024.4.30.15.10.38/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 chatllm-2024.4.30.15.10.38/chatllm/applications/chataudio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2420 2023-06-29 01:53:20.000000 chatllm-2024.4.30.15.10.38/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)      944 2023-05-29 04:11:25.000000 chatllm-2024.4.30.15.10.38/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2024.4.30.15.10.38/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1693 2023-06-29 07:30:13.000000 chatllm-2024.4.30.15.10.38/chatllm/applications/chatmind.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1350 2023-05-29 07:27:53.000000 chatllm-2024.4.30.15.10.38/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1875 2023-05-25 06:54:08.000000 chatllm-2024.4.30.15.10.38/chatllm/applications/chatwhoosh.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 chatllm-2024.4.30.15.10.38/chatllm/applications/pipeline.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.032952 chatllm-2024.4.30.15.10.38/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 chatllm-2024.4.30.15.10.38/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1077 2023-08-04 07:09:27.000000 chatllm-2024.4.30.15.10.38/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1029 2023-11-10 08:40:49.000000 chatllm-2024.4.30.15.10.38/chatllm/closeai.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.034238 chatllm-2024.4.30.15.10.38/chatllm/completions/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2024-04-22 06:49:57.000000 chatllm-2024.4.30.15.10.38/chatllm/completions/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3259 2024-04-30 07:08:54.000000 chatllm-2024.4.30.15.10.38/chatllm/completions/cf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4031 2024-04-23 03:07:55.000000 chatllm-2024.4.30.15.10.38/chatllm/completions/chat_all.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2771 2024-04-30 05:33:12.000000 chatllm-2024.4.30.15.10.38/chatllm/completions/deeplx.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1950 2024-04-25 05:21:03.000000 chatllm-2024.4.30.15.10.38/chatllm/completions/free.py
+-rw-r--r--   0 betterme   (501) staff       (20)      299 2024-04-22 06:51:47.000000 chatllm-2024.4.30.15.10.38/chatllm/completions/glm.py
+-rw-r--r--   0 betterme   (501) staff       (20)      995 2023-12-08 08:11:25.000000 chatllm-2024.4.30.15.10.38/chatllm/llm_test.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.034461 chatllm-2024.4.30.15.10.38/chatllm/llmchain/
+-rw-r--r--   0 betterme   (501) staff       (20)     2244 2024-02-08 09:53:36.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.040099 chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)      548 2024-01-04 02:22:28.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2636 2024-02-08 02:05:28.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/_chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1603 2024-02-07 08:56:45.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/_chatocr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4126 2024-02-07 08:58:52.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chat4all.py
+-rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chataudio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2365 2024-02-07 08:56:45.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)      394 2023-11-01 04:09:02.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chatbook.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5509 2024-02-07 08:58:52.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chatfile.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5930 2024-03-18 12:05:06.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chatfiles.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1923 2023-09-25 06:22:11.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chatocr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1026 2024-02-07 08:56:45.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chatpicture.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5362 2024-02-07 08:58:52.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chatqa.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3974 2024-01-19 03:11:49.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chaturl.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-10-16 04:07:00.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chatwx.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2728 2024-02-07 08:56:45.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/summarizer.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.040684 chatllm-2024.4.30.15.10.38/chatllm/llmchain/audio/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-12-26 05:06:11.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/audio/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1660 2023-12-26 06:25:37.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/audio/speech.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.041146 chatllm-2024.4.30.15.10.38/chatllm/llmchain/callbacks/
+-rw-r--r--   0 betterme   (501) staff       (20)      353 2023-07-31 03:48:34.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/callbacks/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1554 2023-08-11 07:26:25.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/callbacks/streaming.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.041591 chatllm-2024.4.30.15.10.38/chatllm/llmchain/chat_models/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-07-12 09:45:45.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/chat_models/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1933 2024-02-08 02:04:31.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/chat_models/openai.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.052224 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/
+-rw-r--r--   0 betterme   (501) staff       (20)      509 2023-10-09 06:21:53.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3893 2023-09-11 02:31:54.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/_erniebot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4777 2023-10-09 05:56:00.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/_hunyuan.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2024-01-19 03:12:52.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3660 2024-01-24 07:46:48.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/chat_image.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3585 2024-01-24 07:32:54.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/chat_tts.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2860 2023-09-26 10:14:03.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/chatglm.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14071 2024-04-30 06:29:15.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/chatglm_web.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9862 2024-03-27 05:39:55.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/copilot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6741 2024-01-05 08:26:54.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/deepseek.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3502 2024-04-03 08:20:19.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2521 2023-09-11 03:38:46.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/dify.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4875 2023-09-07 02:40:43.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/ernie.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9701 2024-03-15 05:39:17.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/github_copilot.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11369 2024-02-19 05:45:13.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/github_copilot_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5515 2023-12-20 01:55:07.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/google_enerativeai.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2440 2023-12-14 05:38:47.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/google_enerativeai_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6009 2024-03-18 07:59:15.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/gptall.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2024 2024-02-20 08:41:59.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/groq.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5146 2023-11-29 11:08:32.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/hunyuan.py
+-rw-r--r--   0 betterme   (501) staff       (20)    16320 2024-03-21 10:49:51.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/kimi.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11454 2024-02-29 11:53:22.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/moonshot_kimi.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12421 2024-03-22 06:06:21.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/openai_completions.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12583 2024-02-28 08:56:13.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/openai_completions_bk.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2365 2024-03-25 04:28:28.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/smooth.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4275 2024-01-09 08:28:12.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/smooth_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7397 2023-09-14 07:59:51.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/spark.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4499 2024-04-10 06:35:47.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/stepchat.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8300 2024-04-03 05:48:58.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/suno.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10613 2024-03-27 13:05:43.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/suno_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6454 2024-03-28 05:02:51.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/suno__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11805 2024-04-26 11:07:25.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/suno_api.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7941 2024-04-24 07:17:33.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/suno_api_.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.052599 chatllm-2024.4.30.15.10.38/chatllm/llmchain/decorators/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-07-31 03:48:34.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/decorators/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1982 2024-02-08 02:05:28.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/decorators/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.055095 chatllm-2024.4.30.15.10.38/chatllm/llmchain/document_loaders/
+-rw-r--r--   0 betterme   (501) staff       (20)     2448 2024-02-07 06:21:54.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/document_loaders/FilesLoader.py
+-rw-r--r--   0 betterme   (501) staff       (20)      673 2024-03-18 03:22:30.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/document_loaders/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1713 2024-02-07 06:21:40.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/document_loaders/docx.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4836 2024-03-18 12:05:06.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/document_loaders/file.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3219 2024-03-18 07:47:50.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/document_loaders/file_loader.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2220 2024-02-07 06:21:54.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/document_loaders/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1842 2024-02-07 06:21:54.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/document_loaders/pdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1787 2024-02-07 05:46:15.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/document_loaders/text.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.057327 chatllm-2024.4.30.15.10.38/chatllm/llmchain/embeddings/
+-rw-r--r--   0 betterme   (501) staff       (20)      935 2024-02-07 08:58:55.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/embeddings/ApiEmbeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3534 2024-02-07 08:57:18.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/embeddings/DashScopeEmbeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1332 2024-02-07 08:57:18.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/embeddings/HuggingFaceEmbeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2327 2024-02-07 08:57:18.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/embeddings/OpenAIEmbeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2722 2023-12-20 01:40:26.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/embeddings/XunfeiEmbedding.py
+-rw-r--r--   0 betterme   (501) staff       (20)      507 2023-08-10 08:01:04.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/embeddings/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7482 2024-03-15 05:39:32.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/embeddings/openai_embeddings.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.060089 chatllm-2024.4.30.15.10.38/chatllm/llmchain/llms/
+-rw-r--r--   0 betterme   (501) staff       (20)      546 2023-12-05 07:56:51.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/llms/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1667 2024-02-07 08:56:45.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/llms/basellm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3362 2024-02-07 08:56:45.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/llms/chatglm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3901 2024-02-07 08:56:45.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/llms/ernie.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3395 2024-02-07 08:56:45.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/llms/hunyuan.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2437 2023-12-05 07:50:17.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/llms/kimi.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-07-24 05:47:03.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/llms/minimax.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2286 2024-02-08 01:57:34.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/llms/spark.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.062365 chatllm-2024.4.30.15.10.38/chatllm/llmchain/prompts/
+-rw-r--r--   0 betterme   (501) staff       (20)      243 2023-11-09 05:49:28.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/prompts/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      639 2023-09-25 09:52:28.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/prompts/kb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2963 2023-09-20 01:09:40.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/prompts/ocr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4625 2024-02-07 08:56:45.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/prompts/prompt_templates.py
+-rw-r--r--   0 betterme   (501) staff       (20)      722 2023-07-13 02:06:43.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/prompts/prompt_watch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2488 2024-02-07 08:56:45.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/prompts/rag.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1973 2024-02-07 08:56:45.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/prompts/格式化.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.064105 chatllm-2024.4.30.15.10.38/chatllm/llmchain/textsplitter/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-08-16 06:10:25.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/textsplitter/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1389 2023-05-15 07:48:48.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/textsplitter/ali_text_splitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3356 2023-07-15 06:05:38.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/textsplitter/chinese_text_splitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3179 2023-06-30 13:02:46.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/textsplitter/zh_title_enhance.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.064659 chatllm-2024.4.30.15.10.38/chatllm/llmchain/utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      280 2023-07-31 03:48:34.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2653 2024-02-08 02:05:02.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/utils/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.068069 chatllm-2024.4.30.15.10.38/chatllm/llmchain/vectorstores/
+-rw-r--r--   0 betterme   (501) staff       (20)      910 2024-02-07 08:59:38.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/vectorstores/DocArrayInMemorySearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3891 2024-02-23 03:20:33.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/vectorstores/ElasticsearchStore.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4126 2024-02-07 08:59:38.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/vectorstores/FAISS.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1334 2024-02-07 08:59:38.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/vectorstores/Milvus.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4515 2024-02-07 08:59:38.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/vectorstores/Usearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4593 2024-02-07 08:59:38.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/vectorstores/VectorRecordManager.py
+-rw-r--r--   0 betterme   (501) staff       (20)      661 2023-09-19 01:20:05.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/vectorstores/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1567 2023-07-14 01:13:07.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/vectorstores/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1332 2024-02-07 08:59:38.000000 chatllm-2024.4.30.15.10.38/chatllm/llmchain/vectorstores/index_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.076552 chatllm-2024.4.30.15.10.38/chatllm/llms/
+-rw-r--r--   0 betterme   (501) staff       (20)     1526 2023-06-02 12:11:10.000000 chatllm-2024.4.30.15.10.38/chatllm/llms/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2307 2023-06-30 12:28:42.000000 chatllm-2024.4.30.15.10.38/chatllm/llms/chatglm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1143 2023-07-03 09:18:07.000000 chatllm-2024.4.30.15.10.38/chatllm/llms/chatgpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1559 2023-05-22 08:19:27.000000 chatllm-2024.4.30.15.10.38/chatllm/llms/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2083 2023-05-22 08:39:00.000000 chatllm-2024.4.30.15.10.38/chatllm/llms/llama.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.077229 chatllm-2024.4.30.15.10.38/chatllm/prompts/
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-06-12 03:51:17.000000 chatllm-2024.4.30.15.10.38/chatllm/prompts/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1556 2023-11-20 08:02:57.000000 chatllm-2024.4.30.15.10.38/chatllm/prompts/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.080262 chatllm-2024.4.30.15.10.38/chatllm/schemas/
+-rw-r--r--   0 betterme   (501) staff       (20)     1790 2023-12-11 10:49:08.000000 chatllm-2024.4.30.15.10.38/chatllm/schemas/4v.py
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-07-31 02:38:12.000000 chatllm-2024.4.30.15.10.38/chatllm/schemas/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5022 2024-03-21 06:09:38.000000 chatllm-2024.4.30.15.10.38/chatllm/schemas/chatglm_types.py
+-rw-r--r--   0 betterme   (501) staff       (20)      867 2024-01-11 01:35:59.000000 chatllm-2024.4.30.15.10.38/chatllm/schemas/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.080651 chatllm-2024.4.30.15.10.38/chatllm/schemas/json_schema_extra/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2024-01-19 07:34:54.000000 chatllm-2024.4.30.15.10.38/chatllm/schemas/json_schema_extra/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.081531 chatllm-2024.4.30.15.10.38/chatllm/schemas/kimi/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-11-29 08:43:08.000000 chatllm-2024.4.30.15.10.38/chatllm/schemas/kimi/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2689 2023-12-28 01:16:22.000000 chatllm-2024.4.30.15.10.38/chatllm/schemas/kimi/protocol.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3607 2024-03-21 11:03:35.000000 chatllm-2024.4.30.15.10.38/chatllm/schemas/kimi_types.py
+-rw-r--r--   0 betterme   (501) staff       (20)      340 2023-11-03 10:59:44.000000 chatllm-2024.4.30.15.10.38/chatllm/schemas/metadata.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12801 2024-04-30 01:58:04.000000 chatllm-2024.4.30.15.10.38/chatllm/schemas/openai_api_protocol.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4463 2024-04-30 06:58:48.000000 chatllm-2024.4.30.15.10.38/chatllm/schemas/openai_types.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4662 2024-04-26 09:48:31.000000 chatllm-2024.4.30.15.10.38/chatllm/schemas/suno_types.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.083489 chatllm-2024.4.30.15.10.38/chatllm/serve/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-07-31 02:40:14.000000 chatllm-2024.4.30.15.10.38/chatllm/serve/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    29234 2023-07-31 02:44:27.000000 chatllm-2024.4.30.15.10.38/chatllm/serve/_openai_api_server.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1178 2024-02-07 08:56:45.000000 chatllm-2024.4.30.15.10.38/chatllm/serve/app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1870 2023-07-19 10:34:49.000000 chatllm-2024.4.30.15.10.38/chatllm/serve/constants.py
+-rw-r--r--   0 betterme   (501) staff       (20)    25416 2023-08-24 00:45:22.000000 chatllm-2024.4.30.15.10.38/chatllm/serve/openai_api_server.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.085514 chatllm-2024.4.30.15.10.38/chatllm/utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 chatllm-2024.4.30.15.10.38/chatllm/utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 chatllm-2024.4.30.15.10.38/chatllm/utils/_textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2257 2024-04-24 01:12:25.000000 chatllm-2024.4.30.15.10.38/chatllm/utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2430 2023-05-19 09:28:43.000000 chatllm-2024.4.30.15.10.38/chatllm/utils/gpu_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6342 2023-05-30 08:31:55.000000 chatllm-2024.4.30.15.10.38/chatllm/utils/nbce.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5208 2023-05-30 08:22:36.000000 chatllm-2024.4.30.15.10.38/chatllm/utils/nbce_test.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6132 2024-04-24 01:12:25.000000 chatllm-2024.4.30.15.10.38/chatllm/utils/openai_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.094059 chatllm-2024.4.30.15.10.38/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2747 2023-08-11 06:45:35.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/chat.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1826 2023-12-14 02:59:58.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/chat_copilot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-05-29 07:27:53.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5660 2024-02-07 08:56:45.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/chatbook.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3389 2023-09-25 01:29:31.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/chatbot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4044 2023-08-28 06:36:36.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/chatfile.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5642 2024-02-07 08:56:45.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/chatfile_nesc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1968 2024-03-25 06:05:55.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/chatfile_nesc_glm_v0.1.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2417 2024-03-20 09:52:09.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/chatfile_nesc_last.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5741 2024-02-07 08:56:45.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/chatfile_nesc_v1.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3103 2024-01-12 05:56:43.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/chatfile_nesc_v2.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2781 2024-02-01 14:00:42.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/chatfile_v0.1.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-06-29 07:59:43.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/chatmind.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3103 2023-08-23 04:01:26.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1093 2023-11-06 09:12:04.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/dalle.py
+-rw-r--r--   0 betterme   (501) staff       (20)      554 2023-11-15 06:57:01.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      557 2024-02-07 08:56:45.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/prompt_maker.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4445 2024-02-07 08:59:38.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/qa.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3506 2023-05-26 07:39:23.000000 chatllm-2024.4.30.15.10.38/chatllm/webui/visualglm_st.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.014555 chatllm-2024.4.30.15.10.38/chatllm.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     8984 2024-04-30 07:10:38.000000 chatllm-2024.4.30.15.10.38/chatllm.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     8541 2024-04-30 07:10:38.000000 chatllm-2024.4.30.15.10.38/chatllm.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2024-04-30 07:10:38.000000 chatllm-2024.4.30.15.10.38/chatllm.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2024-04-30 07:10:38.000000 chatllm-2024.4.30.15.10.38/chatllm.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2024-04-30 07:10:38.000000 chatllm-2024.4.30.15.10.38/chatllm.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)      425 2024-04-30 07:10:38.000000 chatllm-2024.4.30.15.10.38/chatllm.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2024-04-30 07:10:38.000000 chatllm-2024.4.30.15.10.38/chatllm.egg-info/top_level.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.101831 chatllm-2024.4.30.15.10.38/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 chatllm-2024.4.30.15.10.38/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2024.4.30.15.10.38/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 chatllm-2024.4.30.15.10.38/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 chatllm-2024.4.30.15.10.38/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2024.4.30.15.10.38/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 chatllm-2024.4.30.15.10.38/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 chatllm-2024.4.30.15.10.38/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 chatllm-2024.4.30.15.10.38/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2024-04-30 07:10:39.105439 chatllm-2024.4.30.15.10.38/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1706 2023-07-19 10:53:05.000000 chatllm-2024.4.30.15.10.38/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-30 07:10:39.102971 chatllm-2024.4.30.15.10.38/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 chatllm-2024.4.30.15.10.38/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1224 2023-12-11 01:53:35.000000 chatllm-2024.4.30.15.10.38/tests/oneapi_test.py
+-rw-r--r--   0 betterme   (501) staff       (20)      224 2023-10-25 08:02:40.000000 chatllm-2024.4.30.15.10.38/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 chatllm-2024.4.30.15.10.38/tests/内存型.ipynb
```

### Comparing `chatllm-2024.4.3.18.28.17/LICENSE` & `chatllm-2024.4.30.15.10.38/LICENSE`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/PKG-INFO` & `chatllm-2024.4.30.15.10.38/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatllm
-Version: 2024.4.3.18.28.17
+Version: 2024.4.30.15.10.38
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -43,25 +43,25 @@
 Requires-Dist: streamlit; extra == "streamlit"
 Requires-Dist: streamlit_chat; extra == "streamlit"
 Provides-Extra: rag
 Requires-Dist: redis; extra == "rag"
 Requires-Dist: minio; extra == "rag"
 Requires-Dist: faiss-cpu; extra == "rag"
 Provides-Extra: all
-Requires-Dist: pymupdf; extra == "all"
 Requires-Dist: sse-starlette; extra == "all"
 Requires-Dist: streamlit; extra == "all"
-Requires-Dist: sse_starlette; extra == "all"
-Requires-Dist: redis; extra == "all"
-Requires-Dist: streamlit_chat; extra == "all"
+Requires-Dist: fastapi; extra == "all"
 Requires-Dist: openai; extra == "all"
-Requires-Dist: faiss-cpu; extra == "all"
 Requires-Dist: minio; extra == "all"
 Requires-Dist: qdrant-client; extra == "all"
-Requires-Dist: fastapi; extra == "all"
+Requires-Dist: pymupdf; extra == "all"
+Requires-Dist: redis; extra == "all"
+Requires-Dist: sse_starlette; extra == "all"
+Requires-Dist: faiss-cpu; extra == "all"
+Requires-Dist: streamlit_chat; extra == "all"
 
 ![image](https://img.shields.io/pypi/v/chatllm.svg) ![image](https://img.shields.io/travis/yuanjie-ai/chatllm.svg) ![image](https://readthedocs.org/projects/chatllm/badge/?version=latest)
 
 <h1 align = "center">🔥ChatLLM 基于知识库🔥</h1>
 
 <div align=center>
 <img src="data/imgs/LLM.drawio.png"/>
```

### Comparing `chatllm-2024.4.3.18.28.17/README.md` & `chatllm-2024.4.30.15.10.38/README.md`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/README.md.bak` & `chatllm-2024.4.30.15.10.38/README.md.bak`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/agent/MultiPrompt.py` & `chatllm-2024.4.30.15.10.38/chatllm/agents/MultiPrompt.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/aigc/common.py` & `chatllm-2024.4.30.15.10.38/chatllm/aigc/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/app.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/app.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/config.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/config.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/datamodels.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/datamodels.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/openai_client.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/openai_client.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/all_chat_completions.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/all_chat_completions.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/all_chat_completions_.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/all_chat_completions_.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/api.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/api.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/audio_speech.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/audio_speech.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_copilot.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions_copilot.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_extra.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions_extra.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_glm.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions_glm.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_gptall.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions_gptall.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_kimi.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions_kimi.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_rag.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions_rag.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_redirect.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions_redirect.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_smooth.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions_smooth.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/chat_completions_suno.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/chat_completions_suno.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         }
         raise HTTPException(status_code=status.HTTP_401_UNAUTHORIZED, detail=detail)
 
     # 轮询
     if "|" in api_key:
         api_key = np.random.choice(api_key.strip().split('|'))
 
-    response = Completions(api_key).create_sse(request)
+    response = Completions(api_key).create_sse(request)  # todo: 缓存
 
     return response
 
 
 if __name__ == '__main__':
     from meutils.serving.fastapi import App
```

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/cocopilot.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/cocopilot.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/embeddings.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/embeddings.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/files.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/files.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/files_moonshot.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/files_moonshot.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/files_moonshot_api.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/files_moonshot_api.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/local_embeddings.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/local_embeddings.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/models.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/models.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/smooth_completions.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/smooth_completions.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routers/utils.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routers/utils.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routes/api.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routes/api.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routes/base.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routes/base.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routes/completions.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routes/completions.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routes/embeddings.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routes/embeddings.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/routes/responses.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/routes/responses.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/sse_api.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/sse_api.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/api/test.py` & `chatllm-2024.4.30.15.10.38/chatllm/api/test.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/applications/Question2Answer.py` & `chatllm-2024.4.30.15.10.38/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/applications/__chatbase.py` & `chatllm-2024.4.30.15.10.38/chatllm/applications/__chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/applications/chatann.py` & `chatllm-2024.4.30.15.10.38/chatllm/applications/chatann.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/applications/chatbase.py` & `chatllm-2024.4.30.15.10.38/chatllm/applications/chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/applications/chatcrawler.py` & `chatllm-2024.4.30.15.10.38/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/applications/chatmind.py` & `chatllm-2024.4.30.15.10.38/chatllm/applications/chatmind.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/applications/chatpdf.py` & `chatllm-2024.4.30.15.10.38/chatllm/applications/chatpdf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/applications/chatwhoosh.py` & `chatllm-2024.4.30.15.10.38/chatllm/applications/chatwhoosh.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/clis/cli.py` & `chatllm-2024.4.30.15.10.38/chatllm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/closeai.py` & `chatllm-2024.4.30.15.10.38/chatllm/closeai.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llm_test.py` & `chatllm-2024.4.30.15.10.38/chatllm/llm_test.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/__init__.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/__init__.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/__init__.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/_chatbase.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/_chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/_chatocr.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/_chatocr.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chat4all.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chat4all.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatbase.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatfile.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chatfile.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatfiles.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chatfiles.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatocr.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chatocr.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatpicture.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chatpicture.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chatqa.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chatqa.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/chaturl.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/chaturl.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/applications/summarizer.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/applications/summarizer.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/audio/speech.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/audio/speech.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/callbacks/streaming.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/callbacks/streaming.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/chat_models/openai.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/chat_models/openai.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/_erniebot.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/_erniebot.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/_hunyuan.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/_hunyuan.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/chat_image.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/chat_image.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/chat_tts.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/chat_tts.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/chatglm.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/chatglm.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/chatglm_web.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/chatglm_web.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @Project      : AI.  @by PyCharm
 # @File         : chatglm_web
 # @Time         : 2024/3/11 18:52
 # @Author       : betterme
 # @WeChat       : meutils
 # @Software     : PyCharm 🧩 🔨[🔨](…….)
 # @Description  : https://github.com/ikechan8370/chatgpt-plugin/blob/32af7b9a74fdfbd329f5977c6e3fb5b3928ed0f1/client/ChatGLM4Client.js#L6
-import httpx
+import shortuuid
 
 from meutils.pipe import *
 from meutils.notice.feishu import send_message
 
 from chatllm.schemas import chatglm_types
 from chatllm.schemas.openai_types import chat_completion, chat_completion_chunk
 from chatllm.schemas.openai_api_protocol import ChatCompletionRequest
@@ -174,19 +174,22 @@
             response.raise_for_status()
 
         # refresh_token = response.get("refresh_token") # 是否去更新
         return response.json().get("result", {}).get("accessToken")
 
     async def put_object_for_openai(
         self,
-        file: Union[str, Path, UploadFile],
+        file: Union[bytes, str, Path, UploadFile],
         purpose: str = "chatpdf_file_upload",  # file_upload
+        filename: Optional[str] = None,
     ):  # filename => file url 预览https://sfile.chatglm.cn/doc_mobile/fdfeeea2-2721-445a-a8f6-b70a7972c1da.pdf
+        if isinstance(file, bytes):
+            filename = filename or f"{shortuuid.random()}.png"
 
-        if isinstance(file, (str, Path)) and Path(file).exists():
+        elif isinstance(file, (str, Path)) and Path(file).exists():
             filename = Path(file).name
             file = Path(file).read_bytes()
         else:
             filename = file.filename or file.file.name
             file = file.file
 
         # base_url = "https://chatglm.cn/chatglm/backend-api/v1/chatpdf_file_upload"
@@ -289,36 +292,36 @@
     #                 }
     #             ]
     #         }
     #
     #     ]
     # }
 
-    data = {
-        # "assistant_id": "65940acff94777010aa6b796",
-        "assistant_id": "65f41c8a9c0ebbcbe28bb9c1",  # 智能体
-        # "conversation_id": "65f41fe143c80c1f80b55150",
-        # "conversation_id": "",
-        # "meta_data": {
-        #     "is_test": False,
-        #     "input_question_type": "xxxx",
-        #     "channel": "",
-        #     "draft_id": ""
-        # },
-        "messages": [
-            {
-                "role": "user",
-                "content": "从业人员可以炒股吗"
-            }
-
-        ]
-    }
+    # data = {
+    #     # "assistant_id": "65940acff94777010aa6b796",
+    #     "assistant_id": "65f41c8a9c0ebbcbe28bb9c1",  # 智能体
+    #     # "conversation_id": "65f41fe143c80c1f80b55150",
+    #     # "conversation_id": "",
+    #     # "meta_data": {
+    #     #     "is_test": False,
+    #     #     "input_question_type": "xxxx",
+    #     #     "channel": "",
+    #     #     "draft_id": ""
+    #     # },
+    #     "messages": [
+    #         {
+    #             "role": "user",
+    #             "content": "从业人员可以炒股吗"
+    #         }
+    #
+    #     ]
+    # }
+    #
+    # for i in Completions().create(ChatCompletionRequest(**data)):
+    #     print(i.choices[0].delta.content, end="")
+    #     # pass
 
-    for i in Completions().create(ChatCompletionRequest(**data)):
-        print(i.choices[0].delta.content, end="")
-        # pass
+    _ = Completions().put_object_for_openai(Path("/Users/betterme/PycharmProjects/AI/QR.png").read_bytes(), "")  # 上传文件
 
-    _ = Completions().put_object_for_openai("/Users/betterme/PycharmProjects/AI/ChatLLM/data/孙子兵法.pdf", "")  # 上传文件
     print(arun(_, debug=True))
     print(_)
     pass
-
```

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/copilot.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/copilot.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/deepseek.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/deepseek.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/demo.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/demo.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/dify.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/dify.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/ernie.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/ernie.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/github_copilot.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/github_copilot.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/github_copilot_.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/github_copilot_.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/google_enerativeai.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/google_enerativeai.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/google_enerativeai_.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/google_enerativeai_.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/gptall.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/gptall.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/groq.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/groq.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/hunyuan.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/hunyuan.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/kimi.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/kimi.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/moonshot_kimi.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/moonshot_kimi.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/openai_completions.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/openai_completions.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/openai_completions_bk.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/openai_completions_bk.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/smooth.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/smooth.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/smooth_.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/smooth_.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/spark.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/spark.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/stepchat.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/stepchat.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,7 +101,10 @@
 
     }
     url = "https://stepchat.cn/api/proto.chat.v1.ChatMessageService/SendMessageStream"
     #
     payload = {"chatId":"83776330600574976","messageInfo":{"text":"11"}}
     #
     response = httpx.post(url, json=payload, headers=headers)
+
+
+
```

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/suno.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/suno.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/suno_.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/suno_.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/completions/suno__.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/completions/suno__.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/decorators/common.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/decorators/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/FilesLoader.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/document_loaders/FilesLoader.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/__init__.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/document_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/docx.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/document_loaders/docx.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/file.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/document_loaders/file.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/file_loader.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/document_loaders/file_loader.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/image.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/document_loaders/image.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/pdf.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/document_loaders/pdf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/document_loaders/text.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/document_loaders/text.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/ApiEmbeddings.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/embeddings/ApiEmbeddings.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/DashScopeEmbeddings.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/embeddings/DashScopeEmbeddings.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/HuggingFaceEmbeddings.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/embeddings/HuggingFaceEmbeddings.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/OpenAIEmbeddings.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/embeddings/OpenAIEmbeddings.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/XunfeiEmbedding.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/embeddings/XunfeiEmbedding.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/embeddings/openai_embeddings.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/embeddings/openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/__init__.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/basellm.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/llms/basellm.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/chatglm.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/llms/chatglm.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/ernie.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/llms/ernie.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/hunyuan.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/llms/hunyuan.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/kimi.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/llms/kimi.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/llms/spark.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/llms/spark.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/kb.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/prompts/kb.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/ocr.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/prompts/ocr.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/prompt_templates.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/prompts/prompt_templates.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/prompt_watch.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/prompts/prompt_watch.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/rag.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/prompts/rag.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/prompts/格式化.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/prompts/格式化.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/textsplitter/ali_text_splitter.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/textsplitter/ali_text_splitter.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/textsplitter/chinese_text_splitter.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/textsplitter/chinese_text_splitter.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/textsplitter/zh_title_enhance.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/textsplitter/zh_title_enhance.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/utils/common.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/utils/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/DocArrayInMemorySearch.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/vectorstores/DocArrayInMemorySearch.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/ElasticsearchStore.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/vectorstores/ElasticsearchStore.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/FAISS.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/vectorstores/FAISS.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/Milvus.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/vectorstores/Milvus.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/Usearch.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/vectorstores/Usearch.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/VectorRecordManager.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/vectorstores/VectorRecordManager.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/__init__.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/vectorstores/__init__.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/base.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/vectorstores/base.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llmchain/vectorstores/index_utils.py` & `chatllm-2024.4.30.15.10.38/chatllm/llmchain/vectorstores/index_utils.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llms/__init__.py` & `chatllm-2024.4.30.15.10.38/chatllm/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llms/chatglm.py` & `chatllm-2024.4.30.15.10.38/chatllm/llms/chatglm.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llms/chatgpt.py` & `chatllm-2024.4.30.15.10.38/chatllm/llms/chatgpt.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llms/demo.py` & `chatllm-2024.4.30.15.10.38/chatllm/llms/demo.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/llms/llama.py` & `chatllm-2024.4.30.15.10.38/chatllm/llms/llama.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/prompts/common.py` & `chatllm-2024.4.30.15.10.38/chatllm/prompts/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/schemas/4v.py` & `chatllm-2024.4.30.15.10.38/chatllm/schemas/4v.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/schemas/chatglm_types.py` & `chatllm-2024.4.30.15.10.38/chatllm/schemas/chatglm_types.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/schemas/embedding.py` & `chatllm-2024.4.30.15.10.38/chatllm/schemas/embedding.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/schemas/kimi/protocol.py` & `chatllm-2024.4.30.15.10.38/chatllm/schemas/kimi/protocol.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/schemas/kimi_types.py` & `chatllm-2024.4.30.15.10.38/chatllm/schemas/kimi_types.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/schemas/openai_api_protocol.py` & `chatllm-2024.4.30.15.10.38/chatllm/schemas/openai_api_protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,16 +73,19 @@
     prompt_filter_result.content_filter_results
     choice.content_filter_results
 
     todo: ['messages', 'model', 'frequency_penalty', 'function_call', 'functions', 'logit_bias', 'logprobs', 'max_tokens', 'n', 'presence_penalty', 'response_format', 'seed', 'stop', 'stream', 'temperature', 'tool_choice', 'tools', 'top_logprobs', 'top_p', 'user']
     """
     model: str = ''  # "gpt-3.5-turbo-file-id"
 
-    # content: [{"type": "text", "text": "hi"}]
-    messages: Union[str, List[Dict[str, Any]]] = [{'role': 'user', 'content': 'hi'}]
+    # [{'role': 'user', 'content': 'hi'}]
+    # [{'role': 'user', 'content':  [{"type": "text", "text": ""}]]
+    # [{'role': 'user', 'content':  [{"type": "image_url", "image_url": ""}]] # 也兼容文件
+    # [{'role': 'user', 'content':  [{"type": "file", "file_url": ""}]]
+    messages: List[Dict[str, Any]] = [{'role': 'user', 'content': 'hi'}]
 
     temperature: Optional[float] = 1
     top_p: Optional[float] = 1.0
     n: Optional[int] = 1
     max_tokens: Optional[int] = None
     stop: Optional[Union[str, List[str]]] = None
     stream: Optional[bool] = False
@@ -91,49 +94,61 @@
     user: Optional[str] = None
 
     # 1106
     response_format: Optional[Any] = None
     function_call: Optional[Any] = None
 
     # 拓展字段
+    last_content: Optional[Any] = None
+
+    payload: Optional[Dict[str, Any]] = Field(default_factory=dict)  # 任意接口转chat api
+    return_raw_response: Optional[bool] = None
+
     additional_kwargs: Optional[Dict[str, Any]] = Field(default_factory=dict)
 
     refs: List[str] = []
     file_ids: List[str] = []
 
     search: Optional[bool] = None
     use_search: Optional[bool] = None  # 自动推断联网
 
     # glm
     assistant_id: str = ""
     conversation_id: str = ""  # kimi、glm4
 
-    # 模型水印
-    watermark: Optional[str] = ""
-
-    # 我是Kimi，由月之暗面科技有限公司开发的人工智能助手
-
     # todo：设计apikey入参
     # rag
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
+        self.last_content: str = self.messages[-1].get('content', '')  # 大部分时间等价于user_content
 
         if file_ids := self.file_ids or self.refs:
             self.file_ids = file_ids
             self.refs = file_ids
 
         if search := self.use_search or self.search:
             self.search = search
             self.use_search = search
 
         # glm
         self.assistant_id = self.assistant_id or "65940acff94777010aa6b796"
 
-        # if isinstance(self.messages[-1].get('content'), list): # [{'type': 'text', 'text': 'hi'}]
+        # deeplx
+        if self.model.startswith('deeplx'):
+            self.payload = {
+                "text": self.last_content,
+                "source_lang": "auto",
+                "target_lang": 'EN' if self.model.endswith('en') else 'ZH',
+                **self.payload
+            }
+
+            # self.return_raw_response
+
+        # if isinstance(self.messages[-1].get('content'), list): # [{'type': 'text', 'text': 'hi'}] # 标准化
         #     part_content = self.messages[-1]['content'][0]
         #
 
     model_config = {
         "json_schema_extra": {
             "examples": [
                 {
```

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/schemas/openai_types.py` & `chatllm-2024.4.30.15.10.38/chatllm/schemas/openai_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         }
     ]
 }
 
 chat_completion_chunk_stop_ = {
     "id": "chatcmpl-8pFbEr4Y0L6RjW5hIGgDwSbiD991v",
     "choices": [
-        {"delta": {"content": None, "function_call": None, "role": None, "tool_calls": None},
+        {"delta": {"content": "", "function_call": None, "role": None, "tool_calls": None},
          "finish_reason": "stop",
          "index": 0,
          "logprobs": None
          }
     ],
     "created": 1707225384,
     "model": "gpt-4-turbo",
@@ -137,9 +137,11 @@
 if __name__ == '__main__':
     # data = {"stream": True, "model": "gpt-3.5-turbo", "messages": [{"role": "user", "content": "你好"}]}
     # print(ChatCompletionRequest(request=data).request)
     # print(chat_completion_error)
     # print(chat_completion_slogan)
 
     # print(chat_completion_chunk_stop)
-    for i in chat_completion_error:
-        print(i)
+    # for i in chat_completion_error:
+    #     print(i)
+
+    pass
```

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/schemas/suno_types.py` & `chatllm-2024.4.30.15.10.38/chatllm/schemas/suno_types.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,23 +7,34 @@
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  :
 
 from meutils.pipe import *
 
 
+class SongRequest(BaseModel):
+    title: str = Field(description="song title")
+    lyrics: str = Field(description="Enter lyrics, example: [Intro]...[Verse]...[Chorus]...")
+    music_style: str = Field(description="the Style of Music, Maximum 10 words", examples=['syncopated country ...'])
+    continue_clip_id: Optional[str] = Field(
+        description="Continue creating based on song id/clip_id",
+        examples=['8c7f666a-4df6-4657-8a83-d630b2b8ab56']
+    )
+    continue_at: Optional[int] = Field(120, description="Continue creating based on a certain point in time, for example at 10s")
+
+
 class Response(BaseModel):
     code: Optional[int] = 0
     msg: Optional[str] = "success"
     data: Optional[Any] = None
 
 
 class GenerateBase(BaseModel):
-    prompt: str=""
-    mv: str = "chirp-v3-0"
+    prompt: str = ""
+    mv: str = "chirp-v3"
     title: str = ""
     tags: str = ""
     continue_at: Optional[str] = None
     continue_clip_id: Optional[str] = None
 
 
 class SunoRequest(BaseModel):
@@ -88,10 +99,9 @@
     continue_clip_id: Optional[str] = None  # "8c7f666a-4df6-4657-8a83-d630b2b8ab56"
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.prompt = self.song_description
 
 
-
 if __name__ == '__main__':
     print(SunoRequest(song_description='一首关于在雨天寻找爱情的富有感染力的朋克歌曲'))
```

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/serve/_openai_api_server.py` & `chatllm-2024.4.30.15.10.38/chatllm/serve/_openai_api_server.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/serve/app.py` & `chatllm-2024.4.30.15.10.38/chatllm/serve/app.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/serve/constants.py` & `chatllm-2024.4.30.15.10.38/chatllm/serve/constants.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/serve/openai_api_server.py` & `chatllm-2024.4.30.15.10.38/chatllm/serve/openai_api_server.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/utils/common.py` & `chatllm-2024.4.30.15.10.38/chatllm/utils/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # @Project      : AI.  @by PyCharm
 # @File         : utils
 # @Time         : 2023/4/20 12:50
 # @Author       : betterme
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  :
-import copy
 
 import torch
 from transformers import AutoTokenizer, AutoModel
 
 from meutils.pipe import *
 from chatllm.utils.gpu_utils import load_chatglm_on_gpus
 
@@ -55,13 +54,12 @@
     if stream and hasattr(model, 'stream_chat'):
         return partial(model.stream_chat, tokenizer=tokenizer)  # 可以在每一次生成清GPU
     else:
         return partial(model.chat, tokenizer=tokenizer)
 
 
 
-
 if __name__ == '__main__':
     # model, tokenizer = load_llm("/CHAT_MODEL/chatglm", device='cpu')
 
     # print(completion_keys)
     pass
```

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/utils/gpu_utils.py` & `chatllm-2024.4.30.15.10.38/chatllm/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/utils/nbce.py` & `chatllm-2024.4.30.15.10.38/chatllm/utils/nbce.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/utils/nbce_test.py` & `chatllm-2024.4.30.15.10.38/chatllm/utils/nbce_test.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/utils/openai_utils.py` & `chatllm-2024.4.30.15.10.38/chatllm/completions/cf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,107 +1,94 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # @Project      : AI.  @by PyCharm
-# @File         : ppu_utils
-# @Time         : 2024/1/8 16:46
+# @File         : cf
+# @Time         : 2024/4/30 13:32
 # @Author       : betterme
 # @WeChat       : meutils
 # @Software     : PyCharm
-# @Description  : 按次计费
-import time
+# @Description  :
 
-import openai
-from openai import OpenAI
 
 from meutils.pipe import *
-from chatllm.schemas.openai_types import completion_keys
-from chatllm.schemas.openai_api_protocol import ChatCompletionRequest
+from meutils.notice.feishu import send_message
 
-from openai.types.chat import ChatCompletion, ChatCompletionChunk
+from chatllm.schemas.openai_types import chat_completion, chat_completion_chunk as _chat_completion_chunk
+from chatllm.schemas.openai_api_protocol import ChatCompletionRequest, UsageInfo
 
+from chatllm.llmchain.completions import chatglm_web
 
-def to_openai_completion_params(
-    request: Union[dict, ChatCompletionRequest],
-    redirect_model: Optional[str] = None
-) -> dict:
-    data = copy.deepcopy(request)
-    if isinstance(request, ChatCompletionRequest):
-        data = request.model_dump()
 
-    extra_body = {}
-    for key in list(data):
-        if key not in completion_keys:
-            extra_body.setdefault(key, data.pop(key))
+class Completions(object):
+    def __init__(self, api_key: Optional[str] = None):  # @cf/bytedance/stable-diffusion-xl-lightning
+        """CLOUDFLARE_ACCOUNT_ID-CLOUDFLARE_API_TOKEN"""
 
-    data['extra_body'] = extra_body  # 拓展字段
-    data['model'] = redirect_model or data['model']
+        api_key = api_key or os.getenv("CLOUDFLARE_API_TOKEN")
+        cloudflare_account_id, api_key = api_key.split('-', maxsplit=1)
+        base_url = f"https://api.cloudflare.com/client/v4/accounts/{cloudflare_account_id}/ai/run/"
 
-    return data
+        headers = {"Authorization": f"Bearer {api_key}"}
 
+        self.httpx_client = httpx.Client(base_url=base_url, follow_redirects=True, timeout=10, headers=headers)
+        self.httpx_aclient = httpx.AsyncClient(base_url=base_url, follow_redirects=True, timeout=10, headers=headers)
 
-# @background_task
-def per_create(api_key: Optional[str] = None, base_url: Optional[str] = None, model: str = 'per'):
-    openai = OpenAI(
-        api_key=api_key,
-        base_url=base_url or "https://api.chatllm.vip/v1",
-        http_client=httpx.Client(follow_redirects=True)
-    )
-    return openai.chat.completions.create(model=model, messages=[{"role": "user", "content": "hi"}])
+    async def acreate(self, request: ChatCompletionRequest):  # todo: minio 兜底
+        payload = {
+            "prompt": request.last_content
+        }
+
+        response: httpx.Response = await self.httpx_aclient.post(request.model, json=payload)
+        if response.status_code != 200:
+            response.raise_for_status()
+            send_message(response.text, title='cf')
+
+        # Path('debug.png').write_bytes(response.content) # debug
+
+        if request.stream:
+            chat_completion_chunk = _chat_completion_chunk.model_copy(deep=True)
+
+            # 前置
+            chat_completion_chunk.choices[0].delta.content = "\n"
+            yield chat_completion_chunk
 
+            # main
+            file_object = await chatglm_web.Completions().put_object_for_openai(response.content, "")
 
-def openai_response2sse(response, redirect_model: Optional[str] = None, n: float = 1.2):
-    """
+            image_url = file_object.filename
+            chunk = f"![]({image_url})"
+            chat_completion_chunk.choices[0].delta.content = chunk
+            yield chat_completion_chunk
 
-    :param response:
-    :param redirect_model: request.model
-    :param n:
-    :return:
-    """
-    from sse_starlette import EventSourceResponse
-
-    # logger.debug(type(response))
-
-    if isinstance(response, ChatCompletion):
-        response.model = redirect_model or response.model
-
-        response.usage.prompt_tokens = int(response.usage.prompt_tokens * n)
-        completion_tokens = response.usage.completion_tokens or len(response.choices[0].message.content)
-        response.usage.completion_tokens = int(completion_tokens * n)
-        response.usage.total_tokens = response.usage.prompt_tokens + response.usage.completion_tokens
-
-        return response
-
-    def do_chunk(chunk):
-        chunk: ChatCompletionChunk
-        chunk.model = redirect_model or chunk.model
-
-        # logger.debug(chunk.choices)
-
-        if chunk.choices and chunk.choices[0].delta.content:  # 跳过首行空值
-            if chunk.choices[0].finish_reason == "stop":
-                chunk.choices[0].delta.content = ""  # "delta":{} "delta":{"content":""}
-                yield chunk.model_dump_json()
-                # yield "[DONE]"  # 兼容标准格式
-                return
-            else:
-                yield chunk.model_dump_json()
-
-
-    if inspect.isasyncgen(response) or isinstance(response, openai.AsyncStream):
-        async def gen():
-            async for chunk in response:
-                for chunk in do_chunk(chunk):
-                    yield chunk
-            yield "[DONE]"  # 兼容标准格式
-
-    else:
-        def gen():
-            for chunk in response:
-                for chunk in do_chunk(chunk):
-                    yield chunk
-            yield "[DONE]"  # 兼容标准格式
+            # 结束标识
+            chat_completion_chunk.choices[0].delta.content = ""
+            chat_completion_chunk.choices[0].finish_reason = "stop"
+            yield chat_completion_chunk
 
-    return EventSourceResponse(gen(), ping=10000)  # sse_response
+        else:
+            chat_completion.usage.completion_tokens = 1
+            chat_completion.choices[0].message.content = chunk
+            yield chat_completion
+
+    # async def acreate(self, request: ChatCompletionRequest, **kwargs):
+    #     pass
 
 
 if __name__ == '__main__':
-    print(per_create())
+    request = ChatCompletionRequest(
+        model='/@cf/bytedance/stable-diffusion-xl-lightning',
+        messages=[{'role': 'user', 'content': '画一条可爱的猫'}],
+        stream=False
+    )
+
+    response = Completions().acreate(request)
+    # print(arun(response))
+    #
+    for i in Completions().create(request):
+        print(i)
+
+    # import tiktoken
+    #
+    # print(tiktoken.get_encoding('cl100k_base').encode('我是谁'))
+
+    import openai
+
+    # openai.OpenAI.chat.completions.create()
```

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/chat.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/chat.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/chat_copilot.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/chat_copilot.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/chatbase.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/chatbook.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/chatbook.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/chatbot.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/chatbot.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/chatfile.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_nesc.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/chatfile_nesc.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_nesc_glm_v0.1.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/chatfile_nesc_glm_v0.1.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_nesc_last.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/chatfile_nesc_last.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_nesc_v1.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/chatfile_nesc_v1.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_nesc_v2.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/chatfile_nesc_v2.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/chatfile_v0.1.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/chatfile_v0.1.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/chatmind.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/chatmind.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/chatpdf.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/dalle.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/dalle.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/demo.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/demo.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/gradio_ui.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/nice_ui.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/prompt_maker.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/prompt_maker.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/qa.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/qa.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm/webui/visualglm_st.py` & `chatllm-2024.4.30.15.10.38/chatllm/webui/visualglm_st.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/chatllm.egg-info/PKG-INFO` & `chatllm-2024.4.30.15.10.38/chatllm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatllm
-Version: 2024.4.3.18.28.17
+Version: 2024.4.30.15.10.38
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -43,25 +43,25 @@
 Requires-Dist: streamlit; extra == "streamlit"
 Requires-Dist: streamlit_chat; extra == "streamlit"
 Provides-Extra: rag
 Requires-Dist: redis; extra == "rag"
 Requires-Dist: minio; extra == "rag"
 Requires-Dist: faiss-cpu; extra == "rag"
 Provides-Extra: all
-Requires-Dist: pymupdf; extra == "all"
 Requires-Dist: sse-starlette; extra == "all"
 Requires-Dist: streamlit; extra == "all"
-Requires-Dist: sse_starlette; extra == "all"
-Requires-Dist: redis; extra == "all"
-Requires-Dist: streamlit_chat; extra == "all"
+Requires-Dist: fastapi; extra == "all"
 Requires-Dist: openai; extra == "all"
-Requires-Dist: faiss-cpu; extra == "all"
 Requires-Dist: minio; extra == "all"
 Requires-Dist: qdrant-client; extra == "all"
-Requires-Dist: fastapi; extra == "all"
+Requires-Dist: pymupdf; extra == "all"
+Requires-Dist: redis; extra == "all"
+Requires-Dist: sse_starlette; extra == "all"
+Requires-Dist: faiss-cpu; extra == "all"
+Requires-Dist: streamlit_chat; extra == "all"
 
 ![image](https://img.shields.io/pypi/v/chatllm.svg) ![image](https://img.shields.io/travis/yuanjie-ai/chatllm.svg) ![image](https://readthedocs.org/projects/chatllm/badge/?version=latest)
 
 <h1 align = "center">🔥ChatLLM 基于知识库🔥</h1>
 
 <div align=center>
 <img src="data/imgs/LLM.drawio.png"/>
```

### Comparing `chatllm-2024.4.3.18.28.17/chatllm.egg-info/SOURCES.txt` & `chatllm-2024.4.30.15.10.38/chatllm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,66 +1,51 @@
-.editorconfig
-.gitignore
-ITEMS.md
 LICENSE
-LLMS.md
 MANIFEST.in
-Makefile
 README.md
 README.md.bak
-TODO.md
-clear_git_history.sh
-git_init.sh
-pypi.sh
-requirements.txt
-requirements_ann.txt
-requirements_api.txt
-requirements_openai.txt
-requirements_pdf.txt
-requirements_rag.txt
-requirements_streamlit.txt
 setup.py
-apps/__init__.py
-apps/allchat.py
 chatllm/__init__.py
 chatllm/closeai.py
 chatllm/llm_test.py
 chatllm.egg-info/PKG-INFO
 chatllm.egg-info/SOURCES.txt
 chatllm.egg-info/dependency_links.txt
 chatllm.egg-info/entry_points.txt
 chatllm.egg-info/not-zip-safe
 chatllm.egg-info/requires.txt
 chatllm.egg-info/top_level.txt
-chatllm/agent/MultiPrompt.py
-chatllm/agent/__init__.py
+chatllm/agents/MultiPrompt.py
+chatllm/agents/__init__.py
+chatllm/agents/glm_agent.py
 chatllm/aigc/__init__.py
 chatllm/aigc/common.py
-chatllm/api/TODO.md
 chatllm/api/__init__.py
 chatllm/api/app.py
 chatllm/api/config.py
 chatllm/api/datamodels.py
 chatllm/api/openai_client.py
 chatllm/api/sse_api.py
 chatllm/api/test.py
 chatllm/api/routers/__init__.py
 chatllm/api/routers/all_chat_completions.py
 chatllm/api/routers/all_chat_completions_.py
 chatllm/api/routers/api.py
 chatllm/api/routers/audio_speech.py
+chatllm/api/routers/chat_all.py
+chatllm/api/routers/chat_cf.py
 chatllm/api/routers/chat_completions_copilot.py
 chatllm/api/routers/chat_completions_extra.py
 chatllm/api/routers/chat_completions_glm.py
 chatllm/api/routers/chat_completions_gptall.py
 chatllm/api/routers/chat_completions_kimi.py
 chatllm/api/routers/chat_completions_rag.py
 chatllm/api/routers/chat_completions_redirect.py
 chatllm/api/routers/chat_completions_smooth.py
 chatllm/api/routers/chat_completions_suno.py
+chatllm/api/routers/chat_deeplx.py
 chatllm/api/routers/cocopilot.py
 chatllm/api/routers/demo.py
 chatllm/api/routers/embeddings.py
 chatllm/api/routers/files.py
 chatllm/api/routers/files_moonshot.py
 chatllm/api/routers/files_moonshot_api.py
 chatllm/api/routers/local_embeddings.py
@@ -82,21 +67,23 @@
 chatllm/applications/chatbase.py
 chatllm/applications/chatcrawler.py
 chatllm/applications/chatdoc.py
 chatllm/applications/chatmind.py
 chatllm/applications/chatpdf.py
 chatllm/applications/chatwhoosh.py
 chatllm/applications/pipeline.py
-chatllm/clis/README.md
-chatllm/clis/TODO.md
 chatllm/clis/__init__.py
 chatllm/clis/cli.py
-chatllm/llmchain/TODO.md
+chatllm/completions/__init__.py
+chatllm/completions/cf.py
+chatllm/completions/chat_all.py
+chatllm/completions/deeplx.py
+chatllm/completions/free.py
+chatllm/completions/glm.py
 chatllm/llmchain/__init__.py
-chatllm/llmchain/suno.md
 chatllm/llmchain/applications/__init__.py
 chatllm/llmchain/applications/_chatbase.py
 chatllm/llmchain/applications/_chatocr.py
 chatllm/llmchain/applications/chat4all.py
 chatllm/llmchain/applications/chataudio.py
 chatllm/llmchain/applications/chatbase.py
 chatllm/llmchain/applications/chatbook.py
@@ -144,14 +131,15 @@
 chatllm/llmchain/completions/smooth_.py
 chatllm/llmchain/completions/spark.py
 chatllm/llmchain/completions/stepchat.py
 chatllm/llmchain/completions/suno.py
 chatllm/llmchain/completions/suno_.py
 chatllm/llmchain/completions/suno__.py
 chatllm/llmchain/completions/suno_api.py
+chatllm/llmchain/completions/suno_api_.py
 chatllm/llmchain/decorators/__init__.py
 chatllm/llmchain/decorators/common.py
 chatllm/llmchain/document_loaders/FilesLoader.py
 chatllm/llmchain/document_loaders/__init__.py
 chatllm/llmchain/document_loaders/docx.py
 chatllm/llmchain/document_loaders/file.py
 chatllm/llmchain/document_loaders/file_loader.py
@@ -210,65 +198,48 @@
 chatllm/schemas/metadata.py
 chatllm/schemas/openai_api_protocol.py
 chatllm/schemas/openai_types.py
 chatllm/schemas/suno_types.py
 chatllm/schemas/json_schema_extra/__init__.py
 chatllm/schemas/kimi/__init__.py
 chatllm/schemas/kimi/protocol.py
-chatllm/schemas/kimi/state.json
 chatllm/serve/__init__.py
 chatllm/serve/_openai_api_server.py
 chatllm/serve/app.py
 chatllm/serve/constants.py
 chatllm/serve/openai_api_server.py
 chatllm/utils/__init__.py
 chatllm/utils/_textsplitter.py
 chatllm/utils/common.py
 chatllm/utils/gpu_utils.py
 chatllm/utils/nbce.py
 chatllm/utils/nbce_test.py
 chatllm/utils/openai_utils.py
-chatllm/webui/!.png
 chatllm/webui/__init__.py
-chatllm/webui/bot.png
 chatllm/webui/chat.py
 chatllm/webui/chat_copilot.py
 chatllm/webui/chatbase.py
-chatllm/webui/chatbook.png
 chatllm/webui/chatbook.py
-chatllm/webui/chatbot.png
 chatllm/webui/chatbot.py
 chatllm/webui/chatfile.py
 chatllm/webui/chatfile_nesc.py
 chatllm/webui/chatfile_nesc_glm_v0.1.py
 chatllm/webui/chatfile_nesc_last.py
 chatllm/webui/chatfile_nesc_v1.py
 chatllm/webui/chatfile_nesc_v2.py
 chatllm/webui/chatfile_v0.1.py
 chatllm/webui/chatmind.py
 chatllm/webui/chatpdf.py
-chatllm/webui/conf.yaml
 chatllm/webui/dalle.py
 chatllm/webui/demo.py
-chatllm/webui/fire.png
 chatllm/webui/gradio_ui.py
-chatllm/webui/logo.png
-chatllm/webui/nesc.jpeg
 chatllm/webui/nice_ui.py
 chatllm/webui/prompt_maker.py
 chatllm/webui/qa.py
-chatllm/webui/run.sh
-chatllm/webui/user.jpg
 chatllm/webui/visualglm_st.py
-chatllm/webui/副本人工智能咨询服务协议 汉洁 南京当月糯 20240105(1)(1).docx
-chatllm/webui/同程报价.xlsx
-chatllm/webui/规丞相.png
-chatllm/webui/酒店百问百答.pdf
-chatllm/webui/附件1：东北证券股份有限公司员工合规手册（2023年12月）.doc
-chatllm/webui/附件1：东北证券股份有限公司员工合规手册（2023年12月）.docx
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/make.bat
```

### Comparing `chatllm-2024.4.3.18.28.17/docs/Makefile` & `chatllm-2024.4.30.15.10.38/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/docs/conf.py` & `chatllm-2024.4.30.15.10.38/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/docs/make.bat` & `chatllm-2024.4.30.15.10.38/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/setup.py` & `chatllm-2024.4.30.15.10.38/setup.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/tests/oneapi_test.py` & `chatllm-2024.4.30.15.10.38/tests/oneapi_test.py`

 * *Files identical despite different names*

### Comparing `chatllm-2024.4.3.18.28.17/tests/内存型.ipynb` & `chatllm-2024.4.30.15.10.38/tests/内存型.ipynb`

 * *Files identical despite different names*

