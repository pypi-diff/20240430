# Comparing `tmp/osc_llm-0.1.0.tar.gz` & `tmp/osc_llm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osc_llm-0.1.0.tar", max compression
+gzip compressed data, was "osc_llm-0.1.1.tar", max compression
```

## Comparing `osc_llm-0.1.0.tar` & `osc_llm-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,45 @@
--rw-r--r--   0        0        0       11 2023-09-16 00:13:46.000000 osc_llm-0.1.0/README.md
--rw-r--r--   0        0        0       68 2023-09-15 22:37:29.000000 osc_llm-0.1.0/osc_llm/__init__.py
--rw-r--r--   0        0        0     8284 2023-09-17 09:47:33.397523 osc_llm-0.1.0/osc_llm/chat.py
--rw-r--r--   0        0        0     8013 2023-09-17 04:55:25.254855 osc_llm-0.1.0/osc_llm/cli.py
--rw-r--r--   0        0        0       25 2023-09-16 01:03:33.000000 osc_llm-0.1.0/osc_llm/layer/__init__.py
--rw-r--r--   0        0        0      636 2023-09-16 01:02:48.000000 osc_llm-0.1.0/osc_llm/layer/norm.py
--rw-r--r--   0        0        0       37 2023-09-15 22:37:29.000000 osc_llm-0.1.0/osc_llm/llm/__init__.py
--rw-r--r--   0        0        0    16174 2023-09-17 03:37:09.220806 osc_llm-0.1.0/osc_llm/llm/llama.py
--rw-r--r--   0        0        0        0 2023-09-17 08:47:55.583378 osc_llm-0.1.0/osc_llm/quantize/__init__.py
--rw-r--r--   0        0        0        0 2023-09-17 08:48:00.519372 osc_llm-0.1.0/osc_llm/quantize/bnb.py
--rw-r--r--   0        0        0        0 2023-09-17 08:48:05.383365 osc_llm-0.1.0/osc_llm/quantize/gptq.py
--rw-r--r--   0        0        0     3434 2023-09-15 22:37:29.000000 osc_llm-0.1.0/osc_llm/tokenizer.py
--rw-r--r--   0        0        0    16082 2023-09-17 00:44:03.706275 osc_llm-0.1.0/osc_llm/utils.py
--rw-r--r--   0        0        0      394 2023-09-17 09:46:59.401202 osc_llm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 osc_llm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      560 2024-04-29 01:55:20.518111 osc_llm-0.1.1/README.md
+-rw-r--r--   0        0        0      253 2024-04-30 00:21:10.635963 osc_llm-0.1.1/osc_llm/__init__.py
+-rw-r--r--   0        0        0       51 2024-04-27 15:22:11.337904 osc_llm-0.1.1/osc_llm/architectures/__init__.py
+-rw-r--r--   0        0        0     8089 2024-04-27 15:21:42.709990 osc_llm-0.1.1/osc_llm/architectures/transformer_decoder.py
+-rw-r--r--   0        0        0     4176 2024-04-30 14:09:39.718502 osc_llm-0.1.1/osc_llm/chat.py
+-rw-r--r--   0        0        0      136 2024-04-29 08:59:09.247275 osc_llm-0.1.1/osc_llm/chat_templates/__init__.py
+-rw-r--r--   0        0        0     1509 2024-04-30 01:49:42.527398 osc_llm-0.1.1/osc_llm/chat_templates/base.py
+-rw-r--r--   0        0        0      891 2024-04-27 15:20:32.266209 osc_llm-0.1.1/osc_llm/chat_templates/chatml.py
+-rw-r--r--   0        0        0     2751 2024-04-30 12:29:13.554688 osc_llm-0.1.1/osc_llm/chat_templates/llama.py
+-rw-r--r--   0        0        0     6659 2024-04-28 23:27:52.946274 osc_llm-0.1.1/osc_llm/cli.py
+-rw-r--r--   0        0        0     1314 2024-04-29 23:11:24.182541 osc_llm-0.1.1/osc_llm/config.py
+-rw-r--r--   0        0        0       48 2024-04-27 15:57:52.529093 osc_llm-0.1.1/osc_llm/demos/__init__.py
+-rw-r--r--   0        0        0     5517 2024-04-27 16:06:43.049671 osc_llm-0.1.1/osc_llm/demos/language_model.py
+-rw-r--r--   0        0        0       83 2024-04-29 23:43:54.288202 osc_llm-0.1.1/osc_llm/engines/__init__.py
+-rw-r--r--   0        0        0     1874 2024-04-30 14:10:01.673484 osc_llm-0.1.1/osc_llm/engines/base.py
+-rw-r--r--   0        0        0     4185 2024-04-30 14:10:16.748812 osc_llm-0.1.1/osc_llm/engines/v1.py
+-rw-r--r--   0        0        0     4916 2024-04-30 14:10:25.104449 osc_llm-0.1.1/osc_llm/engines/v2.py
+-rw-r--r--   0        0        0      725 2024-04-27 15:10:30.684848 osc_llm-0.1.1/osc_llm/layers/__init__.py
+-rw-r--r--   0        0        0      650 2024-04-27 15:10:30.656849 osc_llm-0.1.1/osc_llm/layers/activation.py
+-rw-r--r--   0        0        0     6224 2024-04-27 15:10:30.680848 osc_llm-0.1.1/osc_llm/layers/attention.py
+-rw-r--r--   0        0        0      186 2024-04-27 15:17:53.918752 osc_llm-0.1.1/osc_llm/layers/dropout.py
+-rw-r--r--   0        0        0     2238 2024-04-27 15:10:30.684848 osc_llm-0.1.1/osc_llm/layers/embedding.py
+-rw-r--r--   0        0        0     3371 2024-04-27 15:10:30.684848 osc_llm-0.1.1/osc_llm/layers/feedforward.py
+-rw-r--r--   0        0        0      336 2024-04-27 15:10:30.684848 osc_llm-0.1.1/osc_llm/layers/head.py
+-rw-r--r--   0        0        0     2745 2024-04-27 15:10:30.684848 osc_llm-0.1.1/osc_llm/layers/kv_cache.py
+-rw-r--r--   0        0        0     5657 2024-04-27 15:10:30.688848 osc_llm-0.1.1/osc_llm/layers/linear.py
+-rw-r--r--   0        0        0      823 2024-04-27 15:10:30.688848 osc_llm-0.1.1/osc_llm/layers/normalization.py
+-rw-r--r--   0        0        0      416 2024-04-27 15:17:28.926844 osc_llm-0.1.1/osc_llm/model_helpers/__init__.py
+-rw-r--r--   0        0        0     6262 2024-04-27 15:44:58.586217 osc_llm-0.1.1/osc_llm/model_helpers/base.py
+-rw-r--r--   0        0        0     3054 2024-04-27 15:16:30.027073 osc_llm-0.1.1/osc_llm/model_helpers/llama.py
+-rw-r--r--   0        0        0     3203 2024-04-27 15:34:51.665212 osc_llm-0.1.1/osc_llm/model_helpers/qwen.py
+-rw-r--r--   0        0        0       46 2024-04-27 15:00:44.802617 osc_llm-0.1.1/osc_llm/optimizers/__init__.py
+-rw-r--r--   0        0        0     1376 2024-04-27 15:00:44.802617 osc_llm-0.1.1/osc_llm/optimizers/scheduler.py
+-rw-r--r--   0        0        0      159 2024-04-27 15:10:37.236808 osc_llm-0.1.1/osc_llm/quantizers/__init__.py
+-rw-r--r--   0        0        0      717 2024-04-27 15:10:37.244808 osc_llm-0.1.1/osc_llm/quantizers/base.py
+-rw-r--r--   0        0        0     8861 2024-04-27 15:33:29.096094 osc_llm-0.1.1/osc_llm/quantizers/int4.py
+-rw-r--r--   0        0        0     3347 2024-04-27 15:33:57.584497 osc_llm-0.1.1/osc_llm/quantizers/int8.py
+-rw-r--r--   0        0        0       74 2024-04-27 15:04:12.071947 osc_llm-0.1.1/osc_llm/samplers/__init__.py
+-rw-r--r--   0        0        0      903 2024-04-27 15:04:12.079947 osc_llm-0.1.1/osc_llm/samplers/base.py
+-rw-r--r--   0        0        0     1134 2024-04-27 15:04:12.083947 osc_llm-0.1.1/osc_llm/samplers/top_k.py
+-rw-r--r--   0        0        0     1121 2024-04-27 15:04:12.083947 osc_llm-0.1.1/osc_llm/samplers/top_p.py
+-rw-r--r--   0        0        0     7959 2024-04-30 11:45:44.712285 osc_llm-0.1.1/osc_llm/tokenizer.py
+-rw-r--r--   0        0        0     6252 2024-04-29 07:31:58.187293 osc_llm-0.1.1/osc_llm/utils.py
+-rw-r--r--   0        0        0      495 2024-04-30 14:22:42.505200 osc_llm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 osc_llm-0.1.1/PKG-INFO
```

